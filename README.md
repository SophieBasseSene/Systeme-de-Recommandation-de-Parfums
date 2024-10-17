![9fae028c6e9644a076fdbd8e1eddbfcb](https://github.com/user-attachments/assets/1f5e19f3-21fe-44f6-a472-3b1cc63a68ad)

# Système de Recommandation de Parfums


Trouver un parfum similaire à celui qu'on aime peut être une tâche difficile. Habituellement, cela implique de se rendre en boutique, d'essayer plusieurs parfums et d'espérer en trouver un qui nous plaît, ou de chercher en ligne des parfums similaires. Ce processus peut être long et frustrant.

Ce projet vise à simplifier cette démarche en proposant un système de recommandation de parfums basé sur les notes olfactives et les parfums déjà connus. Grâce à une interface web simple, les utilisateurs peuvent obtenir des suggestions personnalisées en quelques clics seulement.



## Dataset
Le dataset présente des informations sur différents parfums. Il contient trois colonnes : la colonne "brand" indique la marque du parfum, la colonne "perfume" donne le nom du parfum, et la colonne "notes" décrit les accords olfactifs associés à chaque parfum.

<img width="530" alt="Capture d’écran 2024-10-13 183503" src="https://github.com/user-attachments/assets/fc7b37e0-bcad-4b42-b576-d3b804430feb">

## Technologies Utilisées
Python

Pandas

NumPy

Scikit-learn

TfidfVectorizer 

cosine_similarity

Gradio
 
Google Colab et Google Drive 

openpyxl

## Méthodologie

Notre système de recommandation est basé sur le **filtrage basé sur le contenu**, une approche qui recommande des produits similaires à ceux que l'utilisateur apprécie déjà, en se basant sur les caractéristiques du contenu. Dans ce contexte, nous utilisons les notes olfactives des parfums comme caractéristiques principales. Pour évaluer la similitude entre les parfums, nous appliquons la méthode **TF-IDF (Term Frequency-Inverse Document Frequency)**, qui permet de transformer chaque note en un vecteur numérique reflétant son importance. Plus précisément, **TF-IDF** calcule l'importance d'une note en fonction de sa fréquence d'apparition dans un parfum (TF) et de sa rareté dans l'ensemble des parfums (IDF). Ainsi, les notes courantes dans un parfum mais rares dans la base de données globale reçoivent un poids plus important. Cela permet de mieux différencier les parfums en fonction de leurs compositions olfactives. 

Une fois que les notes sont vectorisées, nous appliquons la **similarité cosinus** pour comparer les vecteurs des parfums. Cette technique mesure l'angle entre les vecteurs, et plus ces vecteurs sont proches, plus la similarité entre les parfums est élevée. Ainsi, lorsque l'utilisateur sélectionne des notes ou un parfum qu'il apprécie, le système utilise ces vecteurs pour identifier les parfums ayant des profils olfactifs similaires, et les recommande en fonction des préférences individuelles de l'utilisateur.

## Demo

<img width="774" alt="Capture d’écran 2024-10-14 161506" src="https://github.com/user-attachments/assets/cc2dbc2a-b751-4f30-afba-021c1cfa2a7a">
<img width="811" alt="Capture d’écran 2024-10-14 161652" src="https://github.com/user-attachments/assets/f9956b96-eaae-4ae0-99be-c3392d0b5ad5">
<img width="750" alt="Capture d’écran 2024-10-14 161605" src="https://github.com/user-attachments/assets/459ddca9-4ab0-43cb-8a4c-d8c5a688ab53">
<img width="794" alt="Capture d’écran 2024-10-14 161530" src="https://github.com/user-attachments/assets/cd949416-6144-41d5-a0e4-efb4c694d0d9">
<img width="911" alt="Capture d’écran 2024-10-17 134708" src="https://github.com/user-attachments/assets/d7c05568-926d-4c88-8fa8-3c8758e73dfe">

