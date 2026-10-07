# Organização do repositório

A raiz contém a entrada do site e os arquivos exigidos pelo rastreamento. O HTML continua completo em um arquivo, conforme o briefing; imagens e documentação têm pastas próprias.

| Local | Conteúdo | Publicar na hospedagem? |
| --- | --- | --- |
| `index.html` | Conteúdo, CSS, JavaScript e ícones inline | Sim |
| `robots.txt`, `sitemap.xml` | Rastreamento | Sim |
| `assets/brand/` | Símbolo e assinatura atuais | Sim |
| `assets/icons/` | Favicon atual e fonte vetorial | Sim |
| `assets/social/` | Card de compartilhamento e fonte vetorial | Sim |
| `docs/` | Documentação e referências históricas | Não |
| `README.md`, `.gitignore` | Orientação do repositório | Não |
| `tmp/`, `.deployment/`, `.env*` | Contexto, evidências e credenciais locais | Nunca |

Use nomes em minúsculas, sem espaços, com hífens. Nomear por finalidade: `datalys-symbol.svg`, `datalys-logo.png`, `datalys-favicon-v2.png`, `datalys-compartilhamento-v2.png`. A versão em arquivos públicos de compartilhamento evita reutilizar a URL de uma imagem antiga já armazenada pelas plataformas.

SVG é a fonte editável; PNG é a aplicação raster para serviços que precisam desse formato. As exportações atuais foram renderizadas dos SVGs, preservando a geometria da marca. Não editar apenas o PNG.

A imagem original foi renomeada de `Gemini_Generated_Image_bats2kbats2kbats.jpg` para `docs/brand/references/logo-original.jpg`. A antiga imagem social era uma cópia idêntica e foi removida do repositório para evitar duplicação. O favicon anterior foi movido para a pasta de referências.

O `.gitignore` contém regras para este site estático. As antigas regras de CakePHP foram retiradas porque não correspondem à implementação.

Novas mudanças partem de `develop` em `feature/<objetivo>`. Integração de release e atualização de `main` são realizadas quando solicitadas. Não reescrever commits publicados nem usar force-push.
