<img width="270" height="185" alt="image" src="https://github.com/user-attachments/assets/b5d10b0c-719a-4638-b176-d6af7e46452c" /># 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem vindo ao Projeto Previsão de Estoque Intelgente  com SageMaker Canvas

O objetivo desse projeto foi prever a movimentação e comportamento de um estoque de uma loja com vários produtos, utilizando modelos de Machine Learning. Foram desenvolvidos as seguintes atividades:

### 1. Selecionar Dataset
-  Foi utilizado o Dataset "dataset-1000-com-preco-promocional-e-renovacao-estoque.csv", disponibilizado pela Dio no repositório original desse projeto. Para melhor desempenho editei o arquivo adicionando uma coluna de quantidade de vendida. 

### 2. Construir/Treinar

-   Para Treinamento, importei o arquivo após tratá-lo, para o SageMaker e configurei as variáveis, sendo item id column: ID_PRODUTO, Target Column: VENDAS, E foi escolhido 5 dias para previsão. O modelo considera feiados brasileiros, e reconhece a granularidade dos doados como diário;
- Após a configuração iniciou-se o treinamento que levou por volta de uma hora e meia.
<img width="270" height="185" alt="image" src="https://github.com/user-attachments/assets/3795a3f1-58e6-4149-80ae-ee068e72ec65" />

### 3. Analisar
- Ao análisar o modelo nota-se métricas não tão boas, isso ocorre devido ao pouco volume de dados e padrões irregulares. Para atingir metricas melhores o modelo precisa de mais volume de dados e mais tempo de treinamento
Ainda assim foi possível obter alguns insights razoavelmente satisfatórios.
<img width="1131" height="134" alt="image" src="https://github.com/user-attachments/assets/0aa59ff8-b72e-4750-a9ec-4fc50814e614" />

### 4. Prever

- Após o treinamento foi criado uma inferência para previsão, devido ao baixo volumes de dados o modelo não conseguiu prever todos os produtos, somente alguns (conforme a imagem e a tabela armazenado na pasta de arquivos deste forks)
- Observou-se que as vendas dos produtos 1004, 1017 e 1021, nos próximos 5 dias, não terão um crescimento de demanda, mas também não irão cair drasticamente, a demanda irá manter quase que a média de vendas em relação aos dias anteriores.
- Nota-se também que será necessário repor o estoque dos produtos 1017 e 1021, nos dias 10/02 e 13/02, respectivamente, para que não faltem produtos nos próximos 5 dias.

<img width="1050" height="295" alt="image" src="https://github.com/user-attachments/assets/5a6fda9c-9dc0-423e-8aef-e5a1eacf7cae" />

conclusão
Apesar das métricas não estarem da maneira mais ideal, pude obter insights satisfatórios, além disso foi de grande valia participar desse projeto, adquirindo mais experiência na área de ML, o aprendizado adquirido foi muito grande e pretendo me aprofundar mais, aprimorando meus conhecimentos em modelos de IA. Obrigado equipe DIO e AWS pelo trinamento e Obrigado a todos que irão acessar esse projeto.
