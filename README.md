## Regex

*(Samokształcenie: kurs z Udemy)*


---

<br>

### Rozdział pierwszy: Wprowadzenie

<br>

1. **Jakie problemy rozwiązuje RegEx?** <br>

RegEx rozwiązuje 4 konkretne problemy

<br>


1./
> * Sprawdzenie tekstu ze wzorcem.<br>
> np.:<br>
> Sprawdzenie czy format jest taki jakiego oczekujemy.<br>
Wynik: PRAWDA lub FAŁSZ.

<br>


2./
> * Odnalezienie wzorca w tekście (odnalezienie dopasowania).<br>
>np.:<br>
>Wyszukaj godzinę w tekście.<br>
Wynik: znaleziona godzina, pokazanie pozycji, na której się zaczyna i na której się kończy.

<br>


3./
> * Pocięcie tekstu na fragmenty.<br>
> np.:<br>
>Znaleźć godzinę w tekscie. Podzielić ja na godzinę i minuty.
Wynik: np. godzina 16, minuty 58.

<br>


4./
> * Zamiana tekstu
> np.:<br>
>Zamienić kropkę na dwukropek.
Wynik: RegEx to zrobi.

<br>

<br>

2. **Czy RegEx jest uniwersalny?**

> PCRE<br>
*Perl Compatible Regular Expressions* 

<br>

Javascript posiada bardzo ubogą bibliotekę RegEx (np. Python czy C# ma super) ale jedną linijką można dociągnąć świetną bibliotekę xRegEx.

<br>

<br>

3. **Dopasowanie tekstu**

Bardzo wygodne narzędzie: strona [RegEx](https://regex101.com/).

<br>

<br>

4. **Jak myśli RegEx?**

> * RegEx porusza się od lewej do prawej.
>
> * Jego silnik porusza się po jednym znaku.
>
> * Kiedy RegEx dopasuje pierwszy znak, zapamiętuje swoją pozycję i stara się dopasować kolejny znak.
>
> * Jeśli bieżące dopasowanie się nie powiedzie, RegEx zapomni o dotychczas dopasowanych (tym razem) znakach i wróci do ostatnio zapamiętanej pozycji.
> 
> * Kiedy dopasowanie zakończy się sukcesem to RegEx albo zakończy pracę (brak flagi GLOBAL) albo będzie szukał nowych dopasowań dalej (za ostanio skończonym dopasowaniem) ale **nigdy** nie powróci do tekstu, który już raz został dopasowany.
> 
> * Kiedy RegEx masz szukać wszystkich dopasowań (włączona flaga GLOBAL) to zakończy swoją pracę dopiero po dojściu do samego końca tekstu.

<br>

<br>

5. **Klasy znaków**

