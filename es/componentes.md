# 3. Components

Els components de Decidim són els mecanismes bàsics de participació que s'activen i configuren per als diferents espais de participació o subespais (fases d'un procés, grups de treball d'un òrgan, etcètera).

## 3.1. Propostes

Les propostes són el component més important de Decidim. S'entén per proposta qualsevol element d'un pla estratègic, una normativa, un pla d'inversió, un canvi legislatiu o qualsevol altra unitat mínima de decisió. Les propostes poden tenir els següents **tipus de creadors**: per la mateixa organització que gestiona la plataforma (p. ex. un ajuntament), per participants registrats/ades, pot originar-se en una trobada com a resultat d'un debat o deliberació col·lectiva, o pot generar-los una assemblea o òrgan, o una organització registrada en la plataforma. També poden **crear-se de manera directa o col·laborativa** i estar subjectes a sistemes d’**esmenes**.

Les propostes estan definides per un/a autor/a, un títol i un contingut de text. També podem incloure **imatges**, **geolocalització** i **arxius adjunts**.

Una vegada publicada, una proposta pot estar subjecta a **moderació** (si algú l'etiqueta com a tal i defineix el motiu de moderació).  

Al tauler **d'administració** les propostes poden **ordenar-se** amb diferents criteris, es poden comentar internament (sense que els comentaris siguin públics), **baixar** en format JSON o CSV (compatible amb programari de fulls de càlcul), **recategoritzar**, o **moure** a diferents espais [aquestes dues últimes funcionalitats estan previstes per a 2017Q4, AjB-Lot3Mod1]. A més, les propostes es poden **acceptar**, **rebutjar** o mantenir en estat d'avaluació.

Altres funcionalitats associades a les propostes són les següents:

* **Control de versions**:** **permet mantenir un registre de tots els canvis realitzats en una proposta, així com la generació de codis de verificació d'integritat de la proposta** **[2017Q3, GenCat].

* **Detecció de similars**: Permet, a qui realitzi una proposta nova, trobar-ne d’altres de similars fetes anteriorment a la plataforma i així evitar duplicats [2017Q4, AjB-Lot3Mod1].

* **Relacions entre propostes**: les propostes poden relacionar-se a través d’enllaços a la secció de comentaris, mostrant-se les propostes relacionades com a targetes i notificant sobre l'existència d'una nova relació. [2017Q4, AjB-Lot3Mod1].

* **Adhesió a propostes**: les organitzacions poden adherir-se a les propostes i aquesta adhesió pública es mostrarà en la proposta i notificarà a participants que segueixin l'activitat de l'organització [2017Q4, AjB-Lot3Mod1].

* **Modificació i retirada de propostes**: l'autor/a d'una proposta pot modificar-la o retirar-la abans que s'obri la fase de recollida de suports [2017Q4, AjB-Lot3Mod1].

* **Esmenes**: qualsevol participant pot editar el text d'una proposta i es crearà una proposta "filla" a tall d'esmena (tipus Pull Request a Github), aquesta proposta filla podrà recollir suports, l'autor/a de la proposta mare podrà acceptar o rebutjar l'esmena (o proposta filla). En cas de rebuig, l'autor/a de la proposta filla podrà elevar-la a proposta oficial [2017Q4, AjB-Lot3Mod1].

* **Creació guiada de propostes**: Durant la creació d'una proposta s'acompanya la persona participant a través del procés dividit en passos, amb ajudes contextuals i previsualització abans d'enviar la proposta [2017Q4, AjB-Lot3Mod1].

* **Incubadora de propostes**: Decidim permet la cocreació i la creació col·laborativa de propostes [funcionalitat prevista per a 2018Q1, AjB-Lot3Mod3]. Incorpora les funcionalitats següents:

    * Creació d'esborranys amb múltiples autors/ores.

    * Llista d’esborranys col·laboratius

    * Comentaris a esborranys

    * Sol·licitar ajuda d'altres col·laboradors i acceptar col·laboradors/ores

    * Vincular l'esborrany a una cita presencial

    * Promoure l'esborrany a iniciativa, proposta de procés o projecte.

## 3.2. Textos participatius

Entenem per text participatiu una col·lecció ordenada de propostes que componen un document de text complet. La participació en el text es deriva de la interacció amb les propostes que la componen. Aquest component permet, fonamentalment, tres operacions [funcionalitat prevista per a 2018Q2, AjB-Lot3Mod4]:

* **Descomposició d'un document de text en propostes ordenades** a partir d'un document en formats ODT, XDOC, MarkDown o HTML. Si el text està estructurat en seccions i subseccions, es crearan propostes ordenades a partir de la subsecció de nivell més baix; si el text no està estructurat, es crearà una proposta per cada paràgraf de text. La interfície permet reeditar les propostes, fusionar-les, separar-les, afegir-hi títols, etcètera.

* **Composició de propostes en un text unificat**: a partir d'una conjunt de propostes, aquestes es podran ordenar i generar un text unificat i descarregable.

* **Visualització i interacció** amb documents compostos de propostes: Es mostrarà la col·lecció de propostes com un text unificat i s’hi podran fer esmenes o comentaris al marge.

## 3.3. Resultats

Els resultats són propostes (o modificacions de propostes) que han acabat sent el resultat de la presa de decisió en el Decidim, de manera directa (mitjançant el resultat de l'aplicació d'un sistema de vot) o bé intervinguda per trobades, assemblees o l'equip tècnic o polític a càrrec d'un àmbit de decisió a través de l'administració de la plataforma.

El component de resultats permet gestionar la **resposta** **oficial **a totes les propostes realitzades: amb el motiu del rebuig o acceptació i en quin resultat ha estat acceptada la proposta.

Els resultats recullen les** metadades de la traçabilitat** de les propostes incorporades en el resultat, així com les trobades en què es va debatre o es va crear (assistents a les trobades esmentades) i la suma de suports rebuts.

## 3.4. Seguiment de resultats

El component de seguiment de resultats permet la **conversió de resultats a projectes** o permet descompondre'ls en projectes o subprojectes. Cada un dels projectes esmentats pot descriure's amb més detall i permet **definir l'estat d'execució**, en trams que van des de 0% d'execució al 100%. El component de seguiment permet, a més, a les persones que visiten la plataforma la **visualització del nivell d'execució** (global, per categories o subcategories), dels resultats i dels projectes. Els resultats, projectes i estats es pot actualitzar mitjançant un CVS i manualment mitjançant la interfície d'administració [funcionalitat disponible per a decidim.barcelona i pendent d'integració en decidim-core, previst per a 2017Q3, AjB].

