# Immersion ASE

## 🌿 Liste du matériel : Prototype Serre Connectée

Ce tableau présente les composants nécessaires pour le nouveau support pédagogique de serre automatisée. Ce système est conçu pour être alimenté par la **platine 3.3V / 5V / 12V** déjà utilisée.



| Composant | Fonction principale | Atelier | Prix | Lien RS |
| :--- | :--- | :---: | :---: | :--- |
| :material-check-decagram-outline: **Arduino Uno** | "Cerveau" du système : gestion des cycles. | Tous | Stock | <a href="https://fr.rs-online.com/web/p/processeurs-et-microcontroleurs/7697409" target="_blank">Voir</a> |
| **Capteur Humidité Sol** | Mesure analogique du taux d'eau. | At. 2 | 2,50 € | <a href="https://fr.rs-online.com/web/p/kits-et-cartes-compatibles-arduino/2163778?gb=a" target="_blank">Voir</a> |
| :material-check-decagram-outline: **Capteur DHT22** | Température et humidité de l'air. | At. 2 | 4,50 € | <a href="" target="_blank">Voir</a> |
| **Bande LED RGB** | Gestion du spectre (suivant la variété) et indicateur d'état possible. | At. 1 | 8,00 € | <a href="https://fr.rs-online.com/web/p/rubans-led/1807502" target="_blank">Voir</a> |
| **Mini-pompe (12V)** | Actionneur pour l'irrigation. | At. 4 | 20,00 € | <a href="https://www.lextronic.fr/mini-pompe-a-eau-1-1-l-min-11296.html" target="_blank">Voir</a> ou <a href="https://www.leroymerlin.fr/produits/pompe-submersible-miniature-12-v-cc-3-metres-de-haut-resistante-a-des-temperatures-jusqu-a-60-98813622.html?megaBoost&at_source=google" target="_blank">Voir</a> |
| :material-check-decagram-outline: **Ventilateur (12V)** | Régulation thermique. | At. 4 | 5,00 € | <a href="https://fr.rs-online.com/web/p/ventilateurs-axiaux/1442036" target="_blank">Voir</a> |
| **Module 2 Relais** | Commutation Pompe / Ventilateur. | At. 3 | 4,00 € | <a href="https://fr.rs-online.com/web/p/modules-de-developpement-pour-la-robotique-la-gestion-d-alimentation-et-les-moteurs/2651120" target="_blank">Voir</a> |
| :material-check-decagram-outline: **Écran LCD I2C** | Affichage des données supervisées. | At. 1 | 5,50 € | <a href="https://fr.rs-online.com/web/p/afficheurs-monochromes-lcd/0735064?gb=a" target="_blank">Voir</a> |
| :material-check-decagram-outline: **Capteur LDR** | Mesure de l'ensoleillement. | At. 3 | 1,00 € | <a href="https://fr.rs-online.com/web/p/photoresistances/0596141" target="_blank">Voir</a> |
| **Structure** Plaastique ou plexi| Bac et couvercle. | Tous | 12,00 € | <a href="https://www.ferplast.fr/products/geo-medium target="_blank">Voir</a> ou <a href="https://www.ikea.com/fr/fr/cat/samla-serie-12553/ target="_blank">Voir</a> |
| **Tuyauterie** | Distribution de l'eau. | Tous | 6,00 € | - |
| **TOTAL ESTIMÉ** | | | **~68,00 €** | |

!!! info "A prévoir également :"

	* Gaine thermo, 
	* Colliers de serrage (Rilsan), 
	* Gaine spirale,
	* Fiche JST ou bornier à vis (pour pouvoir séparer facilement le bac de l'alim/contrôle
	* Nappe Ribon pour LCD ?
	* Etiqueteuse pour identifier chaque lot de fils, car le nombre de capteurs peut être important.


> :warning:
> **Attention à l'humidité**

> * **Protection :** Évitez toute projection d'eau sur la platine d'alimentation.
> * **Boucle de goutte :** Faites en sorte que les fils remontent légèrement avant d'entrer dans le boîtier électronique (pour éviter que l'eau ne s'écoule par capillarité vers l'électronique).

---

## ⚙️ Exploitation de la platine d'alimentation existante
Ce projet est conçu pour réutiliser la platine d'alimentation :

* **Sortie 12V :** Dédiée à la puissance (Pompe et Ventilation).
* **Sortie 5V :** Dédiée à la logique (Arduino, Capteurs, Écran) et à la bande LED.
* **Sortie 3.3V :** Disponible pour une future extension IoT.


---

## 🚀 Points clés du prototype

1. **Polyvalence énergétique :** Utilisation du **12V** pour la puissance (pompe/ventilation) et du **5V** pour la commande et la bande LED.
2. **Modularité :** Possibilité d'ajouter un module **ESP32-CAM** pour surveiller la croissance des plantes à distance (mais très peu probable pdt les 2 semaines...).
3. **Sympa :** L'ajout de la **bande LED RGB** permet d'aborder la synthèse additive des couleurs et l'influence des longueurs d'onde (Bleu/Rouge) sur la photosynthèse.

