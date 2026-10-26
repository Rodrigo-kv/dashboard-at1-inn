# Dashboard AT1 INN Retalhos

Estrutura preparada para publicação no GitHub Pages.

## Estrutura

- `index.html`: dashboard com páginas Análise e Analista.
- `manifest.json`: aponta para a base publicada atualmente.
- `dados/AT1-26-10.json.gz`: dados AT1 em JSON compactado.

## Atualizar a base

1. Na página Analista, carregue o CSV e converta para JSON.
2. Compacte o JSON com gzip, preservando a extensão `.json.gz`.
3. Envie o arquivo para a pasta `dados`.
4. Atualize `arquivo`, `periodo`, `registros`, `atualizadoEm` e `sha256` no `manifest.json`.
5. Faça commit na branch `main`. O GitHub Pages publicará a alteração.

O navegador lê primeiro o `manifest.json`, depois busca o arquivo indicado em `arquivo`.
