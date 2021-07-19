---
layout: post
title: EEG Analysis
subtitle: Stroke rehab and machine learning methods
gh-repo: pietro-sillano/Stroke_Rehab_EEG
gh-badge: [star, fork, follow]
tags: [test]
comments: true
cover-img: ../assets/img/eeg.jpeg
---


# Riabilitazione da Ictus con BCI
***
Questo progetto nasce durante l'hackathon BR4IN.IO 2021 organizzato da g-tec. 

Abbiamo analizzato un dataset di segnali ottenuti con una Brain Computer Interfaces (BCI) da **pazienti con ictus cronico**. Negli ultimi anni, le BCI sono state ampiamente utilizzate come **strumenti di riabilitazione** per recuperare la funzionalitá degli arti.

Nello specifico siamo nell'ambito della Motor Imagery (Immaginazione del movimento) grazie ai BCI, possiamo rilevare i segnali cerebrali e usarli per riconoscere la volontà del soggetto di muovere una parte del proprio corpo. Infatti, prima di eseguire un movimento, lo possiamo richiamare nella nostra mente e attiviamo una specifica area cerebrale. 

Questo segnale può essere registrato e interpretato per migliorare una terapia di riabilitazione.

Viene usato un **elettrostimolatore** per far compiere il movimento ai muscoli dell'avambraccio e muovere l'arto. 


#### **Ma qual è il nostro obiettivo?**
Nel nostro caso dovevamo classificare il segnale  mano sinistra o mano destra.

Abbiamo cercato di implementare il miglior classificatore in diverse situazioni:


* miglior classificatore specifico per paziente
* miglior classificatore per modello generalizzato 