## 3.5. Votacions i suports

Les persones participants poden donar suports a propostes. Els suports esmentats poden interpretar-se com a vots, signatures, suports, o de qualsevol altra manera que demostri un acord positiu de conformitat amb la voluntat política pròpia.

Hi ha **diferents sistemes de vot i de gestió** a Decidim. El més senzill permet activar els suports i que les participants puguin emetre un suport únic a cada proposta que vulguin, sense límit de propostes votables. També es pot limitar el nombre de vots (p. ex. 10 per cada participant).

Una altra opció és el sistema de vot ponderat per prioritats. Cada participant té un nombre de suports disponible amb diferents pesos, per exemple 3 suports que valen 3, 2 i 1 respectivament, amb la possibilitat de distribuir-los com es cregui convenient [funcionalitat prevista per a 2017Q4, GenCat].

Des del tauler d'administració és possible **configurar la vista dels resultats** de la votació o bé durant el període de vot o només quan aquest s'acabi.

Hi ha una forma de **vot especial per a pressupostos participatius** que permet a participants votar "gastant" una quantitat equivalent al pressuposat objecte de participació entre els projectes proposats. El nombre de vots està limitat aquí per la quantitat de despesa acumulada dels projectes seleccionats.

## 3.6. Comentaris

Els comentaris són un component especial que sol aparèixer associat a un altre component (propostes, debats, resultats, trobades, etcètera) per permetre un procés deliberatiu sobre un tema o proposta.

El sistema de comentaris de Decidim ha estat dissenyat per afavorir la deliberació. Els comentaris de primer nivell, respecte a la finalitat de debat, es poden classificar de la manera següent: **a favor, en contra o neutral**. Els comentaris es poden **niar** en fils de subcomentaris i es poden **votar**. Decidim permet **ordenar comentaris** pels que estan a favor o en contra, en ordre cronològic i per quantitat de vots a favor. També permet **visualització a dues columnes** amb els comentaris més votats a favor i els més votats en contra [aquesta última funcionalitat està prevista per a 2017Q4, GenCat].

