# Équations du second degré

Une équation du second degré est une équation polynomiale de la forme:
$$
ax^2 + bx + c = 0
$$ (eq-second-degre)

Où $x$ représente la variable, et $a$, $b$ et $c$ sont des constantes avec $a \neq 0$.

## Formule quadratique

La solution à l'équation {eq}`eq-second-degre` est donnée par la formule quadratique:
$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

Cette formule permet de trouver les racines de n'importe quelle équation du second degré.

## Exemple de code

Le code suivant en Python calcule les racines d'une équation du second degré en utilisant la bibliothèque standard `cmath` pour gérer d'éventuelles racines complexes:

```{code-cell} python
import cmath

def resoudre_equation_quadratique(a, b, c):
    # Calculer le discriminant
    d = (b**2) - (4*a*c)
    
    # Trouver deux solutions
    sol1 = (-b - cmath.sqrt(d)) / (2*a)
    sol2 = (-b + cmath.sqrt(d)) / (2*a)
    
    return sol1, sol2

# Exemple avec x^2 - 5x + 6 = 0
a = 1
b = -5
c = 6

racines = resoudre_equation_quadratique(a, b, c)
print(f"Les racines sont {racines[0]} et {racines[1]}")
```
