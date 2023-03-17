# ETL Basics :

- L'objectif de ce flux de travail est de passer d'une série de contrats avec différents clients dans différents pays à une description synthétique sur une ligne pour chacun des clients.

![image](https://user-images.githubusercontent.com/123749462/225282716-31c4ee3e-cd20-4bfb-82e4-f109eb4cf9b4.png)

# Solution part 2 :

- Drag and Drop le noeud GroupBy :

![image](https://user-images.githubusercontent.com/123749462/225307740-e5d701ba-22c5-4452-91c9-dc8bb57e2f0d.png)

- Ajouter une connexion entre le noeud Column Filter et le noeud GroupBy :

![image](https://user-images.githubusercontent.com/123749462/225307979-6d6f667b-82ac-4c25-a2a8-f59ee142a6d5.png)

- Cliquer sur le noeud GroupBy > Boutton Droit > Configure :(GroupeBy le colonne "Cust_ID") :

![image](https://user-images.githubusercontent.com/123749462/225308536-9e3f8559-9229-440e-ae98-3271c9e7cd80.png)

![image](https://user-images.githubusercontent.com/123749462/225311161-c6ea7336-65da-4f9c-b9a0-78972f02bb49.png)


- Cliquer sur le noeud GroupBy > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225311586-dc0fa5d1-5f57-418d-8a78-ea53ebbeef47.png)

- Drag and Drop le noeud GroupBy :

![image](https://user-images.githubusercontent.com/123749462/225307740-e5d701ba-22c5-4452-91c9-dc8bb57e2f0d.png)

- Ajouter une connexion entre le noeud Column Filter et le noeud GroupBy :

![image](https://user-images.githubusercontent.com/123749462/225311846-3471d930-9518-4a75-beb5-f129b88c4b7a.png)

- Cliquer sur le noeud GroupBy > Boutton Droit > Configure :


![image](https://user-images.githubusercontent.com/123749462/225312307-1616fdbd-d1e8-4d49-b797-cd280eeac335.png)


![image](https://user-images.githubusercontent.com/123749462/225312645-b33c19af-1aa4-4235-82ae-91f75c8d2652.png)


- Cliquer sur le noeud GroupBy > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225313468-ded051d4-b2eb-44ec-8914-58e9e1e2c068.png)

- Drag and Drop le noeud Row Filter : 


![image](https://user-images.githubusercontent.com/123749462/225317780-7a435093-52f7-463d-9272-007c12f57fc5.png)

- Ajouter une connexion entre le premier noeud de GroupBy et le Noeud Row Filter :

![image](https://user-images.githubusercontent.com/123749462/225318596-2790b36a-19ad-44f4-b4a9-5751af7fc1ed.png)


- Cliquer sur le noeud Row Filter > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225322968-c8b29968-a15e-41a9-ae51-d00d8005f774.png)
  

- Cliquer sur le noeud Row Filter > Boutton Droit > Execute :


![image](https://user-images.githubusercontent.com/123749462/225325902-138f31b7-4bf8-49b7-9070-5b154716b6a8.png)

- Drag and Drop un autre noeud Row Filter :

![image](https://user-images.githubusercontent.com/123749462/225326373-d7b4e73d-a3d7-410d-b638-e092029324af.png)

- Ajouter une connexion entre le premier Row Filter et le deuxième Row Filter : 

![image](https://user-images.githubusercontent.com/123749462/225326629-b921a958-5076-4936-96a8-9c199b955db7.png)

- Cliquer sur le noeud Row Filter > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225327091-1eaaba4e-30c9-413c-84a1-c6f2ad18b73b.png)

- Cliquer sur le noeud Row Filter > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225327719-81f1ebaf-aaf9-4347-958c-1608a15d61c7.png)

- Drag and Drop un autre noeud Row Filter : 

![image](https://user-images.githubusercontent.com/123749462/225328315-2412d6f9-43d3-4246-851d-8d3fa8480963.png)

- Ajouter une Connexion entre le Noeud GroupBy et le noeud Row Filter : 

![image](https://user-images.githubusercontent.com/123749462/225335411-ae465f4a-6748-416a-8720-df442f7c697b.png)

- Cliquer sur le noeud Row Filter > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225329502-b5985e7c-e26e-412e-98e7-d434d09976d0.png)

- Cliquer sur le noeud Row Filter > Boutton Droit > Execute :
![image](https://user-images.githubusercontent.com/123749462/225335750-478b20a2-8a87-4ec5-9e78-d8db582f33bb.png)


- Drag and Drop un autre nouw Row Filter : 

![image](https://user-images.githubusercontent.com/123749462/225336015-3ba13c13-a1dd-454d-8145-a024e7e52aa1.png)

- Ajouter une connexion entre le troisième Row Filter et le quatrième Row Filter :

![image](https://user-images.githubusercontent.com/123749462/225336396-ae548be0-7fc6-4d2c-b5a0-37a95416882d.png)


- Cliquer sur le noeud Row Filter > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225338176-61036387-729f-45c5-a990-a8f7f3a61fa6.png)

- Cliquer sur le noeud Row Filter > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225339700-a39074b7-814f-411e-bf9f-b334cea267ff.png)
