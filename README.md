# Email Chatbot

## Popis projektu
Tento projekt implementuje jednoduchý SMTP server a chatbota, který automaticky odpovídá na příchozí e-maily na základě jejich obsahu. Projekt je ideální pro testování automatizace e-mailů a řešení častých dotazů.

## Funkce
- **SMTP server:** Běží lokálně na portu `1025` a zpracovává příchozí e-maily.
- **Chatbot:** Automaticky generuje odpovědi na e-maily na základě klíčových slov v těle nebo předmětu zprávy.
- **Testovací scénáře:** Obsahuje předdefinované situace pro ověření funkcionality chatbota.

## Požadavky
- Python 3.8+
- Knihovny:
  - `aiosmtpd`
  - `email`
  - `smtplib`
  - `re`
  - `logging`

## Instalace
1. Nainstalujte potřebné knihovny:
   ```bash
   pip install aiosmtpd
   ```
2. Nakopírujte kód do Python skriptu (například `email_chatbot.py`).

## Použití
1. Spusťte skript:
   ```bash
   python email_chatbot.py
   ```
2. Skript automaticky spustí lokální SMTP server a začne testovací scénáře.

## Testovací scénáře
Skript obsahuje následující testovací situace:
- Dotaz na cenu
- Dotaz na dostupnost zboží
- Reklamace
- Obecný dotaz

Každý test:
1. Odesílá testovací e-mail na server.
2. Generuje odpověď na základě klíčových slov.
3. Loguje přijaté zprávy a odpovědi.

## Jak funguje generování odpovědí
Chatbot vyhledává klíčová slova v těle nebo předmětu zprávy:
- **"ceník", "cena", "ceny"** → Odpovídá s odkazem na ceník.
- **"dostupnost", "skladem"** → Informuje o skladových zásobách.
- **"reklamace"** → Potvrzuje přijetí reklamace.
- **Jiné dotazy** → Obecná odpověď s informací o zpětné vazbě.

## Možná vylepšení
- Napojit chatbot na reálný SMTP server (např. Gmail).
- Vylepšit analýzu obsahu pomocí pokročilých NLP modelů.
- Vytvořit webové rozhraní pro konfiguraci a přizpůsobení odpovědí.

## Licenční podmínky
Tento projekt je distribuován pod licencí MIT. Používejte dle vlastních potřeb.

## Kontakt
Pokud máte dotazy nebo chcete projekt upravit, kontaktujte autora na:
- **E-mail:** lukas.drsticka@gmail.com
- **GitHub:** Lukedaca

# skript můžete jednoduše spustit v google colabu

