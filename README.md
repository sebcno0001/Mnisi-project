MNIST Project
Projekt przedstawia implementację klasyfikatora obrazów ręcznie pisanych cyfr ze zbioru MNIST z użyciem PyTorch.
Opis projektu
Celem projektu było zbudowanie i wytrenowanie sieci neuronowej, która potrafi rozpoznawać cyfry (0–9) zapisane odręcznie.
Proces został podzielony na etapy:
Wczytanie danych i ich wstępna analiza.
Przygotowanie datasetów: łączenie, podział na zbiór treningowy i testowy.
Budowa modelu – definicja warstw sieci neuronowej.
Trening – dobór funkcji straty i optymalizatora.
Ewaluacja – testowanie poprawności predykcji na danych testowych.
Wizualizacja wyników – przykłady poprawnych/niepoprawnych klasyfikacji oraz wykres funkcji straty.
Zapis najlepszego modelu.
Wymagania
Projekt powstał w Pythonie 3.
Niezbędne biblioteki:
pip install torch torchvision pandas numpy matplotlib
Uruchomienie
Sklonuj repozytorium:
git clone https://github.com/twoj-login/mnist-project.git
cd mnist-project
Uruchom notebook Jupyter:
jupyter notebook "Mnist project.ipynb"
Wyniki
Model osiąga wysoką dokładność na zbiorze testowym.
W notebooku znajdują się przykładowe predykcje wraz z wizualizacją.
Dodano wykres strat, aby zobaczyć proces uczenia.
Struktura projektu
mnist-project/
│── Mnist project.ipynb   # Notebook z implementacją
│── README.md             # Dokumentacja
Przykłady wyników
W notebooku znajdują się:
Obrazy testowe z zaznaczoną poprawnością predykcji.
Wykresy strat w kolejnych epokach.
