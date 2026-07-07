# Engenharia de Prompts

Nesta pasta serão documentados os prompts testados, os resultados obtidos e as dificuldades encontradas durante o uso do NotebookLM.

###  Teste de Prompt 1: Mapeamento de Ferramentas
* **Prompt:** Liste todas as ferramentas de Inteligência Artificial mencionadas nas fontes e descreva de forma direta como cada uma pode ser usada para treinar o inglês.
* **Resultado:**
  * **ChatGPT:** Cria cronogramas personalizados, atua como professor 24h tirando dúvidas de gramática e comparando com o português. Ideal para expansão de vocabulário (sinônimos, antônimos, fonética) e prática de conversação real via modo de voz (com feedbacks detalhados). Também cria quizzes, histórias e corrige redações.
  * **Google Gemini:** Estrutura roteiros de aprendizado e se destaca por recomendar materiais de estudo complementares (artigos, livros, vídeos do YouTube). Excelente para prática de *roleplay* (simulação de papéis, como fingir ser um garçom) e geração de desafios.
  * **Be confident (Bfident):** Funciona no WhatsApp focado em pronúncia. Avalia áudios enviados pelo usuário, mostrando a porcentagem de acerto e dicas de entonação.
  * **Speak:** Aplicativo para conversar por áudio com assistente virtual sem a ansiedade de falar com nativos, aplicando checagem gramatical (*grammar check*).
  * **LanguageTool:** Focado em escrita e leitura, detecta automaticamente erros gramaticais e ortográficos em textos curtos e ensina a forma correta.
  * **Grammarly:** Corretor de escrita que ajusta o tom da comunicação (profissional, amigável, etc.).
  * **DeepL, Reverso e Google Tradutor:** Usados para pesquisa de contexto (frases inteiras) e não apenas traduções literais.
  * **Anki:** Utilizado para repetição espaçada através de flashcards alimentados com dados gerados por outras IAs.
* **Observação:** O NotebookLM organizou perfeitamente as ferramentas extraídas dos vídeos, separando as funções nativas das IAs gerais dos aplicativos de nicho.

---

###  Teste de Prompt 2: Plano de Estudos Semanal
* **Prompt:** Crie um plano de estudos semanal prático para aprender inglês sozinho, focando em conversação e leitura, utilizando apenas os recursos gratuitos do ChatGPT e do Gemini citados nos vídeos.
* **Resultado:**
  * **Preparação:** Dar contexto à IA (ex: brasileiro, nível, metas) e pedir para ela agir como professor particular, escolhendo um tema semanal. Use sempre o mesmo chat para manter o histórico e nível.
  * **Segunda-feira (Vocabulário e Leitura):** Pedir lista de vocabulário com traduções e 3 exemplos práticos de frases. Solicitar uma história curta usando esse vocabulário para praticar leitura.
  * **Terça-feira (Aprofundamento e Gramática):** Pedir para simplificar textos difíceis. Solicitar explicações gramaticais comparando com o português, além de sinônimos e antônimos.
  * **Quarta-feira (Conversação Prática):** Usar o recurso de voz para fazer *roleplay* baseado no tema (ex: simular entrevista ou pedido em restaurante). Pedir para a IA falar mais devagar se necessário.
  * **Quinta-feira (Feedback e Correção):** Solicitar relatório de desempenho da simulação anterior, apontando erros gramaticais e sugestões de expressões mais naturais.
  * **Sexta-feira (Desafio sob Pressão):** Conversação por voz simulando um personagem difícil (cliente insatisfeito ou recrutador rigoroso) para construir confiança, com correções imediatas de erros graves.
  * **Sábado (Revisão Ativa):** Pedir um quiz personalizado (múltipla escolha ou preenchimento de lacunas) sobre os erros da semana, com explicações das respostas.
  * **Domingo (Imersão e Planejamento):** Consumir conteúdos recomendados pela IA (artigos, vídeos) e pedir o cronograma para os próximos 7 dias focado nas maiores dificuldades encontradas.
* **Observação:** O plano ficou extremamente acionável e dividiu bem os estímulos de *input* (leitura) e *output* (conversação por voz/escrita).

---

###  Teste de Prompt 3: Engenharia de Prompts (Comandos Úteis)
* **Prompt:** Quais são os comandos específicos (prompts) recomendados pelos autores dos vídeos para fazer a IA atuar como um professor particular e corrigir meus erros de gramática?
* **Resultado:**
  * **Contexto Inicial:** *"Por favor simule que você é o melhor professor de inglês da atualidade e você está com um brasileiro que nunca estudou inglês na vida e eu gostaria que você fosse o professor desse brasileiro. Você consegue me ajudar?"*
  * **Explicação Gramatical:** *"Estou com dificuldade de entender o ponto gramatical X [...] Você pode me explicar? Compare com o português."*
  * **Exercícios Baseados em Erros:** *"Eu erro muito o ponto gramatical X. Por favor crie três tipos de exercícios para mim com base no efeito teste [...] Depois você me corrige e me explica porque eu errei e como posso melhorar."*
  * **Correção em Tempo Real:** *"Estou no nível B1 do inglês e gostaria de melhorar a minha fala. [...] Quando eu errar, me corrija e me ajude a repetir a forma correta logo depois. Mantenha a conversa rolando, me faça perguntas e interaja comigo."*
  * **Feedback Pós-Conversa:** *"Agora que terminamos a conversa, eu gostaria que você avaliasse o meu idioma. Analise o que eu faço bem e o que poderia melhorar para a próxima. Seja específico nas suas observações, de preferência com exemplos do que eu errei para eu entender bem."*
  * **Melhoria de Escrita (Writing):** *"Rewrite this paragraph using more advanced vocabulary"* ou *"Você pode destacar os erros que eu cometi nos envios das minhas atividades e me explicar o porquê."*
* **Observação:** A IA recuperou as aspas exatas ditas nos vídeos, facilitando a reutilização dos comandos pelos estudantes.

---

###  Teste de Prompt 4: Alertas e Cuidados
* **Prompt:** Resuma os principais alertas ou erros que as fontes recomendam evitar ao utilizar a Inteligência Artificial para estudar idiomas.
* **Resultado:**
  * **Não terceirizar o raciocínio:** Deixar a IA resolver tudo impede o cérebro de fazer as conexões necessárias para fixar o aprendizado.
  * **Não confiar 100% nas respostas:** IAs cometem deslizes gramaticais e inventam regras. É vital manter o senso crítico e checar fontes tradicionais.
  * **Não abandonar professores/materiais tradicionais:** A tecnologia é complementar e não substitui a metodologia estruturada e a interação humana.
  * **Evitar comandos genéricos:** Pedir "me ensine inglês" gera respostas superficiais. Contexto detalhado (nível, língua materna e metas) é obrigatório.
  * **Não usar IA de texto para pronúncia:** Plataformas de texto podem simular ou inventar correções de áudio. Pronúncia envolve musculatura facial, sendo melhor estudada via vídeos de humanos ou apps especializados.
  * **Não abrir chats novos constantemente:** Trocar de chat faz a IA perder o histórico, o nível e o contexto do aluno.
  * **Não pedir apenas um exemplo:** Limitar-se a uma tradução ou frase isolada prejudica a associação de contexto. Exija sempre ao menos 3 exemplos diferentes.
* **Observação:** Esse compilado trouxe maturidade técnica ao projeto, alertando sobre as limitações reais de grandes modelos de linguagem (LLMs).
