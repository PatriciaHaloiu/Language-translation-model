# Proiect IA – Traducere automată cu rețele neuronale (Transformers)

Acest proiect demonstrează implementarea unui sistem de traducere automată multilingv, bazat pe rețele neuronale de tip Transformer (modelul mT5 de la Google).

## Scopul proiectului

Construirea unei rețele neuronale profunde care funcționează ca parte a unei conducte de traducere automată, cu scopul de a obține o acuratețe cât mai ridicată pentru traducerea propozițiilor între limbi (ex: engleză - japoneză).

## Importanța traducerii automate

- **Afaceri**: contracte, investiții, comerț internațional
- **Comerț**: servicii, călătorii, suport clienți
- **Media**: publicitate, rețele sociale, localizare
- **Educație**: colaborare, cercetare
- **Guvern**: diplomație, negocieri

## Pașii realizați

1. Alegerea limbilor de intrare și ieșire (EN - JA).
2. Descărcarea setului de date (`opus100`).
3. Procesarea datelor (tokenizare, indexare).
4. Configurarea modelului `google/mt5-small` și a tokenizer-ului.
5. Antrenarea modelului pe date multilingve.
6. Evaluarea modelului pe setul de test.
7. Generarea de traduceri reale din/în japoneză și engleză.

## Tehnologii utilizate

- **Transformers**: `transformers` de la HuggingFace
- **Datasets**: `datasets` pentru opus100 EN-JA
- **PyTorch**: rețea neuronală și antrenare
- **Colab**: rulare în mediu GPU
- **Vizualizare**: matplotlib, seaborn (plot loss)

## Funcționalități incluse

- Preprocesare și tokenizare cu limbaj markerizat (`<en>`, `<jp>`)
- Generator de date pentru batch-uri custom
- Funcții de evaluare și salvare a modelelor
- Grafic al pierderii pe parcursul antrenării
- Exemplu de inferență pentru input manual

## Rezultat

Modelul antrenat este capabil să traducă propoziții din engleză în japoneză (și invers), folosind un encoder-decoder Transformer pre-antrenat, rafinat pe setul opus100.

## Autor

Proiect educațional de inteligență artificială pentru traducere automată neurală. Implementat în Python cu biblioteci open-source de top (HuggingFace, PyTorch).
