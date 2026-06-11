# Pełna instrukcja obsługi plakatów i repertuaru kina

**System ekranów informacyjnych MOKSiAL / Miasto Szklarska Poręba**

**Repozytorium:** `MOKSiAL-ekrany-nowe`  
**Wersja:** z opisem daty, wag `W1-W10` oraz dopisku `_dluzej`

---

## Spis treści

1. [Najważniejsze linki do wyświetlaczy](#1-najważniejsze-linki-do-wyświetlaczy)
2. [Podstawowa zasada](#2-podstawowa-zasada)
3. [Gdzie wrzucać plakaty](#3-gdzie-wrzucać-plakaty)
4. [Jak nazywać plakaty](#4-jak-nazywać-plakaty)
5. [Zasady nazw plików](#5-zasady-nazw-plików)
6. [Format i wymiary plakatu](#6-format-i-wymiary-plakatu)
7. [Wagi W1-W10](#7-wagi-w1-w10)
8. [Dopisek _dluzej](#8-dopisek-_dluzej)
9. [Przykłady poprawnych nazw](#9-przykłady-poprawnych-nazw)
10. [Jak działa automatyczna lista plakatów](#10-jak-działa-automatyczna-lista-plakatów)
11. [Tryby wyświetlania](#11-tryby-wyświetlania)
12. [Repertuar kina](#12-repertuar-kina)
13. [Jak działa kolejka z repertuarem](#13-jak-działa-kolejka-z-repertuarem)
14. [Licznik i 6 kropek](#14-licznik-i-6-kropek)
15. [QR „Jak dotrzeć”](#15-qr-jak-dotrzeć)
16. [Cache i odświeżanie](#16-cache-i-odświeżanie)
17. [Co może edytować osoba nietechniczna](#17-co-może-edytować-osoba-nietechniczna)
18. [Szybka ściąga dla MOKSiAL](#18-szybka-ściąga-dla-moksial)
19. [Szybka ściąga dla Miasta / Informacji Turystycznej](#19-szybka-ściąga-dla-miasta--informacji-turystycznej)

---

## 1. Najważniejsze linki do wyświetlaczy

| Tryb | Link |
|---|---|
| Ekran tylko MOKSiAL | [Otwórz ekran MOKSiAL](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=moksial) |
| Ekran tylko Miasto | [Otwórz ekran Miasto](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=miasto) |
| Ekran hybrydowy, czyli MOKSiAL + Miasto | [Otwórz ekran Hybryda](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=hybryda) |
| Ekran hybrydowy + repertuar kina | [Otwórz ekran Hybryda + Kino](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/index-kino.html?ekran=hybryda) |

---

## 2. Podstawowa zasada

Osoby wrzucające plakaty **NIE powinny edytować plików technicznych**.

W normalnej obsłudze wystarczy:

1. przygotować plakat,
2. dobrze nazwać plik,
3. wrzucić go do właściwego folderu,
4. poczekać, aż lista plakatów utworzy się sama.

Folder decyduje o tym, czy plakat jest miejski, czy MOKSiAL.

---

## 3. Gdzie wrzucać plakaty

| Rodzaj plakatu | Folder |
|---|---|
| Plakaty MOKSiAL | `Plakaty-MOKSiAL` |
| Plakaty Miasta | `Plakaty-Miasto` |

Nie należy mieszać plakatów między folderami.

System rozpoznaje logo po lokalizacji pliku:

- plakat z folderu MOKSiAL = logo MOKSiAL,
- plakat z folderu Miasta = logo Miasta Szklarska Poręba.

---

## 4. Jak nazywać plakaty

Najlepszy podstawowy schemat:

```text
RRRR-MM-DD_Nazwa_wydarzenia.jpg
```

Przykład:

```text
2026-07-15_Koncert_na_skwerze.jpg
```

Data na początku jest ważna, ponieważ:

1. pomaga zachować porządek w folderze,
2. informuje, którego dnia dotyczy plakat,
3. pozwala systemowi automatycznie zdjąć plakat po zakończeniu danego dnia.

Przykład:

```text
2026-07-15_Koncert_na_skwerze.jpg
```

Taki plakat dotyczy **15.07.2026** i po zakończeniu tego dnia powinien sam zniknąć z ekranów.

Jeżeli wydarzenie trwa kilka dni, najlepiej wpisać datę ostatniego dnia wydarzenia.

Przykład:  
Wydarzenie trwa od 15 do 17 lipca 2026:

```text
2026-07-17_Festiwal_miejski.jpg
```

---

## 5. Zasady nazw plików

### Dobrze

```text
2026-07-15_Koncert_na_skwerze.jpg
2026-08-01_Festyn_rodzinny.png
2026-08-20_Wystawa_fotografii.jpg
2026-07-31_Kalendarz_wydarzen_W8_dluzej.jpg
```

### Źle

```text
Koncert na skwerze.jpg
Święto Miasta 2026.png
plakat finał ostateczny !!!.jpg
2026/07/15 koncert.jpg
```

### Zasady

- bez polskich znaków,
- bez spacji,
- zamiast spacji używać podkreślnika: `_`,
- bez znaków specjalnych: `/ \ ? % # & : ; !`,
- nie używać bardzo długich nazw,
- data powinna być na początku w formacie `RRRR-MM-DD`.

---

## 6. Format i wymiary plakatu

### Obsługiwane formaty

```text
.jpg
.png
.webp
.gif
```

### Najbezpieczniejsze formaty

```text
.jpg
.png
```

### Nie wrzucać

```text
PDF
DOCX
PPTX
ZIP
plików Canva
bardzo ciężkich plików roboczych
```

### Najlepszy układ plakatu

Pionowy `9:16`

### Przykładowe rozdzielczości

```text
1080 x 1920 px
1440 x 2560 px
2160 x 3840 px
```

Plakat powinien być czytelny z daleka:

- duży tytuł,
- duża data,
- duża godzina,
- mało drobnego tekstu,
- mocny kontrast,
- bez nadmiaru małych logotypów i opisów.

Plakat poziomy też może się wyświetlić, ale na pionowym ekranie będzie mniejszy.

---

## 7. Wagi W1-W10

Waga plakatu określa jego priorytet w wyświetlaniu.

W nazwie pliku można dodać dopisek:

```text
_W1
_W2
_W3
_W4
_W5
_W6
_W7
_W8
_W9
_W10
```

Najprościej:

| Waga | Znaczenie |
|---|---|
| `W1` | najniższa waga |
| `W5` | średnia waga |
| `W10` | najwyższa waga |

Im wyższa waga, tym plakat powinien być traktowany jako ważniejszy w kolejce.

Przykład plakatu ze standardową nazwą:

```text
2026-07-15_Koncert_na_skwerze.jpg
```

Przykład plakatu z wagą:

```text
2026-07-15_Koncert_na_skwerze_W5.jpg
```

Przykład ważnego plakatu:

```text
2026-07-15_Koncert_na_skwerze_W10.jpg
```

### Kiedy używać wyższych wag?

| Waga | Kiedy używać |
|---|---|
| `W7-W10` | bardzo ważne wydarzenia, wydarzenia miejskie o wysokim priorytecie, komunikaty pilne, informacje, które mają być mocniej promowane |
| `W4-W6` | standardowe wydarzenia, plakaty informacyjne, typowe wydarzenia kulturalne lub miejskie |
| `W1-W3` | informacje mniej pilne, plakaty, które mogą pojawiać się rzadziej, materiały uzupełniające |

Jeżeli nie wpiszemy wagi w nazwie, plakat powinien być traktowany jako standardowy.

---

## 8. Dopisek _dluzej

Dopisek `_dluzej` oznacza, że plakat ma być wyświetlany dłużej na ekranie.

Przykład:

```text
2026-07-31_Kalendarz_wydarzen_dluzej.jpg
```

Można połączyć wagę i dłuższy czas wyświetlania:

```text
2026-07-31_Kalendarz_wydarzen_W8_dluzej.jpg
```

### Różnica między wagą a `_dluzej`

| Dopisek | Znaczenie |
|---|---|
| `W1-W10` | priorytet / waga plakatu w kolejce |
| `_dluzej` | dłuższy czas wyświetlania pojedynczego plakatu |

### Kiedy używać `_dluzej`?

- kalendarz wydarzeń,
- plakat z dużą ilością tekstu,
- ważny komunikat,
- informacja organizacyjna,
- treść, którą odbiorca musi przeczytać spokojnie.

### Kiedy nie używać `_dluzej`?

- prosty plakat jednego wydarzenia,
- grafika z małą ilością informacji,
- plakat promocyjny, który nie wymaga dłuższego czytania.

---

## 9. Przykłady poprawnych nazw

| Rodzaj plakatu | Przykład nazwy |
|---|---|
| Zwykły plakat | `2026-07-15_Koncert_na_skwerze.jpg` |
| Plakat z wagą średnią | `2026-07-15_Koncert_na_skwerze_W5.jpg` |
| Plakat bardzo ważny | `2026-07-15_Koncert_na_skwerze_W10.jpg` |
| Plakat wyświetlany dłużej | `2026-07-31_Kalendarz_wydarzen_dluzej.jpg` |
| Plakat ważny i wyświetlany dłużej | `2026-07-31_Kalendarz_wydarzen_W8_dluzej.jpg` |
| Wydarzenie kilkudniowe, które kończy się 17 lipca | `2026-07-17_Festiwal_miejski_W7.jpg` |

---

## 10. Jak działa automatyczna lista plakatów

Po wrzuceniu plakatu do odpowiedniego folderu lista plakatów powinna utworzyć się automatycznie.

Najważniejsze listy techniczne:

```text
plakaty-moksial.json
plakaty-miasto.json
plakaty-hybryda.json
```

Osoby wrzucające plakaty nie muszą ich edytować.

Mechanizm działania:

1. Plakat trafia do folderu `Plakaty-MOKSiAL` albo `Plakaty-Miasto`.
2. GitHub Actions uruchamia automatyczną aktualizację list.
3. System ekranów pobiera aktualną listę plakatów.
4. Ekrany pokazują aktualne plakaty.

Jeżeli plakat nie pojawia się od razu:

- poczekać chwilę,
- odświeżyć stronę `Ctrl + F5`,
- sprawdzić nazwę pliku,
- sprawdzić folder,
- sprawdzić rozszerzenie pliku.

---

## 11. Tryby wyświetlania

| Tryb | Link | Opis |
|---|---|---|
| MOKSiAL | [Otwórz](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=moksial) | Pokazuje plakaty MOKSiAL |
| Miasto | [Otwórz](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=miasto) | Pokazuje plakaty Miasta |
| Hybryda | [Otwórz](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=hybryda) | Pokazuje razem plakaty MOKSiAL i Miasta |
| Hybryda + Kino | [Otwórz](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/index-kino.html?ekran=hybryda) | Pokazuje plakaty MOKSiAL i Miasta oraz slajd repertuaru kina |

---

## 12. Repertuar kina

Repertuar kina działa na osobnej wersji ekranu:

```text
index-kino.html?ekran=hybryda
```

Ustawienia repertuaru są w pliku:

```text
config-kino.json
```

Najważniejsze pola:

| Pole | Znaczenie |
|---|---|
| `enabled` | Czy repertuar jest włączony. `true` = włączony, `false` = wyłączony |
| `json` | Adres pliku z repertuarem kina |
| `posterBase` | Adres folderu z plakatami filmów |
| `every` | Co ile plakatów ma pojawiać się repertuar |
| `duration` | Czas wyświetlania repertuaru w milisekundach |
| `maxItems` | Maksymalna liczba filmów pokazywanych na slajdzie repertuaru |
| `mapQr` | Czy pokazywać QR „Jak dotrzeć” |
| `mapQrImage` | Nazwa pliku QR do trasy kina |

Przykład:

```text
"every": 5
```

Oznacza to, że repertuar pojawia się po każdych 5 plakatach.

Przykład:

```text
"duration": 20000
```

Oznacza 20 sekund.

Przykład:

```text
"maxItems": 8
```

---

## 13. Jak działa kolejka z repertuarem

Repertuar kina jest liczony jako normalna pozycja w kolejce.

Przykład:  
Jeżeli jest 10 plakatów i repertuar ma pojawiać się co 5 plakatów, kolejka wygląda tak:

```text
01 plakat
02 plakat
03 plakat
04 plakat
05 plakat
06 repertuar kina
07 plakat
08 plakat
09 plakat
10 plakat
11 plakat
12 repertuar kina
```

Licznik na ekranie pokazuje aktualną pozycję w całej kolejce.

---

## 14. Licznik i 6 kropek

Na ekranie jest pasek czasu, licznik i 6 kropek.

Licznik pokazuje pozycję w kolejce:

```text
03 / 12
```

Kropki:

- jest zawsze 6 kropek,
- zapalają się po kolei,
- po szóstej kropce cykl zaczyna się od pierwszej,
- repertuar kina też liczy się do kolejności kropek.

---

## 15. QR „Jak dotrzeć”

Kod QR do trasy kina jest plikiem:

```text
KOD_QR_KINO_TRASA.png
```

Pokazuje się tylko podczas repertuaru kina.

Jeżeli trzeba zmienić QR:

1. przygotować nowy plik PNG,
2. nazwać go `KOD_QR_KINO_TRASA.png`,
3. podmienić plik w repozytorium,
4. odświeżyć ekran `Ctrl + F5`.

---

## 16. Cache i odświeżanie

GitHub Pages i przeglądarka mogą trzymać starą wersję strony.

Jeżeli po zmianach nic się nie zmienia:

- nacisnąć `Ctrl + F5`,
- albo dopisać do linku parametr, np. `&odswiez=1`.

Przykład:

```text
https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/index-kino.html?ekran=hybryda&odswiez=1
```

---

## 17. Co może edytować osoba nietechniczna

Osoba nietechniczna powinna edytować tylko:

- zawartość folderu `Plakaty-Miasto`,
- zawartość folderu `Plakaty-MOKSiAL`,
- same pliki plakatów.

Nie powinna edytować:

- `index.html`,
- `index-kino.html`,
- plików `.json`,
- `config-kino.json`,
- workflow GitHub Actions,
- plików technicznych.

---

## 18. Szybka ściąga dla MOKSiAL

| Element | Wartość |
|---|---|
| Folder | `Plakaty-MOKSiAL` |
| Nazwa zwykłego plakatu | `2026-07-15_Koncert_letni.jpg` |
| Nazwa plakatu z wagą | `2026-07-15_Koncert_letni_W5.jpg` |
| Nazwa plakatu wyświetlanego dłużej | `2026-07-31_Kalendarz_wydarzen_W8_dluzej.jpg` |
| Link do ekranu MOKSiAL | [Otwórz ekran](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=moksial) |

---

## 19. Szybka ściąga dla Miasta / Informacji Turystycznej

| Element | Wartość |
|---|---|
| Folder | `Plakaty-Miasto` |
| Nazwa zwykłego plakatu | `2026-07-20_Wydarzenie_miejskie.jpg` |
| Nazwa plakatu z wagą | `2026-07-20_Wydarzenie_miejskie_W6.jpg` |
| Nazwa plakatu wyświetlanego dłużej | `2026-07-31_Kalendarz_miejski_W8_dluzej.jpg` |
| Link do ekranu Miasta | [Otwórz ekran](https://szajac217-dev.github.io/MOKSiAL-ekrany-nowe/?ekran=miasto) |

> **Najważniejsza zasada:**  
> Nie edytować plików technicznych. Wrzucać tylko dobrze nazwane plakaty do właściwego folderu.
