# Dashboard AT1 INN - Ranking de Bairros e Ruas Expansíveis

Dashboard estático em HTML, preparado para publicação no GitHub Pages.

## Publicar no GitHub Pages

1. Crie um repositório novo no GitHub.
2. Extraia este pacote e envie os arquivos `index.html`, `README.md` e `.nojekyll` para a raiz do repositório.
3. No repositório, acesse **Settings > Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch **main** e a pasta **/(root)**, depois clique em **Save**.
6. Aguarde a publicação. O GitHub mostrará o endereço público do dashboard.

## Observações

- O dashboard usa Leaflet e Leaflet Heat carregados pelo CDN `unpkg.com`, portanto precisa de internet para exibir o mapa.
- O arquivo principal já foi renomeado para `index.html`, que é o nome esperado pelo GitHub Pages.
- Antes de publicar como repositório público, revise se os dados presentes no dashboard podem ser divulgados externamente.
