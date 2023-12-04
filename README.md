# O Faxineiro Implacável

Neste projeto, trabalhamos na normalização e reestruturação de uma base de dados de uma biblioteca fictícia. O objetivo foi corrigir erros na estrutura inicial, separar informações de autores e editoras em tabelas distintas e criar relacionamentos entre elas e a tabela de livros.

## Problema inicial

O script inicial continha alguns erros que impediam a renderização completa da base de dados. As correções necessárias foram:

1. Correção de erros no esquema da tabela `Livros`.
2. Criação de tabelas separadas para `Autores` e `Editoras`.
3. Utilização de chaves estrangeiras para referenciar autores e editoras na tabela `Livros`.

## Passos realizados

### 1. Correções na tabela `Livros`
- Adição da regra `AUTO_INCREMENT` para a chave primária `livros_id`.
- Remoção dos dados referentes ao ID dos livros do script de inserção.

### 2. Criação das tabelas `Autores` e `Editoras`
- Criadas tabelas separadas para armazenar informações sobre autores e editoras.
- Inserção dos dados de autores e editoras nessas novas tabelas.

### 3. Utilização de chaves estrangeiras
- Utilização de `ALTER TABLE` para remover as colunas 'autor' e 'editora' da tabela `Livros`.
- Adição das colunas 'autor_id' e 'editora_id' como chaves estrangeiras referenciando as novas tabelas.

### 4. Reestruturação do script de inserção de dados
- Correção do script de inserção para incluir as chaves estrangeiras `autor_id` e `editora_id`.

## Script Final
O script finalizado pode ser encontrado na pasta

## Como executar

Para executar este projeto localmente, siga estes passos:

1. Clone este repositório: `git clone https://github.com/seu-usuario/nome-do-repositorio.git`
2. Execute o script SQL em seu banco de dados.
3. Verifique a estrutura da base de dados e os dados inseridos.

Sinta-se à vontade para contribuir, abrir issues ou sugerir melhorias!

**Observação:** Este projeto foi realizado como parte de uma atividade no PROA. As informações e dados utilizados são fictícios e foram criados apenas para fins educacionais.
