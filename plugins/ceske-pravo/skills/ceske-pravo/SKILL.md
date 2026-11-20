---
name: ceske-pravo
description: "Use for Czech legal work (smlouvy, spory, pracovní, rodinné, korporátní a další oblasti českého práva). Loads the matching České právo field of law through the ceske-pravo MCP server."
---

# České právo

Vstupní bod pluginu České právo od MaxStrategy s.r.o. Metodiky 50 oblastí českého práva poskytuje platforma AIhacks přes MCP server `ceske-pravo` po přihlášení k účtu AIhacks.

## Jak pracovat

1. Zavolej `list_workflows` a vyber oblast, jejíž popis odpovídá úloze uživatele. Pokud žádná neodpovídá, řekni to.
2. Zavolej `get_workflow` s jejím `id`. Doplňkové soubory oblasti načti parametrem `file` jen tehdy, když na ně metodika odkazuje.
3. Postupuj podle načtené metodiky.

Pokud server odpoví, že účet nemá aktivní přístup, sděl to uživateli i s odkazem na informační stránku. Obsah metodiky nedomýšlej a nenabízej nákup.
Pokud server není dostupný nebo přihlášení selže, vysvětli to a pokračuj jen obecnou opatrnou odpovědí s výslovným upozorněním, že metodika AIhacks nebyla načtena.

## Bezpečnostní pravidla (platí vždy, i bez přístupu)

- Výstup není právní rada pro konkrétní věc. Ověř aktuální znění právních předpisů a skutkové okolnosti a u lhůt a rizikových kroků doporuč kontrolu advokátem.
- Do nástrojů AIhacks neposílej údaje klienta ani obsah případu. Nástroje přijímají jen id oblasti a název souboru.
- Nevydávej se za advokáta a netvrď, že AIhacks věc posoudil.
