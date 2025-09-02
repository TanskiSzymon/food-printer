# Food Printer — od MVP do platformy „FoodOS”
![Pierwszt MVP](images/Render_front.png)
---

## 1. Cel projektu i kontekst
Projekt dotyczy opracowania domowego systemu druku żywności, łączącego automatyzację przygotowania posiłków z personalizacją żywieniową. Adresuje on podstawę piramidy Maslowa (odżywianie) i bieżące problemy rynku żywności: wysoki poziom przetworzenia, marnotrawstwo, nieprzejrzyste łańcuchy dostaw oraz wzrost chorób dietozależnych. Zakładany wpływ społeczny obejmuje łatwiejszy dostęp do zdrowych, spersonalizowanych posiłków oraz redukcję odpadów i zużycia energii.

**Teza projektu:** druk żywności w warunkach domowych może być technicznie wykonalny, ekonomicznie uzasadniony i korzystny społecznie – pod warunkiem zapewnienia powtarzalności procesu, higieny (CIP) i zgodności z normami bezpieczeństwa.


## 2. Fazy i status

Projekt realizowany jest w czterech etapach. Każdy etap ma wyraźnie określone cele i kryteria przejścia.

| Etap | Status | Ramy czasowe | Cel etapu (skrót) |
|------|--------|--------------|-------------------|
| **Etap 1 — PoC** | **zakończony** | 2023-10-02 → 2024-09-11 | potwierdzenie technicznej wykonalności druku naleśników w różnych kształtach/kolorach i wstępna walidacja ekonomiczna |
| **Etap 2 — MVP** | **w toku** | 2025-07-01 → 2026-04-18 | urządzenie reprezentatywne dla użytkownika: stabilne dozowanie (bez pulsacji), system pieczenia warstwowego, komora klimatyczna, szybka wymiana wkładów, GUI z CIP, dokumentacja serwisowa |
| **Etap 3 — Iteracje rynkowe** | planowany | 2026-04-19 → 2026-09-15 | feedback z pilotaży, iteracyjne poprawki HW/SW, optymalizacja menu startowego, walidacja KPI (NPS, waste, repeatability) |
| **Etap 4 — Certyfikacja i pilotaże komercyjne** | planowany | 2026-09-15 → 2027-01-13 | przygotowanie i złożenie dokumentacji HACCP/CE, audyty, pilotaże w docelowych lokalizacjach (szkoły, HoReCa, eventy) |

Każdy etap kończy się oceną kryteriów wyjścia (exit criteria) i raportem techniczno-biznesowym, stanowiącym podstawę do decyzji o kontynuacji prac i pozyskaniu kolejnych środków.

---

```mermaid
gantt
  title Food Printer — Roadmapa (etapy + kamienie milowe)
  dateFormat YYYY-MM-DD
  excludes  weekends

  section Etapy
  Etap 1 — PoC (zakończony)                    :done,    poc1, 2023-10-02, 2024-09-11
  Etap 2 — MVP (rozwój / stabilizacja)         :active,  mvp2, 2025-07-01, 292d
  Etap 3 — Iteracje rynkowe i uczenie          :         it3,  2026-04-19, 150d
  Etap 4 — Certyfikacja i pilotaże             :         cer4, 2026-09-15, 120d

  section Kamienie milowe
  M1  — PoC zakończony (dowód koncepcji)                     :milestone, m1,  2024-09-11, 0d
  M2.1— Konstrukcja zoptymalizowana (DFM/BOM)                :milestone, m21, 2025-09-30, 0d
  M2.2— Systemy pieczenia zintegrowane (bottom + top)        :milestone, m22, 2026-01-15, 0d
  M2.3— Pompa + elektronika bez pulsacji (RC)                :milestone, m23, 2026-02-15, 0d
  M2.4— Integracja systemowa ukończona                       :milestone, m24, 2026-03-17, 0d
  M2.5— MVP Release Candidate (gotowe do pilotażu)           :milestone, m25, 2026-04-18, 0d
  M3  — Walidacja rynkowa / wyniki pilotaży                  :milestone, m3,  2026-09-01, 0d
  M4  — Złożenie dokumentacji certyfikacyjnej                :milestone, m4,  2026-10-20, 0d
  M5  — Start pilotaży komercyjnych                          :milestone, m5,  2026-11-15, 0d
  M6  — Go-to-market / pierwsze wdrożenia                    :milestone, m6,  2027-03-01, 0d
```




