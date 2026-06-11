# sistema-controle-de-biblioteca
# ControleBiblioteca

## Descrição

O projeto **ControleBiblioteca** é uma aplicação simples de console desenvolvida em **C#** utilizando os conceitos de **Programação Orientada a Objetos (POO)**.

O sistema tem como objetivo auxiliar no controle de uma biblioteca, permitindo cadastrar livros e alunos, visualizar informações cadastradas e simular o empréstimo de livros.

---

## Objetivo do Projeto

Criar um sistema que represente uma biblioteca utilizando:

- Classes
- Objetos
- Atributos
- Métodos
- Construtores
- Listas para armazenamento de dados

---

## Tecnologias Utilizadas

- C#
- .NET Console Application
- Programação Orientada a Objetos

---

## Funcionalidades

O sistema permite:

- Cadastrar livros
- Cadastrar alunos
- Exibir informações dos livros
- Exibir informações dos alunos
- Controlar disponibilidade dos livros
- Realizar empréstimo de livros
- Listar todos os livros cadastrados

---

## Estrutura do Projeto

```
ControleBiblioteca
│
├── Program.cs
│
├── Classe Livro
│   ├── Titulo
│   ├── Autor
│   ├── AnoPublicacao
│   ├── Disponivel
│   ├── ExibirDetalhes()
│   └── Emprestar()
│
└── Classe Aluno
    ├── Nome
    ├── Matricula
    ├── Turma
    └── ExibirDados()
```

---

## Classes do Sistema

### Livro

Representa os livros da biblioteca.

Possui os atributos:

- **Titulo** → Nome do livro
- **Autor** → Autor da obra
- **AnoPublicacao** → Ano em que foi publicado
- **Disponivel** → Controla se está disponível ou emprestado


Métodos:

`ExibirDetalhes()`

Exibe as informações do livro no console.


`Emprestar()`

Altera a situação do livro de disponível para emprestado.

---

### Aluno

Representa os alunos que utilizam a biblioteca.

Possui os atributos:

- **Nome**
- **Matricula**
- **Turma**


Método:

`ExibirDados()`

Mostra os dados do aluno cadastrado.

---

## Construtores

O projeto utiliza dois tipos de construtores:

### Construtor padrão

Cria um objeto vazio que pode receber valores posteriormente.

Exemplo:

```csharp
Livro livro = new Livro();
```

---

### Construtor com parâmetros

Cria um objeto já preenchido com informações.

Exemplo:

```csharp
Livro livro = new Livro(
"Dom Casmurro",
"Machado de Assis",
1899
);
```

---

## Exemplo de Funcionamento

Saída esperada no console:

```
LISTA DE LIVROS CADASTRADOS

Título: Dom Casmurro | Autor: Machado de Assis | Ano: 1899 | Situação: Disponível

Título: O Pequeno Príncipe | Autor: Antoine de Saint-Exupéry | Ano: 1943 | Situação: Emprestado

Título: Harry Potter e a Pedra Filosofal | Autor: J.K. Rowling | Ano: 1997 | Situação: Disponível


ALUNOS CADASTRADOS

Nome: Ana Souza | Matrícula: 2026001 | Turma: Informática

Nome: Carlos Oliveira | Matrícula: 2026002 | Turma: Informática


ALUNO RESPONSÁVEL PELO EMPRÉSTIMO

Nome: Ana Souza | Matrícula: 2026001 | Turma: Informática
```

---

## Como Executar

### 1. Clone o projeto

```bash
git clone https://github.com/seuusuario/ControleBiblioteca.git
```

### 2. Entre na pasta

```bash
cd ControleBiblioteca
```

### 3. Execute o projeto

```bash
dotnet run
```

---

## Conceitos de Programação Utilizados

- Encapsulamento através de propriedades
- Criação de classes
- Instanciação de objetos
- Métodos
- Sobrecarga de construtores
- Coleções (`List<T>`)
- Estruturas condicionais

---

## Autor

Desenvolvido como atividade acadêmica de Programação Orientada a Objetos em C#.
