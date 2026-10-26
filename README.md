# 🌿 Eco em Ação — Sustentabilidade no Dia a Dia

Landing page (página única) sobre pequenas atitudes sustentáveis que podem ser colocadas em prática na rotina. trabalho desenvolvido para a disciplina de Programação Front-end, com o professor **Lucas José de Souza**.

🔗 **Site publicado:** https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/

---

## 🎯 Sobre o projeto

O tema escolhido faz parte da **Agenda 2030**: *Sustentabilidade no Dia a Dia*. A página mostra que pequenas ações, como economizar água, separar o lixo e consumir com consciência, ajudam o planeta.

A página apresenta:

- o que significa viver de forma mais sustentável (Reduzir, Reutilizar e Repensar);
- seis práticas sustentáveis para a rotina, em cards;
- um formulário para o visitante compartilhar a própria ideia sustentável.

## 🧩 Componentes do Bootstrap utilizados

| Componente | Onde aparece |
|---|---|
| **Navbar** | Menu fixo no topo, responsivo (vira "hambúrguer" no celular) |
| **Carousel** | Três slides de destaque no início da página |
| **Cards** | Seção "Práticas sustentáveis" |
| **Form** | Seção "Compartilhe sua ideia sustentável" (`form-control`, `form-select`, `form-check`) |
| **Badge, Alert e Buttons** | Categorias dos cards, mensagem de sucesso do formulário e botões |
| **Grid** (`row`, `col-*`) | Layout responsivo da página inteira |

## 📱 Responsividade

A página usa o sistema de grid do Bootstrap (`col-12 col-md-6 col-lg-4`). Os cards ficam em 1 coluna no celular, 2 no tablet e 3 no computador. O menu também se adapta ao tamanho da tela.

## 📝 Formulário

O formulário pede nome, e-mail, categoria da ideia, cidade (opcional), a ideia em si e o aceite de compartilhamento. A validação usa os recursos do HTML5 e as classes de validação do Bootstrap (`needs-validation` e `was-validated`), que mostram os erros em vermelho.

> ⚠️ O formulário é uma **demonstração visual**. Como o projeto não tem servidor, os dados não são enviados nem armazenados: ao enviar, aparece apenas uma mensagem de sucesso.

## 🛠️ Tecnologias

- HTML5
- CSS3 (arquivo próprio `css/style.css`)
- [Bootstrap 5.3.8](https://getbootstrap.com/) via CDN
- JavaScript (validação do formulário e componentes do Bootstrap)
- GitHub Pages (publicação)

## 📁 Estrutura de arquivos

```text
├── index.html
├── css/
│   └── style.css
├── .nojekyll
├── GUIA-INTEGRACAO.md
└── README.md
```

## ▶️ Como executar

1. Baixe ou clone o repositório:
   ```bash
   git clone https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
   ```
2. Abra a pasta no Visual Studio Code.
3. Abra o arquivo `index.html` no navegador (ou use a extensão Live Server).

## 👥 Equipe

| Integrante | Responsabilidade |
|---|---|
| Pedro Frazão | Estrutura da página, navbar, carousel, seção de apresentação, publicação no github pages, html e css |
| Willyan de Lima Farias | Cards de práticas sustentáveis, formulário e estilos dessas seções, readme.md do projeto, html e css |

## 🤖 Uso de IA

Conforme permitido na atividade, utilizamos inteligência artificial como apoio no desenvolvimento. Todo o código foi revisado e testado pela equipe.

## 🖼️ Créditos

Imagens do carousel: [Unsplash](https://unsplash.com/).