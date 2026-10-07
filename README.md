# Datalys

Site institucional em português: **“Otimizamos os seus dados para cuidar do seu negócio.”**

HTML5, Tailwind via CDN, CSS e JavaScript em um único index.html, sem etapa de build. Abra o arquivo no navegador para visualizar. O CSS próprio mantém o layout sem o CDN; o menu, os gráficos e o formulário recebem melhorias com JavaScript.

## Estrutura

| Caminho | Conteúdo |
| --- | --- |
| index.html | Página institucional completa |
| robots.txt e sitemap.xml | Rastreamento e URL canônica |
| assets/brand/ | Símbolo e logo atuais em SVG/PNG |
| assets/icons/ | Favicon em SVG/PNG |
| assets/social/ | Imagem de compartilhamento e fonte SVG |
| docs/brand/ | Direção de identidade e referências originais |
| docs/estrutura.md | Convenções dos arquivos |
| docs/publicacao.md | Procedimento de publicação |
| tmp/ e .deployment/ | Contexto, backups e ferramentas locais, ignorados pelo Git |

## Comunicação e produtos

“Dados em ordem. Decisões com confiança.” reforça a associação entre marca, organização e tomada de decisão. A origem do nome fica na documentação da marca; o site comunica benefícios concretos.

O menu **Produtos** oferece links para **Integradata**, **BI** e **IA**. Cada produto tem descrição, benefícios e um CTA que preenche o interesse no contato. A seção Soluções apresenta as necessidades atendidas; O Método explica as quatro etapas de trabalho.

O símbolo usa seis braços fluidos e um núcleo de seis pontas sugerido pelo espaço negativo. Cabeçalho, rodapé, favicon e compartilhamento usam a mesma geometria. Leia [a direção da marca](docs/brand/identidade.md).

## Contato

Canal oficial: faleconosco@datalys.com.br. O formulário prepara uma mensagem no aplicativo de e-mail; o visitante revisa e conclui o envio por lá. Há alternativas para copiar e baixar o texto. Nenhum envio automático é simulado.

Para integrar atendimento por servidor, configure CONTACT_CONFIG.endpoint com uma URL HTTPS que aceite POST de FormData: name, email, company, message e subject.

## Validação e publicação

As verificações cobrem HTML, referências internas, metadados, navegação por teclado, menu móvel, gráfico/tabela, formulário e privacidade em DOM simulado. A revisão não certifica WCAG completa; layout em navegador, dispositivos e leitores de tela reais exige avaliação própria.

O domínio é https://datalys.com.br/. A versão de 06/10/2026 foi publicada e conferida. A revisão de comunicação e identidade de 07/10/2026 está preparada nesta feature; a publicação depende de acesso válido à hospedagem, pois a conta FTP anterior foi fornecida para uso temporário no dia 06/10.

Os metadados estáticos de compartilhamento apontam para assets/social/datalys-compartilhamento-v2.png (1200 × 630). robots.txt, sitemap, canonical HTTPS e JSON-LD auxiliam o rastreamento. A notificação IndexNow anterior retornou HTTP 202; isso não confirma indexação.

Siga [o procedimento de publicação](docs/publicacao.md) e [as convenções do repositório](docs/estrutura.md). Credenciais, chaves, backups e contexto temporário ficam fora do Git.
