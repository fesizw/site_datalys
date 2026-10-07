# Publicação e conferência

O site usa a hospedagem externa do domínio https://datalys.com.br/. Não exige build ou aplicação de servidor.

1. Confirmar que as credenciais da hospedagem estão válidas e autorizadas para o período de uso. A conta fornecida em 06/10/2026 era temporária para aquele dia; não reutilizar sem renovação.
2. Preservar backup do HTML e da configuração existente em `.deployment/`, fora do Git.
3. Enviar `assets/` com os novos nomes antes de trocar o HTML. Conferir os arquivos por leitura remota e hash.
4. Enviar o novo HTML com nome temporário, comparar os bytes recebidos por HTTPS e ativá-lo como `index.html`.
5. Enviar `robots.txt` e `sitemap.xml`. Preservar a configuração original do servidor.
6. Conferir a URL literal da raiz, sem parâmetro: HTML atual, canonical, Open Graph, imagem social, favicon e dados estruturados.
7. Conferir redirecionamentos de HTTP, www e index.html para a URL canônica HTTPS.
8. Se a raiz continuar antiga, limpar o cache NGINX no cPanel e verificar novamente. Receber o HTML correto com uma query diferente não confirma a versão canônica.

Enviar somente os arquivos públicos descritos em `estrutura.md`. Não subir `.git`, `docs`, `tmp`, `.deployment`, arquivos `.env` ou notas locais.

Manter os assets públicos antigos na hospedagem enquanto puderem existir referências em cache; sua retirada do repositório não exige apagá-los imediatamente do servidor.

Chaves operacionais e credenciais nunca entram em comandos visíveis, código versionado ou contexto do projeto. No procedimento FTPS usado anteriormente, as credenciais foram passadas pela entrada padrão, com validação do certificado.

Notificar IndexNow somente após confirmar a raiz atualizada. Recebimento de uma notificação não garante indexação. As prévias de compartilhamento também dependem do processamento das plataformas.
