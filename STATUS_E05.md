# E05 — Site e captura

Estado: em trabalho.

## Estrutura criada

- página inicial;
- página do livro;
- página sobre o autor;
- página de errata;
- folha de estilos responsiva;
- página 404;
- formulário Brevo integrado à página inicial;
- chamada para cadastro adicionada à página do livro.

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

## Evidência e risco de entregabilidade

O primeiro e-mail de double opt-in do teste foi classificado como spam pelo Gmail, apesar do domínio e do remetente estarem autenticados. O e-mail final, enviado após a confirmação, chegou à caixa de entrada. Registrar como risco de reputação inicial de domínio/remetente novo, não como falha funcional do fluxo.

## Gate de captura

**APROVADO** — formulário, consentimento, double opt-in, confirmação e inclusão na lista foram validados de ponta a ponta.

## Governança

O desenvolvimento ocorre na branch `e05-site-captura`. O conteúdo do site ainda não foi liberado para publicação pela branch `main`.

## Pendências para concluir a E05

- criar a página de privacidade coerente com o tratamento efetivo dos dados;
- configurar e testar o domínio autoral no GitHub Pages;
- validar a navegação em desktop e mobile;
- publicar a versão aprovada do site somente após essas validações.
