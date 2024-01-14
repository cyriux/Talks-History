Si vous intervenez sur des architectures logicielles modernes, avec des micro-services ou des monolithes modulaires, alors les termes d'orchestration ou de chorégraphie vous sont probablement déjà familiers. Pourtant de nombreuses confusions existent, avec des interrogations sur les détails de mise en œuvre.

À travers un exercice de code spécialement dédié et très simple, nous examinerons pas-à-pas comment transformer un système d'une de ces approches à l'autre. Nous aborderons ainsi par la pratique les avantages des garanties fortes offertes par l'orchestration, par contraste avec la chorégraphie qui favorise le découplage et facilite ainsi une architecture évolutive.

En s'appuyant sur cet exercice, nous préciserons ce qui distingue ces deux styles et comment les mettre en œuvre de façon concrète pour en tirer le meilleur bénéfice et éviter les travers classiques. Nous ferons le lien avec les patterns correspondants et sur les critères pour choisir sereinement le style adapté à chaque contexte. L'Event-Driven Architecture n'aura alors plus de secret pour vous !

-----
Ce sujet est tiré de l'exercice-phare de notre formation Pragmatic Architecture, qui est une de nos plus populaires (lien Github en notes)
 
Il s'agit de construire un modèle réduit d'un système, d'abord en orchestration, puis de le refactorer en choregraphie en ajoutant un bus. Pour aller vite, tout se fait en simple code, sans aucune technologie lourde. Cela permet donc de jouer très vite avec les alternatives de conception pour bien comprendre les tenants et aboutissants de chaque approche, et ce de façon très concrète.

Puis une fois la pratique vue, nous concluons avec la théorie (slides) pour récapituler et consolider ce qui a été compris. Nous abordons alors les patterns de Domain Events, utiles pour découpler, le pattern "Smart Endpoint et Dumb Pipes" de Sam Newman, le besoin d'un service de type Control Tower pour superviser le tout, et des références à Kafka et les équivalents Cloud pour mettre en oeuvre.

https://github.com/arolla/choreography-kata 
