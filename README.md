# przewidywanie-jakosci-wina-regresja
## Przewidywanie jakości wina - model regresji
Modyfikacja projektu zaliczeniowego w ramach przedmiotu *Uczenie maszynowe w języku Python* studiów podyplomowych.

### Opis problemu
Pozyskano dwa zbiory danych w postaci pliku csv (dla wina czerwonego i białego) ze strony:

https://archive.ics.uci.edu/dataset/186/wine+quality.

Zbiór danych posiada 11 atrybutów warunkowych oraz 
* 1599 przypadków w zbiorze wina czerwonego,
* 4898 przypadków w zbiorze wina białego.

Ostatnia kolumna reprezentuje cechę decyzyjną (ocenę jakości). Dane nie są zbalansowane (jest dużo więcej rekordów win o normalnej jakości w porównaniu do win wyśmienitych i słabych).

Celem jest znalezienie modelu regresji o najwyższej jakości i dokładności spośród rozważanych, który przewidywałby jakość wina w zalezności od zadanych parametrów.

Rozważone zostaną dwa warianty podejścia do zadania:
* w pierwszym modele trenowane będą osobno dla wina czerwonego i białego
* w wariancie 2 oba zbiory danych zostaną połączone, kolor wina będzie traktowany jako kolejny atrybut.

### Aspekt techniczny
W projekcie porównano ze sobą:
* DecisionTreeRegressor,
* KNeighborsRegressor,
* GradientBoostingRegressor,
* RandomForestRegressor,
* LinearRegression

Pozostałe zagadnienia:
* mean_squared_error,
* mean_absolute_error,
* r2_score

*Tools: pandas, numpy, matplotlib, sklearn*

