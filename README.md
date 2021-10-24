## Cenário 1
#### O cliente deseja ter um cadastro de PRODUTO, onde seja possível adicionar, atualizar e remover os produtos.

#### Regras
1. Os produtos devem ser únicos
2. Os produtos devem possuir categorias
3. Os produtos devem possuir status 

## Cenário 2
#### O cliente deseja ter um cadastro onde consiga adicionar, atualizar e remover os produtos da VITRINE

#### Regras
1. O produto adicionado na vitrine deve ter um período de exibição (início/ fim)
2. Só deve ser exibido os produtos dentro do período de exibição e que estejam com status em produção
3. Só deve ser possível adicionar produto na vitrine caso o produto esteja ativo
4. Não deve ser possível adicionar o mesmo produto dentro da vitrine
5. Para adicionar o produto na vitrine o mesmo precisa ser homologado e aprovado
6. Para efetuar uma atualização de um produto dentro da vitrine, deve ser gerado uma cópia do produto em produção, o mesmo precisa ser homologado e aprovado, e após isso ele irá substituir o que estava em produção

## TO DO
1. Adicionar request/ response para as controllers
2. Controllers devem acionar os casos de uso para persistirem/ retornar os dados
3. Adicionar camada core, com entidades, input/ ouput (caso necessário), validações de negócio, casos de uso e contrato para chamar a persistência/ busca dos dados
4. Adicionar camada infra, com acesso a dados, implementação dos contratos da camada core, para persistência
