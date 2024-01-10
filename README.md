
# Controlador de Ar Condicionado - Lógica Fuzzy

## Descrição
Este projeto implementa um sistema de controle Fuzzy para um ar condicionado. Utiliza-se lógica fuzzy para inferir a temperatura de operação do ar condicionado com base em dois parâmetros de entrada: temperatura e umidade.

### Especificações
- A temperatura varia entre -20 ºC e 50 ºC.
- A umidade varia entre 0% e 100%.
- O funcionamento do ar condicionado varia entre 12 ºC e 35 ºC.

### Regras de Decisão
1. Se a **Temperatura** é **Baixa**, então o **Sistema** deve funcionar no **Aquecer2**.
2. Se a **Temperatura** é **Média** e a **Umidade** é **Alta**, então o **Sistema** deve funcionar no **Aquecer**.
3. Se a **Temperatura** é **Média** e a **Umidade** é **Média** ou **Baixa**, então o **Sistema** deve permanecer **Desligado**.
4. Se a **Temperatura** é **Alta** e a **Umidade** é **Baixa**, então o **Sistema** deve funcionar no **Esfriar1**.
5. Se a **Temperatura** é **Alta** e a **Umidade** é **Média** ou **Alta**, então o **Sistema** deve funcionar no **Esfriar2**.

### Conjuntos Fuzzy
- **Temperatura**: Baixa, Média, Alta.
- **Umidade**: Baixa, Média, Alta.
- **Sistema**: Esfriar2, Esfriar1, Desligar, Aquecer1, Aquecer2.

## Instalação de Pacotes Necessários
Para executar este projeto, é necessário instalar determinados pacotes, como o `skfuzzy`. Consulte o notebook para detalhes sobre a instalação.

## Implementação
O projeto começa com a configuração das variáveis fuzzy e segue com a definição das funções de pertinência e regras de decisão. Para mais detalhes, consulte o código-fonte no notebook fornecido.
