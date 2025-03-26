# Bot de Chamados via Slack

Este bot responde ao comando `/chamado` no Slack e abre um formulário interativo para envio de dados de chamado.

## O que ele faz

- Abre formulário modal no Slack
- Coleta dados de chamado
- Envia uma mensagem formatada para o canal #ticket

## Como usar

1. Crie um Slack App em https://api.slack.com/apps
2. Ative os escopos:
   - commands
   - chat:write
   - app_mentions:read
   - im:write
   - channels:read
   - users:read
3. Ative o Socket Mode e gere `SLACK_APP_TOKEN`
4. Configure um comando `/chamado` com a URL apontando pro seu bot (ex: Railway)
5. Rode com Python:
   ```bash
   pip install -r requirements.txt
   python app.py
   ```

Use `.env.example` como base para suas variáveis.
