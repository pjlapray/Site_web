# La Métastabilité

En logique séquentielle, le respect du timing est crucial. Si l'entrée **D** change d'état précisément au moment du front d'horloge (**CLK**), la bascule entre dans un état instable appelé **métastabilité**.

## Le danger
Dans cet état, la sortie $Q$ ne sait pas si elle doit passer à `0` ou à `1`. Elle peut rester bloquée entre deux tensions pendant quelques nanosecondes ou osciller follement.



!!! warning "Conséquence système"
    Un signal métastable peut provoquer des erreurs imprévisibles (crashs) car il pourrait être interprété différemment par les circuits logiques qui suivent.


## Représentation du signal instable
wavedrom (
{ "signal": [
  { "name": "CLK", "wave": "p..p..p" },
  { "name": "D",   "wave": "0.x0.x1", "desc": "Violation du setup time" },
  { "name": "Q",   "wave": "0.x..=.", "data": ["Stable"] }
],
  "head": { "text": "Zone d'incertitude temporelle" }
}
)

## Comment l'éviter ?
Pour sécuriser un signal asynchrone (comme un bouton-poussoir), on utilise un **synchroniseur** : on place deux bascules D en série.
1. La première bascule encaisse l'instabilité potentielle.
2. La deuxième bascule récupère un signal stabilisé au coup d'horloge suivant.
