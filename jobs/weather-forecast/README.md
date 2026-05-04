# Clima Fazenda Trapia - Diario 7h

## Descrição

Cron job que verifica diariamente o clima da Fazenda Trapia, localizada em Serra do Vento, Belo Jardim, Pernambuco.

## Configuração

- **ID**: `410e8c8c7a3d`
- **Agendamento**: Diariamente às 07:00 (fuso de Brasília) - `0 10 * * *` (UTC)
- **Entrega**: WhatsApp (Bruno Herbert)
- **Status**: Ativo

## Funcionamento

1. Consulta a API wttr.in usando coordenadas exatas da Fazenda Trapia:
   - Latitude: -8.2248961
   - Longitude: -36.2860249

2. Extrai informações:
   - Temperatura atual e sensação térmica
   - Condição do tempo
   - Umidade e velocidade do vento
   - Previsão para os próximos 5 dias

3. Formata e envia relatório via WhatsApp com emojis e formatação clara

## Coordenadas

📍 **Fazenda Trapia - Serra do Vento, Belo Jardim, PE**
- Latitude: -8.2248961
- Longitude: -36.2860249

## Exemplo de Saída

```
🌤️ CLIMA FAZENDA TRAPIA (Serra do Vento, Belo Jardim - PE)

📍 Localização: Fazenda Trapia - Serra do Vento, Belo Jardim, PE
📍 Coordenadas: -8.2248961, -36.2860249
🕐 Atualizado em: 04/05/2026 07:00

🌡️ AGORA:
- Temperatura: 26°C (sensação 28°C)
- Condição: Parcialmente nublado
- Umidade: 65%
- Vento: 12 km/h

📅 PRÓXIMOS 5 DIAS:
Segunda-feira (04/05): Parcialmente nublado - 22°C a 30°C
Terça-feira (05/05): Ensolarado - 21°C a 32°C
Quarta-feira (06/05): Chuva leve - 20°C a 27°C
Quinta-feira (07/05): Ensolarado - 21°C a 31°C
Sexta-feira (08/05): Parcialmente nublado - 22°C a 29°C

⚠️ ALERTAS (se houver):
- [Nenhum alerta no momento]
```

## Dependências

- Terminal (curl para wttr.in)
- WhatsApp (entrega)

## Histórico

- **Criado em**: 03/05/2026
- **Última execução**: 03/05/2026 16:24 (sucesso)
- **Execuções concluídas**: 3
