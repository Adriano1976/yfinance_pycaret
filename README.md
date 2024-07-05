# yfinance PyCaret

Este estudo tem como objetivo principal empregar técnicas avançadas de aprendizado de máquina (machine learning) para desenvolver um `Modelo Preditivo` capaz de estimar com precisão o preço de fechamento das ações da Petrobras ou de outras empresas extraido do site <a href="https://br.financas.yahoo.com/screener">Yahoo Finanças</a>. A abordagem escolhida para esta análise é a regressão linear, um método estatístico robusto e amplamente utilizado para modelar a relação entre variáveis e fazer previsões.<br>

Para alcançar este objetivo, utilizaremos a biblioteca <a href="https://pycaret.org/">PyCaret</a>, Este estudo tem como objetivo principal empregar técnicas avançadas de aprendizado de máquina (machine learning) para desenvolver um Modelo Preditivo capaz de estimar com precisão o preço de fechamento das ações da Petrobras, uma das maiores empresas petrolíferas do mundo e um dos pilares da economia brasileira. A abordagem escolhida para esta análise é a regressão linear, um método estatístico robusto e amplamente utilizado para modelar a relação entre variáveis e fazer previsões.
Para alcançar este objetivo, utilizaremos a biblioteca `PyCaret`, uma ferramenta de código aberto e baixo código (low-code) projetada para simplificar e automatizar o processo de criação de modelos de machine learning em Python. A `PyCaret` oferece uma série de vantagens significativas para este projeto:<br>

- **`Eficiência`**: Permite a rápida experimentação e comparação de múltiplos modelos de regressão.
- **`Facilidade de uso`**: Sua interface intuitiva reduz a complexidade do desenvolvimento de modelos, tornando-o acessível mesmo para profissionais com experiência limitada em programação.
- **`Automação`**: Oferece funcionalidades automatizadas para pré-processamento de dados, seleção de features, treinamento de modelos e otimização de hiperparâmetros.
- **`Flexibilidade`**: Suporta uma ampla gama de algoritmos de machine learning e permite fácil integração com outras bibliotecas populares do ecossistema Python.

Ao longo deste estudo, exploraremos diversas variáveis que podem influenciar o preço das ações, como indicadores econômicos, preços de uma empresa no mercado internacional, dados fundamentalistas da empresa e análises técnicas do mercado de ações. O **Modelo de Regressão Linear** será treinado com dados históricos e sua performance será avaliada utilizando métricas apropriadas, como o erro médio quadrático (MSE) e o coeficiente de determinação (R²).<br>

Além disso, discutiremos as implicações práticas deste `Modelo Preditivo`, suas limitações e possíveis aplicações no contexto do `Mercado Financeiro` e da tomada de decisões de investimento. Este estudo não apenas demonstrará a aplicação prática de técnicas de **Machine Learning em Finanças**, mas também fornecerá insights valiosos sobre os fatores que influenciam o comportamento das ações de empresas do Brasil e de outros paises.<br>

A função `compare_models` organiza o *ranking* de modelos se baseando no coeficiente de determinação R², que é uma métrica muito utilizada para observar o quão bem o modelo se ajusta ao conjunto de dados utilizado. Com isso, podemos ver que `MAE`, `MSE`, `RMSE`, `R2`, `RMSLE` e `MAPE` são todas métricas utilizadas para avaliar a acurácia do nosso modelo:<br>

- **MAE (Mean Absolute Error)**: `MAE` é a média dos valores absolutos das diferenças entre os valores previstos e reais. *Menor valor indica melhor performance.* 🔻
- **MSE (Mean Squared Error)**: `MSE` é a média dos quadrados das diferenças entre os valores previstos e reais. *Menor valor indica melhor performance.* 🔻
- **RMSE (Root Mean Squared Error)**: `RMSE` é a raiz quadrada do MSE. *Menor valor indica melhor performance.* 🔻
- **R² (Coefficient of Determination)**: `R²` varia de 0 a 1, sendo 1 o ideal, indicando que a variância dos dados é completamente explicada pelo modelo. *Quanto maior, melhor performance.* 🔺
- **RMSLE (Root Mean Squared Logarithmic Error)**: `RMSLE` é usado principalmente em previsões de séries temporais ou quando os valores são exponencialmente distribuídos. *Menor valor indica melhor performance.* 🔻
- **MAPE (Mean Absolute Percentage Error)**: `MAPE` mede a média dos erros percentuais absolutos. *Menor valor indica melhor performance.* 🔻<br><hr>
