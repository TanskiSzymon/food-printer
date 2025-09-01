# Arkusz kosztów — prosty przykład (Faza 1)

**Źródła danych:** wartości pochodzą z dostarczonych materiałów (przepis, ceny za 100g/100ml, koszty energii). Wszystkie kwoty w PLN (zł).
Założenia: używamy cen jednostkowych z tabeli „Cena za 100g/100ml/1 szt” i danych z arkusza energii.

---



## 1) Składniki przepisu (ilości i koszty)

| Składnik | Ilość | Cena za 100g / 100ml / 1 szt | Koszt (PLN) |
|---|---:|---:|---:|
| Mąka | 500 g | 0,20 zł / 100g | 1,00 |
| Mleko | 500 ml | 0,40 zł / 100ml | 2,00 |
| Oliwa | 10 g | 6,00 zł / 100g | 0,60 |
| Barwnik | 0,5 g | 100,00 zł / 100g | 0,50 |
| Aromat | 0,5 g | 100,00 zł / 100g | 0,50 |
| Woda | 300 ml | 0,20 zł / 100ml | 0,60 |
| Jajka | 2 szt. | 1,00 zł / 1 szt. | 2,00 |
| **Suma (koszty składników)** | | | **7,20** |

**Waga całkowita masy ciasta:** 1,5 kg (1500 g)

---

## 2) Koszt jednostkowy surowca i koszt porcji

- Koszt na 1 g ciasta = `7,20 / 1500` = **0,0048 zł/g**  
- Przykładowa porcja (naleśnik) = **70 g**  
- Koszt składników na 70 g = `70 * 0,0048` = **0,336 zł ≈ 0,34 zł**

---

## 3) Energia elektryczna (na wydruk jednego naleśnika)

Dane: cena za 1 kWh = **0,75 zł**, moc urządzenia ≈ **2,35 kW**, czas wydruku ≈ **0,05 h**.

- Zużycie energii = `2,35 kW * 0,05 h` = **0,1175 kWh**  
- Koszt energii = `0,1175 kWh * 0,75 zł/kWh` = **0,0881 zł ≈ 0,09 zł**

---

## 4) Całkowity koszt porcji (ingrediencje + energia)

- Koszt składników (70 g) = **0,336 zł**
- Koszt energii = **0,088 zł**
- **Razem = 0,424 zł ≈ 0,42 zł / naleśnik**

> Uwaga: powyższe wyliczenia nie obejmują kosztów amortyzacji urządzenia, kosztów wkładów eksploatacyjnych (opakowania), kosztów pracy/serwisu ani kosztów logistycznych. Są to koszty bezpośrednie surowcowo-energetyczne dla jednej porcji.

---

## 5) Szybkie podsumowanie (wartości zaokrąglone)
- Koszt surowcowy na porcję (70 g): **0,34 zł**
- Koszt energii na porcję: **0,09 zł**
- Koszt całkowity na porcję (surowce + energia): **0,42 zł**

---
