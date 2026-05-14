# JOVI — Sprint 2 · Front-End

> Protótipo de interface mobile para o aplicativo de câmera **JOVI**, desenvolvido como entrega da Sprint 2 da disciplina de Front-End.

---

## 📱 Sobre o Projeto

Um aplicativo de câmera inteligente com foco em uso educacional. O protótipo cobre o fluxo completo de telas em HTML/CSS puro, simulando a experiência de um smartphone (frame 320×690px), com design system próprio baseado em Flexbox, paleta dark com azul elétrico e tipografia Rajdhani.

### Telas implementadas

| Arquivo | Tela |
|---|---|
| `index.html` | Splash Screen — animação de abertura do app |
| `camera.html` | Câmera principal — viewfinder, modos, Smart-Pop IA |
| `outrosModos.html` | Grade de modos extras de câmera |
| `configuracao.html` | Configurações — câmera, IA e armazenamento |
| `editar.html` | Editor de modos — reordenar/adicionar modos |
| `joviEdu.html` | JOVI Edu — câmera educacional com viewfinder inteligente |
| `materias.html` | Lista de matérias — Professor IA por disciplina |
| `chat.html` | Chat com o Professor IA — respostas, fórmulas e passos |

---

## 🗂 Estrutura do Repositório

```
JOVI-Sprint2FrontEnd/
├── index.html
├── pages/
│   ├── camera.html
│   ├── outrosModos.html
│   ├── configuracao.html
│   ├── editar.html
│   ├── joviEdu.html
│   ├── materias.html
│   └── chat.html
├── css/
│   └── style.css
├── imgs/
│   ├── TelaFundo.png
│   └── Anima.gif
└── INTEGRANTES.txt
```

---

## 🎨 Design System

- **Fonte:** Rajdhani (500, 600, 700) via Google Fonts
- **Cor principal:** `#0A6CFF` (JOVI Blue)
- **Fundo:** gradiente `#040c1a → #060f1e → #020609`
- **Layout:** Flexbox em todas as telas; CSS Grid apenas nos cards de modos
- **Variáveis CSS:**

```css
--jovi-blue:      #0A6CFF
--jovi-blue-dim:  rgba(10, 108, 255, 0.16)
--jovi-blue-glow: rgba(10, 108, 255, 0.35)
--border-white:   rgba(255, 255, 255, 0.10)
--text-muted:     rgba(255, 255, 255, 0.40)
--font-display:   'Rajdhani', sans-serif
```

---

## 👥 Integrantes e Responsabilidades

O CSS foi desenvolvido de forma modular: cada integrante foi responsável pelo HTML da sua tela e pela seção correspondente do `style.css`.

---

### Guilherme Pereira Ruiz da Silva — RM: 573360

**Telas:** `index.html` · `chat.html`

**CSS — Splash Screen**
Classes: `.status-bar`, `.animacao`, `.time`, `.icon-svg`, `.battery-container`, `.battery-level`, `.battery-cap`

**CSS — Chat com Professor IA**
Classes: `.chat-screen`, `.chat-header`, `.chat-header-avatar`, `.chat-header-info`, `.chat-header-actions`, `.chat-bubble-wrap`, `.chat-bubble`, `.chat-bubble-left`, `.chat-bubble-right`, `.chat-bubble-sender`, `.chat-bubble-time`, `.chat-ia-avatar`, `.chat-formula`, `.chat-step`, `.chat-step-num`, `.chat-content-card`, `.chat-card-*`, `.chat-online-dot`, `.chat-status-pulse`, `.chat-date-sep`, `.chat-suggestions`, `.chat-suggestion`, `.chat-input-area`, `.chat-input-box`, `.chat-attach-btn`, `.chat-send-btn`

---

### Antonio do Nascimento Ferreira de Sousa — RM: 573706

**Telas:** `outrosModos.html` · `editar.html`

**CSS — Mais Modos**
Classes: `.camera-modes-screen`, `.modes-status-bar`, `.modes-header`, `.modes-back-btn`, `.modes-page-title`, `.modes-header-ghost`, `.modes-hint`, `.modes-grid-wrap`, `.modes-grid`, `.mode-card-jovi`, `.mode-card-icon`, `.mode-card-label`, `.modes-home-bar`

**CSS — Editar Modos**
Classes: `.edit-screen`, `.edit-header`, `.edit-action-btn`, `.edit-action-confirm`, `.edit-body`, `.edit-section-head`, `.edit-section-title`, `.edit-section-hint`, `.edit-grid`, `.edit-grid-main`, `.edit-grid-more`, `.edit-card`, `.edit-card-active`, `.edit-card-highlight`, `.edit-card-empty`, `.edit-card-icon`, `.edit-card-icon-ghost`, `.edit-card-label`, `.edit-card-label-ghost`, `.edit-badge`, `.edit-badge-add`, `.edit-badge-remove`, `.edit-divider`

