# Hermes Cron Work

Repositório para versionamento e controle de configurações de cron jobs do Hermes Agent criados por Bruno Herbert.

## 📁 Estrutura do Projeto

```
hermes-cron-work/
├── README.md                    # Este arquivo
├── CHANGELOG.md                # Histórico de alterações
├── .gitignore                  # Arquivos ignorados pelo Git
├── docs/                       # Documentação adicional
│   └── setup.md               # Instruções de configuração
├── jobs/                       # Configurações individuais dos cron jobs
│   ├── email-summary/         # Resumo de emails (padrão)
│   ├── email-groq/            # Resumo de emails (GROQ)
│   ├── calendar-events/       # Compromissos do dia
│   └── weather-forecast/      # Previsão do tempo (Fazenda Trapia)
└── scripts/                    # Scripts auxiliares (se houver)
```

## 🚀 Cron Jobs Ativos

| ID | Nome | Schedule | Skill | Status |
|----|------|----------|-------|--------|
| `7074fa1a2497` | Resumo de Emails (4h) | `0 */4 * * *` | google-workspace | ✅ Ativo |
| `79960fc80b97` | Compromissos do Dia (7h) | `0 10 * * *` | google-workspace | ✅ Ativo |
| `c702f7a813f4` | Resumo de Emails GROQ (4h) | `0 */4 * * *` | google-workspace | ✅ Ativo |
| `410e8c8c7a3d` | Clima Fazenda Trapia (7h) | `0 10 * * *` | - | ✅ Ativo |

## 📝 Como Contribuir / Atualizar

1. Edite os arquivos de configuração no diretório `jobs/`
2. Atualize o `CHANGELOG.md` com as alterações
3. Faça commit com mensagem descritiva seguindo [Conventional Commits](https://www.conventionalcommits.org/)
4. Push para o repositório

## 🔗 Links Úteis

- [Documentação do Hermes Agent](https://hermes-agent.nousresearch.com/docs)
- [GitHub MCP Server](https://github.com/modelcontextprotocol/servers)

## 📄 Licença

Este projeto é privado e pertence a Bruno Herbert.
