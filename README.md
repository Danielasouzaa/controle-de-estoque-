# Sistema de Controle de Estoque

## Descrição

O Sistema de Controle de Estoque é um projeto para gerenciar produtos, fornecedores e pedidos de reposição. O sistema permite armazenar e consultar informações sobre produtos e fornecedores, além de gerenciar pedidos de reposição para manter o estoque atualizado.

## Estrutura do Banco de Dados

O banco de dados é composto pelas seguintes tabelas:

- **Fornecedores**: Armazena informações sobre os fornecedores.
  - `id_fornecedor`: Identificador único do fornecedor (chave primária).
  - `nome_fornecedor`: Nome do fornecedor.
  - `telefone`: Telefone do fornecedor.
  - `email`: E-mail do fornecedor.

- **Produtos**: Armazena informações sobre os produtos.
  - `id_produto`: Identificador único do produto (chave primária).
  - `nome_produto`: Nome do produto.
  - `descricao`: Descrição do produto.
  - `preco`: Preço do produto.
  - `quantidade_estoque`: Quantidade disponível em estoque.
  - `id_fornecedor`: Identificador do fornecedor (chave estrangeira referenciando `Fornecedores`).

- **PedidosReposicao**: Armazena informações sobre os pedidos de reposição.
  - `id_pedido`: Identificador único do pedido (chave primária).
  - `id_produto`: Identificador do produto (chave estrangeira referenciando `Produtos`).
  - `quantidade_pedida`: Quantidade solicitada no pedido.
  - `data_pedido`: Data do pedido.

## Instruções de Uso

1. **Criação do Banco de Dados**:
   Execute o script SQL fornecido para criar o banco de dados e as tabelas necessárias.

2. **Inserção de Dados**:
   O script SQL inclui instruções para inserir dados iniciais nas tabelas `Fornecedores`, `Produtos`, e `PedidosReposicao`.

3. **Consultas**:
   O script SQL inclui um exemplo de consulta para listar os produtos com suas informações e o nome do fornecedor.

4. **Atualizações e Exclusões**:
   O script SQL inclui exemplos de como atualizar a quantidade em estoque e como excluir um pedido de reposição.

## Como Contribuir

Se desejar contribuir para este projeto, por favor siga estas etapas:

1. Faça um fork deste repositório.
2. Crie uma nova branch para suas modificações.
3. Realize suas alterações e faça commit.
4. Envie um pull request com uma descrição detalhada das suas alterações.

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## Contato

Para mais informações, entre em contato com [seu-email@email.com](mailto:seu-email@email.com).
