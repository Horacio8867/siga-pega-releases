# SIGA-PEGA - Releases Android

Repositorio oficial de distribuicao do APK nativo do SIGA-PEGA.

## Download

Acesse [Releases](https://github.com/Horacio8867/siga-pega-releases/releases) e baixe **siga-pega.apk**.

**Link direto v1.0.0:**
https://github.com/Horacio8867/siga-pega-releases/releases/download/v1.0.0/siga-pega.apk

## Instalacao

1. Baixe siga-pega.apk
2. Abra no Android
3. Permita instalacao de fontes desconhecidas se solicitado
4. Toque em Instalar
5. Remova o atalho PWA da tela inicial apos instalar

## Para desenvolvedores

Gerar e publicar novo APK:

    .\\scripts\\upload-apk.ps1 -Version '1.1.0' -ReleaseNotes 'Descricao'

Ativar no Supabase:

    UPDATE app_config
    SET value = 'https://github.com/Horacio8867/siga-pega-releases/releases/download/v1.0.0/siga-pega.apk'
    WHERE key = 'apk_download_url';