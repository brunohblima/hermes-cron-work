# Changelog

Todas as alterações notáveis neste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-br/1.0.0/),
e este projeto segue [Semantic Versioning](https://semver.org/lang/pt-BR/).

## [Unreleased]

### Adicionado
- Estrutura inicial do projeto com diretórios organizados
- Configurações completas dos 4 cron jobs ativos
- Documentação básica (README, estrutura de pastas)

## [1.0.0] - 2026-05-04

### Adicionado
- Release inicial com versionamento dos cron jobs do Hermes Agent
- Jobs incluídos:
  - Resumo de Emails (cada 4 horas)
  - Compromissos do Dia (7h da manhã)
  - Resumo de Emails GROQ (cada 4 horas)
  - Clima Fazenda Trapia (7h da manhã)
- Configurações completas com prompts originais
- Estrutura de diretórios organizada por categoria de job

### Configurações
- Repositório configurado como privado
- Formato JSON para fácil leitura e versionamento
- Prompts completos preservados para auditoria

---

## Tipos de mudanças
- `Adicionado` para novas funcionalidades
- `Alterado` para mudanças em funcionalidades existentes
- `Descontinuado` para funcionalidades que serão removidas em breve
- `Removido` para funcionalidades removidas
- `Corrigido` para correções de bugs
- `Segurança` para vulnerabilidades
