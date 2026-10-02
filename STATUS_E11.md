# E11 — Manutenção e continuidade editorial

Estado: **EM ANDAMENTO** em 02/10/2026.

## Objetivo

Manter *Estatística Bayesiana com R e Stan* saudável como obra publicada e transformar o sistema editorial em uma estrutura reutilizável para o catálogo autoral e para o próximo livro.

## E11.1 — Site como portfólio autoral

Branch de trabalho: `e11-site-portfolio-autoral`.

PR: #4 — **E11 — Evoluir site para portfólio autoral**.

### Alterações preparadas

- Home reposicionada de página centrada em um único livro para apresentação autoral;
- criação de `/livros/` como catálogo;
- preservação de `/livro/` para não quebrar links já divulgados;
- inclusão de *Estatística Bayesiana com R e Stan* como obra publicada;
- inclusão de “Próximo livro” como projeto em desenvolvimento;
- integração editorial com artigos, posts e newsletter *Estatística sob Incerteza*;
- página Sobre atualizada para refletir produção autoral contínua;
- errata organizada por obra;
- política de privacidade preparada para comunicações editoriais mais amplas;
- sitemap atualizado;
- componentes de portfólio adicionados ao CSS.

## Dependência antes do merge

O formulário incorporado é gerenciado no Brevo. Antes de integrar o PR, revisar no Brevo:

1. nome interno do formulário;
2. título e texto exibidos;
3. declaração/checkbox de consentimento;
4. finalidade do cadastro;
5. e-mail de confirmação double opt-in;
6. lista de destino, se for renomeada.

A finalidade deve corresponder ao novo sistema editorial: livros, novos projetos, materiais complementares, atualizações, erratas e outros conteúdos autorais relacionados.

O double opt-in deve permanecer ativo.

## Estado do livro publicado no início da E11

- eBook publicado em 10/09/2026;
- 8 unidades processadas em setembro;
- royalties estimados de setembro: US$ 16,08;
- nenhuma avaliação na Amazon registrada no fechamento da E10;
- nenhuma errata registrada;
- campanha inicial de lançamento encerrada em 02/10/2026.

## Próximo gate

**Gate E11.1 — Portfólio autoral publicado**:
- formulário Brevo coerente com a nova finalidade;
- PR revisado visualmente;
- links principais testados;
- PR integrado à `main`;
- deploy do GitHub Pages validado em desktop e mobile.
