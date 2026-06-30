# 🌐 Single Page Configurable Portfolio

Um template de página única (Single Page) moderno, minimalista e altamente customizável, desenvolvido com **HTML5, CSS3 e JavaScript puro (Vanilla JS)**. O projeto foi estruturado especificamente para que qualquer pessoa — mesmo sem experiência profunda em programação — possa criar, editar e publicar sua própria página em minutos, alterando apenas um único bloco de configuração.

---

## 🚀 Funcionalidades Principais

- **Customização Centralizada:** Altere textos, iniciais da logo, títulos e os 4 cards principais modificando apenas o objeto `CONFIG` no código.
- **Paleta de Cores Global (CSS Variables):** Troque a identidade visual do site inteiro alterando poucas linhas de variáveis no `:root` do CSS.
- **Interatividade Avançada (Sol/Lua):** Inclui um arco interativo com física de arrastar (*drag and drop*) para alternar cenários visuais de Dia e Noite após ativar o interruptor principal.
- **Design Responsivo & Fluído:** Layout totalmente adaptável para dispositivos móveis, tablets e desktops utilizando CSS Grid e propriedades modernas como `clamp()`.
- **Proteção Anti-Inspeção Casual:** Sistema JavaScript integrado para dificultar a abertura do DevTools (F12) e clique direito, mantendo a experiência focada no usuário final.

---

## 🛠️ Como Customizar o Seu Site

Para editar as informações da página, você **não** precisa mexer na estrutura do HTML. Abra o arquivo `.html` em um editor de texto (como VS Code ou Bloco de Notas) e modifique os seguintes blocos:

### 1. Alterar Textos, Logo e Cards (JavaScript)
Localize a tag `<script>` no final do arquivo e altere as propriedades dentro do objeto `CONFIG`:

```javascript
const CONFIG = {
  logoInitials: "SUA_LOGO",           // As letras que aparecem dentro do círculo
  siteName: "Nome do Seu Projeto",    // O título principal da página
  heroText: "Escreva aqui a descrição ou bio do seu site de forma simples...",

  // Configuração dos 4 cards (A, B, C, D)
  cards: [
    { letter: "A", text: "Seu Texto Aqui",  color: "#3ddcff", bold: true,  big: false },
    { letter: "B", text: "Outro Texto",     color: "#7c5cff", bold: false, big: true  },
    { letter: "C", text: "Mais Conteúdo",   color: "#ff8a3d", bold: false, big: false },
    { letter: "D", text: "Link ou Info",    color: "#3aff8c", bold: false, big: false },
  ]
};
