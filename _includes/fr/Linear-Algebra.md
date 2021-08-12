Accédez à davantage de fonctions d'algèbre linéaire avec `using LinearAlgebra`.

|                                |                                             |
| ------------------------------ | ------------------------------------------- |
| Matrice identité               | `I  # à utiliser pour remplir une matrice de dimension quelconque` |
| Définir une matrice            | `M = [1 0; 0 1]`                            |
| Dimension d'une matrice        | `size(M)`                                   |
| Sélectionner la ligne `i`      | `M[i, :] # ligne i et toutes colonnes`                                  |
| Sélectionner la colonne `i`    | `M[:, i] # toutes lignes et colonne i`                                   |
| Concaténer horizontalement     | `M = [a b]` or `M = hcat(a, b)`             |
| Concaténer verticalement       | `M = [a ; b]` or `M = vcat(a, b)`           |
| Transposition de matrice       | `transpose(M)`                              |
| Matrice adjointe               | `M'` or `adjoint(M)`                        |
| Trace d'une matrice            | `tr(M)`                                     |
| Déterminant d'une matrice      | `det(M)`                                    |
| Rang d'une matrice             | `rank(M)`                                   |
| Valeurs propres d'une matrice  | `eigvals(M)`                                |
| Vecteurs propres d'une matrice | `eigvecs(M)`                                |
| Matrice inverse                | `inv(M)`                                    |
| Résoudre `M*x == v`            | `M\v` est <a class="tooltip" href="#">meilleur <span> Numériquement plus stable et typiquement plus rapide.</span></a> que `inv(M)*v` |
| Pseudo-inverse de Moore-Penrose| `pinv(M)`                                   |

Julia supporte nativement les [décompositions de 
matrice](https://docs.julialang.org/en/v1.0.0/stdlib/LinearAlgebra/).

Julia essaye d'inférer si les matrices ont un type spécial (symétrique, 
hermitienne, etc.), mais n'y parvient pas toujours. Afin que Julia choisisse
les algorithmes optimaux, les matrices spéciales peuvent être déclarées avec 
des fonctions telles que `Symmetric` , `Hermitian` , `UpperTriangular`, `LowerTriangular`,
`Diagonal` , et davantage.
