# PrintGest - Landing Page

Landing page do **PrintGest**, sistema de gestão e orçamento de rótulos para gráficas. É um **PWA** (Progressive Web App): pode ser instalada no celular ou no computador e abre offline depois da primeira visita.

O código do sistema em Java está em [Projeto-Final-PPA-PrintGest](https://github.com/lucasdbf/Projeto-Final-PPA-PrintGest).

## O que tem na página
- **Simulador de orçamento:** usa a mesma regra de cálculo do sistema em Java (aproveitamento da folha, faixa de preço e taxa fixa).
- **Problema e proposta de valor:** orçamento manual comparado ao PrintGest.
- **Funcionalidades, arquitetura em camadas e banco de dados** do sistema.
- **Passo a passo** para executar o projeto e perguntas frequentes.

## Tecnologias
HTML5, CSS3 e JavaScript puro, sem dependências. PWA com `manifest.webmanifest` e service worker (`sw.js`).

## Estrutura
```text
index.html             # Página
style.css              # Estilos
script.js              # Simulador e interações
manifest.webmanifest   # Manifesto do PWA
sw.js                  # Service worker (cache offline)
icons/                 # Ícones do PWA
demonstracao.gif       # Gravação do menu do sistema
```

## Como executar localmente
O service worker só funciona em `http://localhost` ou `https`. Na pasta do projeto:

```bash
python3 -m http.server 8000
```

Abra `http://localhost:8000`.

## Publicação (GitHub Pages)
Em **Settings → Pages → Build and deployment**, escolha **Deploy from a branch**, branch `main` e pasta `/ (root)`. Como os arquivos estão na raiz, nenhuma configuração extra é necessária.
