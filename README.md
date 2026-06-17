# 📋 SMSI Complet — ISO 27001 pour une ETI de 200 collaborateurs

![Status](https://img.shields.io/badge/Status-Terminé-brightgreen)
![Note](https://img.shields.io/badge/Note%20jury-17%2F20-gold)
![Standard](https://img.shields.io/badge/Standard-ISO%2027001%3A2022-blue)
![Category](https://img.shields.io/badge/Catégorie-GRC%20·%20Conformité-green)

> Conception complète dun Système de Management de la Sécurité de lInformation (SMSI) pour une ETI fictive de 200 collaborateurs, selon ISO 27001:2022. Note jury : 17/20.

## 🎯 Contexte du projet

**Société fictive** : TechCorp SA — ETI spécialisée en services numériques  
**Secteur** : ESN (Entreprise de Services du Numérique)  
**Taille** : 200 collaborateurs, 3 sites (Paris, Lyon, Bordeaux)  
**Enjeux** : Certification ISO 27001, conformité RGPD, appels doffres publics

## 📦 Livrables produits

| Livrable | Description | Statut |
|----------|-------------|--------|
| Analyse de risques EBIOS RM | 5 ateliers complets | ✅ |
| Déclaration dApplicabilité (DdA) | 93 contrôles ISO 27001:2022 | ✅ |
| Plan de Traitement des Risques (PTR) | Priorisation et budget | ✅ |
| PCA / Plan de Reprise dActivité | RTO/RPO définis | ✅ |
| Tableau de bord KPIs RSSI | 15 indicateurs clés | ✅ |
| Politique de Sécurité (PSSI) | Document validé direction | ✅ |
| Procédures opérationnelles | 8 procédures documentées | ✅ |

## 🔍 Analyse de risques — EBIOS Risk Manager

### Atelier 1 — Cadrage et socle de sécurité
- Définition du périmètre SMSI
- Identification des valeurs métier : SI RH, SI Comptable, Plateforme client, Messagerie
- Évaluation du socle de sécurité (62 % des bonnes pratiques appliquées)

### Atelier 2 — Sources de risques
| Source de risque | Motivation | Niveau de menace |
|-----------------|------------|-----------------|
| Cybercriminels | Gain financier | Très élevé |
| Concurrent | Espionnage industriel | Élevé |
| Initié malveillant | Vengeance / profit | Moyen |
| Script kiddie | Notoriété | Faible |
| État étranger | Espionnage | Faible |

### Atelier 3 — Scénarios stratégiques
- Compromission de la plateforme client via vulnérabilité web
- Ransomware sur SI interne via phishing
- Fuite de données RH par initié malveillant
- Déni de service sur infrastructure cloud

### Atelier 4 — Scénarios opérationnels (top 3)
| Scénario | Vraisemblance | Gravité | Criticité |
|----------|--------------|---------|-----------|
| Ransomware phishing | 4/4 | 4/4 | CRITIQUE |
| Fuite données RH | 3/4 | 4/4 | ÉLEVÉE |
| Compromission API client | 3/4 | 3/4 | ÉLEVÉE |

### Atelier 5 — Plan de traitement
- 12 mesures de sécurité priorisées
- Budget estimé : 180 000 € sur 2 ans
- Réduction du risque résiduel : 68 %

## 📊 Déclaration dApplicabilité (extrait)

| Contrôle ISO 27001:2022 | Applicable | Mis en œuvre | Justification |
|-------------------------|------------|--------------|---------------|
| 5.1 Politiques de sécurité | ✅ | ✅ | PSSI validée COMEX |
| 5.7 Threat intelligence | ✅ | 🔄 En cours | Veille ANSSI/CERT-FR |
| 6.1 Screening | ✅ | ✅ | Processus RH documenté |
| 8.7 Protection malware | ✅ | ✅ | EDR déployé |
| 8.8 Gestion vulnérabilités | ✅ | 🔄 En cours | Nessus en déploiement |
| 8.16 Surveillance activités | ✅ | ✅ | SIEM Splunk opérationnel |

**Bilan DdA** : 93 contrôles analysés — 71 applicables — 52 mis en œuvre — 19 en cours

## 📈 KPIs RSSI (tableau de bord)

| Indicateur | Cible | Actuel | Statut |
|-----------|-------|--------|--------|
| Taux de patching critique (< 30j) | 95% | 87% | 🟡 |
| Couverture MFA comptes privilegiés | 100% | 100% | 🟢 |
| Délai moyen détection incident | < 4h | 2h30 | 🟢 |
| Taux formation sécu collaborateurs | 100% | 78% | 🟡 |
| Disponibilité SI critique | 99.5% | 99.8% | 🟢 |
| Vulnérabilités critiques ouvertes | 0 | 2 | 🔴 |

## 🗂️ Structure du repo

```
smsi-iso27001-eti/
├── 01-cadrage/
│   ├── perimetre-smsi.md
│   └── contexte-organisation.md
├── 02-ebios-rm/
│   ├── atelier1-cadrage.md
│   ├── atelier2-sources-risques.md
│   ├── atelier3-scenarios-strategiques.md
│   ├── atelier4-scenarios-operationnels.md
│   └── atelier5-traitement-risques.md
├── 03-declaration-applicabilite/
│   └── dda-iso27001-2022.md
├── 04-politiques/
│   ├── pssi.md
│   └── politique-classification.md
├── 05-pca-pra/
│   └── plan-continuite-activite.md
├── 06-kpis/
│   └── tableau-bord-rssi.md
└── README.md
```

## 🔗 Références

- [ISO/IEC 27001:2022](https://www.iso.org/standard/27001)
- [EBIOS Risk Manager — ANSSI](https://www.ssi.gouv.fr/entreprise/management-du-risque/la-methode-ebios-risk-manager/)
- [Guide SMSI — ANSSI](https://www.ssi.gouv.fr/)
- [CNIL — Guide RGPD](https://www.cnil.fr/fr/rgpd-de-quoi-parle-t-on)

## 👤 Auteur

**Fèmi KPONOU** — Étudiant Bachelor Cybersécurité ESAIP  
🌐 [Portfolio](https://primaelkpfv.github.io) · 💼 [LinkedIn](https://linkedin.com/in/primaelkponou)
