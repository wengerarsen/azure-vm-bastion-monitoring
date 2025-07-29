# 💻 Projet Azure #2 — Déploiement d'une Machine Virtuelle Windows Server avec Bastion et Supervision

Ce projet s’inscrit dans ma démarche de progression vers la certification **AZ-104: Microsoft Azure Administrator**.  
Il consiste à déployer une **machine virtuelle Windows Server** dans Azure, la sécuriser avec **Azure Bastion**, et la superviser à l’aide d’**Azure Monitor**.

---

## 🧱 Objectifs du projet

- Créer un groupe de ressources pour isoler l’environnement
- Déployer un réseau virtuel (VNet) avec sous-réseaux dédiés
- Créer une VM Windows Server dans un sous-réseau privé
- Utiliser **Azure Bastion** pour une connexion RDP sécurisée sans IP publique
- Installer le rôle **IIS (serveur web)** sur la VM
- Activer la supervision avec **Azure Monitor Insights**
- Créer une **alerte** basée sur la consommation CPU

---

## ☁️ Ressources Azure utilisées

| Ressource              | Nom              | Description                                 |
|------------------------|------------------|---------------------------------------------|
| Groupe de ressources   | `rg-projet2`     | Regroupe toutes les ressources du projet    |
| Réseau virtuel         | `vnet-projet2`   | VNet principal avec deux sous-réseaux       |
| Sous-réseau Bastion    | `AzureBastionSubnet` | Requis pour le service Azure Bastion    |
| Sous-réseau VM         | `sous-reseau-vm` | Contient la VM                              |
| Machine virtuelle      | `vm-projet2`     | VM Windows Server B1s                       |
| Azure Bastion          | `bastion-projet2`| Connexion RDP sécurisée                     |
| Azure Monitor / Insights | Activé          | Suivi des performances et alertes           |
| Alerte CPU             | `CPU_High_Usage` | Notifie si l’utilisation CPU > 70 %         |

---

## 🛠️ Étapes principales

1. **Création du groupe de ressources**  
2. **Déploiement du réseau virtuel avec sous-réseaux**  
3. **Création de la machine virtuelle sans IP publique**  
4. **Déploiement d'Azure Bastion**  
5. **Connexion RDP via Bastion depuis le portail Azure**  
6. **Installation d’IIS sur la VM (PowerShell)**  
7. **Activation d’Azure Monitor + création d’une alerte CPU**

---

## 🔐 Sécurité

- Aucun port RDP (3389) ouvert vers Internet
- Connexion sécurisée via Bastion
- Aucun mot de passe transmis en clair

---

## 📸 Captures d’écran
<img width="959" height="454" alt="installation IIS" src="https://github.com/user-attachments/assets/ea799d31-d97b-42f6-9bba-7164d7bbd45c" />
<img width="960" height="479" alt="connection via bastion" src="https://github.com/user-attachments/assets/7243baa4-3ee6-4581-a885-51f15c2e00cb" />
<img width="960" height="449" alt="alertes" src="https://github.com/user-attachments/assets/f999fad9-09b2-44c8-b920-04f1fa2228b6" />
<img width="960" height="449" alt="Vnet et Subnet" src="https://github.com/user-attachments/assets/8b400d1d-f3d2-4f96-a310-7f8e40c8b911" />
<img width="960" height="455" alt="installtion webserver sur ma VM" src="https://github.com/user-attachments/assets/b9ca05d5-7e48-42d4-9235-ad582575d096" />



---

## 🧠 Compétences mises en pratique

- Administration de machines virtuelles Windows sur Azure  
- Sécurité réseau et Bastion  
- Supervision et alertes avec Azure Monitor  
- Automatisation partielle via le portail

---

## 📅 Date du projet

**Juillet 2025**

---

## ✍️ Auteur

**Arsène Kemadjou Nganso**  
www.linkedin.com/in/arsène-kemadjou-nganso-1a5368151
Certification AZ-900 — En préparation pour AZ-104
