# Logique séquentielle

La logique séquentielle diffère de la logique combinatoire par l'introduction de la notion de **mémoire**. L'état des sorties ne dépend plus uniquement des entrées actuelles, mais aussi de l'historique des états précédents.

## Les circuits séquentiels élémentaires

Les briques de base de la logique séquentielle sont les **bascules** (latches et flip-flops), capables de mémoriser un bit d'information.

!!! info "Laboratoire Virtuel : Les Bascules RS, D et JK"
    Utilisez le simulateur interactif ci-dessous pour tester le comportement des différentes bascules. Observez particulièrement la différence entre une commande sur **niveau** (latch) et sur **front** (flip-flop).

    <div class="circuit-container" style="text-align: center; margin: 20px 0;">
        <iframe 
            src="https://circuitverse.org/simulator/embed/elec-num-partie-3-9cc032fe-5536-4bd0-9568-119b1518c853?theme=night-sky&display_title=true&clock_time=false&fullscreen=false&zoom_in_out=true" 
            style="border: 2px solid #2c3e50; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);" 
            name="myiframe" 
            id="projectPreview" 
            scrolling="no" 
            frameborder="0" 
            height="400" 
            width="100%" 
            allowFullScreen>
        </iframe>
    </div>

    [:material-fullscreen: Étudier le circuit en plein écran](https://circuitverse.org/simulator/edit/elec-num-partie-3-9cc032fe-5536-4bd0-9568-119b1518c853){ .md-button .md-button--primary }
    [:material-help-circle: Guide de manipulation](#){ .md-button }

### Points clés à observer :
* **Bascule RS :** Notez l'état interdit ($R=1, S=1$).
* **Bascule D :** Observez comment la donnée est "verrouillée".
* **Horloge (Clock) :** Identifiez si le changement se fait sur le front montant ou descendant.