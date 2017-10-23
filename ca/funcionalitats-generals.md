# 5. Funcionalitats generals

A continuació s’expliquen una sèrie de funcionalitats i característiques generals de la plataforma que no queden recollides en els espais o components ni en les funcionalitats directament associades a participants.

## 5.1. Instal·lació i configuració

Decidim **s'instal·la fàcilment** a través de la línia d'ordres a qualsevol servidor GNU/Linux amb els següents serveis instal·lats: PostgreSQL 9.4+, Ruby 2.4.1, NodeJS amb yarn (JavaScript dependency manage), ImageMagick i PhantomJS. Un script automàtic d'instal·lació permet desplegar tot el sistema de dependències, llibreries, bases de dades i altres serveis requerits de manera automàtica a Heroku o Docker [funcionalitat prevista per al 2018].

La **configuració** del portal permet una **personalització** amb els camps següents, que s'omplen en un formulari des del tauler d'administració: Nom del portal, perfils de xarxes socials (Twitter, Facebook, Instagram, Youtube, Github), descripció breu, text de benvinguda, idioma per defecte, imatge de portada, logotip de l'organització, favicon, prefix de referència (identificador únic que s'aplicarà als elements del portal) i URL de l'organització.

## 5.2. Integració amb altres serveis i compatibilitat/creació de serveis addicionals

Decidim es pot integrar fàcilment amb els serveis següents, que poden instal·lar-se o configurar-se juntament amb Decidim:

* **OpenStreetMap**: per mostrar esdeveniments i propostes geolocalitzades

* **Piwik**: analítica de visites al web

* **Pad**: pissarres d'escriptura col·laborativa en temps real (tecnologia per determinar) [Funcionalitat prevista per a 2018Q1-3 AjB-Lot1]

* **Identitat i signatura digital**: integració amb el sistema de gestió d'identitat digital OAuth2, sistemes basats en blockchain i sistemes de gestió d'identitat i signatura digital institucionals reconeguts [Funcionalitat prevista per a 2018Q1-3 AjB-Lot1].

* **Sistema distribuït d’arxius**: Difusió o rèplica de propostes o altres elements de la plataforma en sistema distribuïts d’arxius (tipus blockchain o IPFS) [Funcionalitat prevista per a 2018Q1-3, AjB-Lot1].

* **Microblogging**: integració/compatibilitat amb un protocol/servei estandarditzat i obert de microblogging tipus GNU Social o StatusNet per a l'activitat de participants (propostes, comentaris i missatges) [Funcionalitat prevista per a 2018Q1-3, AjB-Lot1].

Decidim genera automàticament els serveis següents, a més d'aquells pels quals es pot navegar mitjançant el web o accedir-hi mitjançant l'API:

* **SMTP**: enviament de correus electrònics.

* **Calendari**: integració o compatibilitat amb sistemes de gestió de calendaris i creació i actualització automàtica de calendaris d'esdeveniments, etcètera [Funcionalitat prevista per a 2018Q1-3, AjB-Lot1].

## 5.3. Multitinença

**Múltiples tinences** de la plataforma poden servir-se partint d'una sola instal·lació. En altres paraules, una sola instal·lació de Decidim permet desplegar tants portals com es vulgui amb una configuració específica per a cada una de les instàncies. D'aquesta manera, una organització pot crear portals de participació per a suborganitzacions seves, o diverses organitzacions poden compartir servidor i reduir els costos de manteniment dels seus portals.

## 5.4. Multiidioma

Decidim és una plataforma **multiidioma**. Durant la instal·lació es configuren els idiomes disponibles. Els menús, formularis d'administració i, en general, els textos fixos de la plataforma estan disponibles en diversos idiomes (català, castellà, eusquera, italià, francès, holandès i suomi). Un sistema de **traducció col·laborativa** a [https://crowdin.com/project/decidim](https://crowdin.com/project/decidim) facilita la incorporació d'idiomes nous a la plataforma.

Pel que fa al contingut, una vegada fixats els idiomes oficials de la instància durant la instal·lació, tots els continguts que es creen des del tauler d'administració tenen l'opció de generar-se en els idiomes esmentats. El tauler d'administració permet la **gestió de continguts en diferents idiomes** a través de pestanyes. El contingut generat per les persones usuàries es mostra a la plataforma en un sol idioma (l'escollit per la persona participant a través del selector d'idiomes en la part superior dels menús o automàticament a través de la configuració lingüística del seu navegador).

## 5.5. Estadístiques, dades obertes i baixades

