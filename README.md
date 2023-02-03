# Challenge_Portfolio

## TABLE OF CONTENT

* [TASK 1](#task-1)
* [TASK 2](#task-2)
* [TASK 3](#task-3)
* [TASK 4](#task-4)
   
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
  
  [Test cases for the application Pick Eat Up](https://docs.google.com/document/d/1CartUoaSvK71w28mb8sJpO26JqBTWezALNNZea-6Q0M/edit?usp=sharing)
  
   # TASK 3
 
  ## Subtask 1 i 2
  
  [Bugs Report](https://docs.google.com/document/d/1Ag6beCPENZeE5BKXmksOxh-zIDabtTkhEYozjRtrE3U/edit?usp=sharing)
  
  ## Subtask 3
  
   [Test Report](https://docs.google.com/document/d/1usfaDs6SKqvcSqd9MfontmRI76_McfBrOBAV7sJTf2g/edit?usp=sharing)
   
  ## Subtask 4 :raising_hand:)
  
In progress...

# Task 4

## Subtask 1 i 2

[Testowanie mobilne aplikacji OLX](https://docs.google.com/spreadsheets/d/1oUs1evyJmG12yDra0VEL7oDvgrAoWJkgntjJrCDbHqs/edit?usp=sharing)

## Subtask 3

[Aplikacja mobilna OLX](https://play.google.com/store/apps/details?id=pl.tablica&hl=pl&gl=US&pli=1)

**1. Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?**

Eksplorowana w tym zadaniu aplikacja to platforma ogłoszeniowa. Umożliwia ona użytkownikom aplikacji:

* zamieszczanie ogłoszeń z różnych ategorii (np. sprzedażowych, ogłoszeń o pracę, ogłoszeń związanych z najmem długo i krótko terminowym lokali, wynajmem sprzętów lub pojazdów, organizowaniem iventów np. bali innych imprez zorganizowanych, bądź też oddaniem rzeczy za darmo
* wyszukiwanie interesujących ogłoszeń, a w konsekwencji dokonywanie zakupów, wynajem noclegów, aplikowanie na zamieszczone w portalu oferty pracy, wynajem maszyn lub pojazdów, zakup usług - np. zorganizowanie iventu, pozyskanie darmowych rzeczy.

Głównym celem aplikacji jest cel biznesowy, którym jest wygenerwanie zysku pochodzącego głównie z prowizji za wystawione ogłoszenia, wyróżnianie ogłoszeń oraz z banerów reklamowych. Celem jest zatem również pozyskiwanie nowych klientów, którzy będą te zyski generowali.

**2. Kto ma być użytkownikiem końcowym aplikacji?**

Użytkownikiem końcowym aplikacji może być każdy - zarówno osoba fizyczna jak i przedsiębiorca. Nie wprowadzono ograniczeń wiekowych dla użytkowników aplikacji. 


**3. Czy według Ciebie aplikacja jest user friendly?**

   Można powiedzieć, że aplikacja user-friendly to taka, która daje użytkownikowi pozytywne doświadczenia w trakcie jej użytkowania. Jest intuicyjna  wobsłudze, wszystkie ścieżki prowadzące przez funkcjonalności aplikacji są jasne, prosto zaprojektowane i łatwe do opanowania dla przeciętnej osoby; nie wymagają korzystania z samouczka, a ilość kroków w każdej ścieżce jest ograniczona do minimum. Powoduje to, że użytkownik zaoszczędza czas, nie musi się nadmiernie wysilać przy korzystaniu z aplikacji, a zatem czerpie z tego wyłącznie przyjemność. Ważny jest również ładny i nowoczesny design, nieprzeładowanie elementami, spokojna i niemęcząca oczu kolorystyka, odpowiedniej wielkości czcionka, które będzie wyraźna, prosta ale jednocześnie łatwa. Aplikacja userfriendly musi być wydajna - nie może zawieszać się, cały jej content musi być dostęony (pełne ładowanie całej treści, w tym obrazków, plików itp). Powinna być również dostępna dla osób z różnymi ograniczeniami lub niepełnosprawnościami i zawierać np. teksty alternatywne dla osób niewidomych. Aplikacja user friendly to zatem taka, która spełnia wszystkie, bądź kluczowe potrzeby użytkownika końcowego. 
   
   Aplikacja OLX według mnie w większości spełnia kryteria aplikacji user-friendli. Posiada nowoczesny, przyjemny design, jest dość uporządkowana, wizualnie przyjemna, nie zawiesza się, cały content się ładuje stabilnie. Pochłania mnóstwo baterii - za to minus. Niektóre ścieżki nie są intuicyjne, a wręcz niepotrzebnie skomplikowane, jak chociażby wyszukiwanie ofert pracy po kategoriach. Jednocześnie wszytskie najważnijsze funkcje posiada na wierzchu, dzięki czemu łatwo i szybko można skorzystać z wybranej funkcjonalności. 


**4. Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność?** 

   Zdecydowanie popracowałabym nad ścieżkami w obrębie funkcjonalności wyszukiwania ofert pracy. Według mnie na tle innych znanych portali OLX wypada słabo ze względu na zbyt długą ścieżkę wyszukiwania. Zastanowiłabym się nad wprowadzeniem automatycznego czyszczenia filtru, ponieważ pierwszy wpisany filtr (lokalizacja) pozostaje już z użytkownikiem i istnieje konieczność ciągłego czyszczenia filtrów, co może być na dłuższą metę uciążliwe. Popracowaabym również nad walidacjami, ponieważ wiele komunikatów walidacyjnych jest niezrozumiałych, mogą prowadzać użytkownika w błąd, nie pomagają zrozumieć, dlaczego system dalej nie przepuszcza (jak podczas rejestracji tego samego użytkownika na ten sam adres e-mail). 
   Jako nową funkcjonalność zasugerowałabym rozważenie wprowadzenia, przynajmniej na próbę, zakładki "Szukam", któa polegałaby na tym, że użytkownik, któy nie znalazł w bazie platformy pożądanego produktu/usługi/zwierzątka/nieruchomości itp, będzie mógł dodać ogłoszenie, w którym wskaże czego szuka, opisac parametry takiej rzeczy, jaką kwotę jest w stanie zapłacić (widełki), czy kwota jest do negocjacji, czy poszukuje rzeczy nowej czy używanej, czy chce odebrać na miejscu, czy z przesyłką itp. itd. Osoby, które posiadają taką rzecz/produkt/usługę, mogłyby w tej sprawie kontaktować się z szukającym lub wystawiać pod jego ogłoszeniem swoje oferty. 

**5. Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?**

Przy testowaniu aplikacji internetowej skupimy się na takich elementach jak energochłonność aplikacji (zużycie baterii), jej responsywność (czy jest dobrze dostosowana do danej przeglądarki internetowej) czy nic się nie rozjeżdża, nie urywa w połowie (skalowalność do odpowiedniej rozdzielczości), czy korzystane z aplikacji spowolni działanie internetu oraz innych aplikacji zainstalowanych na urządzeniu. 
Przy testowaniu aplikacji natywnych bardziej skupimy się na tym, czy nie "gryzie się" z innymi modułami urządzenia mobilnego oraz na całej waarstwie UXowej. Aplikacje natywne są o wiele droższe w wytworzeniu i utrzymaniu dlatego testy regresji będą zapewne stosowane z dużą ostrożnością, a co za tym idzie powinno się położyć nacisk na zasadę Left shift testing i zacząć testowanie jak najwcześniej. W ramach testów trzeba się tez skupić bardziej na samym procesie instalacji na danym urządzeniu. Trzeba zatem zadbać aby testy instalacji odbyły się na każdym z dedykowanych urządzeń oraz na systemie Android i iOs

## Subtask 4

In progres...
