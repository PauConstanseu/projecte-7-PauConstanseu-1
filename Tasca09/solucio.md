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

T06 → T08

T03 ↔ T04 (paral·lel després de T02)

**Dependències clau**

T02 depèn de T01

T05 i T06 depenen de T02

T08 depèn de T02 i T06

T03 i T04 depenen de T02

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

---

## 5. Fase 4: Construcció del diagrama de Gantt =

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

[foto diagrama](/Tasca09/img/diagramagantt.png)

---

## 6. Fase 5: Pla de contingència =

### 6.1 Taula de riscos

| Risc | Part afectada | Impacte | Pla de contingència |
|------|--------------|--------|---------------------|
| Problemes en la configuració del servidor (T03) | Infraestructura | Retard en tasques dependents | 1. Afegir temps extra de proves i marge en la planificació.<br>2. Repartir la tasca entre els dos membres per resoldre errors més ràpid. |
| Errors en la web o en l’adaptació legal (T02 / T06) | Web client | Pot impedir publicar la web final | 1. Fer una revisió conjunta abans de donar la web per finalitzada.<br>2. Utilitzar una checklist legal per assegurar que es compleixen tots els requisits. |

### 6.2 Anàlisi dels riscos

Aquests dos riscos són els més importants perquè afecten directament parts clau del projecte: la infraestructura i la web final. Si fallen, poden bloquejar el projecte o retardar-lo. Per això s’han definit mesures concretes per reduir el seu impacte.

---

## 7. Conclusió de la tasca =

En aquesta tasca hem après que planificar un projecte és tan important com fer-lo. No es tracta només de fer les tasques, sinó d’organitzar-les correctament, entendre les dependències i preveure possibles problemes.

El diagrama de Gantt ens ha ajudat a visualitzar el temps del projecte, veure quines tasques es poden fer en paral·lel i identificar punts crítics.

També hem entès la importància de repartir bé el treball i coordinar-nos com a equip per evitar colls d’ampolla.

En general, considerem que la planificació és realista, tot i que sempre poden aparèixer imprevistos que obliguin a adaptar els temps.
