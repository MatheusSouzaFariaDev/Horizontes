# Horizontes — Portfólio Fotográfico do Meio Ambiente

Site acadêmico desenvolvido por estudantes da **Fatec Itu** para apresentar uma coleção fotográfica autoral sobre o **pôr do sol** observado no campus e em seu entorno. O projeto combina sensibilidade fotográfica, educação ambiental e princípios de **Interação Humano-Computador (IHC)**.

---

## ✨ Objetivo

Apresentar, de forma esteticamente cuidadosa e acessível, fotografias do entardecer na Fatec Itu, promovendo:
- valorização da natureza local;
- conscientização ambiental por meio da imagem;
- aplicação prática de boas práticas de design, IHC e acessibilidade web.

---

## 🛠 Tecnologias utilizadas

- **HTML5** semântico
- **CSS3 moderno** (variáveis CSS, `grid`, `flexbox`, `clamp()`, `color-mix()`, `aspect-ratio`)
- **JavaScript (ES6+)** puro, sem frameworks
- Fontes Google: **Inter** (sans) + **Cormorant Garamond** (display)
- 100% estático — pode ser hospedado em **GitHub Pages, Netlify, Vercel, Hostinger** ou qualquer servidor web.

---

## 🧠 Aplicação dos conceitos de IHC

| Princípio | Como foi aplicado |
|---|---|
| **Visibilidade do estado do sistema** | Hover states, foco visível, página atual destacada na navbar, contador na lightbox. |
| **Consistência e padrões** | Design system único (cores, tipografia, espaçamentos, componentes) em todas as páginas. |
| **Reconhecer em vez de lembrar** | Menu fixo, breadcrumbs, ícones com rótulos acessíveis. |
| **Feedback** | Microanimações em botões, transições suaves em imagens, estados pressionados. |
| **Prevenção de erros** | Lightbox fecha com `Esc` e clique no fundo; navegação por setas. |
| **Estética e design minimalista** | Hierarquia visual clara, conteúdo essencial em primeiro plano. |
| **Flexibilidade e eficiência** | Filtros de categoria, tema claro/escuro persistente, atalhos de teclado. |

---

## ♿ Estratégias de acessibilidade (WCAG)

- Botão **“Pular para o conteúdo”** no topo de cada página.
- Estrutura **semântica** (`header`, `nav`, `main`, `section`, `article`, `footer`).
- **`alt`** descritivo em todas as imagens; imagens decorativas com `aria-hidden`.
- **Navegação por teclado** completa (Tab, Shift+Tab, Enter, Esc, ←/→ na lightbox).
- **Foco visível** com contorno reforçado (`:focus-visible`).
- **Contraste AA** ou superior nas combinações de texto/fundo (modo claro e escuro).
- **`aria-label`** em botões com apenas ícones, **`aria-pressed`** em chips de filtro, **`aria-current="page"`** na navegação ativa.
- **`prefers-reduced-motion`**: animações são neutralizadas para usuários sensíveis.
- **`lang="pt-BR"`** no `<html>`, **`role="dialog"`** + **`aria-modal`** na lightbox.

---

## 📁 Estrutura de pastas




```
site/images/fotos/
```


```
foto1.jpeg   foto3.jpeg   foto4.jpeg   foto5.jpeg   foto6.jpeg
foto7.jpeg   foto8.jpeg   foto9.jpeg   foto10.jpeg  foto11.jpeg
foto12.jpeg  foto13.jpeg  foto14.jpeg  foto15.jpeg  foto16.jpeg
foto18.jpeg  foto19.jpeg  foto20.jpeg
```


---

## ▶️ Como executar

Como o projeto é 100% estático, basta abrir o `index.html` no navegador. Para evitar restrições de `file://`, recomenda-se um servidor local simples:

**Python**
```bash
cd site
python3 -m http.server 8080
# abra http://localhost:8080
```

**Node**
```bash
cd site
npx serve .
```

**Hospedagem**: faça upload da pasta `site/` (ou do conteúdo dela) para GitHub Pages, Netlify, Vercel, Hostinger, etc.

---

## 🎨 Decisões de design

- **Paleta natureza**: verde floresta, verde musgo, verde claro, azul céu, azul petróleo, bege areia e branco gelo — evocando o entardecer e os tons orgânicos do campus.
- **Tipografia dupla**: Cormorant Garamond (display, contemplativa) + Inter (texto, legível).
- **Hero cinematográfico** com zoom lento (`heroZoom`) e overlay gradiente para garantir contraste do texto.
- **Mosaico de destaques** com proporções variadas para criar ritmo visual.
- **Galeria masonry** via CSS `columns` — leve, sem JavaScript pesado.
- **Lightbox** elegante, com navegação por teclado, contador e fechamento intuitivo.
- **Dark mode** real, com tokens próprios — não é apenas inversão de cores.
- **Microanimações** sutis (reveal on scroll, hover scale, fade) que orientam sem distrair.

---

## 👥 Créditos da equipe

- **Matheus Souza de Faria** — Criador do site
- **Moisés Alexandre da Cruz Lima** — Fotógrafo
- **Diego Stocco de Oliveira** — Fotógrafo

📧 **Contato:** [contato.portifolio@gmail.com](mailto:contato.portifolio@gmail.com)

---

> *“Olhar com calma também é um ato ambiental.”*