---

### Gustavo Leal — RM: 569361

**Telas:** `materias.html` · `joviEdu.html`

**CSS — Lista de Matérias**
Classes: `.mat-screen`, `.mat-header`, `.mat-header-center`, `.mat-header-title`, `.mat-header-sub`, `.mat-new-btn`, `.mat-search`, `.mat-section-label`, `.mat-list`, `.mat-row`, `.mat-row-icon`, `.mat-row-body`, `.mat-row-top`, `.mat-row-name`, `.mat-row-time`, `.mat-row-preview`, `.mat-badge`, `.mat-cam-btn`

**CSS — JOVI EDU Câmera**
Classes: `.edu-screen`, `.edu-screen-bg`, `.edu-screen-grid`, `.edu-finder`, `.edu-fc`, `.edu-fc-tl`, `.edu-fc-tr`, `.edu-fc-bl`, `.edu-fc-br`, `.edu-scan-line`, `.edu-top-bar`, `.edu-ia-btn`, `.edu-ia-avatar`, `.edu-ia-badge`, `.edu-ia-info`, `.edu-ia-name`, `.edu-ia-sub`, `.edu-ia-notif`, `.edu-screen-title`, `.edu-top-actions`, `.edu-frame-hint`, `.edu-hint-dot`, `.edu-hint-text`, `.edu-footer`, `.edu-chips-row`, `.edu-chip`, `.edu-chip-active`, `.edu-ctrl-row`, `.edu-side-btn`, `.edu-shutter`, `.edu-shutter-inner`

---

### Matheus Mendes Duarte da Silva — RM: 569559

**Tela:** `configuracao.html`

**CSS — Configurações**
Classes: `.cfg-screen`, `.cfg-bg-grid`, `.cfg-bg-halo`, `.cfg-status-bar`, `.cfg-time`, `.cfg-icon-svg`, `.cfg-battery`, `.cfg-battery-level`, `.cfg-battery-cap`, `.cfg-header`, `.cfg-page-title`, `.cfg-back-btn`, `.cfg-header-ghost`, `.cfg-body`, `.cfg-section-label`, `.cfg-row`, `.cfg-row-link`, `.cfg-row-toggle`, `.cfg-row-icon`, `.cfg-row-icon-blue`, `.cfg-row-body`, `.cfg-row-title`, `.cfg-row-sub`, `.cfg-row-arrow`, `.cfg-toggle`, `.cfg-toggle-on`, `.cfg-toggle-thumb`, `.cfg-storage-bar-wrap`, `.cfg-storage-bar`, `.cfg-storage-fill`, `.cfg-storage-labels`

---

### Matheus Sato Oliveira do Prado — RM: 569392

**Tela:** `camera.html`

**CSS — Câmera Principal**
Classes: `.camera-screen`, `.fundoTela`, `.status-bar-cam`, `.header-camera`, `.cam-icon-btn`, `.cam-title`, `.cam-actions`, `.cam-ctrl-btn`, `.cam-ctrl-label`, `.btn-shutter`, `.btn-shutter-inner`, `.smart-pop-wrap`, `.smart-pop`, `.smart-pop-left`, `.smart-pop-pulse-ring`, `.smart-pop-ia-badge`, `.smart-pop-body`, `.smart-pop-label`, `.smart-pop-mode`, `.smart-pop-ok`, `.footer-camera`, `.selector-modos`, `.modo-item`, `.modo-link`, `.shutter-container`, `.home-bar`

> Também inclui os estilos globais compartilhados: variáveis CSS (`:root`), reset (`*`), body, `.phone`, `.icons-group`, `.icon-svg`, `.battery-container` e `@keyframes` (`fadeUp`, `cardIn`, `smartPopIn`, `ringExpand`, `eduScan`).

---

## ⚠️ Nota sobre o Histórico de Commits

Este repositório contém apenas **um commit** com todos os arquivos do projeto. Isso ocorreu porque o integrante responsável pelo repositório, **Guilherme Pereira Ruiz da Silva**, ao finalizar sua parte do desenvolvimento, excluiu acidentalmente o repositório original — que continha o histórico completo de commits de todos os integrantes. Os arquivos estavam salvos localmente em sua máquina e foram então reenviados em um único commit de restauração. O trabalho de todos os integrantes estava concluído e está integralmente presente no repositório.
