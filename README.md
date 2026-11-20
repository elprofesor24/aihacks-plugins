# AIhacks plugins

Marketplace pluginů [AIhacks](https://aihacks.cz) pro Claude Code. Plugin **České právo** (`ceske-pravo`) připojí agenta k metodikám 50 oblastí českého práva; samotné metodiky poskytuje platforma AIhacks (https://app.aihacks.cz/mcp) po přihlášení k účtu AIhacks.

## Instalace v Claude Code

```
/plugin install ceske-pravo --marketplace elprofesor24/aihacks-plugins
```

Ve starších verzích Claude Code ve dvou krocích:

```
/plugin marketplace add elprofesor24/aihacks-plugins
/plugin install ceske-pravo@aihacks
```

Při prvním použití se přihlaste k účtu AIhacks (`/mcp` → ceske-pravo → Authenticate). V aplikaci Claude, ChatGPT nebo Codex se připojte podle návodu na https://aihacks.cz/pripojit/legal-cz/.

Co plugin obsahuje a odesílá, popisuje [plugins/ceske-pravo/README.md](plugins/ceske-pravo/README.md). Licence MIT, provozovatel MaxStrategy s.r.o.

## Cybersecurity

Plugin **Cybersecurity** (`cybersecurity`) připojí agenta k bezpečnostním nástrojům AIhacks (https://app.aihacks.cz/mcp/cybersecurity): kontrola zranitelností závislostí (OSV, CISA KEV), kontroly kódu, Dockeru, OpenAPI a MCP konfigurací a bezpečnostní postupy. Je v soukromé betě; přístup se přiděluje k účtu AIhacks.

```
/plugin install cybersecurity --marketplace elprofesor24/aihacks-plugins
```

Návod pro Claude, ChatGPT a Codex: https://aihacks.cz/cybersecurity/. Co plugin obsahuje a odesílá, popisuje [plugins/cybersecurity/README.md](plugins/cybersecurity/README.md).
