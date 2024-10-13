![9fae028c6e9644a076fdbd8e1eddbfcb](https://github.com/user-attachments/assets/1f5e19f3-21fe-44f6-a472-3b1cc63a68ad)

# Système de Recommandation de Parfums


Trouver un parfum similaire à celui qu'on aime peut être une tâche difficile. Habituellement, cela implique de se rendre en boutique, d'essayer plusieurs parfums et d'espérer en trouver un qui nous plaît, ou de chercher en ligne des parfums similaires. Ce processus peut être long et frustrant.

Ce projet vise à simplifier cette démarche en proposant un système de recommandation de parfums basé sur les notes olfactives et les parfums déjà connus. Grâce à une interface web simple, les utilisateurs peuvent obtenir des suggestions personnalisées en quelques clics seulement.



## Dataset
Le dataset présente des informations sur différents parfums. Il contient trois colonnes : la colonne "brand" indique la marque du parfum, la colonne "perfume" donne le nom du parfum, et la colonne "notes" décrit les accords olfactifs associés à chaque parfum.
## Technologies Utilisées
Python

Pandas

NumPy

Scikit-learn

TfidfVectorizer 

cosine_similarity

Gradio
 
Google Colab et Google Drive 

## Méthodologie

Notre système de recommandation est basé sur le **filtrage basé sur le contenu**, une approche qui recommande des produits similaires à ceux que l'utilisateur apprécie déjà, en se basant sur les caractéristiques du contenu. Dans ce contexte, nous utilisons les **notes olfactives** des parfums comme caractéristiques principales. En vectorisant ces notes à l'aide du **TF-IDF** (Term Frequency-Inverse Document Frequency) et en calculant la **similarité cosinus** entre les vecteurs, nous pouvons mesurer à quel point deux parfums sont similaires en termes de composition olfactive. Ainsi, lorsque l'utilisateur sélectionne des notes qu'il aime ou un parfum qu'il apprécie, le système analyse ces informations pour recommander des parfums ayant des profils olfactifs proches, permettant une personnalisation des suggestions en fonction des préférences individuelles.
## Demo



