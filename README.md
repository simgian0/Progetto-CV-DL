# Progetto Computer Vision and Deep Learning

## Indice
- [Introduzione](#intro)
- [Installazione](#install)
- [Funzionamento](#usage)

- [Autori](#autors)

<a name="intro"></a>
## Introduzione
In questo progetto abbiamo preso come caso di studio una rete COIGAN (Controllable Object Inpainting Generative Adversarial Network), analizzando 
in primis la ricerca che ha portato alla creazione di questa rete e, successivamente, andando
a valutare le performance di quest'ultima rispetto a diversi  generatori di immagini presentanti diverse configurazioni

<a name="install"></a>
## Installazione

Per eseguire questo codice è necessario eseguire un container docker che implementi la struttura della rete COIGAN.
Dopo aver eseguito l'accesso al container è necessario sostituire gli script python del modello U-Net in COIGAN/models 
e sostituire i file di configurazione con quelli corrispondenti nella cartella COIGAN/configs.

Per l'installazione completa fare riferimento al repository ufficiale del progetto COIGAN: https://github.com/vrai-group/COIGAN-controllable-object-inpainting

<a name="usage"></a>
## Funzionamento

Per avviare il processo di training è sufficente avviare il comando seguente avendo impostato adeguatamente i file di configurazione.

```
python3 scripts/training.py
```
Per avviare il processo di valutazione del FID score è sufficente avviare il comando seguente avendo impostato adeguatamente i file di configurazione.

```
python3 scripts/evaluate.py
```

## Autori
Il progetto è stato sviluppato dai seguenti studenti dell'Università Politecnica delle Marche:
* Marco Incipini
* Simone Giano
