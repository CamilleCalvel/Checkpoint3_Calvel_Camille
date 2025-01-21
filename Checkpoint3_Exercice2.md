# Partie 1 : Gestion des utilisateurs

**Q.2.1.1**

![Capture d'écran 2025-01-17 115055](https://github.com/user-attachments/assets/b0c6f921-ec96-4737-9372-bf013b193ac2)

**Q.2.1.2**

Les préconisations que je proposes concernant ce compte :
- Utilisation d'un **mot de passe complexe** avec des majuscules, minuscules, chiffres et symboles
- Application des **principes de moindre privilège** :
  - Accès uniquement aux ressources dont il a besoin
  - Utilisation des mécanismes d'élévation temporaire de privilèges (sudo)
    
# Partie 2 : Configuration de SSH

**Q.2.2.1**

![Capture d'écran 2025-01-17 121142](https://github.com/user-attachments/assets/0a25ecea-c0ff-42b5-a5a6-390f0826da96)

**Q.2.2.2**

![Capture d'écran 2025-01-17 121552](https://github.com/user-attachments/assets/3bd0f069-e9b6-4ab6-bc06-509a5df4e407)

**Q.2.2.3**

![Capture d'écran 2025-01-17 122425](https://github.com/user-attachments/assets/117b3d52-192c-4ed2-9e21-f4311ae4dd86)

![Capture d'écran 2025-01-17 123843](https://github.com/user-attachments/assets/1ab46435-5189-43d9-a06a-ce3d30862517)

# Partie 3 : Analyse du stockage

**Q.2.3.1**

![Capture d'écran 2025-01-17 125005](https://github.com/user-attachments/assets/0bf4620a-7b54-4166-ae7e-5083aaa987a3)

**Q.2.3.2**

![Capture d'écran 2025-01-21 170443](https://github.com/user-attachments/assets/c4dc3900-9d3b-4884-9a66-e399564d3623)

**Q.2.3.3**

![Capture d'écran 2025-01-17 130813](https://github.com/user-attachments/assets/f0711d95-4283-4cb8-9203-937ab43cab6f)

![Capture d'écran 2025-01-17 130757](https://github.com/user-attachments/assets/568fbd4c-b005-44d6-b2c6-4b6a327b546c)

![Capture d'écran 2025-01-17 130850](https://github.com/user-attachments/assets/1a157028-0839-46f6-977b-e9707ab8327f)

**Q.2.3.4**

**Q.2.3.5**

# Partie 4 : Sauvegardes

**Q.2.4.1**

Les rôles des 3 composants bareos :
  - bareos-dir : Il est responsable de la planification, du contrôle et du lancement des tâches de sauvegardes. Il contrôle l'ensemble des autres composants. Il est installé sur le serveur en charge de la gestion des sauvegardes.
  - bareos-sd : Il gère le stockage physique des données sauvegardées et le processus de lecture/écriture des volumes de sauvegarde.
  - bareos-fd : Il est en charge de collecter les informations à sauvegarder et de les envoyer au Bareos Storage Daemon. Ce composant est installé sur chaque machine devant être sauvegardée.

# Partie 5 : Filtrage et analyse réseau

**Q.2.5.1**

![Capture d'écran 2025-01-17 132531](https://github.com/user-attachments/assets/5c1cb503-3f82-489d-9fb6-92100ada6f56)

**Q.2.5.2**

Les types de communications autorisées :
- SSH
- ICMP
- ICMPv6

**Q.2.5.3**

Il n'y a pas de communications interdites

**Q.2.5.4**

# Partie 6 : Analyse de logs

**Q.2.6.1**
journalctl -u ssh | grep 'Failed password' | tail -n 10
