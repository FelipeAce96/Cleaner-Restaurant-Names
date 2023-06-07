# Cleaner-Restaurant-Names 🍔
Fine tuned model (T5-Google) for clean restaurant names (remove address and stow words automatically) [Spanish]

Given a dataset of inputs (regular name) and outputs (cleaned name) train a sequence to sequence model to learn how to clean names.

## The Model is Saved in Huggingface 🤗

```python
from transformers import AutoTokenizer, AutoModelForSeq2SeqLM

tokenizer = AutoTokenizer.from_pretrained("felipeace96/cleaner-restaurant-names")
model = AutoModelForSeq2SeqLM.from_pretrained("felipeace96/cleaner-restaurant-names")     
```

## RESULTS:

    REGULAR NAME: KFC 232 PIN SAN ANTONI.
    CLEANED NAME: KFC

    REGULAR NAME: SANDWICH DEL CLUB PARQUE LELOIR.
    CLEANED NAME: SANDWICH DEL CLUB


    REGULAR NAME: PIZZAS Y PASTAS BY PPC 39 GIRARDOT.
    CLEANED NAME: PIZZAS Y PASTAS BY PPC


    REGULAR NAME: BURGER KING EUCLIDES MIRAGAIA 22518.
    CLEANED NAME: BURGER KING


    REGULAR NAME: ARROZ PAISA EL ORIGINAL FLORIDABLANCA.
    CLEANED NAME: ARROZ PAISA EL ORIGINAL


    REGULAR NAME: DUNKIN DONUTS COMAS.
    CLEANED NAME: DUNKIN DONUTS


    REGULAR NAME: TOP FRIES CENTRO MAX.
    CLEANED NAME: TOP FRIES
