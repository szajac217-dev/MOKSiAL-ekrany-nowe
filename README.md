# Nowe ekrany informacyjne MOKSiAL

Gotowa paczka do wdrożenia na GitHub Pages.

## Tryby ekranu

- `?ekran=moksial` – plakaty z folderu `Plakaty-MOKSiAL`
- `?ekran=miasto` – plakaty z folderu `Plakaty-Miasto`
- `?ekran=hybryda` – najpierw MOKSiAL, potem Miasto

## Wymagane foldery

Utwórz w repozytorium foldery:

- `Plakaty-MOKSiAL`
- `Plakaty-Miasto`

Jeżeli GitHub nie pozwala utworzyć pustego folderu, dodaj w nim plik `.gitkeep`.

## Logo

W głównym katalogu powinny być pliki:

- `logo-moksial.png`
- `logo-szklarska.png`

W trybie hybryda logo przełącza się automatycznie zależnie od aktualnego plakatu:

- plakat z `Plakaty-MOKSiAL` → `logo-moksial.png`
- plakat z `Plakaty-Miasto` → `logo-szklarska.png`

Jeśli `logo-moksial.png` nie będzie jeszcze wrzucone, ekran spróbuje użyć awaryjnie `logo-moksial.svg`.

## QR

Wielkość kodów QR w `index.html`:

Szukaj:

```css
.qri{width:clamp(84px,9vw,132px);height:clamp(84px,9vw,132px);
```

oraz:

```css
.qri img{width:92%;height:92%;object-fit:contain}
```

Dla większych QR można ustawić np.:

```css
.qri{width:clamp(110px,11.5vw,170px);height:clamp(110px,11.5vw,170px);
.qri img{width:96%;height:96%;object-fit:contain}
```

## GitHub Pages

Settings → Pages → Deploy from a branch → `main` → `/root`.
