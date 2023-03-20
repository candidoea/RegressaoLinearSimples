Na Regressão Linear Simples do Notebook 'RelacaoCAbecaVolume' foi utilizado o método dos mínimos quadrados:
Para isto segue-se a metodoligia abaixo:

Calculo da média das variáveis deprendente e explanatória:

As variáveis x (volume da Cabeça em cm³) e y (peso da cabeça em g) são as variáveis explanatória e dependente, respectivamente, e são usadas para ajustar a regressão linear.
np.mean() é uma função do pacote NumPy que calcula a média das observações em um array.
x_mean e y_mean são as médias das variáveis x e y, respectivamente.
len() é uma função que retorna o número de observações no dataset.
n é o número de observações no dataset.

Cálculo dos coeficientes a e b:

Numerador e denominador são variáveis usadas para calcular os coeficientes a e b da equação da reta y = a + bx.
O for loop percorre cada observação no dataset e atualiza numerador e denominador em cada iteração.
O numerador é o somatório do produto das diferenças em relação às médias de x e y.
O denominador é o somatório dos quadrados das diferenças em relação à média de x.
b é a inclinação da reta de regressão, que representa a mudança na variável y para cada unidade de mudança em x.
a é o intercepto da reta de regressão, que representa o valor de y quando x é igual a zero.
O método dos mínimos quadrados é utilizado para encontrar os valores de a e b que minimizam a soma dos quadrados dos erros (diferença entre os valores previstos e reais de y) em relação à linha de regressão. A inclinação b é encontrada dividindo a soma dos produtos das diferenças em relação às médias de x e y pelo somatório dos quadrados das diferenças em relação à média de x. O intercepto a é encontrado subtraindo o produto entre a inclinação b e a média de x da média de y. Juntos, a e b formam a equação da linha de regressão, que pode ser usada para prever os valores de y com base nos valores de x.