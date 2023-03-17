# ETL Basics :

- L'objectif de ce flux de travail est de passer d'une série de contrats avec différents clients dans différents pays à une description synthétique sur une ligne pour chacun des clients.

![image](https://user-images.githubusercontent.com/123749462/225282716-31c4ee3e-cd20-4bfb-82e4-f109eb4cf9b4.png)

# Solution part 3 :
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

![image](https://user-images.githubusercontent.com/123749462/225353088-ba7c0306-3238-4175-9316-cbe37a34ea1c.png)

- Cliquer sur le noeud CSV Writer > Boutton Droit > Execute :

![image](https://user-images.githubusercontent.com/123749462/225350454-830e94b5-0347-4551-8373-80b3d789e6fa.png)

- Vous pouvez maintenant voir le fichier qu'on a obtenu comme Output dans le chemain que vous avez spécifier





