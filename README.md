# Gravador de ligações

Grava as ligações feitas pela Clint em dois canais (SDR e Lead), salva o áudio no Google Drive e cria uma guia no Google Docs com o resumo para o closer e a transcrição (Gemini).

- `index.html`: o gravador, publicado pelo GitHub Pages.
- O processamento (Gemini, Drive e Docs) roda num projeto do Google Apps Script (`Codigo.gs` + `appsscript.json`, que **não** ficam neste repositório).

## Publicar

1. **Apps Script**
   - Cole `Codigo.gs` e `appsscript.json` no projeto. Os arquivos `Index` e `Gravador` antigos podem ser apagados.
   - Execute `criarCodigoAcesso()` e anote o código que aparece no log.
   - Implantar → Nova implantação → App da Web: executar como **Eu**, acesso **Qualquer pessoa**.
   - Copie a URL que termina em `/exec`.
2. **index.html**: troque `COLE_AQUI_A_URL_DO_WEB_APP` pela URL copiada.
3. **GitHub**: envie o `index.html` para este repositório e ative em Settings → Pages → Deploy from a branch → `main` / `(root)`.
4. Abra `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO` no Chrome e digite o código de acesso.

## Uso

1. Clique em **Iniciar gravação**, escolha a aba da Clint e marque **Compartilhar áudio da aba**; depois permita o microfone.
2. Preencha nome e telefone quando o lead atender; o SDR é obrigatório para salvar.
3. **Encerrar e salvar** gera a guia no Docs; **Descartar** joga a ligação fora; **Nova chamada** limpa a tela.

Use fone de ouvido. Funciona no Chrome ou Edge no computador.
