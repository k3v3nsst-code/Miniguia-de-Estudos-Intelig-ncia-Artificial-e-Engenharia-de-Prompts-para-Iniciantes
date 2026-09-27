# 🧠 Miniguia de Estudos: Inteligência Artificial e Engenharia de Prompts para Iniciantes

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge" alt="Status Concluído">
  <img src="https://img.shields.io/badge/Plataforma-Google_NotebookLM-4285F4?style=for-the-badge&logo=google" alt="NotebookLM">
  <img src="https://img.shields.io/badge/Desafio-DIO-orange?style=for-the-badge" alt="DIO Desafio">
  <img src="https://img.shields.io/badge/N%C3%ADvel-Iniciante-blue?style=for-the-badge" alt="Nível Iniciante">
</p>

Repositório criado para o desafio de projeto da **DIO (Digital Innovation One)**, focado na utilização do **Google NotebookLM** como catalisador de **aprendizagem ativa**, curadoria de fontes abertas da internet e engenharia de prompts.

---

## 📌 1. Contexto e Objetivos

### 🎯 Contexto
Com a grande quantidade de ferramentas de IA Generativa surgindo diariamente, estudantes iniciantes enfrentam dois obstáculos comuns:
1. **Sobrecarga de informação:** Dificuldade em filtrar artigos e fontes que sejam confiáveis e didáticas.
2. **Alucinações e respostas vagas:** Frustração ao formular perguntas genéricas e receber respostas prolixas ou incorretas da IA.

Neste projeto, utilizamos o **Google NotebookLM** — uma ferramenta fundamentada (*grounded*) em fontes reais fornecidas pelo usuário — para transformar artigos abertos da internet em uma base de conhecimento confiável para acelerar os estudos em tecnologia.

### 🎯 Objetivos de Aprendizagem
- [x] Selecionar **5 fontes abertas e oficiais da internet** sobre IA e Engenharia de Prompts.
- [x] Aprender a estruturar prompts no modelo **C-P-I-F** (Contexto, Papel, Instrução e Formato).
- [x] Registrar os testes práticos, dificuldades (*cicatrizes*) e soluções no diálogo com o NotebookLM.
- [x] Entregar um Miniguia de Estudos consolidado com resumos, glossário e prompts reutilizáveis.

---

## 📚 2. Curadoria de Fontes da Internet

Foram selecionadas **5 fontes abertas e conceituadas disponíveis publicamente na internet**. Os arquivos com resumos e transcrições estão salvos na pasta [`fontes/`](./fontes) e os links originais estão listados abaixo:

