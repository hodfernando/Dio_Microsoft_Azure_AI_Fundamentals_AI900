# Links utilizados para a pratica

Esses links são para a prática do curso de Microsoft Azure AI Fundamentals + AI 900 pela Dio.me.

O primeiro link é para a prática de Machine Learning e o segundo para a prática de Content Safety.

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html

# Criando um modelo de regressão com Azure Machine Learning

## Criando um workspace

Vá ao portal do Azure (https://portal.azure.com) e procure por "Machine Learning" selecione "Azure Machine Learning".

Com o workspace criado, clique em "Iniciar Estudio" para abrir o Azure Machine Learning Studio.

## Criando um novo trabalho de ML automatizado

Com o workspace pronto procure por "ML automatizado" e assim começar a criar um novo trabalho:

## Vamos criar um aprendizado de maquina para a previsão de aluguel de bicicletas:

![Pagina inicial](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/1.png)
![Criando workspace](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/2.png)
![Iniciar workspace](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/3.png)
![Criando ML Automatizado](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/4.png)
![Configurando ML - Básico](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/5.png)
![Configurando ML - Tipo de tarefa](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/6.png)
![Configurando ML - Seleção de dados](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/7.png)
![Configurando ML - Fonte de dados](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/8.png)
![Configurando ML - URL Web](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/9.png)
![Configurando ML - Visualizando dados](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/10.png)
![Configurando ML - Esquema de dados](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/11.png)
![Configurando ML - Examinar dados](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/12.png)
![Configurando ML - Confirmar](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/13.png)
![Configurando ML - Configurando Tarefas](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/14.png)
![Configurando ML - Configurando Tarefas](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/15.png)
![Configurando ML - Configurando Tarefas (Adicionais)](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/16.png)
![Configurando ML - Setando recursos computacionais](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/17.png)
![Configurando ML - Examinar e enviar trabalho](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/18.png)
![Tarefas concluido](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/19.png)
![Selecionando resultado do modelo](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/20.png)
![Apresentando resultado do modelo](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/21.png)
![Valores preditos e verdadeiros](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/22.png)
![Valores residuais](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/23.png)
![Pontos de extremidades](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/24.png)
![Resultado final](https://github.com/hodfernando/Dio_Microsoft_Azure_AI_Fundamentals_AI900/raw/main/Desafio%201/imagens/25.png)

## Teste do modelo

JSON de teste para o modelo de previsão de aluguel de bicicletas:

``` JSON
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
```

O resultado da previsão: 358.7627
