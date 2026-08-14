# NextPhase 🚀
**Osobní organizér a správce projektů**

NextPhase je komplexní webová aplikace sloužící jako osobní organizér. Je navržena primárně pro studenty a freelancery, kteří potřebují mít absolutní přehled o svých školních či osobních projektech, úkolech a termínech na jednom místě. Cílem projektu je eliminovat nutnost používat několik různých aplikací pro time management a sjednotit veškerou agendu do přehledného rozhraní.

## 🌟 Hlavní funkce

*   **Správa projektů** – Vytváření projektů, jejich rozřazování do kategorií a evidence spojených úkolů a deadlinů[cite: 1].
*   **Správa úkolů (To-do list)** – Centrální správa úkolů pro jednotlivé projekty i samostatných osobních/školních úkolů s možností nastavení termínu splnění[cite: 1].
*   **Tagovací systém** – Tvorba vlastních barevných štítků (tagů) pro lepší filtraci a organizaci jednotlivých úkolů[cite: 1].
*   **Dashboard** – Hlavní přehledová obrazovka zobrazující aktuální stav a úkoly na probíhající týden[cite: 1].
*   **Kalendář** – Vizuální zobrazení deadlinů a událostí s možností okamžitého přidávání nových[cite: 1].
*   **Notes (Rychlé poznámky)** – Prostor pro ukládání rychlých nápadů, poznámek nebo užitečných odkazů pro pozdější využití[cite: 1].

## 🛠️ Použité technologie

*   **Backend:** PHP
*   **Databáze:** MySQL
*   **Frontend:** HTML, CSS
*   **Vývojové prostředí:** Vyvíjeno s využitím PHPStorm (lze spustit v libovolném prostředí)

## 🗄️ Architektura databáze

Aplikace využívá relační databázi s následující strukturou[cite: 1]:

*   `Users`: user_id (PK), jméno, e-mail, hash_hesla
*   `Projects`: project_id (PK), user_id, název, kategorie, deadline
*   `Tasks`: task_id (PK), project_id, název, stav, datum_splnění
*   `Tags`: tag_id (PK), user_id, název, barva_tagu
*   `Task_Tags`: task_id (FK), tag_id (FK)
*   `Events`: event_id (PK), user_id, project_id, popis, start_datetime, end_datetime

## 🚀 Instalace a spuštění lokálně

1. Naklonujte si tento repozitář na svůj lokální server:
   ```bash
   git clone [https://github.com/vase-uzivatelske-jmeno/nextphase.git](https://github.com/vase-uzivatelske-jmeno/nextphase.git)
