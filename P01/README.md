# 📜 P01: Memòria tècnica de la proposta

- **Autors:** Pau Constanseu i Pol Serrano
- **Data:** 04/05/2026

---

## 📚 1. Índex:

- **1/** Índex.
- **2/** Introducció a la tasca.
- **3/** Anàlisi de necessitats.
- **4/** Proposta de la solució.
- **5/** Arquitectura i disseny tècnic.
- **6/** Pressupost.
- **7/** Planificació.
- **8/** Conclusió Final.

---

## ⚙️ 2. Introducció a la tasca:

En aquesta tasca es desenvolupa la memòria tècnica de la proposta de solució per a l’empresa FoodLogístic S.A., amb l’objectiu de presentar de manera clara, estructurada i professional totes les decisions tècniques del projecte. Aquest document permet al client entendre el funcionament de la proposta, avaluar-ne la viabilitat i prendre decisions informades abans de la seva implementació.

La memòria integra tant la descripció dels sistemes com la seva representació visual mitjançant diagrames, taules i evidències gràfiques, seguint criteris professionals de documentació. Així, no només es mostra què s’ha desenvolupat, sinó també com i per què s’han pres determinades decisions, demostrant la capacitat de planificar, justificar i comunicar una solució tecnològica completa.

---

## 🌐 3. Anàlisi de necessitats

L’empresa FoodLogístic S.A. es troba en una fase de creixement i expansió que ha posat en evidència diverses limitacions en la seva infraestructura tecnològica actual. Aquest escenari genera la necessitat d’implementar solucions que garanteixin la continuïtat del negoci, la seguretat de la informació i una millora en la productivitat dels treballadors.

En primer lloc, a nivell d’infraestructura, es detecta una manca d’alta disponibilitat en serveis crítics com el servidor de fitxers i el sistema d’impressió. Aquesta situació pot provocar interrupcions en les operacions diàries, especialment en entorns logístics on l’accés constant a documents i la impressió d’etiquetes són essencials. Per tant, és necessari assegurar sistemes redundants i fiables que evitin parades del servei.

En segon lloc, pel que fa a la comunicació interna, el sistema de correu actual presenta problemes de fiabilitat. Això afecta directament la coordinació entre departaments i pot generar pèrdua d’informació. Es fa imprescindible migrar cap a una solució al núvol que ofereixi estabilitat, accessibilitat i eines col·laboratives que millorin el treball en equip.

A nivell de seguretat, l’empresa mostra preocupació pel tractament de dades personals, especialment amb l’augment de la plantilla. És necessari garantir el compliment de la normativa vigent (LOPD), així com formar els treballadors en bones pràctiques per evitar riscos legals i de seguretat.

Finalment, la presència web actual de l’empresa no compleix amb els estàndards moderns ni amb la normativa legal, fet que pot afectar la seva imatge corporativa i generar possibles sancions. Es requereix una nova pàgina web funcional, actualitzada i adaptada a la legislació, que permeti establir un canal de comunicació directe amb clients potencials.

---

## 👌 4. Proposta de solució

### 🖥️ 4.1 Infraestructura i alta disponibilitat

#### 4.1.1 = Recerca de empreses =

1- [Sistemas Informátics del Maresme (SIMA)](https://simaresme.com/contacte.html)

- **Ubicació:** Maresme  
- **Mida:** PIME  
- **Serveis:**
  - Sistemes i servidors  
  - Xarxes  
  - Suport IT  
  - Solucions cloud  
- **Perfil:** Empresa tècnica orientada a empreses locals amb necessitats d’infraestructura i manteniment

2- [Microsistemes](https://shop.rsmicro.es/)

- **Ubicació:** Premià de Mar / seu a Sabadell
- **Mida:** Microempresa / PIME petita  
- **Serveis:**
  - Manteniment informàtic  
  - Xarxes  
  - Suport tècnic  
  - Venda d’equipament  
- **Perfil:** Empresa local enfocada a petites i mitjanes empreses

3- [TecnoMaresme](https://maresmetecnic.com/)

- **Ubicació:** Maresme  
- **Mida:** Microempresa  
- **Serveis:**
  - Reparació d’equips  
  - Manteniment IT  
  - Suport tècnic  
- **Perfil:** Servei molt proper, orientat a clients petits i amb pressupost ajustat

#### 4.1.2 Organigrama:

A continuació us mostrem un model d’organigrama per a una empresa de serveis informàtics com és el cas de FooLogístic S.A:

```bash

@startuml
title Organigrama empresa serveis informàtics

* Direcció General
** Departament Tècnic
*** Sistemes
*** Xarxes
*** Ciberseguretat
** Suport / Helpdesk
*** Tècnics nivell 1
*** Tècnics nivell 2
** Departament Comercial
*** Vendes
*** Màrqueting
** Administració
*** Comptabilitat
*** Recursos Humans

@enduml

```

Aquest organigrama l'hem volgut representar com una estructura funcional típica en empreses del sector de distribució alimentària.

#### 4.1.3: Radiografia de departaments

👨‍💼 **Direcció General:** S’encarrega de la definició de l’estratègia empresarial, la presa de decisions i la coordinació global de l’organització.

🖥️ **Departament Tècnic:** Instal·lació i configuració de servidors, la gestió de xarxes, la implementació de solucions cloud i la ciberseguretat.

🛠️ **Suport / Helpdesk:** Gestiona la resolució d’incidències, dona assistència als usuaris i realitza tasques de manteniment preventiu.

🌐 **Departament Comercial:** S’ocupa de la captació de nous clients, l’elaboració de pressupostos i el seguiment comercial.

#### 4.1.4 = Proposta de valor

La nostra empresa es posicionarà amb els següents valors diferencials:

- **Proximitat:** Som una empresa local, cosa que ens permet oferir un tracte directe i ràpid.
- **Rapidesa de resposta:** Assistència remota immediata i intervencions ràpides en cas d’incidència.
- **Seguretat i continuïtat:**
- **Especialització en:**
  - Alta disponibilitat
  - Protecció de dades
  - Compliment normatiu

#### 4.1.5 = Recursos necessaris

Per donar servei a **FoodLogístic S.A.** es considera necessari el següent equip:

- Administrador de sistemes
- Tècnic de suport
- Especialista en solucions cloud
- Comercial / gestor de client

### 4.2 Serveis al núvol

S’han estudiat quatre proveïdors principals de correu corporatiu:

- Microsoft 365 Business  
- Google Workspace  
- Zoho Workplace  
- Lark Suite  

#### 4.2.1 = Comparativa de característiques

#### 4.2.1.1 = Descripció de cada servei

**Microsoft 365 Business:** Incorpora Outlook, OneDrive, Teams i tota la suite Office. Destaca per la seguretat i el control.

**Google Workspace:** Suite molt coneguda i intuïtiva, amb Gmail, Drive, Meet i Docs. Excel·lent per a col·laboració en temps real.

**Zoho Workplace:** Econòmica i completa, amb correu, eines d’ofimàtica i integració amb CRM.

**Lark Suite:** Plataforma moderna amb xat, calendari i documents integrats. Molt orientada a col·laboració, però poc estesa a Europa.

#### 4.2.1.2 = Taula comparativa

| Característica        | Microsoft 365     | Google Workspace   | Zoho            | Lark Suite        |
|----------------------|------------------|--------------------|-----------------|-------------------|
| Tipus                | Business Basic   | Business Starter   | Standard        | Enterprise Starter|
| Preu/usuari/mes      | 5€               | 7€                 | 3€              | 7€                |
| Emmag. correu        | 50 GB            | 30 GB              | 30 GB           | 30 GB             |
| Emmag. núvol         | 1 TB             | 30 GB              | 100 GB          | 5 TB              |
| Eines                | Teams, Office... | Meet, Docs, Sheets | Zoho Docs, Cliq | Docs, Chat, Meetings |
| Seguretat            | MFA, control avançat i compliment normatiu | IA AntiSpam, protecció phishing | MFA i filtres antispam | MFA i xifratge |

#### 4.2.2 = Càlcul de costos i implementació

Després de comparar funcionalitats, seguretat i cost, la millor opció per a **FoodLogistic** és: Microsoft 365 Business Basic

**Raons:**
- Seguretat empresarial robusta  
- Integració amb eines d’ofimàtica (Word, Excel, PowerPoint)  
- 1 TB d’emmagatzematge per usuari  
- Control administratiu avançat  

**Preu:** 5€/usuari/mes  

Càlcul:

- 5€ × 35 empleats = **175€ / mes**  
- 175€ × 12 mesos = **2.100€ / any**  

Eines de migració: Microsoft ofereix eines oficials per migrar correus des de serveis IMAP:

- Microsoft Exchange Online Migration Tool  
- IMAP Migration Wizard  
- Eina de migració de Google Workspace a Microsoft 365  

Aquestes eines permeten migrar:

- Missatges  
- Carpetes  
- Contactes  
- Calendari  

### 🔐 4.3 Seguretat i LOPD

En aquesta activitat s’ha treballat la creació de materials audiovisuals per a la campanya interna de FoodLogistic S.A., sota el lema “Dades Segures, Logística Eficient”. L’objectiu principal és conscienciar els treballadors sobre la importància de protegir les dades personals en el seu dia a dia dins l’empresa 🔐.

Us deixem els enllaços als guions i vídeos sobre l'integració de la seguretat als treballadors de TransLogistic i LOPD:

- Enllaç guió vídeo 1: [Aquí](https://github.com/classesSMX2n/projecte-7-polserrano/blob/main/Tasca_05/guio1.md)
- Enllaç guió vídeo 2: [Aquí](https://github.com/classesSMX2n/projecte-7-polserrano/blob/main/Tasca_05/guio2.md)
- Enllaç al vídeo 1: [Aquí](https://youtu.be/ErjS40srjOg)
- Enllaç al vídeo 2: [Aquí](https://www.youtube.com/watch?v=o5fob59rfgI)

---

## 🧰 5. Arquitectura i disseny tècnic:

Aquí us adjutem el enllaç de la pàgina web corporativa d'en Pau Constanseu i en Pol Serrano: [Aqui](https://classessmx2n.github.io/web-projecte7-PauConstanseu/). Seguidament us adjuntem també imatges de la pàgina.

![foto 1 web](/P01/img/web1.png)
![foto 2 web](/P01/img/web2.png)
![foto 3 web](/P01/img/web3.png)

Aquesta pàgina web va ser la definitiva, ja que vam volguer fusionar les dues pàgines webs individuals, ja que consideravem que ambdues webs tenien coses dolentes i bones, i descarta una web estariem descartant coses bones de l'altre, aqui us compartim les altres pàgines individuals:

- Pàgina de Pau Constanseu: [Aquí](https://pauconstanseu.github.io/web-corporativa/)
- Pàgina de Pol Serrano: [Aquí](https://polserrano.github.io/web-corporativa/)

Vam considerar que l'aspecte de la pàgina d'en Pau era més intuïtiu i més enfocat cap al tema de l'empresa. En canvi la part de les cookies i el peu de pàgina la informació que contenia la part d'en Pol era millor ja hi había més.

---

## 💵 6. Pressupost:

### 6.1 = Infraestructura (Alta disponibilitat al núvol):

Es proposa una solució basada en Microsoft Azure amb alta disponibilitat:

- 2 màquines virtuals (producció + rèplica)
- Emmagatzematge gestionat
- Còpies de seguretat automàtiques

**Cost inicial:**  
- Configuració inicial: **0 €** (model de pagament per ús)

### 6.2 = Llicències inicials SaaS:

S’implementa Microsoft 365 Business Standard:

- 35 usuaris  
- Sense cost inicial (subscripció mensual)

### 6.3 = Mà d’obra (30 €/hora):

| Tasca | Hores | Cost |
|------|------|------|
| Configuració servidors Azure | 20 h | 600 € |
| Alta disponibilitat i backups | 15 h | 450 € |
| Migració a Microsoft 365 | 20 h | 600 € |
| Configuració d’usuaris i serveis | 10 h | 300 € |
| Creació vídeo formatiu LOPD | 10 h | 300 € |
| Disseny web (UX/UI) | 15 h | 450 € |
| Desenvolupament web (WordPress) | 20 h | 600 € |

**Total hores:** 110 h  
**Total mà d’obra:** **3.300 €**

### 6.4 = TOTAL IMPLANTACIÓ:

**3.300 €**

### 6.5 = Costos recurrents (mensuals):

### Microsoft 365
- Pla Business Standard: ~12 €/usuari/mes  
- 35 usuaris:

**420 €/mes**

### 6.6 = Infraestructura Azure:

- 2 màquines virtuals + emmagatzematge + backups:

**150 €/mes (aprox.)**

### 6.7 = Hosting i domini:

- Hosting web professional:

**10 €/mes**

- Domini:

**1 €/mes (12 €/any)**

### 6.8 = Suport i manteniment:
Inclou:
- Còpies de seguretat
- Actualitzacions
- Suport tècnic

**200 €/mes**

### 6.9 = TOTAL MENSUAL:

**781 €/mes**

### 6.10 = Resum econòmic:

- Cost inicial: **3.300 €**
- Cost mensual: **781 €/mes**

### 6.11 = Preu per hora:

S’ha establert un cost de **30 €/hora**, d’acord amb el mercat per a tècnics informàtics de nivell mitjà a Espanya, equilibrant qualitat i competitivitat.

### 6.12 = Elecció de Microsoft 365:

S’ha escollit Microsoft 365 Business Standard per:
- Integració completa (correu, Teams, OneDrive)
- Alta disponibilitat
- Escalabilitat per a 35 treballadors

### 6.13 = Ús de Microsoft Azure:

S’ha optat per Azure per:
- Alta disponibilitat
- Model de pagament per ús
- Elevat nivell de seguretat

### 6.14 = Desenvolupament web amb WordPress:

WordPress permet:
- Reduir costos
- Facilitar el manteniment
- Accelerar el desenvolupament

### 6.15 = Manteniment mensual:

El servei inclou tasques essencials per garantir:
- Seguretat
- Continuïtat del negoci
- Resolució d’incidències

---

## 🗺️ 7. Planificació:

### 7.1 = Identificació de tasques i dependències

L’ordre lògic d’execució del projecte segueix principalment la seqüència T01 → T02 → T05, mentre que en paral·lel també es desenvolupa la cadena T06 → T08. A més, un cop finalitzada T02, les tasques T03 i T04 es poden executar simultàniament.

Pel que fa a dependències, T02 depèn de T01, i tant T05 com T06 depenen de T02. La tasca T08 necessita que estiguin completades T02 i T06, mentre que T03 i T04 també depenen de T02 per iniciar-se.

Algunes tasques es poden realitzar en paral·lel per optimitzar el temps, com ara T03 amb T04, T05 amb T06, i també T07, que es pot desenvolupar al mateix temps que T03 i T04.

Hi ha, però, tasques bloquejants importants: T02 (proposta web) condiciona gran part del projecte, i T06 (legal web) és imprescindible abans de poder arribar a T08 (publicació).

Finalment, es detecten possibles colls d’ampolla, sobretot per la forta dependència de T02 i per l’acumulació de tasques que es generen un cop aquesta finalitza. Això passa perquè són processos seqüencials amb poc marge de retard, de manera que qualsevol incidència pot afectar directament el conjunt del projecte.

- **Per què?**

Per què son tasques seqüencials i no tenen marge de retard, a part qualsevol retard afecta tot el projecte

---

### 7.2 = Fase 2: Estimació d’esforç amb criteri =

### 7.2.1 Estimació de tasques

| Tasca | Hores | Justificació             |
| ----- | ----- | ------------------------ |
| T01   | 3h    | Recerca i anàlisi        |
| T02   | 3h    | Disseny i estructura web |
| T03   | 8h    | Configuració servidor    |
| T04   | 4h    | Configuració impressió   |
| T05   | 3h    | Creació vídeo            |
| T06   | 3h    | Adaptació legal          |
| T07   | 4h    | Migració cloud           |
| T08   | 3h    | Decisió final            |

---

### 7.2.2 = Fase 3: Assignació de recursos + diagrama de Gantt =

| Tasca |   Pol S.    |   Pau C.    |
| ----- | ----------- | ----------- |
| T01   | Responsable | Suport      |
| T02   | Act. indivi.| Act indivi. |
| T03   | Act. indivi.| Act. indivi.|
| T04   | Act. indivi.| Act. indivi.|
| T05   | Suport      | Responsable |
| T06   | Act. indivi.| Act. indivi.|
| T07   | Responsable | Suport      |
| T08   | Act. indivi.| Act. indivi.|

```bash

@startgantt
Project starts 2026-04-07

[Recerca i anàlisi] as [T01] starts 2026-04-07 and ends 2026-04-07
[Disseny web] as [T02] starts 2026-04-07 and ends 2026-04-10
[Creació vídeo] as [T05] starts 2026-04-13 and ends 2026-04-14

[T02] starts at [T01]'s end
[T05] starts at [T02]'s end

[Configuració servidor] as [T03] starts 2026-04-08 and ends 2026-04-09
[Configuració impressió] as [T04] starts 2026-04-10 and ends 2026-04-10

[T03] starts at [T02]'s start
[T04] starts at [T03]'s end

[Migració cloud] as [T07] starts 2026-04-09 and ends 2026-04-09

[Adaptació legal] as [T06] starts 2026-04-21 and ends 2026-04-21
[Decisió final] as [T08] starts 2026-04-27 and ends 2026-04-28

[T08] starts at [T06]'s end

[T01] is colored in LightBlue/Blue
[T02] is colored in LightBlue/Blue
[T05] is colored in LightBlue/Blue

[T03] is colored in LightGreen/Green
[T04] is colored in LightGreen/Green
[T07] is colored in LightGreen/Green

[T06] is colored in Orange/Red
[T08] is colored in Orange/Red

@endgantt

```

A la següent imatge podeu veure com ens a quedat finalment el diagrama de gantt que hem realitzat:

![foto diagrama](/Tasca09/img/diagramagantt.png)

---

### 7.3 = Fase 5: Pla de contingència =

| Risc | Part afectada | Impacte | Pla de contingència |
|------|--------------|--------|---------------------|
| Problemes en la configuració del servidor (T03) | Infraestructura | Retard en tasques dependents | 1. Afegir temps extra de proves i marge en la planificació.<br>2. Repartir la tasca entre els dos membres per resoldre errors més ràpid. |
| Errors en la web o en l’adaptació legal (T02 / T06) | Web client | Pot impedir publicar la web final | 1. Fer una revisió conjunta abans de donar la web per finalitzada.<br>2. Utilitzar una checklist legal per assegurar que es compleixen tots els requisits. |

Aquests dos riscos són els més importants perquè afecten directament parts clau del projecte: la infraestructura i la web final. Si fallen, poden bloquejar el projecte o retardar-lo. Per això s’han definit mesures concretes per reduir el seu impacte.

---

## 👋 8. Conclusió Final:

Amb la realització d’aquesta memòria tècnica s’ha definit i justificat una proposta completa de solució per a FoodLogístic S.A., integrant tots els elements clau del projecte: infraestructura, serveis al núvol, seguretat, presència web, planificació i pressupost. El document reflecteix una visió global i coherent del sistema, mostrant com cada decisió tècnica respon a les necessitats reals del client i contribueix a construir una solució eficient, segura i escalable.

A més, l’ús d’elements visuals, estructures clares i documentació detallada ha permès facilitar la comprensió del projecte i millorar la seva presentació professional. Aquesta memòria no només valida la viabilitat de la proposta, sinó que també demostra la capacitat de l’equip per analitzar, planificar i comunicar solucions tecnològiques en un entorn real, establint una base sòlida per a la seva futura implementació.

---

### GRÀCIES PER LA VOSTRA ATENCIÓ!
- [Tornar Enrere](./.)
