# 📅 **T09: Estimació temporal de projecte (Diagrama de Gantt professional)**
**Autor:** Pol Serrano Aromí i Pau Constanseu Ros
**Data:** 20/04/2026  

---

## 1. Índex:

**1/** Índex.
**2/** Fase 1: Anàlisi real del projecte.
**3/** Fase 2: Estimació d’esforç amb criteri.
**4/** Fase 3: Assignació de recursos.
**5/** Fase 4: Construcció del diagrama de Gantt.
**6/** Fase 5: Pla de contingència.
**7/** Conclusió de la tasca.

---

## 2. Fase 1: Anàlisi real del projecte =

### 2.1 Identificació de tasques i dependències

**Ordre lògic d’execució**

T01 → T02 → T05

T06 → T08 → T09

T03 ↔ T04 (paral·lel després de T02)

T07 → T10

**Dependències clau**

T02 depèn de T01

T05 i T06 depenen de T02

T08 depèn de T02 i T06

T03 i T04 depenen de T02

T09 depèn de T01

T10 depèn de T07

**Tasques en paral·lel**

Es poden fer al mateix temps:

T03 i T04

T05 i T06

T07 pot anar en paral·lel amb T03/T04

**Tasques bloquejants**

T02 (proposta web) → bloqueja gran part del projecte

T06 (legal web) → necessari abans de publicar (T08)

**Possibles colls d’ampolla**

1- Dependència forta de T02
2- Acumulació de tasques després de T02

**Per què?**

Per què son tasques seqüencials i no tenen marge de retard, a part qualsevol retard afecta tot el projecte

---

## 3. Fase 2: Estimació d’esforç amb criteri =

### 3.1 Estimació de tasques

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
| T09   | 3h    | Planificació             |
| T10   | 3h    | Pressupost               |
| T11   | 4h    | Configuració Wordpress   |
| T12   | 7h    | Recerca d'informació     |

### 3.2 Factors tinguts en compte

El que hem tingut amb compte a sigut:

1- Temps d’anàlisi
2- Implementació tècnica
3- Errors i proves
4- Documentació
5- Coordinació
6- Imprevistos

---

## 4. Fase 3: Assignació de recursos =

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
| T09   | Responsable | Suport      |
| T10   | Suport      | Responsable |
| T11   | Act. indivi.| Act. indivi.|
| T12   | Act. indivi.| Act. indivi.|

---

## 5. Fase 4: Construcció del diagrama de Gantt =

bash

@startgantt
Project starts 2026-04-07

[T01 - Anàlisi] lasts 2 days
[T02 - Web] lasts 3 days
[T03 - Fitxers] lasts 2 days
[T04 - Impressió] lasts 2 days
[T05 - LOPD] lasts 1 days
[T06 - Legal] lasts 2 days
[T07 - Cloud] lasts 2 days
[T08 - Web final] lasts 1 days
[T09 - Gantt] lasts 3 days
[T10 - Pressupost] lasts 2 days
[T11 - WordPress]
[T12 - StartUP]

T02 starts after T01
T03 starts after T02
T04 starts after T02
T05 starts after T02
T06 starts after T02
T08 starts after T06
T09 starts after T01
T10 starts after T07

@endgantt




---

## 6. Fase 5: Pla de contingència =

---

## 7. Conclusió de la tasca =
