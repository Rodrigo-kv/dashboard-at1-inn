# Dashboard AT1 atualizado por GitHub Releases

Este pacote evita o download do asset da Release diretamente pelo navegador. O GitHub Actions baixa o arquivo `AT1-AA-MM.json`, valida o JSON e publica uma copia no mesmo dominio do GitHub Pages. Isso evita falhas de CORS e redirecionamento.

## Arquivos do pacote

- `index.html`: paginas Analise e Analista.
- `.github/workflows/deploy-pages.yml`: automacao de download e publicacao.
- `.nojekyll`: configuracao do Pages.

## Instalacao

1. Envie os tres itens acima para a raiz da branch `main`.
2. No repositorio, abra `Settings > Pages`.
3. Em `Build and deployment > Source`, selecione `GitHub Actions`.
4. Abra `Actions` e execute `Publicar dashboard pela ultima Release` usando `Run workflow`.
5. Verifique se o workflow terminou com marca verde.
6. Abra o site e pressione `Ctrl+F5`.

## Atualizacao mensal

1. Crie uma nova Release publicada, nao Draft.
2. Anexe um unico arquivo no padrao `AT1-AA-MM.json`, por exemplo `AT1-26-11.json`.
3. Publique a Release.
4. O workflow sera executado automaticamente.
5. O workflow valida se o JSON e uma lista e mostra a quantidade de registros.

## Resultado esperado

O dashboard exibira uma mensagem como:

`Release AT1-26-10 carregada: AT1-26-10.json, 26.223 registros.`

Se o asset estiver ausente, vazio ou invalido, o workflow falhara e a versao anterior do Pages permanecera publicada.
