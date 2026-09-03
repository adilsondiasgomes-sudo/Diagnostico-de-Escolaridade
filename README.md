# Diagnóstico de Escolaridade — GCM Ipatinga

Página única (HTML/CSS/JS, sem build) com o diagnóstico de escolaridade do efetivo
da Guarda Civil Municipal de Ipatinga: painel consolidado, gráfico de barras
interativo, consulta nominal e emissão de relatórios (impressão/PDF e CSV).

- **`index.html`** — aplicação completa. O brasão está embutido no próprio arquivo
  (base64); `brasao-gcmi.png` fica no repositório apenas como fallback.
- Única dependência externa: Google Fonts (carregado via CDN).

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `diagnostico-escolaridade-gcmi`), **público**.
2. No diretório deste projeto:

   ```bash
   git remote add origin https://github.com/SEU_USUARIO/diagnostico-escolaridade-gcmi.git
   git push -u origin main
   ```

3. No GitHub: **Settings → Pages → Build and deployment**
   - *Source*: `Deploy from a branch`
   - *Branch*: `main` / `/ (root)` → **Save**
4. Em ~1 minuto o site fica no ar em:
   `https://SEU_USUARIO.github.io/diagnostico-escolaridade-gcmi/`

Esse é o link para enviar a terceiros. Cada `git push` novo atualiza a página.

## Observação sobre Supabase

Não é necessário: a página é 100% estática e não usa banco de dados. Se no futuro
os dados passarem a vir de uma tabela, o Supabase pode ser adicionado como origem
de dados — hoje o conjunto está embutido em `index.html`.
