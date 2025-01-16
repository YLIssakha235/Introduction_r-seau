 
# Documentation Réseau


## Modèles OSI et TCP/IP

### Modèle OSI
- Modèle en 7 couches, référence universelle pour les réseaux.

### Modèle TCP/IP
- Simplification du modèle OSI, utilisé pour les communications internet.

## Les différentes couches du modèle OSI

### Couche 1 : Physique
- **Rôle** : Transmission des données sous forme de signaux électriques (câbles, fibres, etc.).

### Couche 2 : Liaison de données
- **Rôle** : Communication fiable entre appareils, détection et correction des erreurs (Adresses MAC, Switch).

### Couche 3 : Réseau
- **Rôle** : Acheminement des paquets entre différents réseaux grâce aux adresses IP (Routeurs, adresses IP).

### Couche 4 : Transport
- **Rôle** : Transport fiable ou rapide des données entre hôtes via des numéros de ports (TCP, UDP).

### Couche 5 : Session
- **Rôle** : Gestion des connexions entre applications et synchronisation (Protocole PPTP).

### Couche 6 : Présentation
- **Rôle** : Traduction des données pour l’application (compression, chiffrement) (MP4, MP3).

### Couche 7 : Application
- **Rôle** : Interface utilisateur permettant la communication avec le réseau (HTTP, SMTP, FTP).

---

## Protocoles et Ports

### ARP
- **Rôle** : Traduction d’une adresse IP (couche 3) en une adresse MAC (couche 2).

### Ports communs
- **HTTPS** : Port 443 (affichage sécurisé des pages web).
- **SSH** : Port 22 (connexion console à distance).
- **SCP** : Port 22 (transfert de fichiers via SSH).

---

## Firewalls
- Protection réseau via des filtres entrants/sortants.
- Création de zones avec des règles différentes (LAN, DMZ).

---

## Chiffrement
- **Symétrique** : Même clé pour chiffrer/déchiffrer.
- **Asymétrique** : Clés publique/privée.
- **Hybride** : Combinaison des deux.

---

## IPv4 et IPv6

### IPv4
- 32 bits, notation décimale (ex : `192.168.1.1`).
- Limité en espace, utilise NAT pour compenser.
- Sécurité : IPSec externe.

### IPv6
- 128 bits, notation hexadécimale (ex : `fe80::1`).
- Espace illimité, IPSec intégré, performances améliorées.

---

## Protocoles TCP/UDP

### TCP
- **Orienté connexion** : Ouverture et fermeture de session.
- **Fiable** : Accusés de réception, ordre des paquets, checksum.
- **Usage** : HTTP, HTTPS, FTP, emails.

### UDP
- **Sans connexion** : Moins fiable mais rapide.
- **Usage** : Jeux en ligne, DNS.

---

## Switch vs Hub

### Hub
- Diffuse les données à tous.
- Couche 1 (physique), bande passante partagée.

### Switch
- Dirige les données au destinataire.
- Couche 2 (liaison de données), bande passante dédiée.

---

## VLAN
- **Avantages** : Sécurité, optimisation de la bande passante, administration simplifiée.
- **Protocole** : Tag VLAN via 802.1Q.

---

## Fibre optique vs Paire torsadée

### Fibre optique
- **Avantages** : Haute vitesse, longue distance, sécurité, résistance.
- **Inconvénients** : Coût élevé, installation complexe.

### Paire torsadée
- **Avantages** : Coût faible, installation facile.
- **Inconvénients** : Distance limitée, moins rapide.

---

## Configuration manuelle du réseau
- **Adresse IP** : `192.168.1.100`
- **Masque de sous-réseau** : `255.255.255.0`
- **Passerelle par défaut** : `192.168.1.1`
- **Serveurs DNS** : `8.8.8.8`

---



