## Diagrama de Classes Biblioteca Virtual

##### Classes:

##### Atributos:

- Livro;
- Emprestimo;
- Categoria;

- Pessoa (classe pai):
- Usuário;
- Bibliotecária;

###### Livros:

lista de atributos: codigoLivro (int), titulo(string) e autor (string) ---------> categoria é uma relação de classe, precisa ver qual se encaixa: eu achei esse site aqui : https://www.edrawsoft.com/pt/article/class-diagram-relationships.html?gclid=Cj0KCQjwyLGjBhDKARIsAFRNgW_p0--EZLX2I5UP2YVuDQ-EmQkxeTsKtmClmHBrhnSjhibOBI-pWzkaAijHEALw_wcB#:~:text=Relacionamento%20Entre%20Classes


###### Emprestimo:

lista de atributos: codigoLivro(int), titulo(string), autor (string), status (string) e nome (string);

###### Categoria:

lista de atributos: codigoCategoria (int), tipo (string)

#### Usuário (classe pai):

###### Leitor:

lista de atributos:  RA(long), nome (string), email (String).

###### Biblitecaria:
lista de atributos: nome (string) CPF (String), email (String 


##### Operações:

###### Livro:

lista de operações: getCodigoLivro(): int, getTitulo(): string, getAutor(): string, getCategoria()
###### Usuarios:

lista de operações: getRA(): long, getNome():string

###### Emprestimo:

lista de operações: getCodigoLivro(): int, getTitulo():string, getAutor():string, getStatus():string, getNome():string, setStatus():string

###### Categoria:

lista de operações: getCodigoCategoria(): int, getTipo():string 

(faltam a de usuário) acho que é algo do tipo: getId(): long

getNome(): string




-----------------------

BibliotecaVirtual

---------------------------------

livro: Lista<Livros>

usuario: Lista<Usuarios>

emprestimo: Lista <Emprestimo>

categoria: Lista <Categoria>

--------------------------------

criarLivro(livro: Livro): void

removerLivro(livro: Livro): void

alterarLivro(livro: Livro): void

criarUsuario(usuario: Usuario): void

removerUsuario(usuario: Usuario): void

adicionarHistorico(historico: Historico): void

criarCategoria(categoria: CategoriaLivro): void
  
alterarCategoria(categoria: CategoriaLivro): void

-------



---------------------

Livro                

---------------------

codigoLivro: int

titulo: string   

autor: string  

categoria: categoria      - precisa ver como a gente relaciona essa com outra classe 

---------------------

getCodigo(): int

getTitulo(): string

getAutor(): string

getCategoria(): int
  
setCodigo(): int

setTitulo(): string

setAutor(): string

setCategoria(): int

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

getCodigo(): int

getNome(): string
  
setCodigo(): int

setNome(): int
  
---------------------