---

## 2. Fazy i status

Projekt realizowany jest w czterech etapach. Każdy etap ma wyraźne cele i kryteria przejścia do kolejnej fazy.

- **Etap 1 — PoC (Proof of Concept)** — *zakończony* (2023-10-02 → 2024-09-11). Cel wykonany: techniczna wykonalność druku naleśników w różnych kolorach i kształtach oraz wstępna weryfikacja sensu ekonomicznego rozwiązania.
- **Etap 2 — MVP (Minimum Viable Product)** — *w toku* (rozpoczęcie: 2025-07-01). Cel: doprowadzenie urządzenia do stanu reprezentatywnego dla użytkownika końcowego — stabilne dozowanie, poprawiona powtarzalność, użyteczny interfejs operatora, podstawowe procedury higieniczne (CIP) i dokumentacja montażowa/serwisowa.
- **Etap 3 — Iteracje rynkowe, badania użytkowników i uczenie** — *planowany*. Cel: zbieranie feedbacku z testów użytkowników i pilotaży, iteracyjne poprawki sprzętowe i software’owe, optymalizacja menu startowego, walidacja założeń biznesowych i metryk KPI (NPS, waste, repeatability). Etap koncentruje się na szybkim cyklu „test → learn → adjust”.
- **Etap 4 — Zgodność, certyfikacja i pilotaże komercyjne** — *planowany*. Cel: przygotowanie i przeprowadzenie działań zgodnościowych (HACCP, wymagania CE/LVD/EMC tam, gdzie stosowne), finalne audyty, oraz wdrożenie pilotaży w środowiskach docelowych (szkoły, eventy, partnerzy HoReCa).

Każdy etap zamykany jest oceną kryteriów wejścia/wyjścia (exit criteria) oraz krótkim raportem technicznym i biznesowym, niezbędnym do decyzji o kontynuacji prac i ewentualnym pozyskaniu finansowania na dalsze prace.

---
```mermaid
gantt
  title Food Printer — Roadmapa (etapy + kamienie milowe)
  dateFormat  YYYY-MM-DD
  excludes    weekends

  section Etapy
  Etap 1 — PoC (zakończony)                    :done,    poc1, 2023-10-02, 2024-09-11
  Etap 2 — MVP (rozwoj / stabilizacja)         :active,  mvp2, 2025-07-01, 230d
  Etap 3 — Iteracje rynkowe i uczenie          :         it3,  2026-03-01, 120d
  Etap 4 — Certyfikacja i pilotaże             :         cer4, 2026-09-15, 120d

  section Kamienie milowe
  M1 — PoC zakończony (dowód koncepcji)        :milestone, m1, 2024-09-11, 0d
  M2 — MVP (beta ready — testy wewnętrzne)     :milestone, m2, 2025-12-15, 0d
  M3 — MVP Release Candidate (RC)              :milestone, m3, 2026-03-15, 0d
  M4 — Walidacja rynkowa / wyniki pilotaży     :milestone, m4, 2026-07-01, 0d
  M5 — Złożenie dokumentacji certyfikacyjnej   :milestone, m5, 2026-10-20, 0d
  M6 — Start pilotaży komercyjnych             :milestone, m6, 2026-11-15, 0d
  M7 — Go-to-market / pierwsze wdrożenia       :milestone, m7, 2027-03-01, 0d
```
## 3. Zakres rzeczowy (skrót)

