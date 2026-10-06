# Datalys

Site institucional publicado e verificado em https://datalys.com.br/.

O código completo está em `index.html`: HTML5, Tailwind CSS via CDN, CSS de apoio e JavaScript. Não exige instalação nem compilação. Para visualizar localmente, abra o arquivo em um navegador.

Inclui navegação responsiva, painel demonstrativo com seleção de período e tabela acessível, animações que respeitam movimento reduzido, formulário validado e aviso de privacidade.

O contato está configurado para `faleconosco@datalys.com.br`. O formulário prepara uma mensagem no aplicativo de e-mail do visitante; ele precisa concluir o envio nesse aplicativo. Também permite copiar ou baixar o texto. Para integrar um serviço de envio, ajuste `CONTACT_CONFIG.endpoint` no HTML com uma URL HTTPS que aceite os campos via POST de FormData.

Validação: HTML sem erros no Nu HTML Checker; testes de comportamento em DOM simulado para menu, foco, gráfico, formulário e diálogo. A renderização em navegador e a experiência com leitores de tela reais não foram verificadas neste ambiente.

Credenciais e arquivos auxiliares de publicação ficam fora do Git (`.env.local` e `.deployment/`).

A configuração da hospedagem consolida HTTP, www e index.html na URL https://datalys.com.br/ com redirecionamentos 301 e preserva parâmetros de consulta. As respostas usam Cache-Control: no-cache para revalidação. A configuração original e as versões anteriores estão preservadas em `.deployment/`.

Compartilhamento: metadados Open Graph e Twitter Card apontam para `assets/datalys-logo-social-v1.jpg`, cópia exata da logo original, com dimensões declaradas de 1408 × 768. O ícone público `assets/datalys-icon-256.png` substitui o antigo favicon inline para permitir rastreamento pelos buscadores.

SEO: título e descrição revisados, endereço canônico HTTPS, metadado robots, dados estruturados JSON-LD de Organization, WebSite, WebPage e serviços. `robots.txt` libera o rastreamento e indica `sitemap.xml`, que contém a única página canônica. O conteúdo e os metadados são entregues no HTML, sem depender de JavaScript para os robôs.

O IndexNow usa um arquivo público de verificação na hospedagem; sua configuração e os registros de envio ficam em `.deployment/`, fora do Git. Aceitação de uma notificação não confirma indexação. Prévia no WhatsApp e exibição em buscadores dependem do processamento das plataformas.
