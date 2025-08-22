# Projekt klasyfikacji obrazów – Dice & EMNIST  

Projekt obejmuje trzy etapy pracy z obrazami zapisanymi w plikach CSV, przy użyciu narzędzi **Python** i **PyTorch**. Dane obejmują zarówno obrazy kostek do gry (`dice_ext.csv`), jak i litery (`emnist_letters.csv`).  
Ze względu na rozmiar plików dane nie są przechowywane w repozytorium.  

## Etap 1 – kontrola danych  
Sprawdzenie poprawności zbioru danych `dice_ext.csv`:  
- weryfikacja dostępności danych,  
- sprawdzenie liczby próbek i ich zgodności z opisem,  
- wizualizacja przykładowego obrazu.  

## Etap 2 – klasyfikacja według liczby oczek  
Celem etapu jest zbudowanie modelu klasyfikującego obrazy kostek (`dice_ext.csv`):  
- jeżeli kostka jest niepoprawna – model rozpoznaje ten fakt,  
- jeżeli kostka jest poprawna – model rozpoznaje liczbę oczek (od 1 do 6).  

Możliwe podejścia:  
- jeden model klasyfikujący,  
- dwa modele połączone (ensemble),  
- jeden model wsparty dodatkowym kodem.  

## Etap 3 – klasyfikacja do domeny  
Budowany jest model rozróżniający domenę obrazu. Wykorzystywane są dwa zbiory:  
- `dice_ext.csv` (kostki – poprawne i niepoprawne),  
- `emnist_letters.csv` (litery).  

Model klasyfikuje każdy obraz do jednej z domen.  
Miara jakości: **dokładność (accuracy)**.  

## Wymagania  
Projekt powstał w Pythonie 3.  
Wymagane biblioteki:  
```bash
pip install torch torchvision pandas numpy matplotlib
```

## Uruchomienie  
1. Sklonuj repozytorium:  
   ```bash
   git clone https://github.com/twoj-login/dice-emnist-classification.git
   cd dice-emnist-classification
   ```
2. Uruchom notebook Jupyter:  
   ```bash
   jupyter notebook "Projekt.ipynb"
   ```  

## Struktura projektu  
```
dice-emnist-classification/
│── Projekt.ipynb          # Notebook z implementacją
│── README.md              # Dokumentacja
```

## Autor  
Projekt wykonany w ramach kursu z zakresu uczenia maszynowego i sieci neuronowych.  
