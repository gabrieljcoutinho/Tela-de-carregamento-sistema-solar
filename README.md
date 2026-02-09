# ☀️ Solar System Loading Animation

Uma tela de carregamento imersiva que utiliza a mecânica orbital do nosso sistema solar para representar o processamento de dados em tempo real.

## 🌌 O Conceito
Em vez de uma linha reta, o progresso é visualizado através de **órbitas planetárias**. Cada planeta girando ao redor do sol representa uma camada diferente de carregamento (assets, banco de dados, autenticação).

### 🪐 Elementos da Animação
* **O Sol (Centro):** Representa o núcleo da aplicação (Kernel/Main Engine).
* **Órbitas Internas:** Processos rápidos e leves (carregamento de scripts).
* **Órbitas Externas:** Processos mais pesados (carregamento de imagens e vídeos 4K).

---

## 🚀 Características Visuais

A animação utiliza propriedades físicas simuladas para criar um efeito realista:

* **Velocidade Orbital:** Planetas mais próximos do centro giram mais rápido, seguindo uma lógica inspirada nas Leis de Kepler.
* **Glow Effect:** Efeito de brilho neon para destacar os corpos celestes em fundos escuros.
* **Rastros de Partículas:** Pequenas "caudas" que indicam a direção do movimento.



---

## 🛠️ Especificações Técnicas

| Componente | Técnica Utilizada | Função |
| :--- | :--- | :--- |
| **Sol** | CSS Pulse Animation | Indica que o sistema está "vivo". |
| **Planetas** | `transform: rotate()` | Controla a progressão do tempo. |
| **Espaço** | Parallax Background | Cria profundidade conforme o mouse se move. |

### Exemplo de Lógica CSS:
```css
.planet {
  animation: orbit 4s linear infinite;
  /* Cada planeta tem um tempo de animação diferente */
}
