# Analyse visuelle des données de vente :

- Filtrer les données sur les colonnes contenant des informations pertinentes
- Filtrer les données sur les lignes que vous souhaitez inclure dans votre analyse
- Visualiser les données à l'aide d'un Stacked Area Chart et d'un Pie/Donut Chart.

![image](https://user-images.githubusercontent.com/123749462/224999108-3fbf2bf8-df31-43d9-9534-765d661d08c6.png)

# Solution
## 1.Accès aux données : 

- Créer un nouveau Knime Workflow :

![image](https://user-images.githubusercontent.com/123749462/225000586-fe6f9846-181d-4cca-9088-2239aa0e0235.png)

- Drag and Drop le noeud CSV Reader :

![image](https://user-images.githubusercontent.com/123749462/225001234-06fc28df-1059-4778-bbcf-2ac388953527.png)

![image](https://user-images.githubusercontent.com/123749462/225001941-be87cc2e-98e2-4d8d-b7a5-dab19b28f4e8.png)

- Cliquer sur CSV Reader > Boutton droit > Configure 
- Ajouter le fichier csv : sales_2008_2011.csv

![image](https://user-images.githubusercontent.com/123749462/225002931-541331b1-b501-46da-a319-be615b19afce.png)

- Cliquer sur CSV Reader > Boutton droit > Execute 

![image](https://user-images.githubusercontent.com/123749462/225004217-3cba9712-ce6b-4b61-b77c-4c2f823f94a1.png)

- Une fois que vous avez exécuter le noeud vous allez avoir la couleur verte sur le noeud :

![image](https://user-images.githubusercontent.com/123749462/225004842-b6ef9238-3897-44a0-9e88-518e19f41e9f.png)
