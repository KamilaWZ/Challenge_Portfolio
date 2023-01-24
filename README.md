# Challenge_Portfolio

## TABLE OF CONTENT

* [TASK 1](#task-1)
* [TASK 2](#task-2)
   
## TASK 1

### Subtask 1
10/10 :sunglasses:


### Subtask 3

Cześć! 	:blush: Mam na imię Kamila i jestem bardzo szczęśliwa, że mogę uczestniczyć w wyzwaniu Dare It Challenge na ścieżce testerskiej. 

  To, co przekonało mnie do wzięcia udziału w projekcie, to możliwość codziennego obcowania z realnymi zadaniami testerskimi i praca nad własnym portfolio. Zainteresowała mnie także informacja o nauce podstaw testowania aplikacji mobilnych, co z pewnością jest cenną umiejętnością poszukiwaną przez pracodawców. 
  
  Moim celem jest ugruntowanie dotychczas samodzielnie zdobywanej wiedzy i zweryfikowanie jej z realiami pracy testera, dzięki wsparciu naszych mentorek. Najbardziej cenię sobie możliwość uczenia się testowania od doświadczonych praktyków. To, że świat testowania pochłonął mnie całkowicie wiem od dawna. Dzięki programowi chciałabym nie tylko mieć z tego frajdę, ale przede wszystkim stawać się coraz lepsza, aby w przyszłości stanowić mocną podporę dla zespołu, z którym będę pracować. :heartpulse:


### Subtask 4

#### Testowanie eksploracyjne 
[Aplikacja dla skautów piłki nożnej](https://scouts-test.futbolkolektyw.pl/pl)


Aplikacja jest przeznaczon dla osób prowadzących bazę piłkarzy i rozegranych meczy. Umożliwia ona zapisywanie informacji o piłkarzach, w tym między innymi dane osobowe, główną pozycję, na której gra pikarz, pozycję alternatywną, do jakiego klubu należy, jaką uzyskał punktację w rankingu, ile zagrał meczy itp. Oprócz danych piłkarzy możliwe jest zapisywanie danych o rozegranych meczach i generowanie raportów dotyczących konkretnego piłkarza z jego gry w konkretnym meczu. 

*  W aplikacji znajdują się trzy funjconalności spośród 4 funkcjonalności CRUD: 
    * tworzenie profilu piłkarza, tworzenie profilu meczu, tworzenie raportu (Create)
    * wyświetlanie profilów piłkarzy, meczy, wyświetlanie raportów z meczy (Read)
    * edytowanie profilów pikarzy, profilów meczy, raportów z meczy (Update)
    * nie ma możliwości usuwania porofilu zawodnika, meczu ani raportu (Delate)
  
* Funkcjonalność dodawania profilu nowego gracza jest dość intuicyjna, widoczny jest przycisk "Dodaj gracza" w centralnej części strony głównej, jednakże myląca jest kategoria, do której przypisano button (forma linku). Dodawanie profilu meczu i raportu jest utrudnione i nie jest możliwe z poziomu strony głównej. Aby dodać mecz należy najpierw wejść w profil dowolnego gracza, dopiero wówczas wyświetlają się przyciski przenoszące do podstron z profilami meczy oraz raportami. 
Bardzo utrudnione jest utworzenie nowego raportu dla konkretnego zawodnika. Aby dodać raport należy wejść w profil danego gracza i utworzyć mecz, w którym grał dany zawodnik, a następnie przejść do tworzenia raportu. Główny przycisk "Utwórz raport" przenosi na podstronę z meczami gracza. Dopiero tam należy klinknąć w ikonę "Akcje" - Utworz Raport, któa przenosi do strony automatycznego generowania raportu (wystarczy kliknąc przycisk "Submit"). Taka konstrukcja jest niewygodna i mało przyjazna dla użytkownika  

* Funkcjonalność edytowania profilu gracza jest według mnie zbyt łatwo dostępna, brakuje osobnej ikony bądź przycisku edycji. Taka konstrukcja może sprzyjać przypadkowemu i niechcianemu edytowaniu informacji o graczu. W przypadku edycji informacji o meczu widoczna jest już ikona ołówka przenosząca na podstronę edycji informacji o meczu. 
W aplikacji istnieje również funkcjonalność rozegrania meczu, do której przechodzi się poprzez profil konkretnego zawodnika, a następnie wejscie w zakładkę "Mecze" i użycie akcji "Rozpocznij mecz". Funkcjonalność jest niezrozumiała, brakuje samouczka, który przedstawiałby zasady gry i obsługę funkcjonalności.

* Wygląd aplikacji jest niedopracowany i nieciekawy, sprawia wrażenie, jakby aplikacja była nadal w budowie. Brak dopracowanej szaty graficznej, na stronie głównej w poszczególnych sekcjach (liczniki) występują przypadkowe kolory. Logo i nazwa aplikacji znajdują się w przypadkowym miejscu, bliżej środkowej części okna przeglądarki. W menu strony brakuje buttonów prowadzących do wszytskich podstron (mecze, raporty). Ponadto menu podzielone jest poziomą linią co sprawia wrażenie dwóch oddzielnych menu. Poszczególne sekcje nie są ładnie rozłożone na stronie (zbyt duże przerwy). Ikona chińskiego znaczka przy przycisku "English" może być myląca i nie wygląda ładnie. Mimo przeglądania strony w wersji polskojęzycznej, przyciski "zapisz" i "wyczyść" występują po angielsku. 

* Aplikacja jest mało intuicyjna i mało przyjazna dla użytkownika końcowego. Jak wyżej opisano, trudno jest odtworzyć sposób generowania raportu. Do podstawowych funkkcjonalności trzeba dostawać się poprzez inne funkcjonalności. Dość dużo czasu zajmuje zapoznanie się z zasadami obsługi aplikacji, która w zasadzie jest wyposażona w proste i podstawowe funkcjonalności. Zaleca sie uproszczenie poruszania się po aplikacji.

* Na stronie znajduje się wiele błędów bądź rozwiązań, które zdecydowanie wymagają poprawienia bądź usprawnienia, m.in:
  * nieprawdiłowa walidacja w formularzu profilu zawodnika, bądź jej całkowity brak np. możliwe jest wprowadzanie imion i nazwisk z małych liter, bądź w formacie innym niż string, w tym również obrazków (brak walidacji)
  * formularz dodawania gracza wymaga podania prawidłowego adresu adresu e-mail z uwgzlędnieniem znaku "@" oraz znakiem ".", jednakże po wprowadzeniu adresu e-mail bez tych znaków nie wyświetla się żaden komunikat walidacyjny, zaś w konsoli DevTools wyświetla się błąd 400 i pojawia się informacja, że zawodnika nie można dopisać do listy, jednakże użytkownik nie wie z jakiego powodu (brak precyzyjnego wskazania niepoprawych danych)
  * funkcjonalność sortowania graczy (strzałka przy nazwach kolumn) jest całkowicie wadliwa (działa jak chce, nie wiadomo według jakich kryteriów)
  * brak możliwości sortowania meczy np. wg ilości bramek
  * nieprawidłowo działa funkcjonalność importu danych do pliku CSV (nieczytelna tabela z krzaczkami zamiast poprawnych danych)
  * funkcja filtrowania nie działa poprawnie
  * istnieje możłiwość wpisania gracza o tych samych danych
  * istnieje możliwość podawania dowolnych dat w tym przyszłych dat urodzenia graczy (np. 22.01.2023). 
  
  ❤️❤️❤️
  
  # TASK 2
  ## Subtask 1
  
  [Test cases based on User stories](https://docs.google.com/document/d/1TrRUwC-ZhLGTpM-TeEHJJNnbrRG2KVV8UPupftnk7U0/edit?usp=sharing)
  
  ## Subtask 2
  
   [Test cases based on experience - exploratory testing](https://docs.google.com/document/d/1rNam7fzTw9favo2SR1Jr4JxTES8Q9yyqaLo_9nFacB8/edit?usp=sharing)
   
  ## Subtask 3 :raising_hand:
  
  ### Po co piszemy przypadki testowe?
  
  Przypadki testowe piszemy po to, by w sposób przejrzysty udokumentować możliwości obsłużenia modułów testowanej aplikacji. W ten sposób również poznajemy aplikację, jej możliwości i funkcjonalności. Projektując przypadki testowe widzimy, czy nie pominęliśmy żadnej funkcjonalności planując nasze testy. Dzięki temu minimalizujemy ryzyko wystąpienia awarii aplikacji w przyszłości. Przypadki testowe stanowią też źródło infomracji dla nowych osób w danej firmie. *Opracowano na podstawie:* [Waldemar Szfraniec - Jak pisać przypadki testowe?](https://www.wyszkolewas.com.pl/przypadki-testowe-przyklady/).
  
  ## Subtask 4 (dodatkowy)
