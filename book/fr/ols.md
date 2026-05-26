# Moindres Carrés Ordinaires (MCO / OLS)

La méthode des **Moindres Carrés Ordinaires** (MCO, ou OLS en anglais) est une technique d'optimisation mathématique utilisée pour trouver la ligne (ou l'hyperplan) qui s'ajuste le mieux à un ensemble de données.

Son objectif principal est de minimiser la somme des carrés des différences (résidus) entre les valeurs observées et les valeurs prédites par le modèle. C'est-à-dire qu'elle cherche les coefficients de régression linéaire qui aboutissent à la plus petite erreur possible.

## Exploration Interactive

Ci-dessous, vous pouvez ajuster manuellement les paramètres d'une régression linéaire simple (l'ordonnée à l'origine $\beta_0$ et la pente $\beta_1$) pour tenter de trouver le modèle qui s'adapte le mieux aux données, ou laisser l'algorithme des moindres carrés calculer la valeur optimale de manière analytique.

```{raw} html
<iframe src="../_static/ols_interactive.html" width="100%" height="800px" frameborder="0" scrolling="no"></iframe>
```

```{raw} latex
\begin{center}
\textbf{Visualisation interactive :} Veuillez consulter la version HTML du livre pour accéder à l'outil interactif des Moindres Carrés Ordinaires (MCO).
\end{center}
```
