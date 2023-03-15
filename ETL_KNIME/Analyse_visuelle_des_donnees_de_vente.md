# Analyse visuelle des données de vente :

- Filtrer les données sur les colonnes contenant des informations pertinentes
- Filtrer les données sur les lignes que vous souhaitez inclure dans votre analyse
- Visualiser les données à l'aide d'un Stacked Area Chart et d'un Pie/Donut Chart.

![image](https://user-images.githubusercontent.com/123749462/224999108-3fbf2bf8-df31-43d9-9534-765d661d08c6.png)

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

## 2.Prétraitement des données : 

- Drag and Drop le noeud Column Filter 

![image](https://user-images.githubusercontent.com/123749462/225006437-d37e6c73-728b-4d0b-bb3c-beec5ac87351.png)

![image](https://user-images.githubusercontent.com/123749462/225006560-54600b9b-0d56-4a42-88ea-5a5a47f6966c.png)


- Ajouter une connexion entre CSV Reader et Column Filter :

![image](https://user-images.githubusercontent.com/123749462/225006831-2993f2d6-6244-4698-9c9b-4eea4c9f0c49.png)

- Cliquer sur CSV Reader > Column Filter > Configure

- Sélectionnez les colonnes "country", "date" et "amount". 

![image](https://user-images.githubusercontent.com/123749462/225007354-701be3e7-0f8b-4e38-9bca-8677c995c1ea.png)

- Cliquer sur Column Filter > Boutton droit > Execute 

![image](https://user-images.githubusercontent.com/123749462/225013758-33063a1d-071c-429e-927f-a2469500d4ca.png)

- Drag and Drop le noeud Row filter :

![image](https://user-images.githubusercontent.com/123749462/225014399-69f32108-40d4-4ebe-ac0a-4b5d295c7548.png)

- Ajouter une connexion entre Column Filter et Row Filter : 

![image](https://user-images.githubusercontent.com/123749462/225014722-c97a23b4-a210-42d0-a09f-036960dd1e4a.png)

- Cliquer sur Row Filter > Boutton droit > Configure 
- Exclure les lignes où "country" est "Unkown"

![image](https://user-images.githubusercontent.com/123749462/225025120-03f2dc07-41e3-43bd-b94c-eedbe730007e.png)

- Cliquer sur Row Filter > Boutton droit > Execute

![image](https://user-images.githubusercontent.com/123749462/225017259-5e5a082b-1f83-4148-98e2-ae33b12f0200.png)

## 3.Visualisation des données :
- Drag and Drop le noeud Stacked Area Chart :

![image](https://user-images.githubusercontent.com/123749462/225022857-95f4b958-0d84-474a-b856-a78701368353.png)

- Ajouter une connexion entre Row filter et Stacked Area Chart :

![image](https://user-images.githubusercontent.com/123749462/225023203-b58dbced-12a1-44aa-8930-2e6056e830dc.png)

- Cliquer sur Stacked Area Chart > Boutton droit > Configure 

![image](https://user-images.githubusercontent.com/123749462/225023838-ec6a9635-1ba8-402e-9574-89bd145f2b66.png)

- Cliquer sur Stacked Area Chart > Boutton droit > Execute
- Cliquer sur Stacked Area Chart > Boutton droit > Interactive View :JavaScript Stacked Area Chart

![image](https://user-images.githubusercontent.com/123749462/225025636-af15bafe-2759-40f7-aded-78bc28675f73.png)

- Drage and Drop le noeud Color Manager :

![image](https://user-images.githubusercontent.com/123749462/225026420-b3a56b7e-6042-4db7-9562-8376a08acd1e.png)

- Ajouter une connexion entre Row Filter et Color Manager : 

![image](https://user-images.githubusercontent.com/123749462/225026730-992279e4-5ab9-4b26-bfb6-e97cd2ef2778.png)

- Cliquer sur Color Manager > Boutton droit > Configure 

![image](https://user-images.githubusercontent.com/123749462/225029706-7cf28d90-33d9-47e0-85e6-ffb52878f297.png)

- Cliquer sur Color Manager > Boutton droit > Execute
- Drag and Drop le noeud Pie/Donut Chart :

![image](https://user-images.githubusercontent.com/123749462/225032071-80feefa9-1c46-41a8-ba5a-3c3749696c99.png)

- Ajouter une connexion entre Color Manager et Pie/Donut Chart :

![image](https://user-images.githubusercontent.com/123749462/225032659-cafacdf7-0020-4e84-ab1f-31256eb99d46.png)


- Cliquer sur Pie/Donut Chart > Boutton droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225033641-7971aec4-49cf-4592-8deb-bc55f88e3642.png)

- Cliquer sur Pie/Donut Chart > Boutton droit > Interactive View :Grouped Pie Chart


![image](https://user-images.githubusercontent.com/123749462/225034039-94245dd3-2511-4487-8205-fe9c5c1bd9da.png)






