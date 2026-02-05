# ReActAgente-FastCamp

Este repositório contém o desenvolvimento de agentes inteligentes utilizando a arquitetura **ReAct** (Reasoning + Acting).

## Conteúdo do Repositório

### 1. ReAct_Agente_Aula.ipynb
Focado na base técnica e prova de conceito.
* **Objetivo:** Ensinar o agente a usar ferramentas de cálculo e consulta de dados astronômicos.
* **Ferramentas inclusas:** `calculate` e `get_planet_mass`.
* **Destaque:** Implementação da classe `Agent` com gerenciamento de memória (histórico de mensagens).

### 2. ReAct_Agente_Pratica.ipynb
Aplicação prática de um sistema de suporte à decisão clínica.
* **Objetivo:** Triagem inteligente baseada em sintomas e histórico.
* **Regras de Segurança:** O agente foi programado com uma hierarquia de prioridades, onde **Red Flags** e **Interações Medicamentosas** interrompem qualquer outra análise por risco de vida.
* **Ferramentas:** * `calculate_bmi`: Cálculo e classificação de IMC.
  * `get_red_flags`: Identificação de sinais de emergência.
  * `check_drug_interaction`: Verificação de conflitos entre fármacos (ex: Warfarin + Aspirina).
  * `get_differential_diagnosis`: Sugestões de hipóteses diagnósticas.

## Tecnologias Utilizadas

* **LLM:** Llama-3.1 (8b) e Llama-3.3 (70b) via **Groq Cloud**.
* **Linguagem:** Python 3.12.
* **Bibliotecas:** `groq`, `re` (Regex para extração de parâmetros), `os`.

## Importante

* **Para testes utilize uma chave API do modelo de sua preferência, inserindo-a na varável: os.environ['GROQ_API_KEY'] = "SUA_CHAVE_AQUI".

