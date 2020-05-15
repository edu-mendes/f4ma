# f4ma

  

## O presente projeto é um Backend de inscrições de um festival de músicas, implementado em Typescript e toda a infraestrutura no AWS.

  

  

### Endpoint de registrar banda.

- O sistema deixar registrado todas as bandas que participarão dos três dias de shows. Para uma banda ser criada, precisamos das informações: nome, gênero musical principal a qual ela se identifica e o nome de um responsável (que pode ser qualquer membro dela). Não podem existir duas bandas com o mesmo nome.

 

### Endpoint de visualização de detalhes sobre a banda.
- Esse endpoint recebe o id ou o nome da banda e retornar as todas as informações salvas sobre ela.

### Endpoint de adicionar um show a um dia.
- Para cadastrar um show, o endpoint precisa do id da banda, o dia (sexta, sábado ou domingo) e o horário em que ela irá se apresentar. Deve haver uma validação para indicar se o horário é válido (ou seja, se está entre 08h e 23h). Além disso os shows só podem ser marcados em horários redondos, ou seja, pode ser 08h - 09h ou 09h - 13h mas não pode ser 09h - 10h30 ou 10h30 - 14h. Caso já exista um show marcado para o dia e o horário em questão, o seu endpoint deve retornar um erro.

### Endpoint de pegar todos os shows de uma data
- Recebe um dia (sexta, sábado ou domingo) e retorna todos os shows daquela data (ordenados pelo horário), mostrando somente o nome da banda e o gênero musical principal.


## Deploy da Aplicação com FutureTube: :dash:

> https://f4tube-e7be0.web.app

  

  

## Linguagens e libs utilizadas :books:

  

  

-  [TypeScript](https://www.typescriptlang.org/)

  

-  [AWS]([https://docs.aws.amazon.com/](https://docs.aws.amazon.com/))





  
## Como rodar a aplicação :arrow_forward:

  

No terminal, clone o projeto:

  
```

git clone https://github.com/eduardomendesnorberto/f4ma.git

```

Entre na pasta do projeto:

  

```

cd f4ma

```

Instale as dependências:



```

npm install

```



Execute a aplicação:

  
```

yarn start

```

Pronto, agora é possível acessar a aplicação a partir da rota http://localhost:3000/

  
  ## Como subir a aplicação para AWS :arrow_forward:

ASW Lambda, criar uma funções e subir o arquivo .zip gerado pela aplicação.
No manipulador de código da função:

 ```

presentation/lambda/index.handler

```



## Status do projeto :heavy_exclamation_mark:

> Status do Projeto: Em desenvolvimento :warning:

  

## Licença :floppy_disk:

  

The [MIT License]() (MIT)

  

Copyright :copyright: 2020 - FutureTube