![Build Status](https://api.travis-ci.com/RDevWasTaken/ts-lekcja-bot.svg?branch=main)

# TS Lekcja Bot
Bot Discord z integracj膮 MS Teams napisany w TypeScript

## 馃攳 Funkcje
- Pobieranie spotka艅 z kalendarza w danym dniu
- Graficzne powiadomienia na Discord
- Oznaczanie odpowiednich grup za pomoc膮 s艂贸w kluczowych
- Mo偶liwo艣膰 dodania niestandardowych spotka艅

## 馃敤 Instalacja
Zalecana wersja Node.JS: 12

Instalacja TypeScript
```sh
npm i -g typescript
npm i -g ts-node
```
Instalacja potrzebnych modu艂贸w
```sh
cd ts-lekcja-bot
npm i
```
Uruchomienie bota (przed tym nale偶y stworzy膰 pliki .env i bot-config.json zgodnie z przyk艂adami)
```sh
npm start
```

## 馃摑 Konfiguracja
W pliku `.env` nale偶y umie艣ci膰 token swojego bota oraz dane logowania do MS Teams.
Przyk艂ad w [`.env.example`](https://github.com/RDevWasTaken/ts-lekcja-bot/blob/main/.env.example)

Om贸wienie pliku `bot-config.js` (przyk艂ad w [`bot-config.json.example`](https://github.com/RDevWasTaken/ts-lekcja-bot/blob/main/bot-config.json.example))
| Sekcja | Rola |
| ------ | ------ |
| Settings | Ustawienia bota |
| Translations | T艂umaczenia r贸偶nych tekst贸w |
| Groups | Lista grup (ID roli Discord oraz s艂owa kluczowe) |
| Custom | Niestandardowe spotkania |

Niekt贸re w艂a艣ciwo艣ci:
 - `defaultPing` - domy艣lne oznaczenie gdy 偶adna z grup nie zosta艂a znaleziona (mo偶e by膰 to oznaczenie roli - `<@&ID_ROLI>`)
 - `exclusivePing` [true/false] - gdy ustawione jest `true` to bot opinguje `defaultPing` gdy liczba grup jest mniejsza od liczby spotka艅

## 馃帹 Rozw贸j projektu
Je艣li chcesz wspom贸c rozw贸j bota, mo偶esz zg艂asza膰 problemy/pomys艂y w zak艂adce *Issues* lub z艂o偶y膰 *Pull Request*!
Z g贸ry dzi臋ki!

## Licencja
MIT