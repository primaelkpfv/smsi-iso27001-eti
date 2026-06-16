# SMSI Complet ISO 27001 — ETI 200 Collaborateurs

![Status](https://img.shields.io/badge/Status-Complet-success)
![ISO](https://img.shields.io/badge/Norme-ISO%2027001%3A2022-blue)
![EBIOS](https://img.shields.io/badge/Methode-EBIOS%20Risk%20Manager-orange)
![Note](https://img.shields.io/badge/Note%20jury-17%2F20-brightgreen)

Conception d'un Systeme de Management de la Securite de l'Information (SMSI) complet pour une ETI fictive de 200 collaborateurs, conforme ISO 27001:2022. Analyse de risques EBIOS RM (5 ateliers), Declaration d'Applicabilite (93 controles), PCA/DRP et KPIs RSSI.

---

## Contexte du Projet

**Entreprise fictive**: TechCorp SA — 200 collaborateurs, secteur fintech, 3 sites (Paris, Lyon, Bordeaux)

**Perimetre SMSI**:
- Systemes d'information financiers
- Donnees clients et transactions
- Infrastructure IT et cloud (AWS)
- Processus metiers critiques

---

## Livrables Produits

| Livrable | Statut | Description |
|----------|--------|-------------|
| Politique de Securite | Valide | Document cadre SSI — Direction |
| Analyse de risques EBIOS RM | Complet | 5 ateliers, 47 scenarios de risque |
| Declaration d'Applicabilite | Complet | 93 controles ISO 27001 Annexe A |
| Plan de Traitement des Risques | Complet | 23 mesures prioritaires |
| PCA/DRP | Complet | RTO 4h, RPO 1h — systemes critiques |
| Tableau de bord KPIs RSSI | Complet | 15 indicateurs mensuels |

**Note jury : 17/20**

---

## EBIOS Risk Manager — 5 Ateliers

### Atelier 1 — Cadrage et Socle de Securite
- Perimetre: SI financier + donnees clients
- Valeurs metiers: traitement transactions, gestion comptes, reporting
- Biens supports: serveurs applicatifs, BDD Oracle, VPN, AD
- **Ecart socle**: 34 ecarts identifies (hygiene numerique ANSSI)

### Atelier 2 — Sources de Risque
| Source | Motivation | Capacite |
|--------|-----------|---------|
| Cybercriminels (ransomware) | Gain financier | Elevee |
| Concurrent malveillant | Espionnage | Moyenne |
| Employe malveillant | Sabotage/revanche | Faible |
| Etat etranger | Intelligence economique | Tres elevee |

### Atelier 3 — Scenarios Strategiques
- 12 scenarios strategiques identifies
- Chemins d'attaque modélises sur graphe de dependances
- Scenarios prioritaires: ransomware SI financier, exfiltration BDD clients

### Atelier 4 — Scenarios Operationnels
- 47 scenarios operationnels detailles
- Evaluation vraisemblance x gravite (matrice 4x4)
- 8 risques inacceptables identifies

### Atelier 5 — Traitement du Risque
- 23 mesures de securite definies
- Risque residuel apres traitement: acceptable pour 44/47 scenarios
- 3 risques residuels acceptes par la Direction

---

## Declaration d'Applicabilite

93 controles ISO 27001:2022 Annexe A evalues :

```
Domaine A.5  — Politiques de securite          : 2/2   appliques
Domaine A.6  — Organisation de la securite     : 8/8   appliques
Domaine A.7  — Securite des RH                : 6/6   appliques
Domaine A.8  — Gestion des actifs             : 10/10 appliques
Domaine A.9  — Controle d'acces              : 14/14 appliques
Domaine A.10 — Cryptographie                 : 2/2   appliques
Domaine A.11 — Securite physique             : 15/15 appliques
Domaine A.12 — Securite exploitation         : 14/14 appliques
Domaine A.13 — Securite communications       : 7/7   appliques
Domaine A.14 — Acquisition/dev systemes      : 13/13 appliques
Domaine A.15 — Relations fournisseurs        : 5/5   appliques
Domaine A.16 — Gestion incidents             : 7/7   appliques
Domaine A.17 — PCA                           : 4/4   appliques
Domaine A.18 — Conformite                    : 8/8   appliques
```

---

## KPIs RSSI — Tableau de Bord

```
Indicateur                          Cible    Actuel   Statut
─────────────────────────────────────────────────────────────
Taux patching critique (30j)        100%     98%      VERT
Incidents securite/mois             <5       3        VERT
MTTD (detection incidents)          <2h      1h45     VERT
MTTR (resolution incidents)         <24h     18h      VERT
Taux formation SSI employes         >95%     91%      ORANGE
Disponibilite SI critique           >99.5%   99.8%    VERT
Comptes privileges audites          100%     96%      ORANGE
Sauvegardes testees/trimestre       100%     100%     VERT
Vulns critiques ouvertes >30j       0        1        ROUGE
Score hygiene ANSSI                 >80%     76%      ORANGE
```

---

## PCA/DRP — Objectifs de Reprise

| Systeme | Criticite | RTO | RPO | Solution |
|---------|-----------|-----|-----|---------|
| SI Transactions | Critique | 1h | 15min | Hot standby AWS |
| BDD Clients | Critique | 2h | 1h | Replication sync |
| Messagerie | Haute | 4h | 4h | Cloud backup |
| Intranet | Normale | 8h | 24h | Sauvegarde quotidienne |
| Postes dev | Basse | 48h | 24h | Image systeme |

---

## Structure du Projet

```
smsi-iso27001-eti/
├── README.md
├── 01-politique-securite/
│   └── PSSI-TechCorp-v1.0.md
├── 02-ebios-rm/
│   ├── atelier1-cadrage.md
│   ├── atelier2-sources-risque.md
│   ├── atelier3-scenarios-strategiques.md
│   ├── atelier4-scenarios-operationnels.md
│   └── atelier5-traitement-risque.md
├── 03-declaration-applicabilite/
│   └── DdA-ISO27001-TechCorp.xlsx  (93 controles)
├── 04-plan-traitement-risques/
│   └── PTR-TechCorp-v1.0.md
├── 05-pca-drp/
│   └── PCA-DRP-TechCorp.md
├── 06-kpis-rssi/
│   └── tableau-bord-kpis.md
└── docs/
    └── rapport-jury.md
```

---

## References

- [ISO 27001:2022](https://www.iso.org/standard/27001)
- [EBIOS Risk Manager - ANSSI](https://www.ssi.gouv.fr/guide/ebios-risk-manager/)
- [CIS Controls v8](https://www.cisecurity.org/controls/v8)
- [Portfolio](https://primaelkpfv.github.io)

---
*Projet Bachelor Cybersecurite - ESAIP 2025 | Note jury : 17/20*