**W zakresie realizacji (Faza 1–4):**
- Mechanika nośna i kinematyka (CoreXY, prowadnice liniowe, konstrukcja modułowa).
- System dozowania (pompa perystaltyczna z kompensacją pulsacji; architektura kanałów dozujących).
- Układ sterowania i elektronika (BTT Octopus / TMC2209; E-stop; zabezpieczenia).
- Firmware i oprogramowanie użytkownika (GUI operatora, pipeline: PNG/SVG → G-code, profile pieczenia).
- Procedury higieniczne i operacyjne (design-for-cleaning, instrukcje CIP/SOP).
- Testy i walidacja (powtarzalność dozowania, pomiary energetyczne, badania sensoryczne).
- Przygotowanie do zgodności i certyfikacji (dokumentacja HACCP draft, ścieżka CE, wymagania materiałowe).
- Materiały komunikacyjne i przygotowanie pilotaży (renderingi, wideo demo, ankiety, raporty pilotażowe).
- Pakiet grantowy (narracja, logframe, workplan, budżet wysokiego poziomu, rejestr ryzyk).

**Poza zakresem obecnych etapów (nie obejmowane w krótkim terminie):**
- Pełna, przemysłowa produkcja wkładów do żywności (skalowanie linii produkcyjnej).
- Zaawansowana diagnostyka medyczna i formalne doradztwo dietetyczne wymagające certyfikowanych usług medycznych.
- Integracja z zewnętrznymi systemami zdrowotnymi wymagającymi przekazywania danych medycznych bez odrębnych analiz prawnych i zgodności.

Zakres prac konstruowany jest modułowo, by umożliwić równoległe prowadzenie prac rozwojowych (mechanika, elektronika, software) oraz przygotowań formalnych (compliance, dokumentacja) niezbędnych dla etapów 3–4.
---

## 4. Rezultaty Fazy 1 (MVP)

Watch the video below to see first prototype in action:

<p align="center">
  <a href="https://www.youtube.com/watch?v=P8IgyybBxyM">
     <img src="https://img.youtube.com/vi/P8IgyybBxyM/0.jpg" alt="Watch the video.">
  </a>
</p>

**Mechanika:** rama z profili aluminiowych 30×30; kinematyka **CoreXY** na paskach **GT2**; oś Z: **NEMA17 + śruba trapezowa T8** (nakrętka kompensująca luz).  
**Napędy i sterowanie:** silniki **NEMA17** ze sterownikami **TMC2209** (wykorzystanie informacji zwrotnej z driverów – podejście hybrydowe), płyta główna **BTT Octopus**, autorski firmware oraz **GUI** dotykowe.  
**Proces termiczny:** elektryczny grill z kontrolą temperatury (stabilizacja wypieku ścieżek).  
**Dozowanie:** własny projekt **pompy perystaltycznej** na NEMA17; przebadano dwa warianty – **A (z kompensacją pulsacji)** i **B (bez kompensacji)**.  
**Macierz decyzji (Pugh):** porównano ślimak/extruder, tłok, perystaltyczną oraz perystaltyczną z kompensacją. Kryteria: koszt, „food-grade”, kompatybilność z systemem, precyzja dozowania, czyszczenie, czas developmentu. **Wybrano wariant A – perystaltyczną z kompensacją.**  
![Macierz pugh](images/pugh_matrix.png)
**Pipeline druku:** grafika (PNG/SVG) → separacja kolorów → mapowanie kanałów → **G-code** → druk.  
**Ekonomia jednostkowa (z prób):** składniki ok. **7,20 zł / 1,5 kg** ciasta; energia ok. **0,09 zł** na wydruk; **~0,42 zł / naleśnik** (założenia w tests/cost_summary.md).  
**Materiały referencyjne:** demo wideo działania MVP, rendery, zdjęcia próbek druku, wyniki porównania pulsacji (A vs B), macierz Pugh.

![Wyniki fazy 1](images/Phase_1_results.png)

---

## 5. Architektura techniczna (skrót)
- **Mechanika:** CoreXY/GT2, prowadnice liniowe, separacja stref napędowej i „czystej” (kontakt z żywnością).  
- **Elektronika:** BTT Octopus, TMC2209, czujniki (temperatura/pozycja), zasilanie i zabezpieczenia (E-stop, bezpieczniki).  
- **Dozowanie i kanały:** pompa perystaltyczna z kompensacją; obecnie moduł przekaźnikowy 4–8 kanałów (rozwiązanie tymczasowe), **docelowo** dedykowana płytka PCB z tranzystorami.  
- **Oprogramowanie:** firmware, GUI operatora, generator ścieżek; profile pieczenia i kalibracje.  
- **Higiena/CIP:** projekt „design-for-cleaning”, szybki demontaż, materiały dopuszczone do kontaktu z żywnością.

