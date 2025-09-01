# Food Printer — od MVP do platformy „FoodOS”

## 1. Cel projektu i kontekst
Celem projektu jest opracowanie domowego systemu druku żywności, łączącego automatyzację przygotowania posiłków z personalizacją żywieniową. Projekt adresuje podstawowe potrzeby żywieniowe (piramida Maslowa) oraz problemy rynku żywności: wysoki poziom przetworzenia, marnotrawstwo składników, nieprzejrzyste łańcuchy dostaw i wzrost chorób dietozależnych. Zakładany wpływ społeczny obejmuje łatwiejszy dostęp do zdrowych, spersonalizowanych i powtarzalnych posiłków oraz redukcję odpadów.

## 2. Fazy i status
- **Faza 1 – Pancake Printer (PoC/MVP)** — zakończona. Potwierdzono wykonalność techniczną i sens ekonomiczny druku naleśników w wielu kolorach i kształtach.
- **Faza 2 – Pre-produkt** — w toku. Cel: zwiększenie powtarzalności, pieczenie kolejnych warstw, modernizacja wkładów i dozowania (CIP), konsultacje z użytkownikami i dobór menu startowego.
- **Faza 3 – Certyfikacja i pilotaże** — planowana. Pakiet HACCP/CE oraz pilotaże w wybranych lokalizacjach.
- **Wizja długoterminowa – „FoodOS”** — platforma do wielu potraw, subskrypcyjny model wkładów oraz komponenty AI wspierające dobór diety, harmonogram i zakupy.

## 3. Zakres rzeczowy (skrót)
**W zakresie:** mechanika (CoreXY), dozowanie (pompa perystaltyczna z kompensacją), sterowanie/GUI, generator ścieżek (PNG/SVG → G-code), proces termiczny, higiena/CIP, przygotowanie zgodności (HACCP/CE), badania użytkowników i pilotaże.  
**Poza zakresem obecnych faz:** zaawansowana diagnostyka medyczna i pełna industrializacja produkcji wkładów.

## 4. Rezultaty Fazy 1 (MVP)
- **Mechanika:** rama z profili aluminiowych 30×30; kinematyka **CoreXY** (paski **GT2**); oś Z: **NEMA17 + śruba T8** (nakrętka kompensująca luz).
- **Napędy/sterowanie:** silniki **NEMA17** ze sterownikami **TMC2209** (feedback ze sterowników – podejście hybrydowe), płyta **BTT Octopus**, autorski firmware i **GUI** dotykowe.
- **Proces termiczny:** elektryczny grill z kontrolą temperatury.
- **Dozowanie:** własny projekt **pompy perystaltycznej** z kompensacją pulsacji (A) oraz wariant B (bez kompensacji). W macierzy decyzji (Pugh) rozwiązanie A uzyskało najlepszy wynik dla kryteriów: koszt, zgodność „food-grade”, kompatybilność z systemem, precyzja dozowania, czyszczenie oraz czas developmentu.
- **Pipeline:** grafika (PNG/SVG) → separacja kolorów → mapowanie na kanały → **G-code** → druk.
- **Ekonomia jednostkowa (z prób):** składniki ok. **7,20 zł / 1,5 kg** ciasta; energia ok. **0,09 zł** na wydruk; koszt jednostkowy ok. **0,34 zł / naleśnik** (założenia w arkuszu kosztów).
- **Artefakty:** demo wideo (MVP), rendery, zdjęcia próbek, porównanie pulsacji (A vs B), macierz Pugh.

## 5. Architektura techniczna (skrót)
- **Mechanika:** CoreXY/GT2, prowadnice liniowe, separacja stref napędowej i „czystej”.
- **Elektronika:** BTT Octopus, TMC2209, czujniki (temperatura/pozycja), zasilanie i zabezpieczenia (E-stop, bezpieczniki).
- **Dozowanie i kanały:** pompa perystaltyczna NEMA17 z kompensacją; obecnie moduł przekaźnikowy 4–8 kanałów (docelowo PCB z tranzystorami).
- **Oprogramowanie:** firmware, GUI operatora, generator ścieżek; profile pieczenia i kalibracje.
- **Higiena/CIP:** konstrukcja DfC (design-for-cleaning), szybki demontaż, materiały dopuszczone do kontaktu z żywnością.

## 6. Plan prac i zarządzanie
**Work Packages:** WP1 Zarządzanie; WP2 Mechanika; WP3 Dozowanie; WP4 Elektronika/bezpieczeństwo; WP5 Firmware/Software; WP6 Testy i walidacja; WP7 Zgodność i certyfikacja; WP8 Pilotaże i wejście na rynek.

**Harmonogram (skrót):**
```mermaid
gantt
  title Roadmap (Faza 1–3)
  dateFormat YYYY-MM-DD
  section Faza 1 – MVP
  Projekt i integracja            :done, 2023-10-02, 2023-12-11
  section Faza 2 – Pre-produkt
  Powtarzalność & CIP             :active, 2025-09-01, 45d
  Pieczenie kolejnych warstw      :2025-10-01, 30d
  Moduł wkładów i UX              :2025-10-15, 30d
  section Faza 3 – Certyfikacja i pilotaże
  HACCP/CE + pilotaże             :2025-11-15, 60d
