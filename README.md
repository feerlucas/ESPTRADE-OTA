# ESPTRADE-OTA

Repositório público do firmware OTA do KrakenTrendBotV2 para LILYGO T-Display-S3.

Estrutura usada pela ESP32:

- `ota/firmware/`: binários `.bin` publicados no branch `main`
- `ota/manifest/`: manifests JSON consultados pela placa por HTTPS

O firmware baixa o manifest em `raw.githubusercontent.com` e, quando existe versão nova, baixa o `.bin` também por URL crua do próprio repositório.
