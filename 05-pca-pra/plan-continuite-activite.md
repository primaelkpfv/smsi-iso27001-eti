# Plan de Continuité dActivité (PCA)
## TechCorp SA — Version 1.0

---

## 1. Objectifs RTO/RPO

| Système | RTO (max) | RPO (max) | Criticité |
|---------|-----------|-----------|-----------|
| Plateforme client | 4h | 1h | CRITIQUE |
| SI Comptable | 8h | 4h | HAUTE |
| Messagerie | 2h | 30min | HAUTE |
| SI RH | 24h | 8h | MOYENNE |
| Intranet | 48h | 24h | FAIBLE |

## 2. Procédures de reprise

### 2.1 Perte du datacenter principal
1. Activation cellule de crise (RSSI + DSI + DG)
2. Basculement DNS vers site secondaire (< 15 min)
3. Démarrage VMs depuis backups Veeam (< 2h)
4. Vérification intégrité données (< 1h)
5. Communication collaborateurs et clients

### 2.2 Ransomware généralisé
1. Isolation immédiate du réseau (couper VPN et accès externes)
2. Identification des systèmes compromis
3. Restauration depuis sauvegardes hors-ligne (bande)
4. Scan antivirus avant remise en production
5. Dépôt de plainte (ANSSI + Police)

### 2.3 Perte accès cloud (AWS/Azure)
1. Activation hébergement de secours (OVH)
2. Restauration depuis snapshots quotidiens
3. Mise à jour DNS

## 3. Tests PCA

| Test | Fréquence | Dernier test | Résultat |
|------|-----------|-------------|----------|
| Simulation panne datacenter | Annuel | 2024-11 | ✅ RTO respecté |
| Restauration backup | Trimestriel | 2025-01 | ✅ Intégrité OK |
| Exercice cellule de crise | Annuel | 2024-09 | ✅ |

## 4. Contacts durgence

| Rôle | Nom | Tel | Email |
|------|-----|-----|-------|
| RSSI | [Nom] | [Tel] | rssi@techcorp.fr |
| DSI | [Nom] | [Tel] | dsi@techcorp.fr |
| DG | [Nom] | [Tel] | dg@techcorp.fr |
| Hébergeur | OVH Support | 1007 | support@ovh.com |
