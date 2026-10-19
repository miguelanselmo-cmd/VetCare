# VetCare — Clínica Veterinária e Centro Diagnóstico 🐾

Solução front-end responsiva desenvolvida como parte das atividades práticas de simulação de ambiente profissional. O projeto consiste em uma *Landing Page* completa para a clínica veterinária fictícia **VetCare**, aplicando conceitos avançados de semântica estrutural, arquitetura CSS e acessibilidade.

---

## 🎯 Objetivo do Projeto
O objetivo principal deste projeto é consolidar habilidades de desenvolvimento front-end com autonomia de layout. A aplicação simula um cenário real onde os requisitos funcionais, não funcionais e a identidade visual (*Design System*) devem ser rigorosamente seguidos para atender tutores de animais de estimação que buscam atendimento especializado de alta qualidade.

---

## 🛠️ Tecnologias e Conceitos Aplicados

### Tecnologias
- **HTML5**: Estruturação semântica avançada da aplicação.
- **CSS3**: Estilização moderna através de variáveis globais, Flexbox e Media Queries.
- **Google Fonts**: Importação da família tipográfica *Poppins* (pesos 400, 500, 600 e 700).
- **Placehold.co**: Consumo de imagens temporárias coerentes com a temática de saúde animal.

### Conceitos e Boas Práticas
- **Metodologia BEM**: Nomenclatura padronizada de classes no HTML e seletores CSS (`Block__Element--Modifier`).
- **Escala REM**: Dimensionamento tipográfico e de espaçamentos baseados estritamente na unidade relativa à raiz do navegador (`html { font-size: 62.5%; }`).
- **Layout Fluido**: Utilização de porcentagens (`%`) para containers flexíveis e unidades de viewport (`vh`/`vw`) para seções em tela cheia.
- **Acessibilidade & Semântica**: Uso correto de tags como `<main>`, `<section>`, `<aside>`, `<details>` e `<summary>`.

---

## 🗂️ Organização da Arquitetura de Arquivos
A estrutura do projeto segue o princípio de separação de responsabilidades, isolando o esqueleto semântico da lógica de estilização:

```text
├── index.html          # Estrutura HTML5 semântica da aplicação
├── css/
│   ├── variables.css   # Definição do Design System (:root e tokens CSS)
│   ├── sidebar.css     # Estilização do Menu Lateral Fixo
│   ├── sections.css    # Estilos das seções principais (Hero, Especialidades, etc.)
│   ├── components.css  # Estilização de cards, FAQ, botões e microinterações
│   ├── footer.css      # Estilização do rodapé fixo
│   └── responsive.css  # Regras de responsividade e Breakpoints (Media Queries)
└── assets/
    └── img/            # Imagens locais (caso aplicável)
```

---

## 🖥️ Funcionalidades Implementadas (Turma B)

- **Menu Lateral Esquerdo Fixo**: Barra de navegação permanente na lateral esquerda em desktops (`position: fixed`).
- **Navegação Suave**: Rolagem fluida com recuo configurado para evitar a sobreposição de conteúdo ao clicar nos links do menu.
- **Seções em Tela Cheia**: Apresentação visual de impacto utilizando componentes organizados com Flexbox (Hero, Especialidades, Corpo Clínico e Infraestrutura).
- **FAQ Interativa**: Central de dúvidas frequentes implementada de forma nativa e semântica com `<details>` e `<summary>`.
- **Rodapé Fixo**: Barra de direitos e localização afixada na base da tela.
- **Botão Flutuante do WhatsApp**: Localizado no canto inferior direito, redirecionando o usuário para a API oficial do WhatsApp utilizando o número oficial da Escola SENAI Henrique Lupo.
- **Microinterações**: Efeitos visuais dinâmicos através de estados `:hover`, `box-shadow` e transições suaves (`transition`).

---

## 🚀 Instruções de Visualização e Execução

### Pré-requisitos
Para visualizar o projeto localmente, basta ter um navegador de internet moderno (Google Chrome, Mozilla Firefox, Edge ou Safari) instalado em sua máquina.

### Executando o Projeto
1. Clone este repositório para a sua máquina local:
   ```bash
   git clone https://github.com
   ```
2. Navegue até a pasta do projeto.
3. Abra o arquivo `index.html` diretamente no seu navegador **OU** utilize a extensão **Live Server** no VS Code para uma pré-visualização em tempo real.

---

## 🧠 Principais Desafios Técnicos e Aprendizados

*(Substitua este texto pelos seus aprendizados reais durante o desenvolvimento! Exemplos abaixo:)*

- **Desafio:** Implementar o recuo correto das seções para que a barra lateral fixa (em desktop) ou o rodapé fixo não cobrissem os títulos ao utilizar a navegação por âncoras.
- **Solução:** Utilização da propriedade `scroll-padding-top` / `scroll-padding-left` no elemento raiz ou margens de compensação nas seções.
- **Aprendizado:** Aprofundamento no uso da metodologia BEM para manter um código CSS limpo, legível e escalável, evitando quebras acidentais de layout ao aplicar responsividade.