A més de la interfície de programació d'aplicacions (API) que proporciona accés a dades públiques de manera automàtica, a la portada de Decidim s’hi troba un **quadre d'estadístiques generals**, amb els següents camps: nombre de participants, processos, proposades, resultats, trobades, comentaris i vots.

Un altre **quadre d'estadístiques de cada procés participatiu **mostra el nombre de trobades, propostes, vots i resultats d'un procés determinat.

Des del tauler d'administració es poden **exportar les propostes, resultats i comentaris **d'un procés de participació a format CSV i JSON i respostes a les enquestes per al seu tractament o integració amb altres sistemes de gestió. Les persones participants poden **baixar els resultats d'un procés participatiu i el seu grau d'execució** mitjançant un fitxer CSV.

Decidim disposa també d'un **mòdul de visualització de dades**, tant a escala general de la plataforma com de manera específica (mostrant dades d'un espai participatiu determinat) [funcionalitat prevista per a 2018Q1, AjB-Lot2Mod4]. Entre els gràfics que es mostren hi ha els següents:

* **Gràfic interactiu** de línia temporal amb l'evolució dels comptadors dels diferents components.

* **Mapa de calor** del total de trobades, propostes o altres continguts geolocalitzables.

* **Diagrames interactius **(de barres, circulars o de sectors) amb els resultats d'un procés (import de cada un dels projectes de pressupostos participatius, filtre per categories i estat de les propostes —seleccionades sí o no—, etcètera).

Totes aquestes visualitzacions venen acompanyades d'una **opció de baixada de les dades** en format CSV [funcionalitat prevista per a 2018Q1, AjB-Lot2Mod4].

## 5.6. API, Disseny web adaptable i aplicació mòbil

Decidim disposa d’una interfície de programació d'aplicacions o API que és un conjunt de crides a serveis i dades de forma independent de la interfície web de Decidim. Això permet a tercers desenvolupar serveis sobre la plataforma, alliberar dades de manera automàtica o desenvolupar noves interfícies o integració d'altres serveis amb Decidim.

L'API ve acompanyada d'una **documentació** i una **ontologia formal** de participació [funcionalitat prevista per a 2018Q1-3, AjB-Lot1]

El **disseny** web de Decidim és completament **adaptable** (*responsive*), seguint la filosofia de disseny *mobile-first* (primer es dissenya per al mòbil, després s'expandeix per a sistemes d'escriptori i tauletes tàctils).

Tant el disseny web com l'API faciliten el desenvolupament d'aplicacions mòbils per a Decidim; està previst el desenvolupament d'una **app mòbil** per a finals del 2018 [AjB].

## 5.7. Sistemes de classificació de continguts

Pel que fa a la classificació de continguts, Decidim permet diferenciar i configurar: àmbits, categories i etiquetes (o *tags*).

Els **àmbits** són generals a tota la plataforma i es divideixen en els de tipus **territorial** i **temàtic**. Els àmbits territorials, una vegada definits, permeten classificar elements dels espais territorialment (p. ex. si un procés, o un òrgan o una iniciativa afecta a un districte o dos, a tota la ciutat, a una regió o a un país, depenent de l'organització). Igualment, els àmbits temàtics es defineixen per a tota la plataforma i permeten classificar els diferents elements dels espais de participació [funcionalitat prevista per a 2017Q4, GenCat].

Les **categories i subcategories** serveixen per classificar continguts dins dels diferents espais i es defineixen per a cada una de les instàncies dels espais. Així, per exemple, un procés de participació pot incloure diverses categories i subcategories (les defineix l'administrador/a del procés) i les trobades, enquestes, propostes o altres components del procés es poden classificar sota aquestes categories.

A diferència dels àmbits i les categories, les **etiquetes** o *tags* són transversals, són lliurement definides per les persones participants i es poden aplicar a qualsevol instància o component. Des del tauler d'administració es poden crear etiquetes, niar-les i definir-les. Un sistema de suggeriment d'etiquetes permet a les persones que participen escollir etiquetes similars a les que estan proposant per etiquetar qualsevol element de la plataforma. Es podrà navegar pels elements per etiquetes i mostrar les etiquetes més populars [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod1].

## 5.8. Sistema d'ajuda contextual, tests d'usabilitat i valoració

Decidim inclou un sistema **d'ajudes contextuals editables** per guiar persones participants i administratives en l'ús de la plataforma. Igualment, inclou un sistema que permet fer **experiments d'usabilitat** amb tests i estadístiques d'ús, així com també **enquestes de valoració automàtiques** a les participants de cara a identificar errors d'usabilitat, de procediments de participació i millorar la qualitat democràtica i d'experiència del programari [funcionalitat prevista per a 2018Q1-3, AjB-Lot1].
