
---

But what is a neural network? | Deep learning chapter 1— 3Blue1Brown (Grant Sanderson) 🔗 https://www.youtube.com/watch?v=aircAruvnKk

---

## 1. O que é Inteligência Artificial 

>área da ciência da computação que desenvolve sistemas capazes de realizar tarefas que normalmente exigiriam inteligência humana (raciocínio, percepção, aprendizado, tomada de decisão). 

>IA é um **guarda-chuva** que engloba várias subáreas e técnicas — nem toda IA "aprende com dados". É crucial diferenciar:

|Técnica|Aprende com dados?|Definição|
|---|---|---|
|**Lógica Booleana**|❌ Não|Álgebra de verdadeiro/falso, regras fixas|
|**Busca Heurística**|❌ Não|Encontra soluções usando "atalhos inteligentes" pré-definidos (ex: A*)|
|**Programação Linear**|❌ Não|Otimização matemática com restrições fixas|
|**Algoritmo Genético**|⚠️ Parcial|Otimiza soluções simulando evolução (seleção, mutação) — explora, mas não "aprende" no sentido de ML|
|**Redes Neurais Artificiais**|✅ Sim|**Ajustam pesos internos a partir de exemplos**, melhorando desempenho progressivamente|

---

## 2. Machine Learning 

>**subárea da IA focada em sistemas que **melhoram seu desempenho automaticamente através da experiência (dados)**, sem serem explicitamente programados regra por regra para cada situação.

### Os 3 tipos principais

|Tipo|Como funciona|Exemplo|
|---|---|---|
|**Supervisionado**|Aprende com dados **rotulados** (entrada + resposta correta)|Classificar e-mail como spam/não-spam|
|**Não supervisionado**|Encontra padrões em dados **sem rótulo**|Agrupar clientes por comportamento de compra|
|**Por reforço**|Aprende por **tentativa e erro**, recebendo recompensas/punições|Agente jogando um jogo, otimizando pontuação|

---

## 3. Redes Neurais Artificiais (o conceito da questão)

modelo computacional inspirado no cérebro humano, formado por **camadas de "neurônios" artificiais** conectados, que ajustam seus **pesos** internos a partir de exemplos (dados) — é o mecanismo central por trás do aprendizado em Machine Learning e Deep Learning.

**Como "aprende":**

1. Recebe uma entrada (ex: imagem de um número escrito à mão)
2. Processa através de camadas (multiplicações, pesos, funções de ativação)
3. Gera uma saída (ex: "isso é o número 7")
4. Compara com a resposta certa → calcula o erro
5. **Ajusta os pesos** pra errar menos da próxima vez (esse é o "aprendizado")
6. Repete o processo com milhares/milhões de exemplos → desempenho melhora ao longo do tempo

> 🎯 **É exatamente essa mecânica de "ajustar e melhorar repetidamente a partir de dados" que faz da Rede Neural a resposta mais direta pra pergunta "o que aprende com dados e melhora desempenho ao longo do tempo".**

---

## 4. Modelos Generativos e LLMs (Modelos de Linguagem)

>modelos de IA (geralmente redes neurais muito grandes, tipo Transformer) treinados para **gerar** conteúdo novo (texto, imagem, código) a partir de padrões aprendidos em enormes quantidades de dados.

- **LLM (Large Language Model)** → treinado em texto, prevê a próxima palavra/token com base no contexto (ex: ChatGPT, Claude, Gemini)
- Modelos generativos também existem pra imagem (ex: geração de imagens a partir de texto)

> ⚠️ Esse tópico entrou como **novidade explícita no edital 2026** ("Atualidades e Inteligência Artificial") — vale ficar de olho em notícias recentes sobre o tema, já que a FGV tende a puxar exemplos atuais.

---

## 5. Ética, Governança e Privacidade em IA

Tópico mais conceitual/discursivo — costuma aparecer como questão de "compreensão geral" nas provas:

- **Viés algorítmico** (bias): modelo reproduz preconceitos presentes nos dados de treino
- **Transparência/explicabilidade**: entender por que a IA tomou certa decisão
- **Privacidade de dados**: uso de dados pessoais no treinamento (conexão direta com **LGPD**)
- **Responsabilidade**: quem responde por decisões erradas de um sistema de IA?
