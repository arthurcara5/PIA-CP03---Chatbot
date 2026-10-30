# 🤖 FinMentor AI — Chatbot Especializado em Educação Financeira (CKP03)

**Disciplina:** Prompt Engineering and Artificial Intelligence · FIAP · CC 2026  
**Professor:** Prof. Jorge Luiz Gomes  

## 🎯 Sobre o Projeto
O **FinMentor AI** é um chatbot especializado em **Educação Financeira Pessoal e Planejamento de Investimentos no Brasil**, desenvolvido em Python para o Google Colab utilizando o modelo gratuito **`gpt-oss:120b`** via **Ollama Cloud**.

## ✨ Funcionalidades e Diferenciais Implementados
- **System Prompt Robusto com Guardrails (CKP02):** Regras claras de domínio, proibição de recomendação de ativos específicos (*tickers*) e tratamento contra desvios de escopo (*out-of-scope*).
- **Memória de Conversa (`messages`):** Manutenção completa do histórico (`system`, `user`, `assistant`) a cada turno.
- **Diferencial (+0,5) — Template de Prompt com Variáveis:** Função `montar_prompt(usuario, contexto)` para injetar perfil e objetivo do usuário dinamicamente.
- **Diferencial (+0,5) — Múltiplas Personas:** Dicionário `PERSONAS` com 2 comportamentos distintos:
  - `educador` (*Prof. Thiago Nigro*): Didático, acolhedor e focado em iniciantes.
  - `analista` (*Dilma*): Técnica, direta e estruturada em métricas (Selic, CDI, IOF, liquidez).
- **3 Diálogos Documentados (≥ 3 turnos cada):** Caminho Feliz (*Happy Path*), Caso Difícil (*Tricky*) e Fora do Escopo (*Out of Scope*).

## 🚀 Como Executar no Google Colab
1. Faça upload do arquivo `CKP03_Chatbot_Especializado.ipynb` no [Google Colab](https://colab.research.google.com/).
2. No menu lateral esquerdo do Colab, clique no ícone de **Chave (Secrets)** e adicione a chave `OLLAMA_API_KEY` com o seu token do [Ollama Cloud](https://ollama.com/).
3. Clique em **Ambiente de execução > Executar tudo (Run All)**.
