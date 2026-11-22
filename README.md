# ProjetReseau2
serveur DHCP dédié

Pitch : la distribution des adresses est confiée à un serveur, comme en entreprise.

1. Contexte : un serveur dédié permet de centraliser et de faire évoluer le service sans surcharger le routeur.

2. Topologie : 1 routeur, 1 switch, 1 serveur, <N> PC. Plan d’adressage : <réseau/masque>, passerelle <IP>, serveur <IP>.

3. Étapes

Routeur : adresse sur l’interface LAN et no shutdown.
Serveur : IP Configuration en statique (un serveur ne doit jamais changer d’adresse), avec masque et passerelle.
Service DHCP : Services > DHCP, service On.
Pool : nom, passerelle par défaut, DNS, IP de départ, masque, nombre maximal d’utilisateurs, puis Save.
Clients : mettre les PC en DHCP.

4. Vérification : baux reçus par les PC, ipconfig, ping vers la passerelle, le serveur et entre PC.

5. Comparaison avec le projet 1 : la configuration passe de la ligne de commande à une interface graphique, et le routeur ne fait plus que router.

6. Erreurs fréquentes : serveur laissé en DHCP ; service DHCP non activé ; pool sans passerelle ; plage de début qui chevauche l’IP du serveur.

7. Compétences : configuration d’un serveur, services réseau, adressage statique vs dynamique.
8. <img width="875" height="752" alt="Capture d&#39;écran 2026-11-22 183156" src="https://github.com/user-attachments/assets/082424ee-cf91-42ed-b5c0-eba73d9f6f0b" />
