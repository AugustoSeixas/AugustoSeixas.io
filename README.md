# Sites Úteis em 2026

Curadoria pessoal de recursos para inteligência artificial, programação, pesquisa acadêmica e produtividade.

**Autor:** Augusto Seixas
**Tecnologia:** HTML5 + CSS + JavaScript (vanilla, sem dependências de build)
**Hospedagem:** GitHub Pages

---

## Sobre

Diretório com mais de 160 links organizados em 13 seções temáticas: Inteligência Artificial, Engenharia de Prompt, Programação, DevOps, Ecossistema Python, Estatística e R, Pesquisa, UNICAMP, Programas Úteis, Bancos de Imagens, Tecnologia, Ecossistema Apple e Ecossistema Google.

### Recursos da página

- **Busca instantânea** — filtra links por nome e descrição, com normalização de acentos (buscar "estatistica" encontra "Estatística").
- **Tema claro/escuro** — alternância manual com persistência em `localStorage` e detecção automática da preferência do sistema (`prefers-color-scheme`).
- **Design responsivo** — layout em grade que se adapta de desktop a celular.
- **Acessibilidade** — landmarks semânticos, skip-link para teclado, foco visível e respeito a `prefers-reduced-motion`.
- **Zero dependências de build** — um único arquivo `index.html` autocontido (apenas as fontes vêm do Google Fonts).

---

## Como publicar no GitHub Pages

### Passo 1 — Criar o repositório

1. Acesse [github.com/new](https://github.com/new).
2. Em **Repository name**, use um destes padrões:
   - `seu-usuario.github.io` → o site fica em `https://seu-usuario.github.io/` (raiz do domínio).
   - Qualquer outro nome, por exemplo `sites-uteis` → o site fica em `https://seu-usuario.github.io/sites-uteis/`.
3. Marque o repositório como **Public**.
4. **Não** adicione README, .gitignore ou licença automaticamente (já estão neste projeto).
5. Clique em **Create repository**.

### Passo 2 — Enviar os arquivos

**Opção A — pela interface web (mais simples):**

1. Na página do repositório recém-criado, clique em **uploading an existing file**.
2. Arraste `index.html`, `README.md` e `.gitignore`.
3. Escreva uma mensagem de commit (ex.: "Versão inicial") e clique em **Commit changes**.

**Opção B — pela linha de comando (Git):**

```bash
git init
git add index.html README.md .gitignore
git commit -m "Versão inicial do diretório Sites Úteis em 2026"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPO.git
git push -u origin main
```

### Passo 3 — Ativar o GitHub Pages

1. No repositório, vá em **Settings** → **Pages** (menu lateral).
2. Em **Source**, selecione **Deploy from a branch**.
3. Em **Branch**, escolha `main` e a pasta `/ (root)`.
4. Clique em **Save**.
5. Aguarde de 1 a 2 minutos. O endereço do site aparecerá no topo da mesma página, em "Your site is live at...".

### Passo 4 (opcional) — Domínio personalizado

Se você tiver um domínio próprio (ex.: `sitesuteis.com.br`):

1. Em **Settings** → **Pages** → **Custom domain**, digite o domínio e salve. Isso cria automaticamente um arquivo `CNAME` no repositório.
2. No painel do seu provedor de domínio (Registro.br, Cloudflare, etc.), crie os registros DNS:
   - Para domínio raiz (apex): registros `A` apontando para os IPs do GitHub Pages (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`).
   - Para subdomínio `www`: um registro `CNAME` apontando para `seu-usuario.github.io`.
3. Marque **Enforce HTTPS** após o DNS propagar (pode levar até 24h).

---

## Atualizar o conteúdo

Para adicionar ou editar links, basta editar o `index.html`. Cada link segue o padrão:

```html
<li>
  <a href="https://exemplo.com" target="_blank" rel="noopener noreferrer">Nome do Site</a>
  <span class="desc">Descrição breve e direta.</span>
</li>
```

Depois de editar, faça commit e push (ou edite direto pela interface web do GitHub). O GitHub Pages republica automaticamente em alguns segundos.

---

## Estrutura do projeto

```
.
├── index.html      # Página completa (HTML + CSS + JS embutidos)
├── 404.html        # Página de erro personalizada (servida pelo GitHub Pages)
├── README.md       # Este arquivo
├── LICENSE         # Licença CC BY 4.0
└── .gitignore      # Ignora arquivos de sistema e temporários
```

---

## Licença

Esta obra está licenciada sob a [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.pt).

Você pode compartilhar e adaptar o material para qualquer finalidade, inclusive comercial, desde que dê o crédito apropriado a Augusto Seixas. Veja o arquivo [`LICENSE`](LICENSE) para os termos completos.

---

© 2026 Augusto Seixas. Última atualização: maio de 2026.
