Projet : Routage Statique — Cisco Packet Tracer

Ce projet illustre le fonctionnement du routage statique dans un réseau composé de trois routeurs (R1, R2, R3) connectés en topologie triangulaire, chacun relié à un PC (PC1, PC2, PC3).

Chaque routeur connaît uniquement les réseaux directement connectés. Les routes vers les autres réseaux ont été configurées manuellement à l’aide de la commande (ip route).

Deux versions sont proposées :

🔹 Version 1 — Routage statique de base

Dans cette version, la sélection du chemin se base sur le nombre de sauts (routers).
Le chemin privilégié est celui qui présente le plus petit nombre de routeurs intermédiaires, conformément à la logique classique du routage statique.

🔹 Version 2 — Test ciblé de distance administrative

Dans cette version expérimentale, seule la distance administrative du routeur R3 a été modifiée, et uniquement pour le trafic allant de PC3 vers PC2.
Ainsi, au lieu d’emprunter le chemin direct PC1 → R3 → R2 → PC2, les paquets passent désormais par le chemin plus long : R3 → R1 → R2 → PC2.
Cette configuration partielle permet de démontrer concrètement comment un simple ajustement de la distance administrative peut influencer la sélection du chemin de routage, 
tout en conservant le comportement normal pour les autres destinations (par exemple, PC3 → PC1 continue de privilégier le chemin le plus court).

Ce projet met en pratique :

la configuration manuelle des routes statiques (ip route)

la compréhension du Next-Hop et de l’Exit Interface

le rôle de la distance administrative

la visualisation du routage à l’aide de Cisco Packet Tracer
