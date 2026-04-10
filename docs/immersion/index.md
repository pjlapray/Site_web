# Immersion ASE
## 🌿 Liste du matériel : Prototype Serre Connectée

Ce tableau présente les composants nécessaires pour le nouveau support pédagogique de serre automatisée. Ce système est conçu pour être alimenté par la **platine 3.3V / 5V / 12V** déjà utilisée en TP.

| Composant | Fonction principale | Atelier associé | Prix approx. |
| :--- | :--- | :--- | :--- |
| **Arduino Uno (R3)** | Cerveau du système : gestion des seuils et des cycles d'arrosage. | Atelier 2 | 12,00 € |
| **Capteur d'humidité du sol** | Mesure le taux d'humidité pour déclencher l'irrigation (Analogique). | Atelier 1 | 2,50 € |
| **Capteur DHT22** | Mesure précise de la température et de l'humidité relative de l'air. | Atelier 2 | 4,50 € |
| **Bande LED RGB (WS2812B)** | Simulation du spectre solaire et indicateur d'état (LED horticole). | Atelier 1 / 2 | 8,00 € |
| **Mini-pompe à eau (12V)** | Actionneur pour l'irrigation via le réservoir externe. | Atelier 3 | 7,50 € |
| **Ventilateur PC (12V)** | Régulation thermique par extraction d'air chaud. | Atelier 3 | 5,00 € |
| **Module 2 Relais (5V)** | Interface de puissance pour commuter la pompe et le ventilateur. | Atelier 3 | 4,00 € |
| **Écran LCD 1602 (I2C)** | Affichage en temps réel des constantes biophysiques de la serre. | Atelier 2 | 5,50 € |
| **Capteur de lumière (LDR)** | Mesure de l'ensoleillement pour piloter l'éclairage artificiel. | Atelier 1 | 1,00 € |
| **Structure (Bac/Châssis)** | Enceinte de protection et support pour la culture. | Atelier 5 | 12,00 € |
| **Vannes et tuyauterie** | Distribution de l'eau vers les zones de plantation. | Atelier 5 | 6,00 € |
| **TOTAL ESTIMÉ** | | | **~68,00 €** |

---

## ⚙️ Exploitation de la platine d'alimentation existante
Ce projet est conçu pour valider les acquis de la fabrication de la platine d'alimentation :
* **Sortie 12V :** Dédiée à la puissance (Pompe et Ventilation).
* **Sortie 5V :** Dédiée à la logique (Arduino, Capteurs, Écran) et à la bande LED.
* **Sortie 3.3V :** Disponible pour une future extension IoT (ESP32 / LoRa).


---

## 🚀 Points clés du prototype

1. **Polyvalence énergétique :** Utilisation du **12V** pour la puissance (pompe/ventilation) et du **5V** pour la commande et la bande LED.
2. **Modularité :** Possibilité d'ajouter un module **ESP32-CAM** (déjà présent sur la barrière) pour surveiller la croissance des plantes à distance.
3. **Pédagogie :** L'ajout de la **bande LED RGB** permet d'aborder la synthèse additive des couleurs et l'influence des longueurs d'onde (Bleu/Rouge) sur la photosynthèse.