# 📄 Memòria Econòmica

**Autors:** Pau Constanseu i Pol Serrano 

**Data:** 4 de maig de 2026  

---

## 1. 💰 Cost d’Implantació

### 1.1 Infraestructura (Alta disponibilitat al núvol)
Es proposa una solució d'infraestructura basada en **Microsoft Azure** configurada en alta disponibilitat, que inclou els següents elements:
* **Computació:** 2 màquines virtuals (node de producció + node de rèplica).
* **Dades:** Emmagatzematge gestionat i optimitzat.
* **Seguretat:** Polítiques de còpies de seguretat (*backups*) automàtiques.

> **Cost inicial de desplegament:** 0 € (associat al model de facturació de pagament per ús del proveïdor).

### 1.2 Llicències inicials SaaS
Per al programari com a servei, s’implementa la suite **Microsoft 365 Business Standard**:
* **Abast:** 35 usuaris actius.
* **Cost inicial:** Sense cost d'alta o activació (model de subscripció mensual).

### 1.3 Mà d’obra (Tarifa: 30 € / hora)
A continuació es detalla el desglossament de la dedicació tècnica requerida per a cadascuna de les línies de treball del projecte:

| Tasca Operativa | Hores Dedicades | Cost Associat |
| :--- | :---: | :---: |
| Configuració de servidors a Azure | 20 h | 600 € |
| Alta disponibilitat i polítiques de *backups* | 15 h | 450 € |
| Migració de sistemes a Microsoft 365 | 20 h | 600 € |
| Configuració d’usuaris i serveis corporatius | 10 h | 300 € |
| Creació de vídeo formatiu en normativa LOPD | 10 h | 300 € |
| Disseny web conceptual (Experiència d'usuari UX/UI) | 15 h | 450 € |
| Desenvolupament web adaptat (Plataforma WordPress) | 20 h | 600 € |
| **Totals de Projecte** | **110 h** | **3.300 €** |

### 1.4 Total Cost d'Implantació
$$3.300 \text{ €}$$

---

## 2. 🔁 Costos Recurrents (Mensuals)

Els costos de caràcter operatiu (*OPEX*) necessaris per al manteniment i continuïtat del negoci es desglossen de la següent manera:

* **☁️ Llicències Microsoft 365:**
  * Pla Business Standard (~12 € / usuari / mes) per a 35 usuaris: **420 € / mes**.
* **🌐 Infraestructura Azure:**
  * Manteniment de 2 màquines virtuals, emmagatzematge actiu i *backups*: **150 € / mes** *(aprox.)*.
* **🖥️ Allotjament i Identitat Digital:**
  * *Hosting* web professional: **10 € / mes**.
  * Domini corporatiu: **1 € / mes** *(equivalents a 12 € / any)*.
* **🔧 Suport i Manteniment Preventiu:**
  * Inclou auditories de còpies de seguretat, aplicació d'actualitzacions crítiques i bústia de suport tècnic: **200 € / mes**.

### 2.4 Total Cost Recurrent Mensual
$$781 \text{ € / mes}$$

---

## 3. 📊 Resum Econòmic i Justificació

* **💰 Cost Inicial d'Inversió:** 3.300 €
* **🔁 Cost Fix Mensual:** 781 € / mes

### 3.1 Viabilitat de la Tarifa Horària
S’ha establert un preu de **30 € / hora**, un valor alineat amb els barems de mercat actuals per a perfils de tècnics informàtics i de sistemes de nivell mitjà a Espanya. Aquesta tarifa permet equilibrar la màxima qualitat en el lliurament del projecte amb una proposta altament competitiva.

### 3.2 Idoneïtat de Microsoft 365
La tria de la modalitat *Business Standard* respon a criteris de:
* **Integració nativa:** Unificació de serveis clau com el correu electrònic professional, Teams i emmagatzematge en el núvol amb OneDrive.
* **Disponibilitat i Escalabilitat:** Absència de servidors físics locals i flexibilitat absoluta per gestionar el volum de 35 treballadors de forma elàstica.

### 3.3 Arquitectura de Microsoft Azure
S'ha optat pel núvol d'Azure pels següents vectors tecnològics:
* Arquitectura amb tolerància a fallades gràcies a l'alta disponibilitat.
* Optimització financera mitjançant el model de pagament per ús eficient.
* Alts estàndards de seguretat de la informació i compliment normatiu.

### 3.4 Desenvolupament sobre WordPress
L'ús d'aquest gestor de continguts (CMS) com a base per al portal web aporta els següents avantatges:
* Reducció de la inversió inicial de codificació des de zero.
* Facilitat de transferència de coneixement per al manteniment diari.
* Acceleració del calendari de lliurament del projecte (*Time-to-Market*).

### 3.5 Abast del Manteniment Mensual
La partida mensual assignada al suport tècnic no és un cost estructural buit; garanteix de forma proactiva tres elements vitals: la **securització del sistema**, la **continuïtat del negoci** davant de desastres i la resolució àgil d’incidències tècniques.

---

## ✅ Conclusió

La present proposta econòmica ofereix a l'organització una solució tecnològica d'alt nivell que esdevé completament **escalable**, **segura** i **financerament viable**, minimitzant els costos d'inversió inicial (*CAPEX*) i assegurant un control rigorós de la despesa corrent.
