# Challenge_Portfolio

   
## TASK :one:

### Subtask 1
10/10 :sunglasses:


### Subtask 3

Cześć! 	:blush: Mam na imię Kamila i jestem bardzo szczęśliwa, że mogę uczestniczyć w wyzwaniu Dare It Challenge na ścieżce testerskiej. 

  To, co przekonało mnie do wzięcia udziału w projekcie, to możliwość codziennego obcowania z realnymi zadaniami testerskimi i praca nad własnym portfolio. Zainteresowała mnie także informacja o nauce podstaw testowania aplikacji mobilnych, co z pewnością jest cenną umiejętnością poszukiwaną przez pracodawców. 
  
  Moim celem jest ugruntowanie dotychczas samodzielnie zdobywanej wiedzy i zweryfikowanie jej z realiami pracy testera, dzięki wsparciu naszych mentorek. Najbardziej cenię sobie możliwość uczenia się testowania od doświadczonych praktyków. To, że świat testowania pochłonął mnie całkowicie wiem od dawna. Dzięki programowi chciałabym nie tylko mieć z tego frajdę, ale przede wszystkim stawać się coraz lepsza, aby w przyszłości stanowić mocną podporę dla zespołu, z którym będę pracować. :heartpulse:


### Subtask 4

#### **Opisz testowaną aplikację - do czego służy, jakie zawiera funkcjonalności :grey_question: Czy jest intuicyjna i przyjazna dla użytkownika :grey_question:**
:point_right: [Aplikacja dla skautów piłki nożnej](https://scouts-test.futbolkolektyw.pl/pl)

#### **Opis i cel aplikacji**

Aplikacja jest przeznaczon dla osób prowadzących bazę piłkarzy i rozegranych przez nich meczy. Umożliwia ona zapisywanie informacji o piłkarzach, w tym między innymi dane osobowe zawodników, główną pozycję, na której gra pikarz, pozycję alternatywną, do jakiego klubu należy, jaką uzyskał punktację w rankingu, ile zagrał meczy itp. Oprócz danych piłkarzy możliwe jest zapisywanie danych o rozegranych meczach i generowanie raportów dotyczących konkretnego piłkarza z jego gry w konkretnym meczu. 

Celem biznesowym aplikacji jest generowanie zysków.

#### **Funkcjonalności**

W aplikacji znajdują się trzy funjconalności spośród 4 funkcjonalności CRUD: 
   * tworzenie profilu piłkarza, tworzenie profilu meczu, tworzenie raportu (Create)
   * wyświetlanie profilów piłkarzy, meczy, wyświetlanie raportów z meczy (Read)
   * edytowanie profilów pikarzy, profilów meczy, raportów z meczy (Update)
   * nie ma możliwości usuwania porofilu zawodnika, meczu ani raportu (Delate)
  
**Tworzenie profilu nowego gracza/meczu/raportu**

Funkcjonalność jest dość intuicyjna, widoczny jest przycisk "Dodaj gracza" w centralnej części strony głównej. Myląca jest kategoria, do której przypisano button (forma linku). Dodawanie profilu meczu i raportu jest utrudnione i nie jest możliwe z poziomu strony głównej. Aby dodać mecz należy najpierw wejść w profil dowolnego gracza, dopiero wówczas wyświetlają się przyciski przenoszące do podstron z profilami meczy oraz raportami. 

Bardzo utrudnione jest utworzenie nowego raportu dla konkretnego zawodnika. Aby dodać raport należy wejść w profil danego gracza i utworzyć mecz, w którym grał dany zawodnik, a następnie przejść do tworzenia raportu. Główny przycisk "Utwórz raport" przenosi na podstronę z meczami gracza. Dopiero tam należy klinknąć w ikonę "Akcje" - Utworz Raport, któa przenosi do strony automatycznego generowania raportu (wystarczy kliknąc przycisk "Submit"). Taka konstrukcja jest niewygodna i mało przyjazna dla użytkownika  

**Edycja**

Funkcjonalność edytowania profilu gracza jest według mnie zbyt łatwo dostępna, brakuje osobnej ikony bądź przycisku edycji. Do formularza edycji przechodzi się niepostrzeżenie natychmiast po zapisaniu danych nowoutworzonego gracza. Może to być w zasadzie w ogóle nie zauważalne dla użytkownika. Taka konstrukcja może sprzyjać przypadkowemu i niechcianemu edytowaniu informacji o graczu. 

W przypadku edycji informacji o meczu widoczna jest już ikona ołówka przenosząca na podstronę edycji meczu. 

**Rozgrywka**

W aplikacji istnieje również funkcjonalność rozegrania meczu, do której przechodzi się poprzez profil konkretnego zawodnika, a następnie wejscie w zakładkę "Mecze" i użycie akcji "Rozpocznij mecz". Funkcjonalność jest niezrozumiała, brakuje samouczka, który przedstawiałby zasady gry i obsługę funkcjonalności.

#### **Wygląd aplikacji i User Experience**

Aplikacja jest niedopracowana i nieciekawa wizualnie, sprawia wrażenie, jakby pozostawała w budowie. Brak dopracowanej szaty graficznej, na stronie głównej w poszczególnych sekcjach (liczniki) występują przypadkowe kolory. Logo i nazwa aplikacji znajdują się w przypadkowym miejscu, bliżej środkowej części okna przeglądarki. W menu strony brakuje buttonów prowadzących do wszytskich podstron (mecze, raporty). Ponadto menu podzielone jest poziomą linią co sprawia wrażenie dwóch oddzielnych sekcji. Poszczególne sekcje nie są ładnie rozłożone na stronie (zbyt duże przerwy). Ikona chińskiego znaczka przy przycisku "English" może być myląca (być może ciekawszym rozwiązaniem byłoby zastosowanie ikon z flagami). Mimo przeglądania strony w wersji polskojęzycznej, przyciski "zapisz" i "wyczyść" występują po angielsku. 

Aplikacja jest mało intuicyjna i mało przyjazna dla użytkownika końcowego. Jak wyżej opisano, trudno jest odtworzyć sposób generowania raportu. Do podstawowych funkcjonalności trzeba dostawać się poprzez inne funkcjonalności, zatem ścieżka dotępnu dla użytkownika może być zbyt długa, nużąca, a ostatecznie zniechęcająca. Dość dużo czasu zajmuje zapoznanie się z zasadami obsługi aplikacji, która jest wyposażona jedynie w proste i podstawowe funkcjonalności. Zaleca sie uproszczenie poruszania się po aplikacji i dopracowanie nawigacji.

#### **Zauważalne błędy i sugestie**

Na stronie znajduje się wiele błędów bądź rozwiązań, które zdecydowanie wymagają poprawienia bądź usprawnienia, a są widoczne na pierwszy rzut oka m.in:

  * nieprawdiłowa walidacja w formularzu profilu zawodnika, bądź jej całkowity brak np. możliwe jest wprowadzanie imion i nazwisk z małych liter, bądź w formacie innym niż string, w tym również obrazków
  * formularz dodawania gracza wymaga podania prawidłowego adresu adresu e-mail z uwgzlędnieniem znaku "@" oraz znakiem ".", jednakże po wprowadzeniu adresu bez tych znaków nie wyświetla się żaden komunikat walidacyjny, zaś w konsoli DevTools wyświetla się błąd 400 i pojawia się informacja, że zawodnika nie można dopisać do listy. Ostatecznie użytkownik nie jest w stanie zrozumieć z jakiego powodu system nie przyjmuje podanego adresu e-mail (brak precyzyjnego wskazania niepoprawych danych)
  * funkcjonalność sortowania graczy (strzałka przy nazwach kolumn) działa niepoprawnie (nie wiadomo według jakich kryteriów system wyświetla wyniki)
  * brak możliwości sortowania meczy np. wg ilości bramek
  * istnieje możliwość wpisania gracza o tych samych danych
  * istnieje możliwość podawania dowolnych dat w tym przyszłych dat urodzenia graczy  
  
  
  
  # TASK :two:
  ## Subtask 1
  
  [Test cases based on User stories](https://docs.google.com/document/d/1TrRUwC-ZhLGTpM-TeEHJJNnbrRG2KVV8UPupftnk7U0/edit?usp=sharing)
  
  ## Subtask 2
  
   [Test cases based on experience - exploratory testing](https://docs.google.com/document/d/1rNam7fzTw9favo2SR1Jr4JxTES8Q9yyqaLo_9nFacB8/edit?usp=sharing)
   
  ## Subtask 3 :raising_hand:
  
  ### Po co piszemy przypadki testowe?
  
  Przypadki testowe piszemy po to, by w sposób przejrzysty udokumentować możliwości obsłużenia modułów testowanej aplikacji. W ten sposób również poznajemy aplikację, jej możliwości i funkcjonalności. Projektując przypadki testowe widzimy, czy nie pominęliśmy żadnej funkcjonalności planując nasze testy. Dzięki temu minimalizujemy ryzyko wystąpienia awarii aplikacji w przyszłości. Przypadki testowe stanowią też źródło infomracji dla nowych osób w danej firmie. *Opracowano na podstawie:* [Waldemar Szfraniec - Jak pisać przypadki testowe?](https://www.wyszkolewas.com.pl/przypadki-testowe-przyklady/).
  
  ## Subtask 4 (dodatkowy)
  
  [Test cases for the application Pick Eat Up](https://docs.google.com/document/d/1CartUoaSvK71w28mb8sJpO26JqBTWezALNNZea-6Q0M/edit?usp=sharing)
  
   # TASK :three:
 
  ## Subtask 1 i 2
  
  [Bugs Report](https://docs.google.com/document/d/1Ag6beCPENZeE5BKXmksOxh-zIDabtTkhEYozjRtrE3U/edit?usp=sharing)
  
  ## Subtask 3
  
   [Test Report](https://docs.google.com/document/d/1usfaDs6SKqvcSqd9MfontmRI76_McfBrOBAV7sJTf2g/edit?usp=sharing)
   
  ## Subtask 4 :raising_hand:)
  
In progress...

# Task :four:

## Subtask 1 i 2

[Testowanie mobilne aplikacji OLX](https://docs.google.com/spreadsheets/d/1oUs1evyJmG12yDra0VEL7oDvgrAoWJkgntjJrCDbHqs/edit?usp=sharing)

## Subtask 3

[Aplikacja mobilna OLX](https://play.google.com/store/apps/details?id=pl.tablica&hl=pl&gl=US&pli=1)

**1. Do czego służy ta aplikacja:grey_question: Jaki jest cel tej aplikacji:grey_question:**

Eksplorowana w tym zadaniu aplikacja to platforma ogłoszeniowa. Umożliwia ona użytkownikom aplikacji:

* zamieszczanie ogłoszeń z różnych ategorii (np. sprzedażowych, ogłoszeń o pracę, ogłoszeń związanych z najmem długo i krótko terminowym lokali, wynajmem sprzętów lub pojazdów, organizowaniem iventów np. bali innych imprez zorganizowanych, bądź też oddaniem rzeczy za darmo
* wyszukiwanie interesujących ogłoszeń, a w konsekwencji dokonywanie zakupów, wynajem noclegów, aplikowanie na zamieszczone w portalu oferty pracy, wynajem maszyn lub pojazdów, zakup usług - np. zorganizowanie iventu, pozyskanie darmowych rzeczy.

Głównym celem aplikacji jest cel biznesowy, którym jest wygenerwanie zysku pochodzącego głównie z prowizji za wystawione ogłoszenia, wyróżnianie ogłoszeń oraz z banerów reklamowych. Celem jest zatem również pozyskiwanie nowych klientów, którzy będą te zyski generowali.

**2. Kto ma być użytkownikiem końcowym aplikacji:grey_question:**

Użytkownikiem końcowym aplikacji może być każdy - zarówno osoba fizyczna jak i przedsiębiorca. Nie wprowadzono ograniczeń wiekowych dla użytkowników aplikacji. 


**3. Czy według Ciebie aplikacja jest user friendly:grey_question:**

   Można powiedzieć, że aplikacja user-friendly to taka, która daje użytkownikowi pozytywne doświadczenia w trakcie jej użytkowania. Jest intuicyjna  wobsłudze, wszystkie ścieżki prowadzące przez funkcjonalności aplikacji są jasne, prosto zaprojektowane i łatwe do opanowania dla przeciętnej osoby; nie wymagają korzystania z samouczka, a ilość kroków w każdej ścieżce jest ograniczona do minimum. Powoduje to, że użytkownik zaoszczędza czas, nie musi się nadmiernie wysilać przy korzystaniu z aplikacji, a zatem czerpie z tego wyłącznie przyjemność. Ważny jest również ładny i nowoczesny design, nieprzeładowanie elementami, spokojna i niemęcząca oczu kolorystyka, odpowiedniej wielkości czcionka, które będzie wyraźna, prosta ale jednocześnie łatwa. Aplikacja userfriendly musi być wydajna - nie może zawieszać się, cały jej content musi być dostęony (pełne ładowanie całej treści, w tym obrazków, plików itp). Powinna być również dostępna dla osób z różnymi ograniczeniami lub niepełnosprawnościami i zawierać np. teksty alternatywne dla osób niewidomych. Aplikacja user friendly to zatem taka, która spełnia wszystkie, bądź kluczowe potrzeby użytkownika końcowego. 
   
   Aplikacja OLX według mnie w większości spełnia kryteria aplikacji user-friendli. Posiada nowoczesny, przyjemny design, jest dość uporządkowana, wizualnie przyjemna, nie zawiesza się, cały content się ładuje stabilnie. Pochłania mnóstwo baterii - za to minus. Niektóre ścieżki nie są intuicyjne, a wręcz niepotrzebnie skomplikowane, jak chociażby wyszukiwanie ofert pracy po kategoriach. Jednocześnie wszytskie najważnijsze funkcje posiada na wierzchu, dzięki czemu łatwo i szybko można skorzystać z wybranej funkcjonalności. 


**4. Jak byś usprawnił aplikację:grey_question: Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność:grey_question:** 

   Zdecydowanie popracowałabym nad ścieżkami w obrębie funkcjonalności wyszukiwania ofert pracy. Według mnie na tle innych znanych portali OLX wypada słabo ze względu na zbyt długą ścieżkę wyszukiwania. Zastanowiłabym się nad wprowadzeniem automatycznego czyszczenia filtru, ponieważ pierwszy wpisany filtr (lokalizacja) pozostaje już z użytkownikiem i istnieje konieczność ciągłego czyszczenia filtrów, co może być na dłuższą metę uciążliwe. Popracowaabym również nad walidacjami, ponieważ wiele komunikatów walidacyjnych jest niezrozumiałych, mogą prowadzać użytkownika w błąd, nie pomagają zrozumieć, dlaczego system dalej nie przepuszcza (jak podczas rejestracji tego samego użytkownika na ten sam adres e-mail). 
   Jako nową funkcjonalność zasugerowałabym rozważenie wprowadzenia, przynajmniej na próbę, zakładki "Szukam", któa polegałaby na tym, że użytkownik, któy nie znalazł w bazie platformy pożądanego produktu/usługi/zwierzątka/nieruchomości itp, będzie mógł dodać ogłoszenie, w którym wskaże czego szuka, opisac parametry takiej rzeczy, jaką kwotę jest w stanie zapłacić (widełki), czy kwota jest do negocjacji, czy poszukuje rzeczy nowej czy używanej, czy chce odebrać na miejscu, czy z przesyłką itp. itd. Osoby, które posiadają taką rzecz/produkt/usługę, mogłyby w tej sprawie kontaktować się z szukającym lub wystawiać pod jego ogłoszeniem swoje oferty. 

**5. Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej:grey_question:**

Przy testowaniu aplikacji internetowej skupimy się na takich elementach jak energochłonność aplikacji (zużycie baterii), jej responsywność (czy jest dobrze dostosowana do danej przeglądarki internetowej) czy nic się nie rozjeżdża, nie urywa w połowie (skalowalność do odpowiedniej rozdzielczości), czy korzystane z aplikacji spowolni działanie internetu oraz innych aplikacji zainstalowanych na urządzeniu. 
Przy testowaniu aplikacji natywnych bardziej skupimy się na tym, czy nie "gryzie się" z innymi modułami urządzenia mobilnego oraz na całej waarstwie UXowej. Aplikacje natywne są o wiele droższe w wytworzeniu i utrzymaniu dlatego testy regresji będą zapewne stosowane z dużą ostrożnością, a co za tym idzie powinno się położyć nacisk na zasadę Left shift testing i zacząć testowanie jak najwcześniej. W ramach testów trzeba się tez skupić bardziej na samym procesie instalacji na danym urządzeniu. Trzeba zatem zadbać aby testy instalacji odbyły się na każdym z dedykowanych urządzeń oraz na systemie Android i iOs

## Subtask 4

In progres...

# TASK 5

## Subtask 1

* Podstawowe zapytania SQL:

   * SELECT TOP() FROM
   * SELECT * FROM NAZWA_TABELI
   * SELECT * FROM SCHEMAT.NAZWA_TABELI
   * SELECT NAZWY_KOLUMN FROM NAZWA_TABELI
   * SELECT NAZWA_KOLUMNY AS ALIANS FROM NAZWA_TABELI
   * SELECT * FROM nazwa_tabeli ORDER BY nazwa_kolumny ASC/ DESC
   * SELECT * FROM nazwa_tabeli ORDER BY nazwa_kolumny, nazwa_kolumny2
   * SELECT * FROM nazwa_tabeli ORDER BY nazwa_kolumny DESC, nazwa_kolumny2 
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny = "warunek"
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny BETWEEN "warunek" AND "warunek2"
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny LIKE "%XXX%"
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny LIKE "_aszanka"
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny = x AND nazwa_kolumny2 = y
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny = x OR nazwa_kolumny = y OR nazwa_kolumny = z
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny IS NULL
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny IS NOT NULL
   * SELECT * FROM nazwa_tabeli WHERE nazwa_kolumny IN (X, Y)
   * SELECT * FROM nazwa_tabeli AS nazwa_aliasu ORDER BY nazwa_aliasu 
   * SELECT GETDATE()
   * SELECT GETDATE() AS aliand
   * SELECT UPPER(łańcuch znaków)
   * SELECT LOWER(łańcuch znaków)
   * SELECT DATEDIFF(HOUR, data_1, data_2)
   * SELECT DATEDIFF(MONTH, data_1, data_2)
   * SELECT DATEDIFF(YEAR, data_1, data_2)
   * SELECT MIN(nazwa_kolumny) FROM nazwa_tabeli
   * SELECT MAX(nazwa_kolumny) FROM nazwa_tabeli
   * SELECT DATEDIFF(YEAR, GETDATE, data_2)
   * SELECT COUNT(*) FROM nazwa_tabeli
   * SELECT SUM(nazwa_kolumny) FROM nazwa_tabeli
   * SELECT nazwa_kolumny FROM nazwa_tabeli GROUP BY nazwa_tabeli
   * SELECT * FROM tabela_1 JOIN tabela_2 ON tabela1_kolumnaId = tebela2_kolumnaId
   

## Subtask 2 i 3

**1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.**

SELECT * FROM actors Group BY surname ASC

![sql1](https://user-images.githubusercontent.com/95380844/217948466-604bc385-9126-47a1-83d6-4d9979af3073.png)


**2. Wyświetl film, który powstał w 2019 roku.**

SELECT * FROM `movies` WHERE year_of_production = 2019

![sql4](https://user-images.githubusercontent.com/95380844/217952149-f2ff070a-4869-47cf-86a4-c1b6863f49de.png)


**3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.**

SELECT * FROM `movies` WHERE year_of_production BETWEEN 1990 and 1999

![sql5](https://user-images.githubusercontent.com/95380844/217952625-6a070b2e-e814-485a-9e80-706c44365c4a.png)


**4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$**

SELECT title, price FROM `movies` WHERE price < 7

![wql4](https://user-images.githubusercontent.com/95380844/217950336-9f8fa9e0-c3b4-43a9-ba29-94c104b47a42.png)


**5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.**
SELECT * FROM `actors` WHERE (actor_id = 4 and name = "Jack") OR (actor_id = 5 and name = "Harrison") OR (actor_id = 6 and name = "Anne") OR (actor_id = 7 and name = "Helena")

![11](https://user-images.githubusercontent.com/95380844/218681874-73b939f2-27a6-4cf2-a2dc-ef7ae42c2260.png)


**6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.**

SELECT * FROM `customers` WHERE customer_id = 2 OR customer_id = 4 OR customer_id = 6

![SQLL](https://user-images.githubusercontent.com/95380844/218094446-a3093ddd-5454-467d-9770-c313d7e87a74.png)


**7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.**

SELECT * FROM `customers` WHERE customer_id IN (1, 3, 5)

![SQ](https://user-images.githubusercontent.com/95380844/218094824-50c84263-04a0-47e9-9b69-d472195e3e8b.png)

**8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.**

SELECT * FROM `actors`WHERE name LIKE "An%"

![aa](https://user-images.githubusercontent.com/95380844/218095153-eab933de-d142-4232-9e78-0a17dec02dd8.png)


**9. Wyświetl dane klienta, który nie ma podanego adresu email.**

SELECT * FROM `customers` WHERE email IS NULL

![AAA](https://user-images.githubusercontent.com/95380844/218095420-3ef0e8b6-7c75-4561-8491-93da172bb269.png)


**10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.**

SELECT * FROM `movies` WHERE (price > 9) AND (movie_id BETWEEN 2 AND 8)

![AAAA](https://user-images.githubusercontent.com/95380844/218096020-cd2720e5-ca83-456d-8c23-90c6d0e50c0f.png)

11. Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd 🙈

UPDATE customers SET surname = 'Miler' WHERE customer_id = 3

![a](https://user-images.githubusercontent.com/95380844/219694679-4d4eaaf0-2e98-4f44-bfab-cb1651d203e6.png)

12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.

SELECT customers.name, customers.email FROM `customers` JOIN sale ON customers.customer_id = sale.customer_id WHERE movie_id = 4

![a1](https://user-images.githubusercontent.com/95380844/219696855-15a75814-691b-453b-a01a-e3c0484224f6.png)


13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com

UPDATE customers SET email = 'pati@mail.com' WHERE customer_id = 4 

![A2](https://user-images.githubusercontent.com/95380844/219698342-62b219a0-618f-4c75-b53a-22a3585608b1.png)

14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).

SELECT sale.sale_date, customers.name, customers.surname, movies.title FROM `customers`INNER JOIN sale ON customers.customer_id = sale.customer_id INNER JOIN movies ON sale.movie_id = movies.movie_id

![sale](https://user-images.githubusercontent.com/95380844/219702746-82250f43-80fd-4552-b173-0d99319e0038.png)

15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag

ALTER TABLE customers ADD COLUMN pseudonimy varchar(100)
...

16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.

SELECT DISTINCT movies.title FROM `movies` JOIN sale ON movies.movie_id = sale.movie_id

![SALE2](https://user-images.githubusercontent.com/95380844/219707383-19afb721-7396-4c50-bb40-c28405031432.png)


17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)

SELECT name FROM actors UNION SELECT name FROM customers ORDER BY name ASC

![3](https://user-images.githubusercontent.com/95380844/219708576-330c8d9e-d914-4298-b23c-bce547b1241f.png)


18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).


19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał

SELECT actors.name, actors.surname, movies.title FROM actors INNER JOIN cast ON actors.actor_id = cast.actor_id INNER JOIN movies ON movies.movie_id = cast.movie_id WHERE actors.actor_id = 4

![222](https://user-images.githubusercontent.com/95380844/219710850-e87bc55d-f9e2-4172-9fde-ecd36d734f49.png)

20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa

INSERT INTO customers VALUES (7, 'Honia', 'Stuczka-Kucharska', 'honia@mail.com', 'Hoa');

![hi](https://user-images.githubusercontent.com/95380844/219712290-4ac67dd0-c90a-4119-9f5a-89ef177fcc26.png)


