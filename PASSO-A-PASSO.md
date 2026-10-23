# Publicar a Aurum Flow V8

## 1. Cloudflare Worker
1. Acesse https://dash.cloudflare.com/ e entre ou crie uma conta.
2. Abra **Workers & Pages**.
3. Selecione **Create application** e crie um Worker a partir do exemplo Hello World.
4. Use o nome `aurum-flow-api`.
5. Abra **Edit code**, apague o exemplo e cole todo o conteúdo de `worker.js`.
6. Selecione **Deploy**.
7. Copie o endereço `workers.dev` do Worker.
8. Abra esse endereço com `/api/health` no final. O retorno esperado contém `"ok":true`.

## 2. Configurar o frontend
1. Abra `config.js`.
2. Troque `COLE-AQUI-A-URL-DO-WORKER` pelo endereço do Worker, sem barra final.
3. Salve.

## 3. GitHub Pages
1. Acesse https://github.com/ e selecione **New repository**.
2. Nome sugerido: `aurum-flow-v8`.
3. Marque **Public** e crie o repositório.
4. Selecione **Add file > Upload files**.
5. Envie `index.html`, `config.js`, `.nojekyll`, `README.md` e `PASSO-A-PASSO.md`. `worker.js` pode ser enviado como backup.
6. Confirme em **Commit changes**.
7. Abra **Settings > Pages**.
8. Em **Source**, selecione **Deploy from a branch**.
9. Selecione a branch `main`, pasta `/ (root)` e **Save**.
10. Na mesma tela, copie o endereço publicado quando aparecer.

## 4. Teste
1. Abra o endereço do GitHub Pages.
2. Clique em **Atualizar tudo**.
3. Se aparecer erro de configuração, revise `config.js`.
4. Após alterar `config.js`, pressione `Ctrl+F5` no site.

Não publique senhas, tokens ou dados corporativos. Esta versão não precisa de chave secreta.
