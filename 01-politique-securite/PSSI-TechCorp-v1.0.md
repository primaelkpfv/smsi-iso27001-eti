# Politique de Securite des Systemes d'Information (PSSI)
## TechCorp SA — Version 1.0 — Janvier 2025

**Classification**: INTERNE  
**Proprietaire**: RSSI  
**Approuve par**: Direction Generale  
**Prochaine revision**: Janvier 2026

---

## 1. Objet et Domaine d'Application

La presente PSSI definit les orientations strategiques de TechCorp SA en matiere de securite des systemes d'information. Elle s'applique a l'ensemble des collaborateurs, prestataires et partenaires ayant acces au SI de TechCorp SA.

**Perimetre**: Tous les systemes d'information traitant des donnees financieres, clients et operationnelles de TechCorp SA, incluant les infrastructures on-premise (Paris, Lyon, Bordeaux) et cloud (AWS eu-west-1).

---

## 2. Objectifs de Securite

TechCorp SA s'engage a garantir :

- **Confidentialite**: Les donnees clients et financieres ne sont accessibles qu'aux personnes autorisees
- **Integrite**: Les donnees ne sont pas alterees de maniere non autorisee
- **Disponibilite**: Les systemes critiques sont disponibles selon les engagements SLA (99.5%)
- **Conformite**: Le SI respecte les exigences RGPD, DSP2 et ISO 27001

---

## 3. Principes Directeurs

### 3.1 Moindre Privilege
Tout acces au SI est accorde selon le principe du moindre privilege. Les droits sont revus trimestriellement.

### 3.2 Defense en Profondeur
La securite repose sur des couches successives : perimetre (firewall pfSense), reseau (segmentation VLAN), systeme (durcissement CIS), application (WAF), donnees (chiffrement AES-256).

### 3.3 Securite par Conception
Tout nouveau projet integre la securite des la phase de conception (Security by Design, Privacy by Design).

### 3.4 Sensibilisation Continue
L'ensemble des collaborateurs suit une formation SSI annuelle obligatoire.

---

## 4. Responsabilites

| Acteur | Responsabilites |
|--------|----------------|
| Direction Generale | Engagement, ressources, arbitrages risques |
| RSSI | Pilotage SMSI, politique, audits, incidents |
| DSI | Implementation technique des mesures |
| DPO | Conformite RGPD, registre traitements |
| Managers | Application politique dans leurs equipes |
| Collaborateurs | Respect des regles, signalement incidents |

---

## 5. Regles Essentielles

### 5.1 Mots de Passe
- Longueur minimale : 14 caracteres
- Complexite : majuscules, minuscules, chiffres, caracteres speciaux
- Renouvellement : 90 jours pour comptes standard, 60 jours pour comptes privileges
- MFA obligatoire pour acces VPN, administration, applications critiques

### 5.2 Postes de Travail
- Verrouillage automatique apres 5 minutes d'inactivite
- Chiffrement disque obligatoire (BitLocker/FileVault)
- Installation logiciels interdite sans autorisation DSI
- Antivirus et EDR installes et a jour

### 5.3 Donnees
- Classification obligatoire : Public, Interne, Confidentiel, Secret
- Chiffrement des donnees Confidentiel/Secret au repos et en transit
- Interdiction de stocker des donnees clients sur postes locaux

### 5.4 Acces Distants
- VPN obligatoire pour acces au SI depuis l'exterieur
- Teletravail : utilisation exclusive du poste professionnel
- Interdiction des reseaux WiFi publics sans VPN

---

## 6. Gestion des Incidents

Tout incident ou suspicion d'incident de securite doit etre signale **immediatement** a :
- **Email urgence SSI**: ssi-incident@techcorp.fr
- **Hotline**: +33 1 XX XX XX XX (24h/24)
- **Portail ITSM**: https://itsm.techcorp.fr/incident

Classification des incidents :
- **P1 Critique**: Ransomware, violation majeure — Escalade Direction < 1h
- **P2 Haute**: Compromission compte, fuite donnees — RSSI < 4h
- **P3 Moyenne**: Malware isole, tentative intrusion — Equipe SSI < 24h

---

## 7. Sanctions

Tout manquement a la presente PSSI peut entrainer des sanctions disciplinaires pouvant aller jusqu'au licenciement, sans prejudice des poursuites penales en cas d'infraction caracterisee.

---

*Document valide par : Direction Generale TechCorp SA — Janvier 2025*
