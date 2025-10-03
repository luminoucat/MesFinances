```mermaid
graph TD;

    debut(("`**Commencez <br> ici !**`"))

    capacité_épargne("Avez-vous de quoi épargner ? ")

    objectif_financier("Avez-vous un objectif financier défini ?")

    définir_objectif("Définissez un objectif")

    épargne_sécurité("Avez-vous une déjà constitué une épargne de sécurité? (3 à 6 mois de dépenses courantes)")

    %%peaOuvert("Pensez à prendre date sur un PEA !")

    horizon("Quel est votre horizon de placement ?")

    aversionCT("Quelle est votre aversion pour le risque?")

    éligibleLEP("Êtes-vous éligibles au LEP?")

    avertis("Réservé aux investisseurs avertis ou experts :<br> CAT, Fonds Obligataires, Fonds put/write")

    lep("Livret d'Epargne Populaire (LEP)")

    laldds("Livret A / LDDS")

    plein((Choisissez...))

    ccrémunéré("Comptes courants rémunérés")

    fondsmonétaires("Fonds monétaires (CTO, PEA ou AV)")

    aversionMT("Quelle est votre aversion pour le risque?")

    aversionLT("Quelle est votre aversion pour le risque?")

    123("Produits structurés ?<br>Obligations?")

    456("Part en action?<br>Crowdfunding ?")

    etf("ETF selon vos convictions : <br> MSCI World <br> S&P500 <br> NASDAQ100")

    crypto("2 à 5% de votre patrimoine en Bitcoin")

    objectifetf("Quel est votre objectif?")

    défiscalisation("Il va falloir étudier si la défiscalisation est un facteur d'optimisation important")

    av("Assurance Vie")

    pea("Plan Epargne Action (PEA)")

    cto("Compte-Titre Ordinaire (CTO)")

    per("Plan Epargne Retraite (PERin ou PERECO)")

 

    debut-->capacité_épargne

    capacité_épargne--Non, pas encore-->debut;

    capacité_épargne--Oui, j'arrive à mettre des sous de côté régulièrement et à ne plus y toucher-->objectif_financier;

    définir_objectif-->objectif_financier

    objectif_financier--Oui-->épargne_sécurité

    objectif_financier--Un quoi?-->définir_objectif

    épargne_sécurité--Non-->éligibleLEP

    éligibleLEP--Oui-->lep

    lep--Il est plein-->laldds

    av--Elle est pleine-->cto

    laldds--Il sont pleins-->plein

    plein-->ccrémunéré

    plein-->fondsmonétaires

    éligibleLEP--Non-->laldds

    épargne_sécurité--Oui-->horizon

    horizon--Court terme<br> (0 - 5 ans)-->aversionCT

    horizon--Moyen terme<br> (5 - 10 ans)-->aversionMT

    horizon--Long Terme terme<br> (10 ans et plus)-->aversionLT

    aversionCT--Je ne supporte pas le risque-->éligibleLEP

    aversionCT--Je tolère le risque-->avertis

    aversionMT--Je ne supporte pas le risque-->123

    aversionMT--Je tolère le risque-->456

    aversionLT--Je n'aime pas le risque-->etf

    aversionLT--Je tolère le risque-->crypto

    etf--Oui mais sur quel support ?-->objectifetf

    objectifetf--Transmission-->av

    objectifetf--Retraite-->défiscalisation

    défiscalisation--Oui, il l'est-->per

    défiscalisation--Non, il ne l'est pas-->pea

    objectifetf--Autre-->pea

    pea--Il est plein-->cto

   

    %%click capacité_épargne callback "Commençons par le début ! Si vous avez du mal à arrondir vos fins de mois, alors l'investissement n'est pas (encore) pour vous."

    click ccrémunéré "https://www.comparabanques.fr/comparatif-banque/compte-remunere" _blank

     %%style crypto fill:#f9f,stroke:#333,stroke-width:4px

    %%style etf fill:#f9f,stroke:#333,stroke-width:4px
```
Ce diagramme est uniquement à titre informatif pour aider les néophytes à s'y retrouver. Les produits et placements discutés sont à destination de résidents fiscaux Français.
Il ne constitue en rien un conseil en investissement et reflète simplement l'avis d'amateurs éclairés.
Tout placement financier comporte des risques d'illiquidité, de pertes partielles ou totales.
Certaines analyses et avis se basent sur des performances passées. Elles ne garantissent en rien les performances futures.



