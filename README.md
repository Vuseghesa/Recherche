
Attaque par empoisonnement : une menace réel sur les données ?

Objectif de notre étude : examiner le phénomène de l’attaque par empoisonnement de données et son impact sur la sécurité des méthodes d’apprentissage automatique.

Description du contenu de deux fichiers

Nous avons deux fichier différents: l’un contient les codes du modèle normal ou original et l’autre contient les codes du modèle original mais adaptés à notre étude. C’est-à-dire, il y a eu des suppressions, des modifications et des ajouts pour permettre les comparaisons en fonction des besoins de notre recherche. Le principal ajout à ce modèle original, c’est un script qui permet l’empoisonnement à travers lequel nous testons le trois types d’empoisonnement qui constituent la base de notre expérimentation.
	
Nous exploitons dans ces fichiers un ensemble de données (Cf. fichier : Iot_temp.csv ) contenant les relevés de température des dispositifs IoT installés à l'extérieur et à l'intérieur d'une pièce anonyme. Le dispositif était en phase de test. Il a donc été désinstallé ou éteint plusieurs fois pendant toute la période de relevé (du 28-07-2018 au 08-12-2018).

Comme détails techniques, le jeu de données original a 5 colonnes  dont les étiquettes sont : id : identifiants uniques pour chaque relevé,  room_id/id : identifiant de la pièce dans laquelle l'appareil a été installé (à l'intérieur et/ou à l'extérieur), noted_date : date et heure du relevé, temp : relevés de température et out/in : si le relevé a été effectué à partir d'un appareil installé à l'intérieur ou à l'extérieur de la pièce. Au total, ce jeu de données contient 97606 lignes. (Cf. https://www.openml.org/search?type=data&status=active&id=43351&sort=runs ).
Cependant, dans le fichier adapté, nous avons ajouté au jeu de données original deux colonnes : inside et outside pour répondre à certains tests d’analyse dont nous avions besoins. Nous y avons également modifié certaines structures des données sans toucher au contenu afin de faciliter la lecture des résultats. 

Bref, l’étude que nous avons effectuée sur ce jeu de données contenant les relevés des températures, nous permet d’analyser et de comprendre l’impact des attaques par empoisonnement sur la sécurité des méthodes d’apprentissage automatique. Elle nous permet également d’ouvrir notre perspective vers le développement des techniques de défense et de contre-mesures pour atténuer les différents risques liés à ces attaques devenues récurrentes ces derniers temps.
