## Diagrama de Classes Biblioteca Virtual

##### Classes:

##### Atributos:

- Livros;

- Usuários;

- Historico (Emprestimos);

- Categorias.

###### Livros:

lista de atributos: codigoLivro (int), titulo(string) e autor (string) ---------> categoria é uma relação de classe, precisa ver qual se encaixa: eu achei esse site aqui : https://www.edrawsoft.com/pt/article/class-diagram-relationships.html?gclid=Cj0KCQjwyLGjBhDKARIsAFRNgW_p0--EZLX2I5UP2YVuDQ-EmQkxeTsKtmClmHBrhnSjhibOBI-pWzkaAijHEALw_wcB#:~:text=Relacionamento%20Entre%20Classes

###### Usuarios:

lista de atributos:  RA(long) e nome (string).

###### Historico/Emprestimo:

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

(faltam a de usuário) acho que é algo do tipo: getId(): long

getNome(): string




-----------------------

BibliotecaVirtual

---------------------------------

livros: Lista<Livros>

usuarios: Lista<Usuarios>

emprestimo: Lista <Emprestimo>

categorias: Lista <Categoria>

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

genero: string     (eu acho que não tem esse dai, por ser relação) - caso for referencia da tabela relacional seria (int cod_livro, int cod_categoria) 

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

getCodigo(): int

getNome(): string
  
setCodigo(): int

setNome(): int
  
---------------------






