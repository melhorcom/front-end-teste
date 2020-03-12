# Teste de Front-End (ReactJS)

### Proposta

Uma empresa vai lançar um novo app para venda de celulares e com isso gostaríamos que você construísse um website para gerenciar o cadastro de novos celulares.

### Requisitos

1. O App deverá ser feito em ReactJs.
2. Poderá ser utilizado qualquer biblioteca.
3. Deverá ser entregue o link do respositório git com a resolução.

### Solução

A solução consistirá em criar uma aplicação frontend usando ReactJS.

### Descrição do modelo

| Campo     | Tipo        | Descrição                          | Restrições                                                                                        |
| --------- | ----------- | ---------------------------------- | ------------------------------------------------------------------------------------------------- |
| model     | Texto       | Nome do modelo do celular          | Alfanumérico com no mínimo 2 e no máximo 255 caracteres, desprezando espaço em branco.            |
| price     | Número real | Preço do celular                   | Número positivo                                                                                   |
| brand     | Texto       | Nome da marca do celular           | Alfanumérico com no mínimo 2 e no máximo 255 caracteres, desprezando espaço em branco.            |
| startDate | Data        | Data de início da venda do celular | Data no formato “dd/MM/yyyy” (31/12/2018). A data de início deve ser posterior ao dia 25/12/2018. |
| endDate   | Data        | Data de fim da venda do celular    | Data no formato “dd/MM/yyyy” (31/12/2018). A data de fim deve ser posterior a data de início.     |
| color     | Lista fixa  | Cor do celular                     | Essa campo admite apenas os seguintes valores: BLACK, WHITE, GOLD, PINK.                          |
| code      | Texto       | Código de identificação do celular | Alfanumérico de 8 caracteres. Não deve se repetir.                                                |

### Requisitos funcionais

- Deve ser possível **cadastrar, editar, excluir e listar** todos os celulares.
- O sistema deve validar todas as entradas no cadastro de celulares com mensagens de erro de acordo com a validação dos campos acima.
- Será avaliado a capacidade de lógica dos dados e fidelidade ao protótipo.
- Responsividade é um adicional.

### Protótipo

[https://xd.adobe.com/view/3d42f39f-0dfb-459b-45fa-a9e4b0bef673-4b73/](https://xd.adobe.com/view/3d42f39f-0dfb-459b-45fa-a9e4b0bef673-4b73/)

### API

| Tipo   | Url   | Descrição                 |
| ------ | ----- | ------------------------- |
| GET    | teste | listar todos os celulares |
| GET    | teste | listar um celular         |
| DELETE | test  | para deletar              |
| POST   | teste | Criar um novo celular     |
| PATCH  | teste | Editar um celular         |
