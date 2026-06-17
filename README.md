# Ames Iowa Housing - Análise Exploratória e Machine Learning 🏡

Este projeto tem como objetivo realizar o ciclo completo de Ciência de Dados (Data Science End-to-End) utilizando o famoso dataset **Ames Housing (Iowa)**. O desafio principal consiste em prever o preço de venda de propriedades residenciais com base em diversas características dos imóveis.

O projeto serve como um marco de consolidação de conceitos de manipulação de dados com Pandas, análise estatística exploratória e engenharia de recursos (*Feature Engineering*).

## 🚀 Status do Projeto
- [x] Extração e Entendimento do Domínio dos Dados
- [x] Limpeza e Higienização de Dados Nulos (Tratamento Avançado)
- [ ] Análise Exploratória de Dados Visual (EDA)
- [ ] Feature Engineering (Engenharia de Recursos)
- [ ] Treinamento e Validação de Modelos de Machine Learning
- [ ] Deploy/Construção de Interface Gráfica (Streamlit)

## 📁 Estrutura do Repositório

* **`data/raw/`**: Arquivos originais obtidos publicamente.
* **`data/processed/`**: Base de dados tratada, contendo o zero absoluto de valores nulos (`NaN`) após tratamento estatístico.
* **`notebooks/`**: Jupyter Notebooks com o passo a passo detalhado do desenvolvimento.

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Python 3**
* **Pandas** & **NumPy** (Manipulação de Dados)
* **Matplotlib** & **Seaborn** (Visualização Estatística de Dados)
* **Google Colab** (Ambiente de Desenvolvimento)

## 🧠 Conceitos Aplicados até o Momento

Durante a fase de Higienização de Dados, foram aplicadas estratégias de preenchimento de valores ausentes (`NaN`) baseadas em conhecimento de domínio e estatística descritiva:
1. **Falso Nulo Categórico:** Colunas textuais onde o nulo significava a ausência do recurso (ex: `Pool QC` para sem piscina) foram tratadas com `.fillna("None")`.
2. **Imputação pela Moda:** Tratamento de variáveis de texto pontuais (ex: sistema elétrico) utilizando o valor mais frequente do dataset.
3. **Imputação pela Mediana:** Utilização da mediana para anos de construção de garagem para evitar distorções causadas por *outliers*.
4. **Imputação Condicional Agrupada (Groupby):** Preenchimento da calçada frontal (`Lot Frontage`) calculando a mediana específica de cada bairro (`Neighborhood`), respeitando a distribuição geográfica real dos lotes.

---
*Desenvolvido como projeto de portfólio profissional para demonstração de habilidades técnicas no GitHub.*
