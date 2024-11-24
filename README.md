# Sistema Inteligente de Precificação para Assistência 24 Horas

Este projeto utiliza **Machine Learning** para classificar e prever a demanda de serviços de assistência 24 horas para veículos, com o objetivo de oferecer uma precificação justa baseada em dados históricos. O sistema visa resolver a problemática de cobrança fixa, garantindo que modelos de veículos com maior demanda sejam precificados adequadamente, enquanto veículos de menor demanda sejam beneficiados por preços mais competitivos.

---

## 📋 Funcionalidades do Sistema

- **Classificação Baseada em Dados:** Utiliza algoritmos de machine learning para prever a categoria de demanda de assistência.
- **Treinamento e Teste:** Divide os dados históricos em 70% para treinamento e 30% para teste do modelo.
- **Avaliação de Performance:** Gera métricas de desempenho para validar a precisão do modelo antes da produção.
- **Pipeline de Produção:** Implementa o modelo em produção caso a performance atinja os critérios estabelecidos.

---

## 🚀 Tecnologias Utilizadas

- **Python**
- **Pandas e NumPy:** Para manipulação e processamento de dados.
- **Scikit-learn:** Para construção e avaliação dos modelos de classificação.
- **Streamlit:** Para interface interativa com o usuário.
- **Matplotlib/Seaborn:** Para visualização dos dados e das métricas.

---

## 📂 Estrutura do Repositório

```
│   ├── car.csv            # Conjunto de dados de veículos para treinamento e teste.
│   ├── carros.py          # Código principal do projeto de classificação.
│   ├── LICENSE            # Arquivo de licença do projeto.
│   ├── README.md          # Documentação e descrição detalhada do projeto.
│   └── requirements.txt   # Lista de dependências para execução do projeto.
```

---

## 📊 Pipeline de Machine Learning

1. **Divisão dos Dados:**
   - 70% dos dados históricos para **treinamento**.
   - 30% para **teste** e avaliação.

2. **Treinamento do Modelo:**
   - Utilização de algoritmos de classificação (ex.: Random Forest, Logistic Regression).
   - Ajuste dos hiperparâmetros para maximizar a performance.

3. **Avaliação do Modelo:**
   - Métricas como **acurácia**, **precisão**, **recall** e **F1-Score** são analisadas.
   - Apenas modelos com desempenho superior ao limiar definido são considerados para produção.

4. **Produção:**
   - Implementação do modelo em um ambiente de produção para uso em tempo real.

---

## 📈 Exemplo de Fluxo

1. **Dados históricos de demanda** são carregados no sistema.
2. Os dados são divididos em conjuntos de treino (70%) e teste (30%).
3. Um algoritmo de Machine Learning é treinado e avaliado.
4. Se o modelo atender aos critérios de performance, ele é implantado em produção.
5. O modelo classifica a demanda de assistência de um veículo com base nos atributos fornecidos, como:
   - Modelo do veículo.
   - Ano de fabricação.
   - Histórico de assistência.

---

## 🎨 Interface

- **Entrada de Dados:** O usuário insere informações sobre o veículo (ex.: modelo, ano, etc.).
- **Saída do Modelo:** O sistema retorna a classificação de demanda (ex.: **Alta**, **Média**, **Baixa**) e o preço sugerido para o serviço.
- **Visualização de Desempenho:** Métricas e gráficos de avaliação são exibidos para análise do modelo.

---

## ⚙️ Como Rodar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/nayarasobral/project-ML-classificacao-pv.qualidade_do_veiculo
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd sistema-precificacao
   ```
3. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```
4. Execute o aplicativo Streamlit:
   ```bash
   streamlit run src/carros.py
   ```

---

## 🗂️ Dataset

O conjunto de dados utilizado (`car.csv`) inclui os seguintes atributos:

- **Modelo do Veículo:** Nome e especificações do veículo.
- **Ano de Fabricação:** Ano de produção do veículo.
- **Histórico de Assistência:** Frequência de serviços solicitados.
- **Categoria de Demanda:** Classificação da demanda (Alta, Média, Baixa).

---

## 🔮 Resultados Esperados

- **Classificação Precisa:** O modelo prevê a demanda com alta acurácia.
- **Precificação Justa:** Sugestões de preço com base na categoria de demanda.
- **Satisfação do Cliente:** Redução de insatisfação causada pela cobrança fixa.

---

## 🛠️ Melhorias Futuras

- Adicionar novos atributos ao modelo, como localização geográfica e tempo médio de serviço.
- Implementar modelos mais avançados, como redes neurais.
- Suporte para upload de novos conjuntos de dados via interface.

---

## 📝 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](https://github.com/nayarasobral/project-ML-classificacao-pv.qualidade_do_veiculo/blob/main/LICENSE) para mais detalhes.

---

## 🧑‍💻 Autor

- **[Nayara Sobral](https://www.linkedin.com/in/nayara-sobral-oficial/)**  
  Cientista de Dados  
  - **Email:** nayysobrall@gmail.com
  - **GitHub:** [nayarasobeal](https://github.com/nayarasobral)

---

Sinta-se à vontade para dar feedback ou contribuir! ⭐
```