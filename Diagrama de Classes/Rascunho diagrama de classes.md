## Diagrama de Classes Biblioteca Virtual

##### Classes:

##### Atributos:

- Livros;

- Usuários;

- Historico (Emprestimos);

- Categorias.

###### Livros:

lista de atributos: codigoLivro (int), titulo(string), autor (string) e categoria (string). 

###### Usuarios:

lista de atributos:  RA(long) e nome (string).

###### Historico:

lista de atributos: codigoLivro(int), titulo(string), autor (string), status (string) e nome (string);

###### Categorias:

lista de atributos: codigoCategoria (int), tipo (string)





##### Operações:

###### Livros:

lista de operações: getCodigoLivro(): int, getTitulo(): string, getAutor(): string, getCategoria() 

###### Usuarios:

lista de operações: getRA(): long, getNome():string

###### Historico:

lista de operações: getCodigoLivro(): int, getTitulo():string, getAutor():string, getStatus():string, getNome():string, setStatus():string

###### Categoria:

lista de operações: getCodigoCategoria(): int, getTipo():string





-----------------------

BibliotecaVirtual

---------------------------------

livros: Lista<Livros>

usuarios: Lista<Usuarios>

historico: Lista <Historico>

categorias: Lista <Categoria>

--------------------------------

adicionarLivro(livro: Livro): void

removerLivro(livro: Livro): void

adicionarUsuario(usuario: Usuario): void

removerUsuario(usuario: Usuario): void

adicionarHistorico(historico: Historico): void

adicionarCategoria(categoria: CategoriaLivro): void

-------



---------------------

Livro                

---------------------

codigoLivro: int

titulo: string   

autor: string  

genero: string       

---------------------

getCod(): int

getTitulo(): string

getAutor(): string

getGenero(): int

---------------------



--------------------- 

Usuario

---------------------

RA: long

nome: string

---------------------

getId(): long

getNome(): string
  
alugaLivro()

devolveLivro()

---------------------



---------------------

 Historico            

---------------------

codigoLivro: int

titulo: string  

autor: string

status: string

nome: string  

---------------------

getCod(): int

getTitulo(): string

getAutor(): string

getStatus(): string

setStatus():string

getNome():string
  
VerificaStatus():bool

---------------------



---------------------

Categoria

---------------------

codigoCategoria: int

tipo: string

---------------------

getCodigoCategoria(): int

getNome(): string
 
---------------------






