# Concepts de réseaux et protocles 

### le model OSI : est une référence universelle pour comprendre et développer les réseaux. Elle est divisée en 7 couches, chaque couche à un rôle spécifique.

### les differentes couches 
- couche 1 : Physique
    - Rôle: Transmission des données sous forme de signaux électriques, signaux lumineux ou signaux radio
- couche 2 : Liaison de données
    - Rôle : assure une communication fiable entre deux appareils, détecte et corrige les erreurs de transmission (adresse MAC, Switch...)
- couche 3 : Réseau
    - Rôle : acheminement des paquets entre différente réseaux, utilisations des adresses IP pour les identifier ( Routeurs, adresse IP)
- couche 4 : Tranport
    - Rôle : gère le transport fiable ou rapide des données entre hôtes, utilise des numéros de ports pour identifier les applications ( TCP, UDP)
- couche 5 : Session
    - Rôle: gère les connexions entre applications et synchronisations
- couche 6 : Présentation
    - Rôle : Traduction des données pour qu'elles soient comprehensible par l'application ( compression, chiffrement)
- couche 7: Application
    - Rôle : Interface utilisateur permettant aux applicaitons de communiquer avec le réseau ( http, SMTP (email))
    - 
