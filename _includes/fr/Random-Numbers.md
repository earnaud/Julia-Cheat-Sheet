Plusieurs fonctions de nombre aléatoire requièrent `using Random`.

|                                  |                                                               |
| -------------------------------- | ------------------------------------------------------------- |
| Définir une *seed*               | `seed!(seed)`                                                 |
| Nombres aléatoires               | `rand()   # uniform [0,1)`<br>`randn()  # normal (-Inf, Inf)` |
| Aléatoire depuis une Autre Distribution   | `using Distributions`<br>`my_dist = Bernoulli(0.2) # For example`<br>`rand(my_dist)` |
| Sous-échantillon aléatoire d'éléments depuis A avec une probabilité d'inclusion p | `randsubseq(A, p)` |
| Permutations aléatoires de A     | `shuffle(A)`                                                  |
