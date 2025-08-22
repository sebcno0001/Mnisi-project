# MNIST Project  

Projekt przedstawia implementację klasyfikatora obrazów ręcznie pisanych cyfr ze zbioru **MNIST** z użyciem **PyTorch**.  

## Opis projektu  
Celem projektu było zbudowanie i wytrenowanie sieci neuronowej, która potrafi rozpoznawać cyfry (0–9) zapisane odręcznie.  
Proces został podzielony na etapy:  
1. Wczytanie danych i ich wstępna analiza.  
2. Przygotowanie datasetów: łączenie, podział na zbiór treningowy i testowy.  
3. Budowa modelu – definicja warstw sieci neuronowej.  
4. Trening – dobór funkcji straty i optymalizatora.  
5. Ewaluacja – testowanie poprawności predykcji na danych testowych.  
6. Wizualizacja wyników – przykłady poprawnych/niepoprawnych klasyfikacji oraz wykres funkcji straty.  
7. Zapis najlepszego modelu.  

## Wymagania  
Projekt powstał w Pythonie 3.  
Niezbędne biblioteki:  
```bash
pip install torch torchvision pandas numpy matplotlib
```

## Uruchomienie  
1. Sklonuj repozytorium:  
   ```bash
   git clone https://github.com/twoj-login/mnist-project.git
   cd mnist-project
   ```
2. Uruchom notebook Jupyter:  
   ```bash
   jupyter notebook "Mnist project.ipynb"
   ```

## Wyniki  
- Model osiąga wysoką dokładność na zbiorze testowym.  
- W notebooku znajdują się przykładowe predykcje wraz z wizualizacją.  
- Dodano wykres strat, aby zobaczyć proces uczenia.  

## Struktura projektu  
```
mnist-project/
│── Mnist project.ipynb   # Notebook z implementacją
│── README.md             # Dokumentacja
```

## Przykłady wyników  
W notebooku znajdują się:  
- Obrazy testowe z zaznaczoną poprawnością predykcji.  
- Wykresy strat w kolejnych epokach.  

## Autor  
Projekt wykonany w ramach nauki głębokiego uczenia z wykorzystaniem PyTorch.  
