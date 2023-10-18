# Dominando o SQLite: Um Guia Prático

Bem-vindo à exploração do poderoso SQLite, uma ferramenta essencial para desenvolvedores. Prepare-se para uma jornada de descoberta com exemplos de consultas à medida que você aprimora suas habilidades.

## Ferramentas e Ambientes

### Escolhendo a Ferramenta Certa

Comece com o [DB Browser for SQLite](https://sqlitebrowser.org/), uma ferramenta confiável. Instale e configure para um início tranquilo.

## Dominando Comandos SQL

A magia começa com comandos SQL. Aprenda a usar:

- `SELECT`: Consulte seus dados.
  Exemplo: `SELECT nome, idade FROM clientes;`

- `INSERT`: Adicione novos registros.
  Exemplo: `INSERT INTO clientes (nome, idade) VALUES ('Maria', 30);`

- `UPDATE`: Atualize registros existentes.
  Exemplo: `UPDATE clientes SET idade = 31 WHERE nome = 'Maria';`

- `DELETE`: Exclua o que não precisa.
  Exemplo: `DELETE FROM clientes WHERE idade > 60;`

- `CREATE TABLE`: Crie tabelas personalizadas.
  Exemplo: `CREATE TABLE pedidos (id INT, total DECIMAL);`

- `ALTER TABLE`: Modifique a estrutura de tabelas.
  Exemplo: `ALTER TABLE pedidos ADD COLUMN data_pedido DATE;`

## Criando e Povoando o Banco de Dados

Aventure-se na criação do seu mundo de dados:

1. Crie um banco de dados:
   Exemplo: `CREATE DATABASE meubanco;`

2. Crie tabelas e defina sua estrutura.
   Exemplo: `CREATE TABLE produtos (id INT, nome TEXT, preço DECIMAL);`

## Consultando e Modelando

Use consultas para revelar segredos e moldar dados:

- Consulta Simples:
  Exemplo: `SELECT nome, preço FROM produtos;`

- Filtragem com `WHERE`:
  Exemplo: `SELECT nome FROM produtos WHERE preço > 50;`

## Atualizando e Excluindo

Revitalize seus dados e elimine o que não é mais necessário:

- Atualização:
  Exemplo: `UPDATE produtos SET preço = 60 WHERE nome = 'Celular';`

- Exclusão:
  Exemplo: `DELETE FROM produtos WHERE nome = 'Tablet';`

## Níveis Avançados

### Chaves de Relacionamento

Aprofunde-se nas relações de dados:

- Chaves Primárias:
  Exemplo: `CREATE TABLE pedidos (id INT PRIMARY KEY, total DECIMAL);`

- Chaves Estrangeiras:
  Exemplo: `CREATE TABLE itens_pedido (pedido_id INT, produto_id INT, quantidade INT, FOREIGN KEY (pedido_id) REFERENCES pedidos(id), FOREIGN KEY (produto_id) REFERENCES produtos(id));`

### Transações e Integridade

Mantenha a integridade dos dados com transações:

Exemplo:

```sql
BEGIN TRANSACTION;
UPDATE produtos SET estoque = estoque - 5 WHERE nome = 'Notebook';
INSERT INTO histórico (produto_id, quantidade) VALUES (2, -5);
COMMIT;

## Exportação e Importação de Dados

Saiba como exportar um banco de dados SQLite para backup e importá-lo novamente. Instruções para exportar dados em diferentes formatos, como CSV, também serão fornecidas.

## Boas Práticas e Otimização

Sugestões de boas práticas ao trabalhar com bancos de dados SQLite, incluindo o uso de índices e otimização.

# Conclusão

Este tutorial oferece uma visão abrangente do uso do SQLite no desenvolvimento de aplicativos. Esperamos que você se sinta encorajado a praticar e explorar mais o SQLite em seus projetos, aproveitando ao máximo sua versatilidade e eficiência.

Fique à vontade para entrar em contato se tiver alguma dúvida ou quiser discutir mais sobre o SQLite e seu uso. Feliz desenvolvimento!
```

## Colaboradores

- [@Marco Antonio](https://github.com/marco0antonio0)
- [@Diosne Marlon](https://github.com/DiosneMarlon)
- [@Vinicius de Souza](https://github.com/vinivini204)
- [@Pedro Gabriel](https://github.com/Pedro-Gabriel-Souza)