[Szczegóły etapu 1](phases/Phase_1.md)


---

## 6. Plan prac i zarządzanie

### 6.1 Work Packages (WP)
WP1 Zarządzanie; WP2 Mechanika; WP3 Dozowanie; WP4 Elektronika/bezpieczeństwo; WP5 Firmware/Software; WP6 Testy i walidacja; WP7 Zgodność i certyfikacja; WP8 Pilotaże i wejście na rynek.

### 6.2 Harmonogram (skrót)
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
```

### 6.3 WBS (orientacyjnie)
```mermaid
mindmap
  root((Food Printer))
    WP1 Zarządzanie
    WP2 Mechanika
    WP3 Dozowanie
    WP4 Elektronika
    WP5 FW/SW
    WP6 Testy
    WP7 Zgodność
    WP8 Pilotaże
```

**Proces i jakość:** repozytorium Git z szablonami Issue/PR, tablicą Kanban, przeglądami tygodniowymi, checklistami jakości i wersjonowaniem artefaktów.

---

## 7. KPI i kryteria sukcesu
- **Techniczne:** odchyłka dozowania ≤ 5%; **CIP ≤ 10 min**; awaryjność < 2% / 100 h; energia ≤ 0,1 kWh / porcję.  
- **Użytkowe:** NPS ≥ 40; czas przygotowania porcji ≤ 3 min; satysfakcja smaku ≥ 4/5.  
- **Środowiskowe:** odpad ≤ 5 g / porcję.  
- **Biznesowe:** koszt porcji konkurencyjny wobec alternatyw; ≥ 2–3 listy intencyjne na pilotaże.

---

## 8. Ryzyka i działania ograniczające
- **Higiena/CIP** — ryzyko niewystarczającej czystości; działanie: design-for-cleaning, testy ATP, materiały „food-grade”.  
- **Pulsacja przy gęstych pastach** — ryzyko jakości ścieżek; działanie: kompensacja pulsacji, profil prędkości, opcjonalne grzanie przewodów.  
- **Zgodność (HACCP/CE)** — ryzyko wydłużenia terminu; działanie: równoległy pre-audyt i wcześniejsze przygotowanie dokumentacji.  
- **Akceptacja rynku** — ryzyko niskiego NPS; działanie: iteracje menu, badania UX, materiały instruktażowe.

---

## 9. Struktura repozytorium publicznego (skrót)
- `tests/` — powtarzalność, energia, protokoły.  
- `docs/` — Gantt/WBS (Mermaid), macierz Pugh, zgodność (HACCP draft, ścieżka CE, GDPR/DMP).  
- `images/` — zdjęcia, rendery.  
- `phases/` — szczegółowe opisy poszczególnych faz

---

## 10. Moduł grantowy (skrót dla wniosków)
**Cel:** zapewnić spójny pakiet aplikacyjny pod programy grantowe (np. SWPS Startup Booster for Social Impact, PARP).  
**Elementy:**
- **Narracja skrócona** (streszczenie, wpływ społeczny, plan WP, KPI).  
- **Workplan** (WP/Deliverables/Milestones).  
- **Budżet wysokiego poziomu** (personel, prototypy, zgodność, pilotaże).  
- **Logframe** (cel, rezultat, wskaźniki, źródła weryfikacji).  
- **Rejestr ryzyk** (P×I, działania ograniczające).  
- **KPI i metody pomiaru** (Repeatability, Energy, Waste, NPS, PrepTime).  
- **Etyka i GDPR/DMP** (zakres danych, zgody, retencja, bezpieczeństwo).

> Rekomendacja: każdy wniosek utrzymywać w `grants/submissions/<program>/<rok>/` wraz z załącznikami: rendery, wideo demo, listy intencyjne, CV.

---
