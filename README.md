# Administrando dados de empréstimos de uma biblioteca

## Levantameno de requisitos
### O QUE O SISTEMA PRECISA FAZER  
* Mínimo 
    - CRUD de leitores cadastrados (precisa ter um registro no sistema para pegar um livro emprestado);
    - Administrar empréstimos com datas de saída, data limite e data de retorno para maior controle sobre atrasos;
    
* Opicional 
    - Login de funcionários da biblioteca

### Entidades:
- **Leitor:** é necessário um cadastro de leitores para ter controle sobre coisas como: quantos livros a pessoa já pegou emprestado, se costuma devolver livros com atraso, etc
- **Empréstimo:** útil para armazenar dados como as informações do livro, do leitor, datas e status do empréstimo
- **Livro:** armazena informações importantes como se o livro está disponível, isbn, gênero, título, etc
    - Aqui levamos em conta que cada livro é único, mesmo que ele tenha cópias identicas em questão de ISBN, pois cada livro terá um código único, e não trabalharamos com um sistema que se pareca com "estoque"
- **Funcionário:** informações para melhor controle sobre os empréstimos, deixando claro qual funcionário fez cada empréstimo, além de informações como número de celular, cpf e turno