## 3.7. Pàgines informatives

Es tracta d'una pàgina amb contingut html i un títol que apareix al menú interior dels espais de participació. Permet incorporar imatges, vídeos encastats i text enriquit.

## 3.8. Debats

Permet obrir debats sobre preguntes o temes específics definits pels administradors o pels participants. [Aquesta funcionalitat està activa només per a decidim.barcelona, s'espera la funcionalitat integrada a Decidim-core per a 2017Q3, GenCat].

## 3.9. Enquestes

El component d'enquestes permet dissenyar, realitzar i visualitzar els resultats d'enquestes que poden activar-se en diferents espais de participació.

* **Configurador d'enquestes**: permet a administradors/ores crear preguntes i respostes (obertes, tipus test, selecció múltiple, etcètera) i activar l'enquesta, i baixar-ne també les respostes en format csv.

* **Interfície d'enquestes per a participants**: permet a les participants respondre a les preguntes de l'enquesta.

* **Visualitzador de resultats**: permet visualitzar els resultats de les enquestes de manera gràfica. [funcionalitat prevista per a 2017Q3, GenCat].

## 3.10. Trobades presencials

Aquest component permet convocar trobades, **establir un calendari**, **geolocalitzar**, penjar les **actes** de la trobada, **debatre**, crear **propostes associades** a la trobada (indicant el tipus de suport col·lectiu a la proposta), recollir el **nombre** de participants, penjar **fotos** de la trobada i **categoritzar** la trobada dins d'un espai.

La **configuració** d'una trobada inclou els **camps bàsics** següents: Títol, descripció, adreça, ubicació, detalls de la ubicació, hora d'inici i acabament, àmbit, categoria i aforament màxim.

També s'inclouen els **camps avançats** següents: caràcter (públic, obert, tancat), grup organitzador, existència d'espai de conciliació, adequació a persones amb diversitat funcional, existència de traducció simultània, tipus de trobada (informatiu, creatiu, deliberatiu, decisiu, avaluatiu, rendició de comptes, d'altres) [funcionalitat prevista per a [2017Q4, AjB-Lot2Mod2]

Les trobades relacionades amb una instància d'un espai (un procés específic o un òrgan) poden mostrar-se en un **mapa** i es poden **ordenar per dates o categories**. També poden mostrar-se totes les trobades en **mode calendari**, amb la possibilitat d'exportar-les a calendaris del mòbil o altres aplicacions [funcionalitat prevista per a [2017Q4, AjB-Lot2Mod2].

Algunes funcions avançades del component trobada inclouen les següents:

* **Sistema d'inscripció i assistència** [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod2]:

    * Permet administrar el **tipus d'inscripció** d'una trobada (obert i automàtic, tancat i accessible només a cert tipus de participants, etcètera), definir el **nombre de places **per a assistents, realitzar **reserves** de places, la **inscripció manual**, enviar **invitacions** i definir tipus de **condicions** que caldrà acceptar per acudir a la trobada (p. ex. cessió de drets d'imatge) i el** registre d'assistència **de participants.

    * Permet a les persones participants la **inscripció** per a una trobada, sol·licitar **servei de conciliació familiar **(ludoteca, espai de cures) i obtenir un **codi per acreditar-se** en presentar-se en la trobada.

    * Les persones inscrites que hagin anat a la trobada tindran** permisos especials** per poder avaluar-la o deixar comentaris i altres accions.

    * Participants o administradors/ores podran rebre **notificacions** sobre l'obertura del període d'inscripció, el nombre de places que queden per inscriure's, recordatoris de la trobada, publicació d'actes.

* **Gestió de l'ordre del dia**: una secció d'ordre del dia permet definir la durada de la trobada, la creació de ítems i subítems de l'ordre del dia, el títol, contingut i durada estimada. Els participants poden proposar punts per a l'ordre del dia. [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod2].

* Sistema de** redacció, publicació i validació d'actes** de reunions [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod2]:

    * Les actes es poden penjar en format vídeo, àudio i text.

    * Les actes en mode text van associades a una **pissarra d'escriptura col·laborativa** integrada a Decidim.

    * Les actes passen per quatre **fases d'elaboració**: 1. Escriptura col·laborativa durant el transcurs de la trobada, 2. Elaboració d'un esborrany oficial de les actes, 3. Fase d'esmenes a l'esborrany, 4. Publicació i validació final de les actes.

    * Les actes es poden **comentar** amb el component de comentaris.

    * Es poden afegir també **documents adjunts** a les actes.

* **Autoconvocatòria**: les persones participants verificades podran convocar reunions a través de la plataforma de manera directa, amb el suport d'un nombre determinat d'altres persones participants s'activarà la trobada públicament i les participants convocants tindran accés al tauler d'administració [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod2]

* **Visualització i exportació de trobades**: les trobades es poden visualitzar en mode mapa (per espais o de manera general a la plataforma), en mode calendari, i es podran exportar a gestors d'agendes i calendaris (en format iCalendar) [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod2].

## 3.11. Jornades

Entenem jornades com un conjunt de trobades que tenen algunes característiques específiques (programa interactiu i descarregable, sistema d'inscripcions, sistema de generació de certificats d'assistència o diplomes).

Decidim disposa d'un configurador i generador de pàgines de jornades, que permet crear un **web intern per a la realització d'esdeveniments** relacionats amb un procés participatiu o un altre espai de participació. [El component Jornades està previst per a 2018Q2, AjB-Lot2Mod5]

Les opcions de configuració inclouen les següents:

* Generació d'un **programa interactiu** de les jornades (en el cas de comptar amb ponents convidats, se n'inclou el nom, càrrec, organització, petita bio, enllaços a altres webs).

* Enviament d’**invitacions** per correu electrònic.

* **Generació de diplomes** de manera automatitzada per a les persones que ho sol·licitin, a través d'un tauler d'assistència que un administrador pugui verificar.

* Enllaços a plataformes de **vídeo i materials** de les jornades en el programa i la documentació.

* Enllaços automàtics a webs de mitjans digitals que donin cobertura a les jornades.

* Seguiment de les jornades per **xarxes socials** (p. ex. incorporant un *feed* de Twitter).

## 3.12. Blog

El blog és un component que permet crear i visualitzar **notícies** en ordre cronològic. Les entrades d'un blog són un altre tipus de contingut, han d'estar associades a una instància d'un espai de participació. Les entrades del blog estan relacionades amb el sistema de classificació de continguts de la plataforma. Els **comentaris associats** a les entrades del blog seran tractats com la resta de comentaris de la plataforma, ja descrits anteriorment [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod1].

## 3.13. Newsletter general i selectiva

Decidim permet enviar una **newsletter** (un correu electrònic) a totes les persones inscrites a la plataforma que hagin acceptat, en les condicions d'ús, rebre el correu electrònic esmentat a tall de butlletí informatiu. La tramesa és personalitzada amb el nom d'usuari/ària i en diversos idiomes (s'envia per defecte en l'idioma escollit per l'usuari/ària).

També poden enviar-se **newsletters selectives** a grups d'usuaris que hagin decidit seguir un procés, òrgan o iniciativa [funcionalitat prevista per a 2017Q3, GenCat].

Les persones participants podran **donar-se de baixa** de manera automàtica i directa des del mateix correu electrònic fent clic en un enllaç, i es podrà fer un **seguiment de visites** derivades dels newsletters [funcionalitat prevista per a 2017Q4, AjB-Lot2Mod1].

## 3.14. Cercador

El **cercador** permet realitzar recerques entre tots els continguts indexables de la plataforma, tant a escala general com en l’àmbit específic, fent la recerca dins d'un procés participatiu concret, o dins dels seus components (propostes, resultats, etcètera) mitjançant la cerca avançada.

La **pàgina navegable i filtrable de resultats de la cerca** mostra els continguts segons la seva tipologia i ordenats segons la prioritat que s'hagi definit (p. ex., que es mostrin primer els termes trobats dins d'assemblees, i a continuació es mostrin els processos participatius.) [funcionalitat prevista per a 2017Q4, AjB-Lot3Mod2]
