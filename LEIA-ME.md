# Dev's Creators — arquivos para publicação

## Publicar o site
1. Extraia o arquivo ZIP.
2. Envie o arquivo `index.html` para a pasta principal do seu domínio (normalmente `public_html`, `www` ou `htdocs`).
3. Confirme que o arquivo se chama exatamente `index.html` (tudo minúsculo).
4. Abra seu domínio em uma janela anônima ou atualize a página.

O `index.html` já contém o HTML, CSS e JavaScript do site. Não é necessário criar pastas adicionais para a página inicial.

## Recursos que ainda precisam de configuração
O site pode ser publicado como página estática, mas alguns recursos dependem de configuração externa:
- Login Discord e Google: os IDs de cliente estão vazios no objeto `CONFIG` do JavaScript.
- Banco de dados online: `FIREBASE` está como `null`. Sem Firebase, o site usa armazenamento local/de demonstração; dados não ficam compartilhados entre visitantes.
- WhatsApp: confira os links/botões de contato no código e substitua o número de exemplo pelo número comercial correto, se ainda não estiver configurado.

Não coloque senhas, chaves privadas ou segredos de servidor dentro do HTML público. Para autenticação e dados reais, configure os serviços no painel próprio e use regras de segurança adequadas.

## Teste antes de publicar
Abra `index.html` no navegador para uma prévia. Para testar exatamente como hospedado, publique em um serviço de hospedagem estática ou use um servidor local.
