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
