# Neural Network from Scratch

Implementazione di una **Rete Neurale Artificiale** costruita esclusivamente con **NumPy**. 

La rete offre una struttura felssibile, è possibile scegliere il numero di Hidden Layers e neuroni.
La struttura è capace di risolvere vari tipi di problemi tra cui:
    - **Regressione** (output lineare).
    - **Classificazione Binaria** (attivazione Sigmoide).
    - **Classificazione Multiclasse** (attivazione Softmax).
Include una implementazione manuale dello Stochastic Gradient Descent (SGD) e un sistema di Backup per il salvataggio automatico dei "Best Weights" durante l'addestramento per prevenire l'overshooting.
---
## Struttura del Codice
Il cuore del progetto è la classe `NeuralNetwork`, che include:
1. **Inizializzazione**: Pesi estratti da una distribuzione uniforme e bias ottimizzati in base all'attivazione scelta.
2. **Forward Pass**: Calcolo delle matrici di attivazione ($A$) e pre-attivazione ($Z$) per ogni layer.
3. **Backward Pass**: Calcolo dei gradienti $\delta$ partendo dall'errore di output e risalendo la rete.
4. **Training**: Ciclo di ottimizzazione con monitoraggio delle metriche (Accuracy o MSE) in tempo reale.
---
## Dataset Testati
La rete è stata validata su tre diversi scenari:
1. Regressione: Predizione del prezzo delle abitazioni.
2. Classificazione Binaria: Diagnosi medica del cancro alla Mammella (benigno/maligno).
3. Classificazione Multiclasse: Riconoscimento di cifre scritte a mano (dataset NMIST).
---
