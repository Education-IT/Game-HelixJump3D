![enter image description here](https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/banner.png?token=GHSAT0AAAAAAB2TICAR6ZT3K4Q2WZFDBRW6Y3JEIDA)
<img src="https://github.com/Education-IT/Game-HelixJump3D/blob/main/images/game.gif?raw=true" alt="Ball jumping" height=655 align="right">

### Projekt zaliczeniowy na przedmiot - ***Labolatorium Systemów Mobilnych*** - **UAM** 

> **Zrealizowano w czwartym semestrze studiów informatycznych.**



Zadanie polegało na stworzeniu aplikacji mobilnej zawierającej wyznaczone przez prowadzącego - elementy. Stworzyłem kopię znanej gry - **Helix Jump**. Mój projekt stworzyłem w **Unity** za pomocą języka **C#**.  To była moja pierwsza styczność z tym środowiskiem. Gra działa wyłącznie na telefony z systemem Android. Znajdują się w niej **powiadomienia** zachęcające do gry jak i komunikujące postęp w grze (**osiągnięcia**). Umieściłem również **reklamy** unity - **banery**. Głównym celem tej gry jest pokonanie przeszkód (okręgów - a dokładniej *czerwonych* elementów)  i dotarcie do *mety* - naszą postacią - *kulką*. 



 ![enter image description here](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white) ![enter image description here](https://img.shields.io/badge/Android-3DDC84.svg?style=for-the-badge&logo=Android&logoColor=white) ![enter image description here](https://img.shields.io/badge/blender-%23F5792A.svg?style=for-the-badge&logo=blender&logoColor=white) ![enter image description here](https://img.shields.io/badge/Unity-100000?style=for-the-badge&logo=unity&logoColor=white)[ ![enter image description here](https://img.shields.io/badge/website-000000?style=for-the-badge&logo=About.me&logoColor=white)](https://education-it.pl/)
 ### *Gra Helix-Jump :*
 ***Menu gry:***
 <ol type=A>
<li>wyciszenie gry. </li>
<li>wyjście z aplikacji - generuje to 3 powiadomienia które to mają zachęcić do powrotu do gry. Odpowiednio zostaną wyświetlone po 3s / 15 min / 1 godz. </li>
<li>Zmiana "skórki" - naszej kulki - którą gramy. Mamy do wyboru 4 opcje: Piłkę nożną, jabłko, cebulę i piłkę golfową.</li>
<li>Restart naszego postępu - restuje się High Score / poziom / skórka kulki.</li>
<li>Rozpoczęcie gry.</li>
</ol>



--------------------------------------
<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/changeCharacter.jpg" height=200 align=right>

1. Wszystkie elementy w grze zostały stworzone własnoręcznie za pomocą dostępnych darmowych narzędzi.
Okręgi są **generowane losowo** z "bazy okręgów". Wszystkie obiekty 3D - Okręgi / Skórki kulki -> zostały również stworzone przeze mnie za pomocą programu **Blender**.

2. Gra zaczyna się od pierwszego poziomu na którym należy pokonać jedną przeszkodę ( okrąg ) każdy następny poziom to analogicznie -> **numer poziomu = ilość przeszkód**.

---

3. Po upadnięciu na *zielone* pole - nalicza się ogólna ilość skoków naszej kulki (**osiągnięcia**). Po każdym upadku,
kulka zostawia po sobie mokrą plamkę której rozmiar jest wybierany **losowo** przez metodę `random()`.

4. Po upadnięciu na *czerwone* pole - *przegrywamy*! Pojawia się ekran "Game Over" i możliwość powrotu do menu głównego. Wyświetlany jest **baner reklamowy** na samym dole ekranu. Mogą pojawić się powiadomienia o ile zdobyliśmy jakieś osiągnięcie. W trakcie faktycznej gry baner reklamowy znika - aby nie irytować użytkownika.

5. Po upadnięciu na ostatni - *czarny okrąg* - zwyciężamy i możemy przejść do następnego poziomu. Pojawia się ekran "wygranej". Pojawia się baner reklamowy na samym dole ekranu. Możliwe pojawienie się powiadomień o ile zdobyliśmy jakieś osiągnięcie. W trakcie faktycznej gry baner znika - aby nie irytować użytkownika.

<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/addBaner.PNG" align=middle width=100%>

--------------------------------------

6. Po *"Przefrunięciu"* przez dziurę w okręgu - naliczają się punkty które następnie trafiają do zmiennej `HighScore`. HighScore jak i numer poziomu **NIE** resetują się po wyjściu z aplikacji. 
Po pokonaniu okręgu, następuje jego zniszczenie i rozlecenie na wszystkie strony. 

7. W trakcie gry widać pasek postępu oraz ilość zdobytych punktów bez "skucia".
HighScore zapisuje się dopiero w **trakcie przegranej**. 

8. W trakcie bycia w menu / na ekranie "game Over" / "win" - kulka nie nalicza skoków do łącznej puli skoków (osięgnięcia-powiadomienia) mimo że się odbija. 

--------------------------------------

9. Nowe powiadomienia nadpisują/usuwają stare - niewyświetlone powiadomienia - jest to system antyspamowy - aktualnie widoczne powiadomienie - zawiera najbardziej aktualną informację.
<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/Notification2.PNG" height=250>

<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/Notification1.PNG" height=200 >

----

10. Muzyka została przeze mnie skrócona i zapętlona. Wszystkie dźwięki są na licencji umożliwiającej mi wszelkie zmiany i czerpanie korzyści majątkowych z mojej aplikacji.

--------------------------------------

11. Aplikacja jest stabilna - nie zawiera łatwo wykrywalnych błędów. W aktualnej wersji ich nie dostrzegam. (przez cały etap produkcji miałem dostęp do opinii moich testerów - partnerki, siostry i rodziców. Dzięki czemu wszelkie błędy zostały zidentyfikowane i niezwłocznie naprawione. 


## Instalacja:
1. Zezwól swojemu smartphon'owi na instalowanie **"nieznanych aplikacji"** z **"moich plików"** (na przykładzie `samsung galaxy S5 NEO`):
- Wejdź w **ustawienia**.
- Wejdź w **"biometria i zabezpieczenia"**.
- Wejdź w **"zainstaluj nieznane aplikacje"**.
- Znajdź **"Moje pliki"** i następnie zaznacz opcję: **"Zezwalaj z tego źródła"**.
2. Pobierz grę `helixjump3D` z mojego repozytorium.
3. Wejdź w **"Moje pliki"** i wyszukaj pobraną grę **"xHelixJump3D"** - następnie kliknij w jej ikonę i zaznacz **"instaluj"**.
4. Zainstalowaną grę można znaleźć już wśród innych aplikacji.
5. Dobrej zabawy! 🥇 ( wersja gry w repozytorium - **NIE ZAWIERA REKLAM!** 😃 )


## Czego się nauczyłem:
<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/apple.gif" align=right>

- Miałem ogromny problem ze skryptem niszczącym pokonywane okręgi - ponieważ wykorzystywałem do tego metodę  `AddExplosionForce()` która sprawiała, że moja piłeczka obłędnie mocno przyspieszała, co generowało liczne bagi.   Szukałem rozwiązań przez wiele godzin. Wpadłem jednak na pomysł aby znacznie zmniejszyć ciężar/wagę owych okręgów z wartości **1** *na* **0.05**. Dzięki tej zmianie - okręgi reagują bardzo mocno nawet na mikroskopijny wybuch który niemal  w ogóle nie wpływa na piłkę :)
- Mimo że w trakcie trwania semestru na zajęciach używaliśmy Kotlina i Android Studio - postawiłem sobie wyzwanie aby stworzyć grę za pomocą innych wcześniej mi nie znanych narzędzi. Wybrałem **Unity3D**. Była to moja pierwsza styczność z nim, za równo jak i z **Blenderem** i *tworzeniem gier*. Dzięki temu projektowi poznałem mnóstwo nowych narzędzi, możliwości i rozwiązań.
- Spędziłem ponad **50 godzin** tworząc ten projekt. Do tego czasu doliczam również naukę podstaw każdego z narzędzi, tworzenie obiektów i widoków oraz wielokrotne testowanie aplikacji. Projekt wychodził mocno ponad oczekiwania wykładowcy, dzięki czemu uzyskałem za niego 750/600 pkt.  
