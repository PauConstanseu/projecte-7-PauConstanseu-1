# 🚀 Implementació d'Infraestructura de Fitxers: FoodLogistic

## 📌 Introducció
En entorns corporatius on el volum de negoci creix de manera exponencial, la gestió de la informació esdevé un factor crític. **FoodLogistic** ha presentat dificultats derivades de la compartimentació de dades, on cada departament gestionava la documentació de forma local, impedint una visió global i segura de la situació empresarial.

Aquest projecte neix de la necessitat de centralitzar, organitzar i protegir els actius digitals de l'empresa mitjançant la implementació d'una infraestructura de fitxers segura, organitzada i amb control d'espai sota **Windows Server**.

## 🎯 Objectius del Projecte
L'objectiu principal és desplegar un entorn de dades que garanteixi la confidencialitat i l'eficiència mitjançant:
* **Seguretat jeràrquica:** Establiment de permisos NTFS i SMB basats en rols d'Active Directory.
* **Eficiència administrativa:** Demostració de competència en les tres vies de gestió (Explorador de fitxers, Server Manager i PowerShell).
* **Control d'emmagatzematge:** Implementació de quotes i polítiques de filtratge (FSRM) per evitar l'ús indegut dels recursos del servidor.

---

## 🛠️ Resum de la Configuració

A continuació es detalla l'estructura de recursos compartits implementada:

| Carpeta | Camí UNC | Grups amb Accés | Mètode de Creació | Característiques Especials |
| :--- | :--- | :--- | :--- | :--- |
| **Public** | `\\SRV\Public` | Tothom (Everyone) | Explorador de Fitxers | Quota 200MB (Hard) |
| **Operacions** | `\\SRV\Operacions` | Transport | Server Manager (FSSM) | Access-Based Enumeration (ABE) |
| **Confidencial** | `\\SRV\Direccio$` | Direccio | PowerShell Avançat | Recurs Ocult / Unitat Z: per GPO |

---

## 🏗️ Fites del Projecte

1.  **Preparació d'Active Directory (AD):** Disseny d'una estructura d'Unitats Organitzatives (OU) coherent i creació dels grups de seguretat (`Administracio`, `Transport`, `Direccio`).
2.  **Implementació de Recursos Compartits:** Configuració de carpetes utilitzant mètodes gràfics i de línia de comandes, assegurant el desplegament automàtic de unitats de xarxa per als directius.
3.  **Control d'Emmagatzematge (FSRM i Quotes):**
    * Limitació d'espai per volum a nivell de sistema de fitxers (NTFS).
    * Gestió de quotes de carpeta amb alertes personalitzades.
    * Bloqueig de fitxers prohibits (executables i multimèdia) per mantenir la integritat del servidor.
4.  **Verificació i Auditoria:** Proves de camp des de clients Windows 10/11 per validar els permisos efectius i el funcionament del filtratge actiu de fitxers.

---

> **Nota del Consultor:** Aquesta implementació s'ha realitzat seguint les millors pràctiques d'administració de sistemes, garantint que la informació de FoodLogistic estigui disponible només per a qui correspon i protegida contra l'esgotament de recursos.
