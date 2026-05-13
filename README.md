📘 Mandat 1 — Infrastructure hybride + Migration Active Directory



📝 Résumé du projet
Ce projet consiste à concevoir et déployer une infrastructure Active Directory locale, puis à la connecter à Microsoft Azure / Entra ID afin de créer un environnement hybride.
Le mandat inclut la mise en place du domaine, la création des identités, l’installation d’Azure AD Connect, la synchronisation des comptes et la validation des connexions cloud.

Ce dépôt contient : 

des captures d’écran des étapes clés 

des scripts PowerShell utilisés

la documentation technique du mandat

🏗️ Architecture du projet
Environnement local
1 VM Windows Server 2022

Rôles installés :

Active Directory Domain Services (AD DS)

DNS Server

Environnement cloud
1 tenant Microsoft Azure / Entra ID

Service utilisé : Azure AD Connect (synchronisation hybride)

Flux d’identité
AD DS → Azure AD Connect → Entra ID → Authentification cloud

⚙️ Étapes réalisées
1. Création de la VM Windows Server
Installation de Windows Server 2022

Configuration réseau

Renommage de la machine

Préparation pour AD DS

2. Installation d’Active Directory + DNS
Promotion du serveur en contrôleur de domaine

Création du domaine local

Configuration du DNS intégré

3. Création des identités
Création d’utilisateurs

Création de groupes

Organisation dans des OU

4. Création du tenant Azure
Création d’un compte Azure

Configuration d’Entra ID

Vérification du domaine

5. Installation d’Azure AD Connect
Choix du mode de synchronisation

Connexion AD DS ↔ Azure AD

Configuration du filtrage (OU)

6. Synchronisation des comptes
Synchronisation initiale

Vérification dans Entra ID

Validation des attributs synchronisés

7. Tests de connexion cloud
Connexion avec un utilisateur synchronisé

Vérification MFA / SSPR (si activé)

Validation de l’identité hybride

🧠 Compétences développées
Administration Active Directory

Gestion des identités hybrides

Synchronisation AD DS ↔ Azure AD

Déploiement d’Azure AD Connect

Troubleshooting identité cloud

🎓 Certifications liées
AZ‑104 — Azure Administrator

AZ‑800 — Administering Windows Server Hybrid Core Infrastructure

SC‑300 — Identity and Access Administrator
