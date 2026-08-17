# E06 — GitHub Pages

Estado: **EM VALIDAÇÃO** em 17/08/2026.

## Objetivo

Publicar a versão aberta técnica e os materiais complementares sob o domínio profissional, preservando separação entre a edição comercial e a camada pública evolutiva.

## Decisão operacional

A versão técnica foi integrada ao mesmo repositório do domínio autoral, `riscotta/riscotta.github.io`, sob `/bayes-r-stan/`.

Motivos:
- o domínio autoral e o GitHub Pages já estão operacionais e validados;
- a E01 prevê um único domínio profissional;
- a E02 definiu uma estrutura pública segura, sem capítulos integrais;
- a E06 preserva a separação entre o site autoral da E05 e a camada técnica versionada.

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

## Reconciliação de 17/08/2026

A implementação realizada no PR #2 foi confrontada com o estado canônico herdado da E05 e com o fechamento aprovado da E02.

Resultado:
- PR #2 permanece mesclado na `main` pelo commit `bbadf92591e75886cc7c902528432bbf4eb9fcc8`;
- a implementação não reabriu o manuscrito canônico nem o EPUB RC07;
- nenhum capítulo integral foi publicado;
- a arquitetura em `/bayes-r-stan/` preserva a Home autoral e separa a camada técnica;
- o sitemap inclui as três rotas canônicas da camada técnica;
- não foi identificada divergência que justifique rollback do PR #2.

O workflow `pages build and deployment` #11 (`32046705239`) permaneceu preso em `queued` após uma primeira falha de deploy por HTTP 503. O GitHub continuou tratando essa execução como ativa e impediu seu cancelamento/rerun normal.

Uma nova alteração na `main` gerou o workflow `pages build and deployment` #12. Em 17/08/2026, a interface do GitHub Actions registrou o #12 como concluído com sucesso (check verde, duração de 48 s). Como o #12 é posterior ao #11 e concluiu normalmente sobre a `main`, o #11 passa a ser tratado como execução órfã/superseded e não como bloqueador da E06.

## Gate

Concluído:
- merge da branch `e06-github-pages` em `main`;
- reconciliação do escopo da E06 com as fontes vigentes;
- deploy GitHub Pages concluído com sucesso em execução posterior (#12), tornando o #11 órfão/superseded;
- presença, na `main`, das três páginas HTML canônicas da camada técnica.

Pendente:
- verificação HTTP das três rotas no domínio profissional:
  - `/bayes-r-stan/`;
  - `/bayes-r-stan/conteudo/`;
  - `/bayes-r-stan/reproducibilidade/`.

A E06 deve ser marcada como concluída após a confirmação de que essas três rotas abrem corretamente no domínio profissional.

## Próxima etapa

Após aprovação do gate: **E07 — Metadados e página comercial**.

Etapa final do plano: **E11 — Manutenção**.
