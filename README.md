 
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

### Dual-stack
- le dual-stack : est une méthode permettant de mettre ensemble le IPv4 et IPv6, c'est à dire ils coexistant mais sans aucune compatibilité.
- exemple : une machie configurée en IPv4 ne peut pas communiquer avec IPv6

---

## Chiffrement
- **Symétrique** : Même clé pour chiffrer/déchiffrer.
- **Asymétrique** : Clés publique/privée.
- **Hybride** : Combinaison des deux.

---

## Routes
- le route est un réseau directement connecté au routeur
- statique : manuellement configurée
   - avantages : economies et sécurité
   - inconvénients : maintenance plus lourde et configuration compliquée.
- Dynamique : route apprise automatiquement par un protocole de routage
   - avantages : maintenance réduite, flexible et réagit automatiquement
   - inconvénients : initialisation difficile, sécurité et bande passante élevée.

---

## IP public et privé

### IP privé 
- c'est un adresse locale, non routable et doit être traduit pour communiquer vers l'exterieur.

### IP public 
- c'est une adresse unique nécessaire pour communiquer sur le internet, routable et assignée par IANA.
## IPv4 et IPv6

### IPv4
- 32 bits, notation décimale (ex : `192.168.1.1`).
- Limité en espace, utilise NAT pour compenser.
- Sécurité : IPSec externe.
- couche 3

---

### IPv6
- 128 bits, notation hexadécimale (ex : `fe80::1`).
- Espace illimité, IPSec intégré, performances améliorées.
- couche 3

### MAC
- l'adresse MAC est une adresse physique unique gravée sur la carte réseau non modifiable (fixe et attribuée par le fabricant)
- 48 bits, notation hexadecimale, divisée par : ou - ( ex : ´00:1A:2B:3B:4D:5E´)
- couche 2

### PORT 
- il est un identifiant numérique qui spécifie un service ou une application. 
- numéro entier ( 0 à 65535)
- couche 4

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
- il segmente un réseau physique en plusieurs réseaux logiques, plus efficace.
- **Avantages** : Sécurité, optimisation de la bande passante, administration simplifiée.
- **Protocole** : Tag VLAN via 802.1Q.

---

## Fibre optique vs Paire torsadée

### Fibre optique
- ces sont des câbles constituées de fibre en verre ou en plastique afin de transmettre des données sous forme de lumière.
- **Avantages** : Haute vitesse, longue distance, sécurité, résistance.
- **Inconvénients** : Coût élevé, installation complexe.

### Paire torsadée
- enroulement en helice de chaque paire de fils
- catégories : indique la vitesse et la capacité de transmission du câble, cat 5 (1000Mbits/s), cat 6 (25000Mbits/s) et cat 7 (10Gbits/s)
- Blindage: protège le cable des interferences électromagnetiques. F (blindage par feuille AL) et S (blindage par tresse Cu).
- **Avantages** : Coût faible, installation facile.
- **Inconvénients** : Distance limitée, moins rapide.

### Cables coaxial
- **Avantages** : Blindé
- **Inconvénients** :  doit passer de machine en machine et fragile.
---

## Configuration manuelle du réseau
- **Adresse IP** : `192.168.1.100`
- **Masque de sous-réseau** : `255.255.255.0`
- **Passerelle par défaut** : `192.168.1.1`
- **Serveurs DNS** : `8.8.8.8`
- adresse MAC

---

### ref 
- wifi IEEE 802.11
- Ethernet IEEE 802.3

---

### internet
- cicuit switching : operateur télephonique
- packet switching : plusieurs chemin
- backbones : ce sont les cables sous-marins, des fibres optiques et d'equipements de routage qui connectent les principaux hubs d'internet à travers le monde.
- ISP : fournisseurs d'accès d'internet.
- AS : autonomius systemes, groupe de reseau sous une meme administration avec un routage unique. (BGP).
- IXP : internet exchange points, ce sont des lieux physuques ou plisieurs réseaux se connectent pour echanger du trafic.
- Transit : il fait reference à un service ou un réseau privé paie un autre pour accéder à internet.
- Peering : est une relation d'echange entre deux reseaux sans transaction financiere afin d'optimiser la performance et reduire les couts.
- Peering public : realise via des points d'echange physique (IXP) ou plusieurs reseaux peuvent se connecter et echanger du trafic.
- Peering privé : Deux reseaux s'accordent pour interconnecter leurs infrastructures dans un lieu specifique.





