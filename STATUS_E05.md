# E05 — Site e captura

Estado: **CONCLUÍDA E APROVADA** em 12/08/2026.

## Estrutura criada

- página inicial;
- página do livro;
- página sobre o autor;
- página de errata;
- página de privacidade;
- folha de estilos responsiva;
- página 404;
- formulário Brevo integrado à página inicial;
- chamada para cadastro adicionada à página do livro;
- política de privacidade vinculada ao formulário e ao rodapé do site.

## Captura

- formulário: `Livro Bayes — Lista de interessados`;
- lista: `Livro Bayes — Interessados`;
- consentimento LGPD habilitado;
- confirmação por double opt-in configurada;
- integração via iframe Brevo;
- domínio `ricardoscotta.com.br` autenticado na Brevo;
- subdomínio de marca `mail.ricardoscotta.com.br` ativo;
- remetente `Ricardo Scotta <livros@ricardoscotta.com.br>` verificado, com DKIM e DMARC válidos;
- fluxo de double opt-in validado de ponta a ponta em 12/08/2026;
- contato de teste confirmado na lista `Livro Bayes — Interessados`;
- e-mail final de confirmação recebido na caixa de entrada do Gmail.

## Privacidade

- controlador informado: Ricardo Scotta;
- contato de privacidade: `livros@ricardoscotta.com.br`;
- coleta declarada: endereço de e-mail e registro de consentimento/double opt-in;
- finalidades limitadas a comunicações sobre o livro, publicação, materiais, atualizações, erratas e conteúdos autorais relacionados;
- Brevo identificada como plataforma operacional do formulário, lista e envio;
- GitHub Pages identificado como hospedagem do site;
- direitos do titular, revogação do consentimento, retenção e eliminação descritos;
- ausência atual de analytics próprios, pixels publicitários e perfilamento registrada.

## Domínio e GitHub Pages

- domínio autoral `ricardoscotta.com.br` verificado na conta GitHub;
- domínio customizado configurado no GitHub Pages;
- arquivo `CNAME` criado na raiz com `ricardoscotta.com.br`;
- DNS do domínio raiz apontado para os quatro endereços IPv4 oficiais do GitHub Pages;
- `www` configurado por CNAME para `riscotta.github.io`;
- DNS check do GitHub: aprovado;
- certificado TLS aprovado para `ricardoscotta.com.br` e `www.ricardoscotta.com.br`;
- HTTPS forçado;
- site acessível em `https://ricardoscotta.com.br/`.

## Validação visual e funcional

Validação executada em 12/08/2026:

- Home em desktop: aprovada;
- Home em mobile, largura simulada de 414 px: aprovada;
- formulário Brevo em mobile: aprovado, sem overflow horizontal;
- navegação mobile: `Livro`, `Sobre`, `Errata` e `Privacidade` aprovadas;
- links e layout sem falhas reportadas nos testes finais.

## Evidência e risco de entregabilidade

O primeiro e-mail de double opt-in do teste foi classificado como spam pelo Gmail, apesar do domínio e do remetente estarem autenticados. O e-mail final, enviado após a confirmação, chegou à caixa de entrada. Registrar como risco de reputação inicial de domínio/remetente novo, não como falha funcional do fluxo.

## Gates

- **Gate de captura: APROVADO** — formulário, consentimento, double opt-in, confirmação e inclusão na lista validados de ponta a ponta.
- **Gate de domínio/HTTPS: APROVADO** — domínio verificado, DNS resolvido, TLS aprovado e HTTPS forçado.
- **Gate responsivo/navegação: APROVADO** — desktop, mobile, formulário e páginas principais validados.
- **Gate de publicação: APROVADO** — PR #1 integrado à `main`, GitHub Pages configurado em `main / (root)` e deploy final confirmado com status `built`.

## Governança

O desenvolvimento e os testes finais ocorreram na branch `e05-site-captura`, preservando a `main` até a aprovação dos gates. A publicação aprovada foi integrada à `main` pelo PR #1. O GitHub Pages publica atualmente a partir de `main / (root)`.

## Próxima etapa

**E06 — GitHub Pages**: publicar e organizar a versão aberta técnica e os materiais complementares sob o endereço profissional.

Etapa final do plano: **E11 — Manutenção**.
