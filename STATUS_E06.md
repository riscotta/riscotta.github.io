# E06 — GitHub Pages

Estado: **EM VALIDAÇÃO** em 17/08/2026.

## Objetivo

Publicar a versão aberta técnica e os materiais complementares sob o domínio profissional, preservando separação entre a edição comercial e a camada pública evolutiva.

## Decisão operacional

A versão técnica foi integrada ao mesmo repositório do domínio autoral, `riscotta/riscotta.github.io`, sob `/bayes-r-stan/`.

Motivos:
- o domínio autoral e o GitHub Pages já estão operacionais e validados;
- a E01 prevê um único domínio profissional;
- a E02 já definiu e validou a estrutura pública segura, sem capítulos integrais.

A fonte privada de produção, o manuscrito canônico e o EPUB RC07 não foram reabertos nem publicados.

## Conteúdo publicado na E06

- landing page da versão técnica;
- página de conteúdo liberado;
- página de reprodutibilidade e direitos;
- fonte Quarto pública mínima preservada em `_source/`;
- integração da página do livro com a versão técnica;
- atualização do sitemap.

## Regra de liberação

Nenhum capítulo integral foi publicado porque não há autorização autoral explícita registrada para uma liberação específica. Novas liberações devem ser versionadas e passar pelas verificações de direitos e proveniência aplicáveis.

## Gate

Pendente até:
- merge da branch `e06-github-pages` em `main`;
- deploy GitHub Pages com status `built`;
- verificação HTTP das novas rotas no domínio profissional.

## Próxima etapa

**E07 — Metadados e página comercial**.

Etapa final do plano: **E11 — Manutenção**.
