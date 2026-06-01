Aqui está uma sugestão de `README.md` detalhada e estruturada para o seu novo projeto. Ele segue a mesma linha educacional e profissional do anterior, destacando agora as métricas ágeis e a inteligência baseada no *Scrum Guide* que você implementou.

---

# 📈 Burndown Command Center

Um painel de controle interativo e responsivo desenvolvido para acompanhar o progresso de Sprints através de um **Gráfico de Burndown**. Esta aplicação ajuda indivíduos e equipes ágeis a monitorarem o ritmo de trabalho (velocidade), identificarem desvios do planejamento e receberem alertas estratégicos com base nas práticas do *Scrum Guide*.

---

## ✨ Funcionalidades

* **Gráfico de Burndown Dinâmico:** Visualização em tempo real comparando a "Linha Ideal" (planejamento) com a "Linha Real" (progresso diário) utilizando Chart.js.
* **Alertas Inteligentes (Scrum Guide):** O sistema analisa a velocidade de queima de horas e emite alertas automáticos (Adiantado, No Prazo, Atrasado, Risco Crítico), sugerindo ações como renegociar o escopo com o PO (*Product Owner*).
* **Métricas e KPIs em Tempo Real:** Acompanhamento automático de Horas Restantes, Total Queimado, Meta Diária Ajustada e Velocidade Atual (h/dia).
* **Persistência de Dados Local:** O progresso da Sprint atual e o histórico de velocidade da Sprint anterior são salvos automaticamente no `localStorage` do navegador, evitando perda de dados ao atualizar a página.
* **Tema Adaptável (Dark/Light Mode):** A interface se adapta automaticamente ao tema claro ou escuro preferido pelo sistema operacional do usuário.

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído em um formato prático de arquivo único (`index.html`), facilitando a distribuição e uso imediato:

* **HTML5:** Estrutura e semântica do painel de comando.
* **CSS3:** Estilização utilizando *CSS Variables* para o controle de temas (Claro/Escuro), *Grid* e *Flexbox* para o layout de cards, e animações (`@keyframes`) para os indicadores de status.
* **JavaScript (Vanilla):** Lógica de negócios para cálculo de métricas ágeis, validação de inputs e manipulação do DOM.
* **Chart.js (via CDN):** Biblioteca externa leve e poderosa utilizada para renderizar o gráfico de linhas interativo.

---

## 🧠 Conceitos Ágeis Abordados

O código traduz conceitos fundamentais da gestão ágil em cálculos matemáticos aplicados na prática:

* **Taxa Ideal vs. Realidade:** A "Taxa Ideal" divide o total de horas pelos dias da Sprint. O sistema mede o "Desvio de Rota" calculando a diferença exata entre onde a equipe deveria estar hoje e onde ela realmente está.
* **Velocidade da Equipe:** A média de horas concluídas por dia. Ao final de uma Sprint, esse dado é guardado para ajudar na previsão de capacidade da Sprint seguinte.
* **Meta Diária Ajustada:** Se a equipe atrasa, o sistema recalcula matematicamente quantas horas por dia serão necessárias nos dias restantes para que a meta final ainda seja atingida.

---

## 🚀 Como Executar

Por ser uma aplicação baseada inteiramente no lado do cliente (*Client-side*), não é necessário instalar dependências (Node.js, Python, etc.) ou configurar servidores:

1. Faça o clone deste repositório ou baixe o arquivo ZIP:
```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git

```


2. Navegue até a pasta onde o arquivo foi salvo.
3. Dê um duplo clique no arquivo `index.html` para abri-lo diretamente em qualquer navegador moderno (Chrome, Firefox, Edge, Safari).

---

## 🕹️ Como Usar

1. **Configuração Inicial:** Na tela de início, defina o **Total de Horas** estimadas para a Sprint e a quantidade de **Dias** que ela vai durar.
2. **Lançamento de Progresso:** A cada dia de trabalho, insira no painel a quantidade de horas que foram efetivamente concluídas (queimadas).
3. **Acompanhamento:** Observe o gráfico se atualizar e leia a caixa de "Status da Sprint" para saber se o seu ritmo atual é suficiente para terminar o trabalho no prazo.
4. **Fechamento:** Ao concluir todos os dias ou zerar as horas, a Sprint é finalizada automaticamente. Um resumo será gerado e a sua velocidade média será salva para a próxima Sprint.
5. **Reiniciar:** A qualquer momento, clique no botão superior "↺ Reiniciar" para descartar a Sprint atual e planejar um novo ciclo.