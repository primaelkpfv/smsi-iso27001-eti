# 📋 SMSI Complet — ISO 27001:2022 pour ETI 200 collaborateurs

[![Repo Badge](https://img.shields.io/badge/GitHub-GRC-green?logo=github&style=flat-square)](https://github.com/primaelkpfv/smsi-iso27001-eti)
[![Standard](https://img.shields.io/badge/Standard-ISO%2027001%3A2022-blue?style=flat-square)](.)
[![Note Jury](https://img.shields.io/badge/Note%20Jury-17%2F20-gold?style=flat-square)](.)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen?style=flat-square)](.)

> Système de Management Sécurité Information complet incluant EBIOS RM (5 ateliers), Déclaration d'Applicabilité (93 contrôles), PCA/DRP et tableau de bord KPIs RSSI. **Note jury : 17/20**

---

## 🎯 Résumé exécutif

<details open>
<summary><b>📊 Dashboard de conformité</b> — Vue d'ensemble ISO 27001</summary>

```
┌──────────────────────────────────────────────────────────┐
│     SMSI — TechCorp SA — Tableau de bord conformité     │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  📋 Contrôles ISO 27001:2022                           │
│  ├─ Total applicables    : 93                           │
│  ├─ Mis en œuvre ✓       : 71 (76%)                    │
│  ├─ En cours 🔄          : 19 (20%)                    │
│  └─ Non applicable ✗     : 3 (4%)                      │
│                                                          │
│  ⚠️  Analyse de risques EBIOS                           │
│  ├─ Scénarios critiques  : 3                           │
│  ├─ Mesures correctives  : 12                          │
│  ├─ Budget 2 ans         : 180 000 €                    │
│  └─ ROI risque réduit    : 68%                         │
│                                                          │
│  🔐 Indicateurs clés (KPIs)                           │
│  ├─ Taux patching        : 87% (cible 95%) 🟡         │
│  ├─ MFA privilégiés      : 100% (cible 100%) 🟢       │
│  ├─ Disponibilité SI     : 99.8% (cible 99.5%) 🟢     │
│  └─ Vulnérabilités ouv.  : 2 critiques (cible 0) 🔴   │
│                                                          │
│  💾 Plans de continuité                                 │
│  ├─ RTO datacenter       : 4h                          │
│  ├─ RPO données          : 1h                          │
│  ├─ Tests PCA            : Trimestriels ✓             │
│  └─ Dernier test         : 2024-11-15 RÉUSSI         │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

</details>

---

## 🏛️ EBIOS Risk Manager — 5 Ateliers

```
┌─────────────────────────────────────────────────────────┐
│          EBIOS RM Methodology (5 ATELIERS)             │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  ATELIER 1️⃣  — Cadrage & Socle sécurité              │
│  ├─ Périmètre SMSI défini
│  ├─ Valeurs métier identifiées (RH, Comptable, API)
│  └─ Socle évalué : 62% bonnes pratiques
│
│  ATELIER 2️⃣  — Sources de risques                   │
│  ├─ Cybercriminels (motivation : gain)
│  ├─ Concurrents (espionnage industriel)
│  ├─ Initiés malveillants (vengeance)
│  └─ États étrangers (espionnage)
│
│  ATELIER 3️⃣  — Scénarios stratégiques              │
│  ├─ Compromission plateforme client (Web exploit)
│  ├─ Ransomware SI interne (phishing)
│  ├─ Fuite données RH (initié malveillant)
│  └─ DDoS infrastructure cloud
│
│  ATELIER 4️⃣  — Scénarios opérationnels             │
│  Criblage des risques par probabilité/impact :
│  ├─ 🔴 CRITIQUE : Ransomware phishing (4/4 × 4/4)
│  ├─ 🟠 ÉLEVÉ    : Fuite RH (3/4 × 4/4)
│  └─ 🟡 MOYEN    : Exploit API (3/4 × 3/4)
│
│  ATELIER 5️⃣  — Plan de traitement                 │
│  12 mesures de sécurité priorisées :
│  ├─ Sensibilisation phishing (budget : 5k€)
│  ├─ EDR déploiement (budget : 40k€)
│  ├─ MFA généralisation (budget : 15k€)
│  └─ Audit de sécurité (budget : 25k€)
│
└─────────────────────────────────────────────────────────┘
```

---

## 📁 Structure

```
smsi-iso27001-eti/
├── 01-cadrage/
│   ├── périmètre-smsi.md
│   └─- contexte-organisation.md
├── 02-ebios-rm/
│   ├── atelier1-cadrage.md ✓
│   ├── atelier2-sources-risques.md ✓
│   ├── atelier3-scenarios-strategiques.md ✓
│   ├── atelier4-scenarios-operationnels.md ✓
│   └── atelier5-traitement-risques.md ✓
├── 03-declaration-applicabilite/
│   └── dda-iso27001-2022.md (93 contrôles)
├── 04-politiques/
│   ├── PSSI.md
│   ├── politique-classification.md
│   └── policy-access-control.md
├── 05-pca-pra/
│   ├── plan-continuite-activite.md
│   ├── plan-reprise-activite.md
│   └── tests-pca-resultats.md
└── 06-kpis-rssi/
    └── tableau-bord-kpis.md (15 indicateurs)
```

---

## ✅ Résultats & Certification

| Élément | Status |
|---------|--------|
| **Analyse EBIOS** | ✅ Complète (5 ateliers) |
| **DdA 93 contrôles** | ✅ Documentée (76% appliquée) |
| **Politiques PSSI** | ✅ Validée direction |
| **PCA/DRP** | ✅ Testes trimestriels |
| **Formation sensibilisation** | ✅ 200/200 collaborateurs |
| **Audit de sécurité** | ✅ 0 criticité en production |
| **Certification ISO 27001** | ⏳ Audit prévu Q1 2025 |

---

## 🔗 Ressources

- 📚 [ISO 27001:2022 Standard](https://www.iso.org/standard/27001)
- 📚 [EBIOS RM - ANSSI](https://www.ssi.gouv.fr/entreprise/management-du-risque/la-methode-ebios-risk-manager/)
- 📚 [CNIL - Conformité RGPD](https://www.cnil.fr/)

---

<p align="center">
  <b>Made with 📋 for Information Security Management</b>
</p>
