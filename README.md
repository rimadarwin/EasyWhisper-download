# EasyWhisper - download

Installer per Windows di **EasyWhisper**: dettatura vocale locale (nessun dato inviato in rete), con widget in ascolto, note vocali e lettura ad alta voce.

## Installazione

1. Scarica `EasyWhisper_<versione>_x64-setup.exe` dalla pagina [Releases](../../releases/latest).
2. Avvialo. Non servono permessi di amministratore.
   L'installer non è firmato: se Windows mostra «PC protetto», clicca **Ulteriori informazioni** e poi **Esegui comunque**.
3. Al primo avvio apri **Impostazioni** e scarica un modello di trascrizione (consigliato: *small*, circa 190 MB) e, se vuoi la lettura ad alta voce, una voce (pulsante **Scarica**).

## Requisiti

- Windows 10 o 11 a 64 bit.
- La trascrizione usa la scheda video tramite Vulkan quando è disponibile; altrimenti passa da sola al processore (più lento, ma funziona ovunque).

## Uso rapido

- Tieni premuto **Ctrl + Win** per dettare nella finestra in primo piano; **Ctrl + Win + Spazio** per le mani libere.
- **Ctrl + Alt + S** attiva il widget in ascolto: di' la parola chiave seguita da un comando (per esempio «registra», «nuova nota», «leggi», «domanda», «schermo», «nascondi», «disattiva»).
- «cambia widget robottino» cambia l'aspetto del widget (reattore, atomo, DNA, fantasmino, robottino); «legenda» apre l'elenco di tutti i comandi; «istruzioni» legge la guida ad alta voce.
- Nella pagina **Voci** puoi creare una voce personale leggendo un testo di circa 40 secondi.

## Componenti scaricati dall'app

Alcune release di questo repository non sono installer ma componenti che EasyWhisper scarica da solo quando servono:

- `qwentts-<commit>`: server Qwen3-TTS per le **voci personali** (pagina **Voci**), compilato da qwentts.cpp (licenza MIT) con ggml (licenza MIT) e backend Vulkan. Le licenze sono incluse nello zip. I modelli Qwen3-TTS (Apache 2.0) e Pocket TTS (CC BY 4.0) si scaricano direttamente da Hugging Face.
