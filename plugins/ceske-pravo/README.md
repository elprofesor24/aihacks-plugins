# České právo

Odborné metodiky 50 oblastí českého práva pro vašeho AI agenta. Plugin připojí Claude ke službě AIhacks: agent si podle úlohy vybere oblast práva (například spotřebitelské, pracovní nebo smluvní právo) a postupuje podle její metodiky. Metodika ho vede k ověření znění předpisů k rozhodnému dni, k oficiálním pramenům a k oddělení doloženého od nejistého.

Výstupy nejsou právní radou pro konkrétní věc a nenahrazují advokáta.

## Instalace v Claude Code

```
/plugin install ceske-pravo --marketplace elprofesor24/aihacks-plugins
```

V aplikaci Claude, ChatGPT nebo Codex se připojte podle návodu na https://aihacks.cz/pripojit/legal-cz/.

## Co plugin obsahuje a co odesílá

- Vstupní skill `ceske-pravo` s pravidly práce a bezpečnosti.
- Připojení k MCP serveru AIhacks na adrese https://app.aihacks.cz/mcp.

Plugin sám nic nespouští ani neinstaluje. Agent volá dva nástroje jen pro čtení: `list_workflows` (seznam oblastí a stav přístupu) a `get_workflow` (metodika jedné oblasti). Na server se odesílá pouze id oblasti a název souboru, nikdy obsah konverzace ani dokumenty.

## Účet a přístup

Při prvním použití se přihlásíte k účtu AIhacks (OAuth). Tři oblasti jsou zdarma: Spotřebitelské právo, Ochrana osobnosti a GDPR a Energetické právo. Ostatní zpřístupňuje předplatné, které se sjednává na webu https://aihacks.cz, ne v pluginu.

## English summary

České právo gives Claude methodologies for 50 fields of Czech law. The plugin is published by MaxStrategy s.r.o. and connects through the AIhacks platform, which exposes two read-only tools; only a field id and a file name are sent, never conversation content. Sign-in uses an AIhacks account; three fields are free.

Provozovatel: MaxStrategy s.r.o. · https://aihacks.cz · info@aihacks.cz · [Podmínky](https://aihacks.cz/podminky/) · [Ochrana osobních údajů](https://aihacks.cz/soukromi/)
