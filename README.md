# 🚦 Sygnalizacja świetlna na skrzyżowaniu

Projekt przedstawia prostą sygnalizację świetlną wykonaną w **Tinkercad Circuits** z wykorzystaniem Arduino.

Układ składa się z **4 świateł**, a każde światło posiada:
- 🔴 czerwoną diodę LED,
- 🟢 zieloną diodę LED.

Światła zmieniają się kolejno zgodnie z ruchem wskazówek zegara.

## 🛠️ Wykorzystane elementy

- Arduino Uno
- płytka stykowa (breadboard)
- 4 × czerwona dioda LED
- 4 × zielona dioda LED
- 8 × rezystor 220 Ω
- przewody połączeniowe

## 🔌 Schemat połączeń

| Skrzyżowanie | 🔴 Czerwona LED | 🟢 Zielona LED |
|---|---:|---:|
| 1 | D2 | D11 |
| 2 | D3 | D10 |
| 3 | D4 | D9 |
| 4 | D5 | D8 |

### Katody

Katody wszystkich 8 diod LED są podłączone do **MASA (GND)** Arduino.

### Anody

Każda anoda LED jest podłączona przez osobny rezystor **220 Ω** do odpowiedniego pinu Arduino.

Schemat pojedynczej diody:

```text
PIN Arduino
     │
     │
  220 Ω
     │
     │
  Anoda LED
     │
  Katoda LED
     │
     │
   MASA
