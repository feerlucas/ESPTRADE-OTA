# OTA Setup

Para a ESP32 baixar firmware remotamente por HTTPS, este repositório precisa estar **public**.

Checklist:

1. Tornar o repo `feerlucas/ESPTRADE-OTA` público.
2. Publicar o binário `KrakenTrendBotV2-2.2.0.bin` em `ota/firmware/`.
3. Manter os manifests em `ota/manifest/` apontando para a URL crua correta do arquivo.
4. Na placa, usar `/checkupdate`, `/version` e `/update` no Telegram.

Observação:

- Se o repo continuar privado, a ESP32 não consegue baixar manifest nem firmware sem autenticação.
- A placa já recebeu via USB a versão `2.2.0` OTA-ready, que migra as credenciais para `Preferences` e prepara futuras atualizações remotas.
