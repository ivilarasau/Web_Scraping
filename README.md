# Respositori de notícies

**Aleix Martínez** i **Ignasi Vilarasau**

## Context

La realització d'aquesta pràctica s'ha dut a terme en el context de l'assignatura _Tipologia i cicle de vida de les dades_ del Màster de _Data Science_ de la _Universitat Oberta de Catalunya (UOC)_.
En concret en aquesta pràctica ens hem centrat en les dues primeres fases del cicle de les dades, la captura i l'emmagatzematge, utilitzant tècniques de _Web Scraping_. 

## Descripció

Imaginem, per exemple, que una marca de roba vol publicitar-se en la pàgina web d'un diari per intentar guanyar nous clients. En aquest sentit, al diari li interessaria poder disposar d'un dataset propi creat amb tot la informació relacionada amb l'històric de notícies que han anat publicat durant un període de temps en la seva pàgina web i en funció dels resultats de l'estudi de mineria de dades poder oferir una proposta de pressupost a la marca de roba interessada en publicitar-se.

D'aquesta forma hem decidit encarar la pràctica en aquest sentit. Hem recopilat informació relacionada amb les notícies publicades en la pàgina web del diari el País ([El País](http://www.elpais.com/)) per poder crear un dataframe respositori de dades i finalment poder estudiar quines notícies acaben sent més vistes i perquè, i d'aquesta forma poder oferir-li al diari per a que pugui negociar amb propostes de pressupost més alt a marques que volen publicitar-se en la pàgina web del diari.

Per crear el dataset final el que hem fet ha estat anar guardant els arxius _.html_ de la pàgina web del diari El País i un cop guardats, els carregàvem per poder realitzar el web scraping a partir de l'arxiu en local.

Pel dataset triat hem decidit que hauria d'incloure com a mínim els següents atributs:
* **_Extraction Date_:** La data de la captura de les dades de la pàgina web del diari o dels arxius _.html_ emmagatzemats.
* **_Publication Date_:** La data de publicació de l'article en el diari.
* **_Publication Hour_:** L'hora de publicació de l'article en el diari.
* **_Title_:** Títol de l'article publicat en el diari.
* **_Author_:** Autor de l'article del que hem emmagatzemat l'hora i dia de publicació, el títol.
* **_Location_:** Ubicació del succés que explica la notícia de la que hem emmagatzemat l'hora i dia de publicació, el títol i l'autor.
* **_Num Comments_:** Número de comentaris realitzats per usuaris registrats en la pàgina web del diari en la notícia de la que hem emmagatzemat l'hora i dia de publicació, el títol, l'autor i la ubicació.
* **_Photo Author_:** Autor de la fotografia que acompanya l'article del que hem emmagatzemat l'hora i dia de publicació, el títol, l'autor, la ubicació i el número de comentaris.
* **_Photo Text_:** Text del peu de foto de la fotografia que acompanya l'article del que hem emmagatzemat l'hora i dia de publicació, el títol, l'autor, la ubicació, el número de comentaris i l'autor de la fotografia esmentada.
* **_Section_:** Secció a la que pertany la notícia emmagatzemada.
* **_Subsection_:** Subsecció a la que pertany la notícia emmagatzemada.


## Fitxers de codi utilitzats per la tècnica del _Web Scraping_:

* **WebScraping_01.ipynb:** En aquest script el que fem és investigar amb la 
* **WebScraping_ElPais.ipynb:** 
* **WebScraping_ElPais_01.ipynb:** 
* **ElPais_Analysis.ipynb:**

## Bibliografia:

1. Lawson, R. (2015). _Web Scraping with Python_. Packt Publishing Ltd. Chapter 2. Scraping the Data.
2. Mitchel, R. (2015). _Web Scraping with Python: Collecting Data from the Modern Web_. O'Reilly Media, Inc. Chapter 1. Your First Web Scraper.
3. Simon Munzert, Christian Rubba, Peter Meißner, Dominic Nyhuis. (2015). _Automated Data Collection with R: A Practical Guide to Web Scraping and Text Mining_. John Wiley & Sons
4. Subirats, L., Calvo, M. (2018). _Web Scraping_. Editorial UOC.
5. Masip, D. (2010). _El lenguaje Python_. Editorial UOC.


