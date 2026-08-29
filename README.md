# Ficha de personagem · Cyberpunk 2020

Ficha preenchivel em uma pagina, feita para uso no celular durante a mesa.
Tudo fica no `localStorage` do proprio aparelho, nada vai para servidor.

## GitHub Pages

Um workflow (`.github/workflows/deploy-pages.yml`) publica o site a cada push
na branch `main`. **Passo unico obrigatorio** antes do primeiro deploy: em
Settings > Pages > Build and deployment > Source, selecione `GitHub Actions`.
(O `GITHUB_TOKEN` do workflow nao tem permissao para ativar o Pages sozinho
na primeira vez, entao esse clique manual e necessario uma unica vez; depois
disso todo push na `main` publica automaticamente.)

Depois de ativado, a ficha fica em:

`https://costa-artur.github.io/cyberpunk_2020_sheet/`

## Instalar no celular

- Android (Chrome): menu > Adicionar a tela inicial.
- iPhone (Safari): botao de compartilhar > Adicionar a Tela de Inicio.

Depois de instalada, a ficha abre em tela cheia e funciona offline.

## Arquivos

| arquivo | para que serve |
| --- | --- |
| `index.html` | a ficha inteira, sem dependencias |
| `manifest.webmanifest` | nome, cor e icones do app instalado |
| `sw.js` | cache offline |
| `icon-*.png` | icones |

## Backup

O botao Exportar gera um `.json` por personagem. O Importar traz de volta em
qualquer aparelho. Limpar os dados do site apaga as fichas salvas.
