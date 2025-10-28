# 🧩 Gra terenowa – Oleśnicka przygoda

Interaktywna gra terenowa w przeglądarce, stworzona z myślą o zabawie drużynowej w terenie.  
Każdy zespół rozwiązuje kolejne zagadki, zdobywa litery i na końcu układa hasło końcowe. 🔠

---

## 🎮 Jak grać

1. **Wpisz nazwę drużyny** na stronie startowej.  
   - Nazwa zostaje zapamiętana, nawet po odświeżeniu strony.  
2. **Rozwiązuj zagadki** na kolejnych stronach (`1.html`, `2.html`, `3.html`…).  
   - Za każdą poprawną odpowiedź otrzymasz **jedną literę**.  
   - Masz ograniczoną liczbę prób – po ich wykorzystaniu odpowiedzi się blokują.  
3. **Na końcu** zobaczysz stronę z gratulacjami i wszystkimi zebranymi literami.  
   - Z nich należy ułożyć hasło końcowe.

---

## 🗺️ Mapa

Na każdej stronie znajduje się niebieski przycisk w prawym górnym rogu.  
Po jego kliknięciu wyświetla się mapa (`obraz.jpg`), która może pomóc w orientacji w terenie.

---

## 💾 Zapamiętywanie postępu

- Gra **automatycznie zapisuje postęp** w pamięci przeglądarki (`localStorage`).
- Po odświeżeniu strony:
  - zachowuje nazwę drużyny,  
  - pokazuje stan prób i zdobyte litery,  
  - uniemożliwia ponowne udzielanie odpowiedzi po zakończeniu zagadki.
- Reset następuje **tylko po zmianie nazwy drużyny**.

---

## ⚙️ Jak dodać nowe zagadki

1. Skopiuj np. `3.html` i zapisz jako `5.html`.  
2. W kodzie zmień:
   - pytanie,  
   - poprawną odpowiedź (`const correctAnswer = "..."`),  
   - literę (`const letter = "..."`),  
   - limit prób (`const maxAttempts = ...`),  
   - oraz odnośnik `const nextPage = "..."`.  
3. W poprzedniej zagadce ustaw `nextPage = "5.html"`.  
4. Gotowe – nowa zagadka działa automatycznie!  




