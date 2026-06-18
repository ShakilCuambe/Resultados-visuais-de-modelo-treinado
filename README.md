Este projeto contém funções auxiliares para visualizar o desempenho de modelos de regressão desenvolvidos com **PyTorch** utilizando **Matplotlib**.

O código disponibiliza duas funções principais:

- **plot_results()**: Plota os dados reais e a linha de previsão gerada pelo modelo treinado.
- **plot_nonlinear_comparison()**: Compara as previsões de um modelo linear com um conjunto de dados que apresenta comportamento não linear.

# Tecnologias Utilizadas

- Python 3
- PyTorch
- Matplotlib

# Estrutura das Funções

#plot_results(model, distances, times)`

Exibe um gráfico contendo:

- Pontos reais do conjunto de dados.
- Linha de previsão produzida pelo modelo.




# `plot_nonlinear_comparison(model, new_distances, new_times)`

Utilizada para demonstrar como um modelo linear se comporta diante de dados não lineares.

O gráfico apresenta:

- Dados reais.
- Linha de previsão do modelo.




As funções executam os seguintes passos:

 Colocam o modelo em modo de avaliação (`model.eval()`).
 Desabilitam o cálculo de gradientes com `torch.no_grad()`.
 Geram previsões utilizando o modelo.
 Criam gráficos utilizando o Matplotlib.
 Exibem:
   - Dados reais em marcadores laranja.
   - Previsões do modelo em linha verde.
   - Título, legenda e grade para melhor visualização.



## Observação

Na função `plot_nonlinear_comparison()` existe uma linha de depuração:

```python
print("snfdjnffkd")
```
