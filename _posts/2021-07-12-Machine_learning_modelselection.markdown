---
layout: post
title: "Korte handleiding voor het selecteren van machine learning modellen"
date: 2021-07-12 13:32:20 +0300
description: Korte handleiding voor het selecteren van machine learning modellen. # Add post description (optional)
img: machine_learn.jpg # Add image post (optional)
tags: [Model selecetion, Machine learning] # add tag
---

Het vinden van het beste algoritme voor machine learning voor uw probleem kan een uitdaging zijn als u genoeg tijd en middelen heeft om alle mogelijke algoritmen uit te proberen en het beste te kiezen. Meestal hebben we daar echter niet genoeg tijd voor. Gegeven de volgende zeven criteria om op te kiezen, wat zal helpen om uw keuzes op een shortlist te zetten zodat u ze in korte tijd kunt toepassen.m op te kiezen, wat zal helpen om uw keuzes op een shortlist te zetten zodat u ze in korte tijd kunt toepassen.

**Verklaarbaarheid**

Het eerste criterium om uw model op te kiezen, is verklaarbaarheid. Als u het model moet uitleggen en waarom het bepaalde output oplevert voor een niet-technisch publiek, zoals belanghebbenden of zakenpartners. Als je model bijvoorbeeld voorspelt dat iemand geen lening zou moeten krijgen, zou je de reden achter deze beslissing moeten kunnen uitleggen, ook dit is een belangrijk punt voor medische AI. Modellen zoals KNN, lineaire regressie en beslissingsbomen zouden een goede keuze zijn, aangezien de beslissingsgrenzen kunnen worden gevisualiseerd en de resultaten in niet-technische termen kunnen worden geïnterpreteerd.
Er is echter een wisselwerking tussen verklaarbaarheid en modelprestaties. Vaak zal het gebruik van een complexer model de prestaties verhogen, maar het zal moeilijker te interpreteren zijn. Daarom, als het niet nodig is om het model en de output aan een niet-technisch publiek uit te leggen, dan zouden meer complexe modellen kunnen worden gebruikt, zoals ensembleleerders en diepe neurale netwerken.

**In geheugen versus uit geheugen**

het is belangrijk om rekening te houden met het relatieve volume van uw gegevens ten opzichte van het opslagvolume van het RAM-geheugen van de server of uw pc waarop de training zal plaatsvinden. Als het RAM-geheugen alle trainingsgegevens aankan, kunt u kiezen uit een breed scala aan machine learning-algoritmen. Als het RAM de trainingsgegevens niet aankan, zijn daarom verschillende incrementele leeralgoritmen, die het model kunnen verbeteren door geleidelijk meer trainingsgegevens toe te voegen, een goede keuze.

**Aantal functies en voorbeelden**

Het aantal trainingsvoorbeelden en het aantal functies per voorbeeld zijn ook zeer belangrijke criteria om uw trainingsmodel op te kiezen. Als je een klein aantal voorbeelden en functies hebt, dan zou een eenvoudige leerling een goede keuze zijn, zoals een beslisboom en KNN. Als u een klein aantal voorbeelden en een groot aantal functies hebt, zouden SVM- en gaussiaanse processen een goede keuze zijn, omdat ze een groot aantal functies aankunnen, maar zeer bescheiden zijn in hun capaciteit. Als je een groot aantal voorbeelden hebt, zijn diepe neurale netwerken en stimulerende algoritmen een goede keuze, omdat ze miljoenen voorbeelden en functies aankunnen. U moet echter voldoende reken- en opslagkracht hebben om ze aan te kunnen.

**Categorische versus numerieke kenmerken**

Het type van uw functies is ook een belangrijk criterium om uw model op te kiezen. Sommige algoritmen voor machine learning kunnen categorische kenmerken zoals lineaire regressies niet aan en u moet ze omzetten in numerieke kenmerken. Anderen kunnen omgaan met categorische kenmerken en numerieke kenmerken zoals beslisbomen en willekeurige bossen.

**Normaliteit van gegevens**

Als uw gegevens lineair scheidbaar zijn of kunnen worden gemodelleerd met behulp van een lineair model, kan SVM met lineaire kernel of logistische regressie of lineair regressiemodel worden gebruikt. Als uw gegevens niet-lineair scheidbaar of niet-lineair gemodelleerd zijn, zouden diepe neurale netwerken of ensembleleerlingen een goede keuze moeten zijn.

**Trainingssnelheid**

De beschikbare tijd voor training is ook een ander belangrijk criterium om je trainingsmodel op te kiezen. Eenvoudige algoritmen zoals logistische en lineaire regressie of beslisbomen kunnen in korte tijd worden getraind. Het is bekend dat complexe algoritmen zoals neurale netwerken en ensembleleerders traag zijn om te trainen. Als u echter toegang heeft tot een multi-core machine, kan dit de trainingstijd van complexere algoritmen aanzienlijk verkorten.

**Voorspellingssnelheid**

De snelheid waarmee de resultaten worden gegenereerd, is een zeer belangrijk criterium om uw model op te kiezen. Als uw model in realtime of in een productieomgeving wordt gebruikt, moet het de resultaten met een zeer lage latentie kunnen genereren. In dit geval zijn algoritmen zoals SVM's, lineaire en logistische regressie en sommige soorten neurale netwerken extreem snel op het voorspellingstijdstip. Houd er ook rekening mee op welke computationele lokalen u uw model gaat implementeren. Als u de modellen gebruikt voor meer analytische of theoretische doeleinden, kan uw voorspellingstijd langer zijn, dan kunt u ensemble-algoritmen en zeer diepe neurale netwerken gebruiken.
Het kiezen van het beste model voor uw probleem kan een uitdagend probleem zijn dat veel praktische ervaring en een diep begrip van verschillende machine learning-modellen vereist. Ik ben echter van mening dat het gebruik van de genoemde criteria u zal helpen de keuzes te verkleinen en u rekenkracht en tijd zal besparen.
