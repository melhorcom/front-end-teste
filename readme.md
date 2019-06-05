# Teste de Front-End (ReactJS)
### Proposta
Uma empresa vai lançar um novo app para venda de celulares e com isso gostaríamos que você construísse uma API para gerenciar o cadastro de novos celulares.

### Solução
A solução consistirá em criar uma aplicação frontend usando ReactJS com a REST API na pasta "/api/".

### Descrição do modelo
| Campo | Tipo | Descrição | Restrições |
| ------ | ------ | ------ | ------ |
| model | Texto | Nome do modelo do celular | Alfanumérico com no mínimo 2 e no máximo 255 caracteres, desprezando espaço em branco. |
| price | Número real | Preço do celular | Número positivo |
| brand | Texto | Nome da marca do celular | Alfanumérico com no mínimo 2 e no máximo 255 caracteres, desprezando espaço em branco. |
| photo | Texto | URL contendo uma imagem que representa o celular | Máximo 255 caracteres, desprezando espaço em branco. |
| startDate | Data | Data de início da venda do celular | Data no formato “dd/MM/yyyy” (31/12/2018). A data de início deve ser posterior ao dia 25/12/2018. |
| endDate | Data | Data de fim da venda do celular | Data no formato “dd/MM/yyyy” (31/12/2018). A data de fim deve ser posterior a data de início. |
| color | Lista fixa | Cor do celular | Essa campo admite apenas os seguintes valores: BLACK, WHITE, GOLD, PINK. |
| code | Texto | Código de identificação do celular | Alfanumérico de 8 caracteres. Não deve se repetir. |

### Operações
Deve ser possível **cadastrar, pesquisar, editar, excluir e listar** todos os celulares. 

### Busca (pode ser sem a API / Um input básico)
Deve ser possível buscar celulares por **qualquer combinação** de seus atributos. Por exemplo, buscar um celular por modelo, ou por marca e cor.

### Validação
O sistema deve validar todas as entradas, tanto no backend quanto no frontend.

O backend deve retorna uma resposta com os códigos HTTP adequado, de acordo com o resultado da validação, além de incluir uma mensagem para cada violação.

O frontend deve validar os campos à medida que o usuário preenche o formulário, e exibir as mensagens de erro correspondentes.

### Passos para a instalação do MongoDB

01. Entrar na pasta /API/ e digitar npm i;
02. Processo de configuração da database
03. Aconselhamos utilizar o mongoDB Atlas para criar um servidor (grátis) para hospedar o seu banco de dados. (https://mongodb.com)
04. A criação da conta é de forma rápida e depois é necessário apenas seguir o próprio passo a passo da mongoDB para ligar o servidor.
05. Com o servidor funcionando, é necessário adicionar a URL de conexão(em forma de nodejs) no arquivo DB.js
06. Com a url no DB.js, digitar npm start no cmd e se tudo der certo, uma mensagem de "Database is connected" irá aparecer.

### API - A chamada deve ser feita para 
http://localhost:4000/business para listar
http://localhost:4000/business/delete/:id para deletar
http://localhost:4000/business/add passando um objeto com os determinados estados para adicionar
http://localhost:4000/business/edit/:id para editar

### Outros testes
Teste Back-End Dev (https://github.com/melhorcom/back-end-teste)
Teste Full-Stack Dev (https://github.com/melhorcom/full-stack-teste)
