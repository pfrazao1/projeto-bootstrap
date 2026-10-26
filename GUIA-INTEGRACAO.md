# Guia rápido do projeto — Eco em Ação

## Estrutura de arquivos

```text
sustentabilidade-bootstrap/
├── index.html
├── css/
│   └── style.css
├── .nojekyll
└── GUIA-INTEGRACAO.md
```

O `index.html` fica na raiz para facilitar a publicação pelo GitHub Pages. O projeto carrega o Bootstrap 5.3.8 por CDN e os estilos próprios a partir de `css/style.css`.

## Para o integrante responsável pelos cards e pelo formulário

No `index.html`, procure pelos comentários `ÁREA DO SEGUNDO INTEGRANTE: CARDS` e `ÁREA DO SEGUNDO INTEGRANTE: FORMULÁRIO`.

- **Cards:** substitua o conteúdo de `<div id="cards-praticas" ...>` pelos cards. Uma boa estrutura é uma `div class="row g-4"` com colunas responsivas (`col-12 col-md-6 col-lg-4`) e cards Bootstrap (`card h-100`).
- **Formulário:** substitua o conteúdo de `<div id="formulario-contato" ...>` por um `<form>`. Use `form-label`, `form-control`, `form-select` quando aplicável, e um botão `btn btn-success`. Cada campo precisa de um `<label for="...">` associado a um `id` único.
- **Não remova** os IDs `praticas` e `contato`, pois a Navbar e os botões do Carousel apontam para essas âncoras.
- O formulário HTML, por si só, não armazena nem envia dados para um servidor. Para um trabalho front-end, pode servir como demonstração visual se isso corresponder ao enunciado.
- Ao integrar, apaguem os textos de “Área reservada…” para eles não aparecerem na versão final.

## Testar localmente

1. Extraia a pasta do ZIP.
2. Abra a pasta inteira no Visual Studio Code.
3. Abra `index.html` no navegador (ou use a extensão Live Server, caso esteja instalada).
4. Teste o menu em tela pequena, os três slides, as setas, os indicadores e os links da Navbar.
5. Verifique se as imagens aparecem com conexão à internet. Elas usam URLs externas do Unsplash.

## Criar o repositório GitHub

1. No GitHub, clique em **New repository**.
2. Use um nome curto, por exemplo `sustentabilidade-no-dia-a-dia`.
3. Escolha **Public** se estiver usando GitHub Free e quiser habilitar Pages sem plano pago; não coloque dados pessoais ou informações privadas.
4. Se for enviar pelo terminal usando os comandos abaixo, crie o repositório vazio, sem inicializar README, `.gitignore` ou licença pelo site. Se preferir fazer upload pelo navegador, pode criar o README no GitHub, mas envie os arquivos de modo que `index.html` fique diretamente na raiz (não deixe o `index.html` preso dentro de uma segunda pasta).

Se já tiver o Git instalado, execute os comandos abaixo no terminal aberto dentro desta pasta, substituindo `SEU-USUARIO` pelo seu nome de usuário do GitHub:

```bash
git init
git add .
git commit -m "Cria landing page de sustentabilidade"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/sustentabilidade-no-dia-a-dia.git
git push -u origin main
```

Se o repositório já existir ou já tiver um remoto configurado, não repita `git init` ou `git remote add origin` sem conferir a configuração. Se o repositório remoto já tiver um README/commit e você iniciar outro histórico local, pode ser necessário sincronizar os históricos antes de enviar.

## Dar acesso ao colega

1. No repositório, abra **Settings → Collaborators** (na seção **Access**).
2. Clique em **Add people**, procure o nome de usuário do colega e envie o convite.
3. O colega precisa aceitar o convite antes de editar o repositório.

Como os dois vão alterar o mesmo `index.html`, conversem antes de substituir trechos. Para diminuir conflitos, cada um pode trabalhar em uma branch e depois combinar as alterações; para um trabalho introdutório, também dá para editar com cuidado uma única cópia e fazer commits frequentes.

## Ativar GitHub Pages

1. Abra o repositório no GitHub.
2. Entre em **Settings → Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**.
4. Selecione a branch `main` e a pasta `/(root)`.
5. Clique em **Save** e aguarde o workflow de publicação terminar.
6. Volte a **Settings → Pages** e abra o endereço exibido em **Visit site**.

O endereço costuma seguir o formato `https://SEU-USUARIO.github.io/sustentabilidade-no-dia-a-dia/`, mas use o link mostrado pelo próprio GitHub para confirmar.

## Checklist final

- [ ] `index.html` está na raiz da branch `main`.
- [ ] Os caminhos para CSS e scripts estão corretos.
- [ ] Navbar abre e fecha em dispositivos móveis.
- [ ] Carousel avança automaticamente e também funciona pelas setas e indicadores.
- [ ] Cada link da Navbar leva à seção correta.
- [ ] Os cards e o formulário substituíram os avisos temporários.
- [ ] O site foi verificado em computador e celular.
- [ ] A página publicada abre pelo GitHub Pages.
- [ ] O colega terminou o `README.md` e vocês fizeram o commit das alterações finais.
