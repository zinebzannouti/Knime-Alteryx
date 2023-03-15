# ETL Basics :

- L'objectif de ce flux de travail est de passer d'une série de contrats avec différents clients dans différents pays à une description synthétique sur une ligne pour chacun des clients.

![image](https://user-images.githubusercontent.com/123749462/225282716-31c4ee3e-cd20-4bfb-82e4-f109eb4cf9b4.png)


- Créer un nouveau Workflow ETL_Basics :

![image](https://user-images.githubusercontent.com/123749462/225283697-12aa84cf-a491-4be4-97ee-107e4fb5bfd8.png)

- Drag and Drop le noeud CSV Reader :

![image](https://user-images.githubusercontent.com/123749462/225284076-2c1d0bfc-d96b-4a20-9a0b-495aa33bb8d6.png)

![image](https://user-images.githubusercontent.com/123749462/225284275-faf707b3-273e-43bc-8454-67b9acee6275.png)

- Cliquer sur le noeud CSV Reader > Boutton Droit > Configure :
- Ajouter le fichier csv sales_2008_2011 :

![image](https://user-images.githubusercontent.com/123749462/225286026-5e1442ad-503a-4c82-92c0-93a5a295af07.png)

- Cliquer sur le noeud CSV Reader > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225286536-b683a97a-b611-4d06-aab9-8135c179cdf9.png)

- Drag and Drop le noeud String to Date&Time :

![image](https://user-images.githubusercontent.com/123749462/225291215-2c19292d-87d7-4c6e-842e-8eaa02c80e02.png)

![image](https://user-images.githubusercontent.com/123749462/225291354-6f9d6047-3db1-4343-970b-cde2a076a561.png)


- Ajouter une connexion entre le noeud CSV Reader et le noeud String to Date&Time :

![image](https://user-images.githubusercontent.com/123749462/225295569-57293c4f-3a9b-449d-9604-43c092a8778a.png)

- Cliquer sur le noeud String to Date&Time > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225298033-ebb729cc-11ee-4004-8bad-3673ebdb76a3.png)

- Cliquer sur le noeud String to Date&Time > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225298909-9a1f09d1-f529-476c-8d81-aba97cef7ea0.png)

- Drag and Drop le noeud Sorter :

![image](https://user-images.githubusercontent.com/123749462/225300642-125ed89b-1fa0-4ffd-8b2f-30981efd41c2.png)

- Ajouter une connexion entre le noeud String to Date&Time et le noeud Sorter :

![image](https://user-images.githubusercontent.com/123749462/225300944-a817956e-5043-4917-8f92-d61a7b1c547c.png)

- Cliquer sur le noeud Sorter > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225301516-adb126c5-5b34-4890-b0a4-21b2fc835fa0.png)

- Cliquer sur le noeud Sorter > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225303453-bd52e0eb-f612-41c3-90a0-4814e56d985f.png)

- Drag and Drop le noeud Column Filter : 

![image](https://user-images.githubusercontent.com/123749462/225304506-ee5caf6e-24c6-4a08-a77e-c470693c9867.png)

- Ajouter une connexion entre le noeud Sorter et le noeud Column Filter :

![image](https://user-images.githubusercontent.com/123749462/225306583-f512db41-d867-466d-995a-e97f4f40c21e.png)


- Cliquer sur le noeud Column Filter > Boutton Droit > Configure :(Exclure le colonne "card")

![image](https://user-images.githubusercontent.com/123749462/225306853-f2ba632b-536e-45ac-bc2b-df77499a6121.png)

- Cliquer sur le noeud Column Filter > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225307220-e9b7ce14-e05f-4eb3-81bd-4decefa5a5f3.png)

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

- Drag and Drop le noeud Concatenate :

![image](https://user-images.githubusercontent.com/123749462/225340180-bb55003d-7c57-46e4-a2a1-3163a7b4e28c.png)

![image](https://user-images.githubusercontent.com/123749462/225340403-5ca713a1-aef5-4f69-8683-7ce172a8bedf.png)

- Ajouter une connexion entre le deuxième noeud Row Filter et le noeud Concatenate :

![image](https://user-images.githubusercontent.com/123749462/225340761-c0da3e8d-8f5a-4d4e-a686-25aaf9d0fdbd.png)

- Ajouter une autre connexion entre le quatrième noeud Row Filter et le noeud Concatenate :

![image](https://user-images.githubusercontent.com/123749462/225341166-f2fe5494-7c3a-47b8-a6b6-c575feec7802.png)

- Cliquer sur le noeud Concatenate > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225342003-901d2d00-432d-4573-8fe7-6440d124a78b.png)

- Drag and Drop le noeud Joiner : 

![image](https://user-images.githubusercontent.com/123749462/225342874-811e593d-df3b-4a37-bafc-705a812f9424.png)


![image](https://user-images.githubusercontent.com/123749462/225342765-a196dacb-28ee-482b-947b-40240a7db432.png)

- Ajouter une connexion entre le noeud concatenate et le noeud Joiner :

![image](https://user-images.githubusercontent.com/123749462/225343209-8038a0a5-d98f-430a-906a-2d359deda919.png)

- Ajouter une autre connexion entre le noeud Column Filter et le noeud Joiner : 

![image](https://user-images.githubusercontent.com/123749462/225343966-b5f7d5df-700c-4d46-abef-e7ea62d84baa.png)

- Cliquer sur le noeud Joiner > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225346954-02eedbc1-d820-4e54-822c-f4d4980cc8ca.png)

- Cliquer sur le noeud Joiner > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225347624-32c27b0d-d024-4a13-8281-bfcd2d0e474f.png)


- Drag and Drop le noeud CSV Writer :

![image](https://user-images.githubusercontent.com/123749462/225349095-f8cf85bc-7f07-43bc-a0f2-f9f928b71740.png)

![image](https://user-images.githubusercontent.com/123749462/225349418-c19687a8-0200-47d4-9015-3760589ca525.png)

- Ajouter une connexion entre Joinner et CSV Writer : 

![image](https://user-images.githubusercontent.com/123749462/225349635-840cfdf6-3708-4b23-ab42-8ec55687104f.png)

- Cliquer sur le noeud CSV Writer > Boutton Droit > Configure :

![image](https://user-images.githubusercontent.com/123749462/225350264-fb3283e2-a565-49a6-a878-2bcedf0b720b.png)

- Cliquer sur le noeud CSV Writer > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225350454-830e94b5-0347-4551-8373-80b3d789e6fa.png)


















