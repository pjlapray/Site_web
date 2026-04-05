<div class="circuit-container" style="text-align: center; margin: 20px 0;">
    <iframe src="https://circuitverse.org/simulator/embed/elec-num-partie-2?theme=default&display_title=false&clock_time=false&fullscreen=true&zoom_in_out=true" style="border: 2px solid #2c3e50; border-radius: 10px;" height="400" width="100%" allowFullScreen></iframe>
</div>

# Additionneur Complet 1 bit

L'additionneur complet (Full Adder) prend en entrée deux bits ($A$ et $B$) ainsi qu'une retenue d'entrée ($C_{in}$), et produit une somme ($S$) et une retenue de sortie ($C_{out}$).

## Expérimentation et Visualisation

!!! info "Objectif pédagogique"
    Explorez les deux facettes de la conception : le schéma logique pur (généré ici par WaveDrom) et sa mise en œuvre technologique sur platine d'essai.

=== ":material-sitemap: Schéma Logique (WaveDrom)"

    Voici la représentation logique de l'additionneur complet :
    * **Somme ($S$)** : Double OU-Exclusif (XOR).
    * **Retenue ($C_{out}$)** : Logique combinatoire des entrées.

    ```wavedrom
    { "assign": [
        ["S", ["^", "A", "B", "Cin"]],
        ["Cout", ["|", ["&", "A", "B"], ["&", "Cin", ["^", "A", "B"]]]]
    ]}
    ```
    


=== ":material-chip: Simulation Techno (Tinkercad)"

    <div style="border: 1px solid #dee2e6; border-radius: 8px; padding: 10px; background: #f8f9fa; margin: 20px 0;">
        <iframe 
            width="100%" height="450" 
            src="https://www.tinkercad.com/embed/cu7zEMnK42q?editbtn=0" 
            frameborder="0" style="border-radius: 5px;" scrolling="no">
        </iframe>
        <p><em>Vue du câblage d'un additionneur complet 1 bit (Série 74HC).</em></p>
    </div>

---

### Table de Vérité

| $A$ | $B$ | $C_{in}$ | $S$ | $C_{out}$ |
|:---:|:---:|:---:|:---:|:---:|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |