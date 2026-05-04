# Setup e Configuração

Este documento descreve como configurar e manter os cron jobs do Hermes Agent versionados neste repositório.

## 🔧 Pré-requisitos

- Hermes Agent instalado e configurado
- Acesso ao GitHub com autenticação configurada
- Skills necessárias: `google-workspace`

## 📁 Estrutura de Arquivos

Cada cron job possui seu próprio diretório sob `jobs/` com a seguinte estrutura:

```
jobs/
├── email-summary/
│   ├── config.json          # Configuração completa do job
│   └── README.md           # Documentação específica do job
├── email-groq/
│   ├── config.json
│   └── README.md
├── calendar-events/
│   ├── config.json
│   └── README.md
└── weather-forecast/
    ├── config.json
    └── README.md
```

## 🚀 Como Atualizar um Cron Job

1. **Edite o arquivo de configuração:**
   ```bash
   vim jobs/email-summary/config.json
   ```

2. **Atualize o CHANGELOG.md** com as alterações feitas

3. **Faça commit das alterações:**
   ```bash
   git add .
   git commit -m "feat(email-summary): atualiza filtros de descarte"
   git push origin main
   ```

4. **Atualize o cron job no Hermes Agent** (se necessário):
   - Use o comando `cronjob action='update'` via Hermes
   - Ou recrie o job com as novas configurações

## 🔄 Sincronização

Para manter o repositório sincronizado com os cron jobs ativos no Hermes:

1. Exporte as configurações atuais:
   ```bash
   # No Hermes Agent
   cronjob action='list'
   ```

2. Atualize os arquivos locais:
   ```bash
   # Edite os arquivos em jobs/*/config.json
   ```

3. Commit e push:
   ```bash
   git add .
   git commit -m "sync: atualiza configurações dos cron jobs"
   git push
   ```

## 📋 Convenções de Commit

Seguimos o padrão [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` - Nova funcionalidade ou job
- `fix:` - Correção de configuração
- `docs:` - Alterações na documentação
- `sync:` - Sincronização com Hermes Agent
- `refactor:` - Reestruturação de arquivos

## ⚠️ Avisos Importantes

- **Nunca** commite credenciais ou tokens de acesso
- Mantenha os prompts atualizados conforme alterações no Hermes
- Sempre atualize o CHANGELOG.md ao fazer alterações
- Teste as alterações no Hermes antes de fazer push
