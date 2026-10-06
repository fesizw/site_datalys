# Datalys

Site institucional da Datalys, publicado em https://datalys.com.br/.

O código completo está em `index.html`: HTML5, Tailwind CSS via CDN, CSS de apoio e JavaScript. Não exige instalação nem compilação. O CDN é carregado com defer e configuração após load; o CSS local mantém o layout e usa site-container para evitar colisões com a biblioteca. Para visualizar localmente, abra o arquivo em um navegador.

Inclui navegação responsiva, painel demonstrativo com seleção de período e tabela acessível, animações que respeitam movimento reduzido, formulário validado e aviso de privacidade. Sem JavaScript, a navegação móvel permanece no fluxo da página e o aviso de privacidade pode ser acessado por links nativos. O gráfico inicial corresponde aos dados da tabela, e seus controles ficam desabilitados até a instalação dos eventos. O foco revela imediatamente os elementos animados e fecha o menu móvel ao sair do cabeçalho.

O contato está configurado para `faleconosco@datalys.com.br`. O formulário prepara uma mensagem no aplicativo de e-mail do visitante; ele precisa concluir o envio nesse aplicativo. O formulário explica esse fluxo antes do clique. Também permite copiar ou baixar o texto, atualizado quando os campos são editados. Se o aplicativo não abrir, a mensagem permanece disponível. Para integrar um serviço de envio, ajuste `CONTACT_CONFIG.endpoint` no HTML com uma URL HTTPS que aceite os campos via POST de FormData.

Revisão de 06/10/2026: HTML sem erros no Nu HTML Checker; testes de comportamento em DOM simulado para menu, Escape, foco no redimensionamento, cliques modificados, saída do menu por foco, foco durante animações, consistência entre gráfico inicial e interativo, controles sem JS, formulário, atualização da mensagem e diálogo. Branco sobre cobre tem contraste aproximado de 6:1. A renderização em navegador e a experiência com leitores de tela reais não foram verificadas neste ambiente; a revisão não certifica conformidade completa com WCAG.

Credenciais e arquivos auxiliares de publicação ficam fora do Git (`.env.local` e `.deployment/`).

A configuração da hospedagem define redirecionamentos 301 de HTTP, www e index.html para https://datalys.com.br/, preservando parâmetros, e Cache-Control: no-cache. A configuração original e as versões anteriores estão preservadas em `.deployment/`.

Publicação confirmada em 06/10/2026: a URL literal https://datalys.com.br/ entrega o HTML atual, idêntico ao arquivo local, com metadados de compartilhamento e SEO e Cache-Control: no-cache. Googlebot e o crawler de compartilhamento também recebem essa versão. HTTP, www e index.html redirecionam com 301 para a URL canônica. A cópia antiga do cache NGINX não apareceu na verificação final.

Compartilhamento: metadados Open Graph e Twitter Card apontam para `assets/datalys-logo-social-v1.jpg`, cópia exata da logo original, com dimensões declaradas de 1408 × 768. O ícone público `assets/datalys-icon-256.png` substitui o antigo favicon inline para permitir rastreamento pelos buscadores.

SEO: título e descrição revisados, endereço canônico HTTPS, metadado robots, dados estruturados JSON-LD de Organization, WebSite, WebPage e serviços. `robots.txt` libera o rastreamento e indica `sitemap.xml`, que contém a única página canônica. O conteúdo e os metadados são entregues no HTML, sem depender de JavaScript para os robôs.

O IndexNow usa um arquivo público de verificação na hospedagem. A notificação da URL canônica foi enviada ao Bing em 06/10/2026 e retornou HTTP 202. A configuração e os registros de envio ficam em `.deployment/`, fora do Git. Aceitação de uma notificação não confirma indexação. Prévia no WhatsApp e exibição em buscadores dependem do processamento das plataformas.
