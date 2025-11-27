# 📊 Análise de Risco de Crédito - Projeto MinerAI

Este projeto apresenta uma solução completa de Data Mining e Machine Learning para a empresa **MinerAI**, visando identificar padrões de comportamento financeiro e prever riscos de inadimplência.

## 👨‍💻 Equipe de Desenvolvimento
* **Bruno**
* **Artur**
* **Denis**
* **Luccas**
* **Marlon**

---

## 🎯 Objetivo
Realizar uma **Análise Exploratória de Dados (EDA)** robusta e desenvolver um **Modelo Preditivo** capaz de classificar clientes entre "Bons" e "Maus" pagadores, auxiliando a empresa na tomada de decisão para concessão de crédito.

---

## 🛠️ Tecnologias e Ferramentas
* **Linguagem:** Python 3.x
* **Ambiente:** Google Colab / Jupyter Notebook
* **Bibliotecas:** Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn

---

## 🔍 Principais Insights da Análise (EDA)
Durante a exploração dos dados, identificamos padrões cruciais:

1.  **O Fator Idade:** Clientes mais jovens apresentam maior tendência à inadimplência. A idade média dos maus pagadores é sensivelmente menor que a dos bons pagadores.
2.  **Renda não define Caráter:** Surpreendentemente, a mediana de renda é idêntica (R$ 500,00) para bons e maus pagadores. Ter um salário alto não isenta o cliente de risco.
3.  **Geografia do Risco:** Identificamos clusters de risco por Estado. Sergipe (SE) apresentou a maior taxa proporcional de inadimplência (34.8%), enquanto Santa Catarina (SC) se mostrou o estado mais seguro (18.4%).
4.  **Tipo de Residência:** Foi identificado um padrão anômalo no "Tipo de Residência 3", onde maus pagadores possuem renda superior aos bons pagadores, sugerindo um perfil específico de risco.

---

## 🤖 Modelagem Preditiva (Machine Learning)
Utilizamos o algoritmo **Random Forest Classifier** com estratégia de balanceamento de classes.

### Performance do Modelo
* **Acurácia Global:** ~74%
* **Variável mais Importante:** IDADE (Validando a hipótese da EDA).

### Matriz de Confusão
O modelo demonstrou ser **conservador**, priorizando a identificação correta de bons pagadores. Devido à grande sobreposição de características entre as classes (dados muito similares), a detecção de fraude (Recall classe 1) é o ponto focal para melhorias futuras com enriquecimento de dados.

---

## 🚀 Como Executar
1.  Clone este repositório.
2.  Abra o arquivo `.ipynb` no Google Colab ou Jupyter.
3.  Execute as células sequencialmente (o dataset é carregado automaticamente do repositório remoto).

---
*Projeto desenvolvido como requisito da disciplina de Mineração de Dados - Prof. Vagner S. Macedo.*