| # | Fonte & Plataforma | Link Original na Internet | Descrição & Por Que Foi Escolhida |
|---|--------------------|----------------------------|-----------------------------------|
| **01** | **Google Cloud Learn** | [O que é IA Generativa?](https://cloud.google.com/learn/what-is-generative-ai?hl=pt-br) | Documentação oficial do Google explicando a base dos modelos de fundação e como a GenAI difere da IA tradicional. |
| **02** | **OpenAI Documentation** | [Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering) | Guia oficial da OpenAI com as 6 melhores práticas e estratégias para criar comandos precisos e sem alucinação. |
| **03** | **W3Schools AI** | [Generative AI Tutorial](https://www.w3schools.com/genai/) | Tutorial didático voltado a iniciantes para entender os limites da IA, uso de personas e técnicas Zero-Shot e Few-Shot. |
| **04** | **Google The Keyword** | [Apresentando o NotebookLM](https://blog.google/technology/ai/notebooklm-google-ai/) | Artigo oficial de lançamento explicando o conceito de *source-grounding* (IA fundamentada em documentos próprios) e o Audio Overview. |
| **05** | **Artigo Aberto Educacional** | [Aprendizagem Ativa e Metodologia](https://pt.wikipedia.org/wiki/Aprendizagem_ativa) | Artigo conceitual sobre técnicas de retenção de conhecimento e a Técnica de Feynman aplicada com auxílio de IA. |

> 💡 **Como essas fontes foram utilizadas:** Os links e conteúdos das 5 fontes foram adicionados ao NotebookLM para que todas as respostas fossem extraídas diretamente de artigos oficiais e verificados.

---

## 🧪 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Documentar as dificuldades encontradas ao formular perguntas e como elas foram resolvidas é um dos critérios mais valorizados para demonstrar raciocínio crítico:

### 🔴 Caso 1: Pergunta Genérica vs. Instrução Parametrizada
- **Prompt V1 (Fraco):** *"Me fale sobre IA."*
  - **Problema / Cicatriz:** A resposta veio acadêmica demais, longa e confusa para quem está no primeiro dia de estudos.
  - **Refinamento (Prompt V2 - C-P-I-F):**
    > *"Atue como um tutor didático de tecnologia. Com base na Fonte 1 (Google Cloud), explique o que é IA Generativa para uma pessoa que nunca programou. Use uma analogia simples do dia a dia e limite a resposta a 2 parágrafos curtos."*
  - **Resultado:** Explicação didática comparando a IA a um assistente de receitas culinárias que aprendeu lendo milhões de livros de culinária. Citação direta com fonte verificada.

---

### 🔴 Caso 2: Síntese Visual e Organização em Tabela
- **Prompt V1 (Fraco):** *"Quais as dicas da OpenAI para fazer prompts?"*
  - **Problema / Cicatriz:** A IA entregou uma lista em bloco de texto difícil de memorizar.
  - **Refinamento (Prompt V2):**
    > *"Com base na Fonte 2 (OpenAI), crie uma tabela comparativa com as 6 estratégias de prompt recomendadas. A tabela deve conter as colunas: Estratégia, Explicação Breve e Exemplo Prático."*
  - **Resultado:** Formato visual limpo e direto, pronto para consulta rápida durante os estudos.

---

### 🔴 Caso 3: Delimitação Estrita para Evitar Alucinações
- **Prompt V1 (Fraco):** *"Qual o melhor modelo de IA para programar em 2026?"*
  - **Problema / Cicatriz:** A pergunta solicitava uma opinião fora do escopo das 5 fontes anexadas, arriscando gerar respostas imprecisas.
  - **Refinamento (Prompt V2 - Strict Grounding):**
    > *"Consulte exclusivamente as 5 fontes anexadas. Há alguma menção expressa sobre ranqueamento de linguagens de programação? Se não houver, responda apenas: 'Informação não presente nas fontes selecionadas'."*
  - **Resultado:** A ferramenta confirmou de forma segura a ausência do dado, sem tentar adivinhar ou inventar fontes fictícias.

---

## 📖 4. Miniguia de Estudos (Entrega Final)

### 📌 Resumo Estruturado dos Aprendizados
1. **O que é IA Generativa:** Modelos estatísticos profundos treinados em grandes volumes de dados que conseguem criar novos textos, códigos e mídias baseando-se em comandos (*prompts*).
2. **O Segredo do Prompt Eficaz:** Um bom prompt não precisa ser rebuscado, mas deve ter clareza: **Contexto** (onde estamos), **Papel** (quem a IA representa), **Instrução** (o que fazer) e **Formato** (tabela, tópicos, parágrafo).
3. **Aprendizagem Ativa com NotebookLM:** Usar a IA para criar quizzes, encontrar lacunas na própria explicação do estudante e gerar resumos em áudio (*Audio Overview*).

---

### 📚 Glossário de Bolso (Termos Essenciais para Iniciantes)

| Termo | O Que Significa na Prática? |
|-------|------------------------------|
| **Prompt** | O comando de texto que você envia para a IA orientando o que ela deve responder. |
| **LLM (Large Language Model)** | Modelo de linguagem treinado com bilhões de parâmetros para entender texto humano. |
| **Alucinação** | Erro em que a IA gera uma informação falsa ou inventada com tom seguro de certeza. |
| **Source-Grounding (Fundamentação)** | Obrigar a IA a responder apenas com base nos documentos ou links fornecidos pelo usuário. |
| **Zero-Shot Prompting** | Fazer uma pergunta direta sem fornecer nenhum exemplo de resposta anterior. |
| **Few-Shot Prompting** | Fornecer 1 ou 2 exemplos do formato esperado antes de pedir a resposta final. |
| **Chain-of-Thought** | Solicitar que a IA explique o passo a passo lógico antes de dar a resposta definitiva. |

---

### 🛠️ 5 Prompts Reutilizáveis para Estudos Futuros

Você pode copiar e colar estes modelos de prompt no NotebookLM ou em qualquer IA para estudar qualquer novo assunto:

```markdown
1. Explicador Didático (Técnica de Feynman):
"Aja como um professor paciente e especialista. Explique o conceito de [INSERIR TEMA] utilizando uma analogia do dia a dia, como se estivesse explicando para alguém iniciante de 12 anos. Evite jargões complexos."

2. Gerador de Quiz com Gabarito:
"Com base no material anexado, elabore um questionário de 5 perguntas de múltipla escolha para testar minha compreensão sobre [TEMA]. No final, adicione o gabarito comentado justificando por que a resposta certa é a correta."

3. Sintetizador Visual em Tabela:
"Sintetize os pontos centrais deste documento em uma tabela de 3 colunas: [Conceito Principal], [Por Que Importa], [Aplicação Prática no Dia a Dia]."

4. Avaliador de Entendimento (Identificador de Lacunas):
"Eu estudei este texto e resumi o seguinte com minhas próprias palavras: '[COLE SEU RESUMO AQUI]'. Aponte com gentileza onde cometi erros conceituais e quais pontos essenciais deixei de fora."

5. Simulador de Entrevista Técnica:
"Você é um entrevistador técnico sênior. Faça 1 pergunta de cada vez sobre [TEMA] no nível júnior/iniciante. Aguarde a minha resposta, avalie meus pontos fortes e fracos, e só depois envie a próxima pergunta."
```

---

## 🚀 Como Utilizar no Google NotebookLM

1. Acesse o **[Google NotebookLM](https://notebooklm.google.com/)** e conecte-se com sua conta Google.
2. Crie um **Novo Caderno** com o nome: `Miniguia - IA para Iniciantes`.
3. Na área de fontes, você pode:
   - Adicionar os **Links Web** das fontes 1 a 5 descritas na tabela acima; ou
   - Fazer o upload dos arquivos da pasta [`fontes/`](./fontes) deste repositório.
4. Execute os prompts documentados na seção de testes para verificar como a IA fundamenta as respostas com base nas fontes.
5. Experimente gerar um **Audio Overview** para ouvir um podcast gerado pela IA resumindo o seu material.

---

## 👨‍💻 Autor & Entrega DIO

Projeto desenvolvido para o Desafio de Projeto da **DIO (Digital Innovation One)**.


