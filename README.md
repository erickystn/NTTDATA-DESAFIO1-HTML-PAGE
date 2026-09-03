<div align="center">

# 🐾 Clínica Veterinária — Portal Institucional Multi-Página

**Website institucional estático e semântico com navegação multi-página, mapa interativo, tabela de plantão e formulário de contato, desenvolvido como Desafio 1 do Bootcamp NTT DATA Diversidade Tech**

[![HTML5](https://img.shields.io/badge/HTML5-Sem%C3%A2ntico-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Flexbox-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
[![Google Fonts](https://img.shields.io/badge/Google%20Fonts-Roboto-4285F4?style=for-the-badge&logo=googlefonts&logoColor=white)](https://fonts.google.com/specimen/Roboto)
[![NTT DATA](https://img.shields.io/badge/NTT%20DATA-Diversidade%20Tech-0019A8?style=for-the-badge)](https://www.nttdata.com/)
[![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=for-the-badge)]()
[![Licença](https://img.shields.io/badge/Licen%C3%A7a-MIT-blue?style=for-the-badge)](./LICENSE)

</div>

---

## 🔗 Referências & Contexto

- **Bootcamp:** NTT DATA Diversidade Tech (Digital Innovation One)
- **Desafio:** Desafio 1 — Construção de uma Página Web Completa com HTML5 e CSS3
- **Identidade Visual:** Paleta em tons de azul institucional (`rgb(0, 133, 190)`) e cinza neutro para transmitir serenidade, higiene e confiabilidade médica.

---

## 📖 Visão Geral

O projeto **Clínica Veterinária** é um portal institucional multi-página estruturado para atender aos requisitos de apresentação de serviços de saúde animal, plantões médicos e agendamentos de consultas. Desenvolvido no módulo introdutório de tecnologias web do programa de formação **NTT DATA Diversidade Tech**, o objetivo principal foi fixar os conceitos primordiais da arquitetura da web: marcação semântica em HTML5, estilização com CSS3 puro utilizando Flexbox para layout responsivo em duas colunas, e incorporação de mídias externas.

A plataforma é dividida em quatro páginas integradas por um menu lateral persistente, oferecendo uma navegação ágil e sem descontinuidades para o tutor do animal.

---

## ✨ Páginas e Funcionalidades

- **🏠 Página Inicial (`index.html`):** Apresentação da identidade visual da clínica veterinária, banner de boas-vindas e introdução institucional.
- **ℹ️ Sobre a Clínica (`pages/about.html`):** Detalhamento dos valores, equipe clínica e infraestrutura hospitalar com cabeçalho fotográfico dedicado (`about.jpg`).
- **🕐 Horário de Atendimento (`pages/opening.html`):** Tabela semântica detalhada (`table`, `thead`, `tbody`) com os turnos de atendimento das especialidades (Clínica Geral, Psicologia Animal, Pediatria e Oftalmologia) divididos entre dias úteis, sábados e feriados, com efeito visual de destaque nas linhas (*hover state*).
- **📞 Central de Contato e Localização (`pages/contact.html`):**
  - Informações de contato telefônico e celular para emergências.
  - Mapa interativo em tempo real incorporado via `<iframe>` do Google Maps.
  - Formulário completo estruturado com `<fieldset>`, `<legend>`, campos com validação de tipo (`text`, `email`), área de texto (`textarea`) e botões de envio e limpeza.

---

## 🎯 Diferenciais e Destaques Técnicos

1. **Arquitetura de Layout com CSS Flexbox:**
   O layout principal é construído através de um container flexível (`.wrapper`), dividindo o espaço proporcionalmente em menu de navegação lateral (15%) e área de conteúdo principal (85%), garantindo alinhamento vertical e harmonia espacial.
2. **Marcação HTML5 Estritamente Semântica:**
   Utilização correta de tags com significado estrutural: `<address>` para localização geográfica, `<fieldset>` e `<legend>` para acessibilidade no formulário, e `<table>`, `<thead>`, `<th>` para dados tabulares.
3. **Cabeçalhos Contextuais por Página:**
   Cada seção interna (`about`, `opening`, `contact`) possui uma classe CSS exclusiva (`.header-about`, `.header-opening`, `.header-contact`) aplicando imagens de fundo personalizadas em alta definição via `background-size: cover`.
4. **Interatividade com JavaScript no Formulário:**
   Inclusão de rotina no botão de envio (`submitBtn`) para alerta de confirmação e redirecionamento automático para a página inicial pós-envio.

---

## 🏗️ Estrutura de Diretórios do Repositório

```text
NTTDATA-DESAFIO1-HTML-PAGE/
├── assets/                     # Recursos gráficos e ilustrações institucionais
│   ├── 124010.png              # Ícone de rede social
│   ├── about.jpg               # Imagem de fundo da página Sobre
│   ├── atendimento.jpg         # Imagem de fundo da página de Horários
│   ├── banner.png              # Banner oficial da clínica veterinária
│   ├── contatos.png            # Imagem de fundo da página de Contato
│   └── icon.png                # Logotipo da clínica
├── css/
│   └── base.css                # Folha de estilos centralizada (layout, fontes, cores e tabelas)
├── pages/                      # Subpáginas do portal
│   ├── about.html              # Página institucional "Sobre a Clínica"
│   ├── contact.html            # Página de contato, mapa e formulário
│   └── opening.html            # Grade de horários e especialidades
├── index.html                  # Página inicial (Home) do portal
└── README.md                   # Documentação técnica consolidada do repositório
```

---

## 🎨 UX e Mapa de Navegação

O fluxo de navegação entre as páginas do portal é demonstrado no diagrama abaixo:

```text
                        [index.html] (Home)
                              │
         ┌────────────────────┼────────────────────┐
         ▼                    ▼                    ▼
[pages/about.html]   [pages/opening.html]   [pages/contact.html]
 (História/Missão)   (Grade de Horários)    (Formulário + Maps)
         │                    │                    │
         └────────────────────┼────────────────────┘
                              │
                              ▼
            [Menu Lateral Persistente em todas as telas]
```

---

## 🧭 Passo a Passo de Uso para o Visitante

1. **Acessar a Home:** Abra o arquivo `index.html` no navegador para visualizar a apresentação da clínica e o menu lateral.
2. **Consultar Horários de Plantão:** Clique em **"Horário de Atendimento"** no menu para inspecionar os turnos das especialidades médicas na tabela comparativa.
3. **Localizar e Enviar Mensagem:** Clique em **"Contato"** para visualizar o endereço no mapa do Google Maps ou preencher o formulário para enviar uma solicitação de consulta.

---

## ⚙️ Requisitos e Como Executar Localmente

Como o projeto é composto por arquivos estáticos nativos da web, não há necessidade de compilação ou instalação de dependências externas.

### Opção 1: Via Extensão Live Server (VS Code)
1. Abra a pasta do repositório no Visual Studio Code.
2. Clique com o botão direito sobre o arquivo `index.html`.
3. Selecione **"Open with Live Server"**. O navegador abrirá a página na porta `5500`.

### Opção 2: Via Python HTTP Server
```bash
# Clone o repositório
git clone https://github.com/erickystn/NTTDATA-DESAFIO1-HTML-PAGE.git

# Acesse o diretório
cd NTTDATA-DESAFIO1-HTML-PAGE

# Inicie o servidor estático local
python3 -m http.server 3000
```
Acesse `http://localhost:3000` no seu navegador.

### Opção 3: Execução Direta
Basta dar um duplo clique no arquivo `index.html` no seu gerenciador de arquivos para visualizá-lo em qualquer navegador web.

---

## 💻 Exemplos de Código em Destaque

### 1. Tabela Semântica com Efeito Hover (`pages/opening.html` e `css/base.css`)
```html
<table class="atendimento">
    <thead>
        <tr>
            <th>Serviços</th>
            <th>Segunda à Sexta</th>
            <th>Sábados</th>
            <th>Feriados</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Clínica Geral</td>
            <td>08h - 19h</td>
            <td>08h - 14h</td>
            <td>08h - 14h</td>
        </tr>
    </tbody>
</table>
```

```css
/* Efeito de destaque nas linhas da tabela ao passar o mouse */
.atendimento tr:hover {
    background-color: rgb(133, 199, 227);
    transition: background-color 0.2s ease;
}
```

### 2. Layout em Duas Colunas com CSS Flexbox (`css/base.css`)
```css
.wrapper {
    width: 95%;
    display: flex;
    margin: 0 auto;
    background-color: rgba(128, 128, 128, 0.3);
}

.menu {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 15%;
    background-color: rgb(0, 133, 190);
    padding-top: 40px;
}

.main {
    display: flex;
    flex-flow: column;
    width: 85%;
}
```

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Função no Projeto |
| :--- | :--- |
| **HTML5** | Estruturação de marcação semântica, formulários de contato e tabelas de horários. |
| **CSS3 (Flexbox)** | Diagramação em duas colunas, cabeçalhos dinâmicos, paleta de cores e estilização de tabelas. |
| **Google Fonts (Roboto)** | Tipografia limpa e moderna para o corpo do texto e cabeçalhos. |
| **Google Maps Embed API** | Incorporação interativa da localização física da clínica via iframe. |
| **JavaScript (Vanilla)** | Manipulação básica de eventos para submissão de formulário e redirecionamento. |

---

## 📈 Melhorias e Próximos Passos (Roadmap)

- [ ] Adaptação para layout responsivo mobile-first com menu hambúrguer para smartphones.
- [ ] Implementação de validação avançada de formulário via JavaScript com mensagens de feedback visual.
- [ ] Envio real do formulário de contato integrado ao EmailJS ou Formspree.
- [ ] Adição de galeria de fotos dos animais atendidos e depoimentos de clientes.

---

## 🤝 Como Contribuir

1. Realize um **Fork** do repositório.
2. Crie uma branch para sua melhoria: `git checkout -b feature/melhoria-layout`.
3. Faça o commit de suas alterações: `git commit -m "feat: adiciona responsividade mobile ao menu"`.
4. Envie a branch para o repositório remoto: `git push origin feature/melhoria-layout`.
5. Abra um **Pull Request**.

---

## 👤 Autor & 📄 Licença

Desenvolvido por **[Ericky Santana](https://github.com/erickystn)** como solução prática do Desafio 1 no bootcamp **NTT DATA Diversidade Tech**.

Este projeto está licenciado sob os termos da licença **MIT** — consulte o arquivo [LICENSE](./LICENSE) para mais detalhes.