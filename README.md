# Esempio di applicazione di classificazione video basata su TensorFlow Lite

## Overview

L'applicazione è stata sviluppata come progetto d'esame per il corso di Sistemi Digitali M. È un esempio di applicazione Android che classifica in modo continuo le azioni svolte in un frame video fornito in input mediante la fotocamera posteriore di uno smartphone e si basa su TensorFlow Lite. L'inferenza è realizzata mediante le API Java fornite da TensorFlow Lite. L'applicazione consente all'utente stesso di utilizzare le diverse varianti dei modelli [MoviNet](https://tfhub.dev/s?deployment-format=lite&q=movinet).

### Modelli

Nell'applicazione vengono forniti 3 modelli, quantizzati con int8:
* MoviNet-A0
* MoviNet-A1
* MoviNet-A2

MoviNet-A0 è il più piccolo, il più veloce, ma il meno accurato rispetto ad A1 e A2, mentre MoviNet-A2 è il più grande, il più lento, ma offre un'accuratezza maggiore.

Downloading, extracting, and placing the model in the assets folder is managed
automatically by 
Download, unzip, e sistemazione del modello nel folder assets sono gestiti automaticamente dal file download.gradle.

## Requisiti

*   Android Studio Bumblebee | 2021.1.1 o successive (installate su una macchina Linux, Mac o Windows)

*   Dispositivo Android in modalità
    [developer mode](https://developer.android.com/studio/debug/dev-options)
    con USB debugging abilitato

*   Cavo USB (per collegare il dispositivo Android al pc)

####Demo
L'applicazione è costituita da una view in cui nella parte superiore è mostrato lo stream video in ingresso, mentre nella parte inferiore sono presenti la label dell'attività, l'accuratezza, il modello MoviNet scelto e un bottone per effettuare il reset del modello.

<img width="491" alt="Screenshot 2023-01-26 alle 14 01 39" src="https://user-images.githubusercontent.com/109990354/214842145-3b26e711-3bd9-40a0-bd9f-a6934d6b662d.png">



