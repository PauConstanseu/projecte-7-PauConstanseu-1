# Informe de Projecte: Administració i Seguretat del Servidor de Fitxers FOOD-03

Aquest informe detalla la configuració avançada realitzada al servidor per garantir la seguretat de les dades, el control de l'espai i l'automatització d'accessos al domini `foodlogistic.test`.

---

## 1. Introducció i Infraestructura de Directori Actiu (AD DS)
La base del projecte és una estructura jeràrquica d'Unitats Organitzatives (OU) que permet una gestió eficient d'usuaris i grups.

Aqui el que he fet ha sigut crear la estructura AD i els grups:

![Captura 1](/Tasca03/img/1.webp)

(Vaig tenir un petit problema i vaig haver de canviar el nom dels grups en castella)

---

## 2. Seguretat del Sistema de Fitxers (NTFS)

S'ha aplicat el **principi de mínim privilegi**, eliminant l'herència de permisos de Windows per garantir que cap usuari accedeixi a dades que no li pertoquen.

### 2.1. Carpeta Public

Configurada per a l'accés de lectura/escriptura de tots els usuaris del domini.

![Permisos Public 1](/Tasca03/img/2.png)

![Permisos Public 2](/Tasca03/img/3.png)

### 2.2. Carpeta Operacions
Accés restringit exclusivament al grup de seguretat `Transport`.

![Permisos Operacions 1](/Tasca03/img/4.png)

![Permisos Operacions 2](/Tasca03/img/5.png)

![Permisos Operacions 3](/Tasca03/img/6.png)

![Permisos Operacions 4](/Tasca03/img/(6).png)

### 2.3. Carpeta Direcció

Creació del directori i assignació de permisos de modificació exclusius per al grup `direccion`.

![Creació carpeta](/Tasca03/img/7.png)

![Permisos Direccio 1](/Tasca03/img/9.png)

---

## 3. Recursos Compartits i Access-Based Enumeration (ABE)

S'han habilitat els recursos a la xarxa activant la tecnologia **ABE**, la qual amaga les carpetes compartides a aquells usuaris que no tinguin permisos NTFS de lectura.

* **Configuració del Share via PowerShell:**
  
![PowerShell SMB Share](/Tasca03/img/8.png)

* **Activació i confirmació de l'ABE al Servidor:**
  
![Activació ABE](/Tasca03/img/basedenum.png)

---

## 4. Automatització: Polítiques de Grup (GPO)

Per optimitzar l'experiència d'usuari, s'ha implementat una GPO que maparà la unitat de xarxa **Z:** automàticament als directius.

* **Configuració del Drive Map (Z:):**
  
![Configuració GPO](/Tasca03/img/10.png)

---

## 5. File Server Resource Manager (FSRM)

S'ha instal·lat el rol de gestió de recursos per aplicar seguretat de contingut i control d'emmagatzematge.

### 5.1. Filtratge de Fitxers

Bloqueig actiu de fitxers executables (`.exe`) a la carpeta d'Operacions per protegir el servidor de programari no autoritzat.

![Configuració Filtre](/Tasca03/img/11.png)

![Error al client en intentar copiar EXE](/Tasca03/img/12.png)

### 5.2. Gestió de Quotes

Límit rígid (Hard Quota) de 200 MB a la carpeta Public i activació de quotes de disc NTFS (500 MB per usuari).

![Configuració Quota Carpeta](/Tasca03/img/13.png)

![Error Quota al client](/Tasca03/img/14.png)

![Activació Quota Volum](/Tasca03/img/15.png)

---

## 6. Verificació de Visibilitat i ABE (Client Windows 11)

Aqui vaig fer uns usuaris i els vaig afegir a cada grup per fer les comprovacions:

![1](/Tasca03/img/16.png)

![2](/Tasca03/img/17.png)

![3](/Tasca03/img/18.png)

Proves reals que demostren que el sistema només mostra el contingut autoritzat.

Primer de tot desde la màquina client ens unirem al domini:

![19](/Tasca03/img/19.png)

* **Usuari u_trans:** Accés a Operacions i Public.
  
![Vista u_trans](/Tasca03/img/29.png)

![Accés Operacions](/Tasca03/img/30.png)

Aqui podem veure que a la carpeta de direccion no tenim permis però en canvi amb els permisos que estan posats al grup de transport si que podriem accedir a les carpetes operacions i public.

* **Usuari u_admin:** Comprovació que l'ABE amaga la resta de carpetes privades.
  
![Vista u_admin](/Tasca03/img/20.png)

![Vistin](/Tasca03/img/21.png)

![Vis_n](/Tasca03/img/22.png)

![Vta u](/Tasca03/img/23.png)

* **Usuari u_dir:** Verificació del mapatge de la unitat Z: i accés al recurs direccion.
  
![Unitat Z u_dir](/Tasca03/img/24.png)

![Accés Direccion](/Tasca03/img/25.png)

---

## 7. Estat Final dels Serveis

Resum de les consoles de gestió confirmant l'estat òptim i la finalització de la configuració.

![Estat Servidor 26](/Tasca03/img/26.png)

![Estat Servidor 27](/Tasca03/img/27.png)

![Estat Servidor 28](/Tasca03/img/28.png)

---
*Fi de la documentació tècnica.*
