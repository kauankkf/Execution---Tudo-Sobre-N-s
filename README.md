# Execution — site oficial

Site estático publicado pelo GitHub Pages. Não usa Supabase, banco de dados, bibliotecas externas nem serviços de terceiros.

## Adicionar músicas

1. Coloque os arquivos `.mp3` diretamente na pasta `musicas/`.
2. O nome de cada arquivo (sem `.mp3`) será o título exibido no site.
3. Envie as alterações para a branch `main` ou `master`.
4. O GitHub Actions gera o catálogo e publica o site automaticamente.

Exemplo:

```text
musicas/
  Nome da primeira música.mp3
  Nome da segunda música.mp3
```

Para mudar o título ou a ordem, renomeie os arquivos. A ordem é alfabética, considerando números no nome. O site não inventa faixas: se a pasta não tiver MP3s, a lista ficará vazia até o próximo envio.

Ative **Settings → Pages → Build and deployment → GitHub Actions** no repositório. O workflow `.github/workflows/pages.yml` publica o site quando houver um push.

O GitHub limita arquivos individuais a 100 MB. Para evitar repositórios grandes, prefira MP3s comprimidos e mantenha cada arquivo abaixo desse limite.
