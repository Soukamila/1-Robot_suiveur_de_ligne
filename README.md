# 1-Robot_suiveur_de_ligne

# Devoir n°1 : Robot suiveur de ligne

## Objectif

Programmer le robot virtuel pour qu'il suive automatiquement une ligne tracée au sol, en corrigeant sa direction selon la position de la ligne.

## Composants

- **Robot virtuel VEX VR** : le robot simulé dans le navigateur.
- **Capteur Down Eye** : capteur dirigé vers le sol qui détecte la couleur sous le robot, donc la ligne.
- **Terrain (Playground)** : Line detector.
- **Programmation par blocs** : catégories Events, Control, Sensing et Motion.

## Fonctionnement

Le robot zigzague le long du bord de la ligne grâce à une boucle de décision :

1. Le programme démarre avec le bloc `When started`.
2. Une boucle `forever` répète les étapes suivantes sans arrêt.
3. Si le capteur Down Eye détecte la couleur de la ligne, le robot tourne légèrement à droite.
4. Sinon, il tourne légèrement à gauche.
5. Dans les deux cas, il avance d'une courte distance.

Ces petites corrections successives le maintiennent sur la ligne.

## Programme (pseudo-code des blocs)

```
When started
forever
    if Down Eye detects [couleur de la ligne] then
        turn right for [5] degrees
    else
        turn left for [5] degrees
    end if
    drive forward for [10] mm
end forever
```

## Résultats obtenus

- Le robot suit la ligne : [oui, sur tout le parcours / oui, avec quelques sorties de ligne].
- Réglages finaux : rotation de [5] degrés, avance de [10] mm.
- Problèmes rencontrés : [ex. le robot sortait de la ligne dans les virages].



