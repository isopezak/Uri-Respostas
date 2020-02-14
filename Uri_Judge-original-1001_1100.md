# Uri Judge → todas as minhas respostas



## Introdução

Nesta obra vou apresentar todas as minhas respostas efetuadas no site Uri_Judge, uma plataforma *‘on-line’* que contém exercícios de programação. Como gosto de todas as linguagens existentes (algumas ainda estou estudando e/ou pretendo estudar melhor “puro *hobby*!“), farei a resolução e indicarei em qual estão executadas. Minha pretensão é apenas treinar meus conhecimentos e usar os exercícios para tirar minhas dúvidas quanto a maneira de executá-los.

Não tenho nenhuma linguagem preferida, gosto de todas, mas as que mais me aproximo no momento de escolher uma para treinar os códigos são: Python 3, Ruby e Lua. Essas linguagens são muito fáceis de aprender e requerem poucas linhas de código para serem executadas. 

Em primeiro lugar apresento a linguagem como algoritmo, com solicitação de dados e tudo, depois sim vem as respostas do uri. Lembrando que todas elas, menos os algoritmos em Portugol e Visualg foram aceitas pela plataforma como corretas.

#### Observação: 

Linguagens em que programo (pelo menos o básico!):

-   Algoritmo Portugol → não vale como linguagem, mas foi um excelente aprendizado.

-   Algoritmo Visualg → não vale como linguagem, mas foi um excelente aprendizado.

-   Python 3;

-   C;

-   C++;

-   C#;

-   Ruby;

-   Pascal → a primeira;

-   Javascript;

-   Lua;

-   Haskell

    Quando o teste for respondido em todas as linguagens acima ele terá um sinal de visto ✔ e quando for respondido também em Haskell haverá um “λ” (lambda) em frente ao visto.
    
    Obs.: Somente para a elaboração dos Algoritmos eu vou pedir explicitamente os valores, fugindo dos princípios dos exercícios para eu melhor compreender o enunciado.
    
    

# `I` URI Online Judge | 1001 ✔ **λ** **#**

## Extremamente Básico

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 2 valores inteiros e armazene-os nas variáveis **A** e **B**. Efetue a soma de **A** e **B** atribuindo o seu resultado na variável **X**. Imprima **X** conforme exemplo apresentado abaixo. Não apresente mensagem alguma além daquilo que está sendo especificado e não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "*Presentation Error*".

### Entrada

A entrada contém 2 valores inteiros.

### Saída

Imprima a mensagem "X = " (letra X maiúscula) seguido pelo valor da variável **X** e pelo final de linha. Cuide para que tenha um espaço antes e depois do sinal de igualdade, conforme o exemplo abaixo.

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 10 <br>9            | X = 19            |
| -10 <br>4           | X = -6            |
| 15<br> -7           | X = 8             |

### Algoritmo em Portugol

```pascal
programa
// Programa em portugol uri_1001 → Extremamente Básico
{
	inteiro n1, n2, soma
	funcao inicio()	     
	{
		escreva("--------Soma dois números---------\n")
		escreva("Por favor digite um número: ")
		leia(n1)
		escreva("Digite outro número: ")
		leia(n2)
		soma = n1 + n2
		escreva("X = " + soma)
		escreva("\n----------------------------------")
	}
}
```

### Algoritmo em Visualg

```pascal
Algoritmo "uri_1001"
// Descrição   : Extremamente Básico
// Autor(a)    : Itamar
// Data atual  : 03/07/2019
Var
// Seção de Declarações das variáveis 
n1, n2: inteiro
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
Escreva("Digite um número: ")
leia(n1)
Escreva("Digite outro número: ")
leia(n2)
Escreva("X = ", n1 + n2)
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# uri_1001 → Python 3
A = int(input())
B = int(input())
X = int(A + B)
print('X = {}'.format(X))

```

Em Python devemos deixar uma linha em branco no final para indicar o final do programa.

### C

```c
#include <stdio.h>
/* uri_1001 → C - Puro */
int main() { 
    int A, B, X;
    scanf("%d", &A);
    scanf("%d", &B);
    X=A+B;
    printf("X = %d\n", X);
    return 0;
}
```

### C++

```c++
#include <iostream>
/* uri_1001 → C++ */
using namespace std; 
int main() { 
    int a, b, X;
    cin >> a >> b;
    X = a + b;
    cout << "X = " << X << endl; 
    return 0;
}
```

### C#

```c#
using System; 
/* uri_1001 → C# */
class URI {

    static void Main(string[] args) { 

          int n1, n2, resultado;
            Console.Write("");
            n1 = int.Parse(Console.ReadLine());

            Console.Write("");
            n2 = int.Parse(Console.ReadLine());

            resultado = n1 + n2;

            Console.WriteLine("X = " + resultado);

    }

}
```

### Ruby

```ruby
# uri_1001 → Ruby
A = gets.to_i
B = gets.to_i
X = A+B
puts "X = #{X}"
```

### Pascal

```pascal
// uri_1001 → Pascal (A primeira linguagem que aprendi)
program uri_1001;
var
  x, y, soma: integer;
begin
  readln(x);
  readln(y);
  soma := x+y;
  writeln('X = ', soma);
  readln();
end.            
```

### Javascript → usando Nodejs

```javascript
// uri_1001 → javascript
// inicio trecho código uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var x = Number(lines.shift());
var y = Number(lines.shift());
console.log('X = ' + (x + y));
```

Os códigos em javascript são mais difíceis de testar, pois temos que, se quisermos dar *input* de valores, mudar a linha que pede os dados para o usuário da seguinte maneira (dependente de caso):

Para o exercício acima e abrindo no navegador ficaria:

☻ em vez de → var x = Number(lines.shift());

☻ ficaria → var x = Number(prompt());

então o código acima para rodar no navegador fica:

### Javascript → navegador Web

```javascript
var x = Number(prompt());
var y = Number(prompt());
alert('X = ' + (x + y));
```

Esta é uma das maneiras mais fáceis de se testar o código. Nesse caso foi testado no site: [https://jsfiddle.net](https://jsfiddle.net/)

Ou podemos usar o próprio navegador como na imagem abaixo:

Bastando dar "enter" quando acabar de escrever o código para ele rodar.

### Lua

```lua
--[[
uri_1001 → Lua
--]]
-- Minha primeira resposta em lua
X = tonumber(io.read())
Y = tonumber(io.read())
print('X = ' .. X + Y)
```

### Haskell

```haskell
-- uri_1001 → Haskell
main :: IO ()
main =
  do num1 <- getLine
     num2 <- getLine
     putStrLn ("X = " ++ show (soma num1 num2))
       where soma num1 num2 = (read num1 :: Int) + (read num2 :: Int)
```

### `II` URI Online Judge | 1002 ✔ **λ** **#**

## Área do Círculo

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

A fórmula para calcular a área de uma circunferência é: **area = π . raio2**. Considerando para este problema que **π  = 3.14159**:

\- Efetue o cálculo da área, elevando o valor de **raio** ao quadrado e multiplicando por **π**.

### Entrada

A entrada contém um valor de ponto flutuante (dupla precisão), no caso, a variável **raio**.

### Saída

Apresentar a mensagem "A=" seguido pelo valor da variável **area**, conforme exemplo abaixo, com 4 casas após o ponto decimal. Utilize variáveis de dupla precisão (double). Como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 2.00                | A=12.5664         |
| 100.64              | A=31819.3103      |
| 150.00              | A=70685.7750      |

### Algoritmo em Portugol

```pascal
programa
{
	funcao inicio()
	{
		real area, raio
		real pi = 3.14159
		escreva("Digite a medida do raio: ")
		leia(raio)
		escreva("A=", pi * (raio * raio))
	}
}
```

### Algoritmo em Visualg

```pascal
Algoritmo "uri_1002"
// Disciplina  :  [Algoritmo] 
// Descrição   : Área do circulo
// Autor(a)    : Itamar
// Data atual  : 04/07/2019
Var
// Seção de Declarações das variáveis 
raio: real
area: real
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
escreval("Digite a medida do raio: ")
leia(raio)
area <- pi * (raio * raio)
escreva("A=", area:8:4)   
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1002 - Área do Círculo
A = float(input())
area = 3.14159 * (A * A)
print('A={:.4f}'.format(area))

```

### C

```c
#include <stdio.h>
/* C → puro → uri_1002 - Área do Círculo */
int main()
{
    double raio, area;
    scanf("%lf", &raio);
    area = 3.14159 * raio * raio;
    printf("A=%.4lf\n", area);
    return 0;
}

```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    //C ++ → uri_1002 - Área do Círculo
    double raio, area;
    cout << fixed;
    cout.precision(4);
    cin >> raio;
    area = 3.14159 * raio * raio;
    cout << "A=" << area << endl; 
    return 0;
}
```

### C#

```c#
using System; 
//C# → uri_1002 - Área do Círculo
class URI {

    static void Main(string[] args) { 

        double raio, area;
        raio = double.Parse(Console.ReadLine());
        area = 3.14159 * (raio * raio);
        Console.WriteLine("A={0}", area.ToString("0.0000"));
    }
}
```

### Ruby

```ruby
# Ruby → uri_1002 - Área do Círculo
a = gets.to_f
area = 3.14159*(a*a)
puts "A=%.4f" % [area]
```

### Pascal

```pascal
// Pascal → uri_1002 - Área do Círculo
program uri_1002;
var
  raio, area: real;
begin
  readln(raio);
  area := 3.14159* raio * raio;
  writeln('A=', area:0:4);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1002 - Área do Círculo
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var raio = Number(lines.shift());
var area = 3.14159 * raio * raio;
console.log(`A=${area.toFixed(4)}`);
```

### Lua

```lua
--[[
Lua → uri_1002 - Área do Círculo
em lua temos que formatar a saída para termos o resultado esperado
em 'termos' de casas decimais, pois para o compilador todos os números
são reais
--]]
local raio = tonumber(io.read())
local area = 3.14159 * raio * raio
d = (string.format("%.4f", area))
print(string.format("A=".. d))
```

### Haskell

```haskell
-- Haskell → uri_1002 - Área do Círculo
module Main (main) where
import Text.Printf
main :: IO ()
main = do 
          r <- readLn :: IO Double
          let area = 3.14159 * (r^2)
          printf "A=%.4f\n" area
```



# `III` URI Online Judge | 1003 ✔ **λ** **#**

## Soma Simples

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia dois valores inteiros, no caso para variáveis A e B. A seguir, calcule a soma entre elas e atribua à variável **SOMA**. A seguir escrever o valor desta variável.

### Entrada

O arquivo de entrada contém 2 valores inteiros.

### Saída

Imprima a variável **SOMA** com todas as letras maiúsculas, com um espaço em branco antes e depois da igualdade seguido pelo valor correspondente à soma de A e B. Como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 30 <br>10           | SOMA = 40         |
| -30 <br>10          | SOMA = -20        |
| 0 <br>0             | SOMA = 0          |

### Algoritmo em Portugol

```pascal
programa
// Programa em portugol → uri_1003 → Soma Simples
{
	inteiro n1, n2, soma
	funcao inicio()	     
	{
		escreva("--------Soma dois números---------\n")
		escreva("Por favor digite um número: ")
		leia(n1)
		escreva("Digite outro número: ")
		leia(n2)
		soma = n1 + n2
		escreva("SOMA = " + soma)
		escreva("\n----------------------------------")
	}
}
```

### Algoritmo em Visualg

```pascal
Algoritmo "uri_1003"
// Descrição   : Soma simples
// Autor(a)    : Itamar
// Data atual  : 04/07/2019
Var
// Seção de Declarações das variáveis 
n1, n2: inteiro
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
Escreva("Digite um número: ")
leia(n1)
Escreva("Digite outro número: ")
leia(n2)
Escreva("SOMA = ", n1 + n2)
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1003 - Soma simples
A = int(input())
B = int(input())
SOMA = A + B
print('SOMA = {}'.format(SOMA))

```

### C

```c
#include <stdio.h>
 /* C → puro → uri_1003 - Soma simples */
int main() { 
    int A, B, SOMA;
    scanf("%d", &A);
    scanf("%d", &B);
    SOMA = A + B;
    printf("SOMA = %d\n", SOMA); 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1003 - Soma simples
using namespace std; 
int main() { 
 int A, B, SOMA;
    cin >> A;
    cin >> B;
    SOMA = A + B;
    cout << "SOMA = " << SOMA << endl;
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1003 - Soma simples
class URI {

    static void Main(string[] args) { 

        int n1, n2, resultado;            
        n1 = int.Parse(Console.ReadLine());                        
        n2 = int.Parse(Console.ReadLine());
        resultado = n1 + n2;
        Console.WriteLine($"SOMA = {resultado}");
    }
}
```

### Ruby

```ruby
# Ruby → uri_1003 - Soma simples
A = gets.to_i
B = gets.to_i
SOMA = A + B
puts "SOMA = #{SOMA}"
```

### Pascal

```pascal
// Pascal → uri_1003 - Soma simples
program uri_1003;
var
  a, b, soma: integer;
begin
  readln(a);
  readln(b);
  soma := a+b;
  writeln('SOMA = ', soma);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1003 - Soma simples
//inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
//fim trecho uri
var x = Number(lines.shift());
var y = Number(lines.shift());   
console.log('SOMA = ' + (x + y));
```

### Lua

```lua
-- Lua → uri_1003 - Soma simples
a = tonumber(io.read())
b = tonumber(io.read())
print('SOMA = ' .. a + b)
```

### Haskell

```haskell
-- Haskell → uri_1003 - Soma simples
main :: IO ()
main =
  do num1 <- getLine
     num2 <- getLine
     putStrLn ("SOMA = " ++ show (soma num1 num2))
       where soma num1 num2 = (read num1 :: Int) + (read num2 :: Int)
```

# `IV` URI Online Judge | 1004 ✔ **λ** **#**

## Produto Simples

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia dois valores inteiros. A seguir, calcule o produto entre estes dois valores e atribua esta operação à variável **PROD**. A seguir mostre a variável **PROD** com mensagem correspondente.   

### Entrada

O arquivo de entrada contém 2 valores inteiros.

### Saída

Imprima a variável **PROD** conforme exemplo abaixo, com um espaço em branco antes e depois da igualdade. Não esqueça de imprimir o fim de linha após o produto, caso contrário seu programa apresentará a mensagem: *“Presentation Error”*.

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 3 <br>9             | PROD = 27         |
| -30 <br>10          | PROD = -300       |
| 0 <br>9             | PROD = 0          |

### Algoritmo em Portugol

```pascal
programa
// Programa em portugol → uri_1004 - Produto simples
{
	inteiro n1, n2, soma
	funcao inicio()	     
	{
		escreva("--------Multiplica dois números---------\n")
		escreva("Por favor digite um número: ")
		leia(n1)
		escreva("Digite outro número: ")
		leia(n2)
		multiplica = n1 * n2
		escreva("PROD = " + multiplica)
		escreva("\n----------------------------------")
	}
}
```

### Algoritmo em Visualg 

```pascal
Algoritmo "uri_1004"
// Disciplina  :  [Algoritmo] 
// Descrição   : Produto simples
// Autor(a)    : Itamar
// Data atual  : 04/07/2019
Var
// Seção de Declarações das variáveis 
n1: inteiro
n2: inteiro
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
escreval("Digite um número: ")
leia(n1)
escreval("Digite outro número: ")
leia(n2)
escreva("PROD = ", n1 * n2)   
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1004 - Produto simples
A = int(input())
B = int(input())
PROD = int(A * B)
print('PROD = {}'.format(PROD))

```

### C

```c
#include <stdio.h>
 /* C - puro → uri_1004 - Produto simples */
int main() { 
    int a, b;
    scanf("%d", &a);
    scanf("%d", &b);
    printf("PROD = %d\n", a * b); 
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    /**
     * C++ → uri_1004 - Produto simples
     */
    int a, b;
    cin >> a;
    cin >> b;
    cout << "PROD = " << a * b << endl; 
    return 0;
}
```

### C#

```c#
using System; 
/* C# → uri_1004 - Produto simples */
class URI {

    static void Main(string[] args) { 

        int n1, n2, resultado;
        n1 = int.Parse(Console.ReadLine());
        n2 = int.Parse(Console.ReadLine());
        resultado = n1 * n2;
        Console.WriteLine($"PROD = {resultado}");
    }
}
```

### Ruby

```ruby
# Ruby → uri_1004 - Produto simples
A = gets.to_i
B = gets.to_i
PROD = A * B
puts "PROD = #{PROD}"
```

### Pascal

```pascal
// Pascal → uri_1004 - Produto simples
program uri_1003;
var
  a, b, mult: integer;
begin
  readln(a);
  readln(b);
  mult := a*b;
  writeln('PROD = ', mult);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1004 - Produto simples
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var x = Number(lines.shift());
var y = Number(lines.shift());   
console.log('PROD = ' + (x * y));
```

### Lua

```lua
--[[
Lua → uri_1004 - Produto simples
--]]
local a = tonumber(io.read())
local b = tonumber(io.read())
print("PROD = ".. a * b)
```

### Haskell

```haskell
-- Haskell → uri_1004 - Produto simples
module Main (main) where
main :: IO ()
main =
  do num1 <- getLine
     num2 <- getLine
     putStrLn ("PROD = " ++ show (produto num1 num2))
       where produto num1 num2 = (read num1 :: Int) * (read num2 :: Int)
```

# `V` URI Online Judge | 1005 ✔ **λ** **#**

## Média 1

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 2 valores de ponto flutuante de dupla precisão A e B, que correspondem a 2 notas de um aluno. A seguir, calcule a média do aluno, sabendo que a nota A tem peso 3.5 e a nota B tem peso 7.5 (A soma dos pesos portanto é 11). Assuma que cada nota pode ir de 0 até 10.0, sempre com uma casa decimal.

### Entrada

O arquivo de entrada contém 2 valores com uma casa decimal cada um.

### Saída

Calcule e imprima a variável **MEDIA** conforme exemplo abaixo, com 5 dígitos após o ponto decimal e com um espaço em branco antes e depois da igualdade. Utilize variáveis de dupla precisão (double) e como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 5.0 <br>7.1         | MEDIA = 6.43182   |
| 0.0 <br>7.1         | MEDIA = 4.84091   |
| 10.0 <br>10.0       | MEDIA = 10.00000  |

### Algoritmo em Portugol

```pascal
programa
{
	inclua biblioteca Matematica --> mat
	
	funcao inicio()
	{
		real nota1, nota2, media
		escreva("Digite a primeira nota: ")
		leia(nota1)
		escreva("Digite a segunda nota: ")
		leia(nota2)
		media = (nota1 * 3.5 + nota2 * 7.5) / 11
		escreva("MEDIA = " + mat.arredondar(media, 5))
	}
}
```

### Algoritmo em Visualg

```pascal
Algoritmo "uri_1005"
// Disciplina  :  [Algoritmo] 
// Descrição   : Média 1
// Autor(a)    : Szak
// Data atual  : 07/07/2019
Var
// Seção de Declarações das variáveis 
n1: real
n2: real
conta: real
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
escreva("Digite um número: ")
leia(n1)
escreva("Digite outro número: ")
leia(n2)
conta <- ((n1 * 3.5) + (n2 * 7.5)) / 11
escreva("MEDIA = ", conta:8:5)
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1005 - Média 1
A = float(input())
B = float(input())
MEDIA = (A * 3.5 + B * 7.5) /11
print('MEDIA = {:.5f}'.format(MEDIA))

```

### C

```c
#include <stdio.h>
 /* C - puro → uri_1005 - Média 1 */
int main() { 
    float A,B,MEDIA;
	scanf("%f", &A);
	scanf("%f", &B);
	MEDIA = (A * 3.5 + B * 7.5) /11;
	printf("MEDIA = %.5f\n", MEDIA);
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    /**
     * C++ → uri_1005 - Média 1
     */
    float A,B,MEDIA;
    cout << fixed;
    cout.precision(5);
	cin >> A;
	cin >>B;
	MEDIA = (A * 3.5 + B * 7.5) /11;
	cout << "MEDIA = " << MEDIA << endl; 
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1005 - Média 1

class URI {

    static void Main(string[] args) { 

        double n1, n2, Resultado;
        n1 = Convert.ToDouble(Console.ReadLine());
        n2 = Convert.ToDouble(Console.ReadLine());
        Resultado = (n1 * 3.5 + n2 * 7.5) / (3.5 + 7.5);
        Console.WriteLine("MEDIA = " + Resultado.ToString("0.00000"));
    }
}
```

### Ruby

```ruby
# Ruby → uri_1005 - Média 1
A = gets.to_f
B = gets.to_f
MEDIA = (A * 3.5 + B * 7.5) /11
puts "MEDIA = %.5f" % [MEDIA]
```

### Pascal

```pascal
// Pascal → uri_1005 - Média 1
program uri_1005;
var
  a, b, media: real;
begin
  readln(a);
  readln(b);
  media := (a*3.5 + b*7.5)/11;
  writeln('MEDIA = ', media:0:5);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1005 - Média 1
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var a = Number(lines.shift());
var b = Number(lines.shift());
MEDIA = (a * 3.5 + b * 7.5) / 11;
console.log(`MEDIA = ${MEDIA.toFixed(5)}`);
```

### Lua

```lua
--[[
Lua → uri_1005 - Média 1
--]]
local a = tonumber(io.read())
local b = tonumber(io.read())
M = ((a * 3.5) + (b * 7.5)) / 11
MEDIA = (string.format("%.5f", M))
print("MEDIA = " ..MEDIA)
```

### Haskell

```haskell
-- Haskell → uri_1005 - Média 1
module Main (main) where
import Text.Printf
main :: IO ()
main = do 
          a <- readLn :: IO Double
          b <- readLn :: IO Double
          let media = (a * 3.5 + b * 7.5) / 11
          printf "MEDIA = %.5f\n" media
```



# `VI`URI Online Judge | 1006 ✔ **λ** **#**

## Média 2

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 3 valores, no caso, variáveis A, B e C, que são as três notas de um aluno. A seguir, calcule a média do aluno, sabendo que a nota A tem peso 2, a nota B tem peso 3 e a nota C tem peso 5. Considere que cada nota pode ir de 0 até 10.0, sempre com uma casa decimal.

### Entrada

O arquivo de entrada contém 3 valores com uma casa decimal, de dupla precisão (double).

### Saída

Imprima a variável **MEDIA** conforme exemplo abaixo, com 1 dígito após o ponto decimal e com um espaço em branco antes e depois da igualdade. Assim como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

| Exemplos de Entrada   | Exemplos de Saída |
| --------------------- | ----------------- |
| 5.0 <br>6.0 <br>7.0   | MEDIA = 6.3       |
| 5.0 <br>10.0 <br>10.0 | MEDIA = 9.0       |
| 10.0 <br>10.0 <br>5.0 | MEDIA = 7.5       |

### Algoritmo em Portugol

```pascal
programa
{
	inclua biblioteca Matematica --> mat
	funcao inicio()
	{
		real nota1, nota2, nota3, media		
		escreva("Digite a primeira nota: ")
		leia(nota1)
		escreva("Digite a segunda nota: ")
		leia(nota2)
		escreva("Digite a terceira nota: ")
		leia(nota3)
		media = ((nota1 * 2) + (nota2 * 3) + (nota3 * 5)) / 10
		escreva("MEDIA = " + mat.arredondar(media, 1))
	}
}
```

### Algoritmo em Visualg

```pascal
Algoritmo "uri_1006"
// Disciplina  :  [Algoritmo] 
// Descrição   : Média 2
// Autor(a)    : Szak
// Data atual  : 07/07/2019
Var
// Seção de Declarações das variáveis 
n1: real
n2: real
n3: real
conta: real
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
escreva("Digite a primeira nota: ")
leia(n1)
escreva("Digite a segunda nota: ")
leia(n2)
escreva("Digite a terceira nota: ")
leia(n3)
conta <- ((n1 * 2) + (n2 * 3) + (n3 * 5)) / 10
escreva("MEDIA = ", conta:4:1)
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1006 Média 2
A = float(input())
B = float(input())
C = float(input())
MEDIA = ((A * 2) + (B * 3) + (C * 5)) / 10
print('MEDIA = {:.1f}'.format(MEDIA))

```

### C

```c
#include <stdio.h>
 /* C - puro → uri_1006 Média 2 */
int main() { 
    double A, B, C, MEDIA;
	scanf("%lf", &A);
	scanf("%lf", &B);
	scanf("%lf", &C);
	MEDIA = ((A * 2) + (B * 3) + (C * 5)) / 10;
	printf("MEDIA = %.1lf\n", MEDIA); 
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    /**
     * C++ → uri_1006 Média 2
     */
    double A, B, C, MEDIA;
    cout << fixed;
    cout.precision(1);
	cin >> A;
	cin >> B;
	cin >> C;
	MEDIA = ((A * 2) + (B * 3) + (C * 5)) / 10;
	cout << "MEDIA = " << MEDIA << endl; 
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1006 Média 2
class URI {

    static void Main(string[] args) { 

        double n1, n2, n3, conta;
        String contatexto;
            
        n1 = Convert.ToDouble(Console.ReadLine());
        n2 = Convert.ToDouble(Console.ReadLine());
        n3 = Convert.ToDouble(Console.ReadLine());
        conta = (n1 / 10 * 2) + (n2 / 10 * 3) + (n3 / 10 * 5);
        contatexto = Convert.ToString(conta.ToString("0.0"));
        Console.WriteLine("MEDIA = " + contatexto);
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1006 Média 2
A = gets.to_f
B = gets.to_f
C = gets.to_f
MEDIA = ((A * 2) + (B * 3) + (C * 5)) / 10
puts "MEDIA = %.1f" % [MEDIA]
```

### Pascal

```pascal
// Pascal → uri_1006 Média 2
program uri_1006;
var
  a, b, c, media: real;
begin
  readln(a);
  readln(b);
  readln(c);
  media := ((a*2) + (b*3) + (c*5)) / 10;
  writeln('MEDIA = ', media:0:1);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1006 Média 2
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var A = Number(lines.shift());
var B = Number(lines.shift());
var C = Number(lines.shift());
MEDIA = ((A * 2) + (B * 3) + (C * 5)) / 10;
console.log(`MEDIA = ${MEDIA.toFixed(1)}`);
```

### Lua

```lua
--[[
Lua → uri_1006 Média 2
--]]
A = tonumber(io.read())
B = tonumber(io.read())
C = tonumber(io.read())
M = ((A * 2) + (B * 3) + (C * 5)) / 10
MEDIA = (string.format("%.1f", M))
print("MEDIA = ".. MEDIA)
```

### Haskell

```haskell
--Haskell → uri_1006 Média 2
module Main (main) where
import Text.Printf
main :: IO ()
main = do 
          a <- readLn :: IO Double
          b <- readLn :: IO Double
          c <- readLn :: IO Double
          let media = ((a * 2) + (b * 3) + (c * 5)) / 10
          printf "MEDIA = %.1f\n" media
```



# `VII`URI Online Judge | 1007 ✔ **λ** **#**

## Diferença

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia quatro valores inteiros A, B, C e D. A seguir, calcule e mostre a diferença do produto de A e B pelo produto de C e D segundo a fórmula: DIFERENCA = (A * B - C * D).

### Entrada

O arquivo de entrada contém 4 valores inteiros.

### Saída

Imprima a mensagem **DIFERENCA** com todas as letras maiúsculas, conforme exemplo abaixo, com um espaço em branco antes e depois da igualdade.

| Exemplos de Entrada  | Exemplos de Saída |
| -------------------- | ----------------- |
| 5 <br>6 <br>7 <br>8  | DIFERENCA = -26   |
| 0 <br>0 <br>7 <br>8  | DIFERENCA = -56   |
| 5 <br>6 <br>-7 <br>8 | DIFERENCA = 86    |

### Portugol

```pascal
programa
{	
	funcao inicio()
	{
		inteiro a, b, c, d, diferenca
		escreva("Digite um valor inteiro: ")
		leia(a)
		escreva("Digite outro valor inteiro: ")
	     leia(b)
	     escreva("Digite outro valor inteiro: ")
	     leia(c)
	     escreva("Digite o último valor inteiro: ")
	     leia(d)
	     diferenca = (a * b) - (c * d)
	     escreva("DIFERENCA = " + diferenca) 
	}         
}
```

### Visualg

```pascal
Algoritmo "uri_1007"
// Disciplina  :  [Algoritmo]  
// Descrição   : Diferença
// Autor(a)    : Szak
// Data atual  : 10/07/2019
Var
// Seção de Declarações das variáveis 
     a: inteiro
     b: inteiro
     c: inteiro
     d: inteiro
     diferenca: inteiro
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
     escreva("Digite um número inteiro: ")
     leia(a)
     escreva("Digite outro valor inteiro: ")
	 leia(b)
	 escreva("Digite outro valor inteiro: ")
	 leia(c)
	 escreva("Digite o último valor inteiro: ")
	 leia(d)
	 diferenca <- (a * b) - (c * d)
	 escreva("DIFERENCA = ", diferenca)
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
'''
Python 3 → uri_1007 - Diferença
'''
a = int(input())
b = int(input())
c = int(input())
d = int(input())
DIFERENCA = int(a*b)-(c*d)
print('DIFERENCA = {}'.format(DIFERENCA))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1007 - Diferença
int main() { 
   int A, B, C, D, DIFERENCA;
	scanf("%d", &A);
	scanf("%d", &B);
	scanf("%d", &C);
	scanf("%d", &D);
	DIFERENCA = (A * B - C * D);
	printf("DIFERENCA = %d\n", DIFERENCA);
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    /**
     * C++ → uri_1007 - Diferença
     */
    int A, B, C, D, DIFERENCA;
	cin >> A;
	cin >> B;
	cin >> C;
	cin >> D;
	DIFERENCA = (A * B) - (C * D);
	cout << "DIFERENCA = " << DIFERENCA << endl;
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1007 - Diferença
class URI {

    static void Main(string[] args) { 

        int a, b, c, d, res;
        a = int.Parse(Console.ReadLine());
        b = int.Parse(Console.ReadLine());
        c = int.Parse(Console.ReadLine());
        d = int.Parse(Console.ReadLine());
        res = (a * b) - (c * d);
        Console.WriteLine("DIFERENCA = {0}", res);
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1007 - Diferença
a = gets.to_i
b = gets.to_i
c = gets.to_i
d = gets.to_i
DIFERENCA = (a*b)-(c*d)
puts "DIFERENCA = #{DIFERENCA}"
```

### Pascal

```pascal
// Pascal → uri_1007 - Diferença
program uri_1007;
var
  a, b, c, d, diferenca: integer;
begin
  readln(a);
  readln(b);
  readln(c);
  readln(d);
  diferenca := (a*b - c*d);
  writeln('DIFERENCA = ', diferenca);
  readln();
end.
```

### Javascript

```javascript
// Javascrit → uri_1007 - Diferença
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var A = Number(lines.shift());
var B = Number(lines.shift());
var C = Number(lines.shift());
var D = Number(lines.shift());
DIFERENCA = (A * B - C * D);
console.log(`DIFERENCA = ${DIFERENCA}`);
```

### Lua

```lua
-- Lua → uri_1007 - Diferença
local A = tonumber(io.read())
local B = tonumber(io.read())
local C = tonumber(io.read())
local D = tonumber(io.read())
DIFERENCA = (A * B - C * D)
print("DIFERENCA = "..DIFERENCA)
```

### Haskell

```haskell
-- Haskell → uri_1007 - Diferença
module Main (main) where
import Text.Printf
main :: IO ()
main = do 
          a <- readLn :: IO Int
          b <- readLn :: IO Int
          c <- readLn :: IO Int
          d <- readLn :: IO Int
          let dif = (a * b - c * d)
          printf "DIFERENCA = %d\n" dif
```

# `VIII` URI Online Judge | 1008 ✔ **λ** **#**

## Salário

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Escreva um programa que leia o número de um funcionário, seu número de horas trabalhadas, o valor que recebe por hora e calcula o salário desse funcionário. A seguir, mostre o número e o salário do funcionário, com duas casas decimais.

### Entrada

O arquivo de entrada contém 2 números inteiros e 1 número com duas casas decimais, representando o número, quantidade de horas trabalhadas e o valor que o funcionário recebe por hora trabalhada, respectivamente.

### Saída

Imprima o número e o salário do funcionário, conforme exemplo fornecido, com um espaço em branco antes e depois da igualdade. No caso do salário, também deve haver um espaço em branco após o $.

| Exemplos de Entrada | Exemplos de Saída              |
| ------------------- | ------------------------------ |
| 25 <br>100 <br>5.50 | NUMBER = 25 SALARY = U$ 550.00 |
| 1 <br>200 <br>20.50 | NUMBER = 1 SALARY = U$ 4100.00 |
| 6 <br>145 <br>15.55 | NUMBER = 6 SALARY = U$ 2254.75 |

### Portugol

```pascal
programa
{
	inclua biblioteca Matematica --> mat
	funcao inicio()
	{
		inteiro a, b
		real c, salario, arredondamento
		escreva("Digite o número do funcionário: ")
		leia(a)
		escreva("Digite as horas trabalhadas: ")
	     leia(b)
	     escreva("Digite o valor do salário hora: ")
	     leia(c)
	     salario = b * c
	     arredondamento = mat.arredondar(salario, 2)
	     escreva("NUMBER = " + a + "\n")
	     escreva("SALARY = U$ " + arredondamento) 
	}         
}
// O problema que surgiu neste exercício é que tem um bug no arredondamento, quando o
// número é arredondado como decimal inteiro (12.00) só fica com uma casa decimal (12.0).
```

### Visualg

```pascal
Algoritmo "uri_1008 - Salário"
// Disciplina  :  [Algoritmo]
// Descrição   : Salário
// Autor(a)    : Szak
// Data atual  : 11/07/2019
Var
// Seção de Declarações das variáveis 
    a, b: inteiro
    c, salario: real
Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 
    escreval("Digite o número do funcionário: ")
    leia(a)
	 escreval("Digite as horas trabalhadas: ")
	 leia(b)
	 escreval("Digite o valor do salário hora: ")
	 leia(c)
	 salario <- b * c
	 escreval("NUMBER = ", a)
	 escreva("SALARY = U$ ", salario:6:2)
Fimalgoritmo
```

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1008 - Salário
a = int(input())# número do funcionário
b = int(input())# horas trabalhadas
c = float(input())# Valor salário hora
SALARIO = b * c
print('NUMBER = {}'.format(a))
print('SALARY = U$ {:.2f}'.format(SALARIO))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1008 - Salário
int main() { 
  	int num, horas;
	float sal;
	scanf("%d", &num);
	scanf("%d", &horas);
	scanf("%f", &sal);
	printf("NUMBER = %d\n", num);
	printf("SALARY = U$ %.2f\n", horas*sal);
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() {
 // C++ → uri_1008 - Salário
 int num, horas;
	float sal;
	cin >> num;
	cin >> horas;
	cin  >> sal;
	cout << "NUMBER = "<< num << endl;
	cout << fixed;
	cout.precision(2);
	cout << "SALARY = U$ " << horas*sal << endl;
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1008 - Salário
class URI {

    static void Main(string[] args) { 

        int n1;
        double n2, n3, conta;
        String contatexto;

        n1 = int.Parse(Console.ReadLine());
        n2 = int.Parse(Console.ReadLine());
        n3 = Convert.ToDouble(Console.ReadLine());
        conta = n2 * n3;
        contatexto = Convert.ToString(conta.ToString("0.00"));
        Console.WriteLine("NUMBER = " + n1);
        Console.WriteLine("SALARY = U$ " + contatexto);
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1008 - Salário
a = gets.to_i
b = gets.to_i
c = gets.to_f
SALARIO = b * c
puts "NUMBER = #{a}"
puts "SALARY = U$ %.2f" % [SALARIO]
```

### Pascal

```pascal
// Pascal → uri_1008 - Salário
program uri_1008;
var
  num, horas: integer;
  sal, valor: real;
begin
  readln(num);
  readln(horas);
  readln(sal);
  valor := horas*sal;
  writeln('NUMBER = ', num);
  writeln('SALARY = U$ ', valor:0:2);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1008 - Salário
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var num = Number(lines.shift());
var horas = Number(lines.shift());
var sal = Number(lines.shift());
console.log(`NUMBER = ${num}`);
console.log(`SALARY = U$ ${(horas*sal).toFixed(2)}`);
```

### Lua

```lua
-- Lua → uri_1008 - Salário
local num = tonumber(io.read())
local horas = tonumber(io.read())
local sal = tonumber(io.read())
print("NUMBER = "..num)
salhor = horas*sal
present = (string.format("%.2f", salhor))
print("SALARY = U$ "..present)
```

### Haskel

```haskell
--Haskell → uri_1008 - Salário
module Main (main) where
import Text.Printf
main :: IO ()
main = do 
          a <- readLn :: IO Int
          b <- readLn :: IO Double
          c <- readLn :: IO Double
          let salario = (b * c)
          printf "NUMBER = %d\n" a
          printf "SALARY = U$ %.2f\n" salario
```

# `IX` URI Online Judge | 1009 ✔ **λ** **#**

## Salário com Bônus

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Faça um programa que leia o nome de um vendedor, o seu salário fixo e o total de vendas efetuadas por ele no mês (em dinheiro). Sabendo que este vendedor ganha 15% de comissão sobre suas vendas efetuadas, informar o total a receber no final do mês, com duas casas decimais.

### Entrada

O arquivo de entrada contém um texto (primeiro nome do vendedor) e 2 valores de dupla precisão (double) com duas casas decimais, representando o salário fixo do vendedor e montante total das vendas efetuadas por este vendedor, respectivamente.

### Saída

Imprima o total que o funcionário deverá receber, conforme exemplo fornecido.

| Exemplos de Entrada               | Exemplos de Saída  |
| --------------------------------- | ------------------ |
| JOAO <br>500.00 <br>1230.30       | TOTAL = R$ 684.54  |
| PEDRO <br>700.00 <br>0.00         | TOTAL = R$ 700.00  |
| MANGOJATA <br>1700.00 <br>1230.50 | TOTAL = R$ 1884.58 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1009 - Salário com Bônus
a = str(input())
b = float(input())
c = float(input())
p = (15 * c) / 100
total = b + p
print('TOTAL = R$ {:.2f}'.format(total))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1009 - Salário com Bônus
int main() { 
    char a[20];
    double b, c, p, total;
    scanf("%s", &a);
    scanf("%lf", &b);
    scanf("%lf", &c);
    p = (15 * c) / 100;
    total = b + p;
    printf("TOTAL = R$ %.2lf\n", total); 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1009 - Salário com Bônus
using namespace std; 
int main() {
    char a[20];
    double b, c, p, total;
    cin >> a;
    cin >> b;
    cin >> c;
    p = (15 * c) / 100;
    total = b + p;
    cout << fixed;
    cout.precision(2);
    cout << "TOTAL = R$ " << total << endl; 
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1009 - Salário com Bônus
class URI {

    static void Main(string[] args) { 

        String nome;
            double n2, n3, conta, salario;
            String contatexto;

            nome = Console.ReadLine();
            n2 = Double.Parse(Console.ReadLine());
            n3 = Double.Parse(Console.ReadLine());
            conta = n2 + ((n3 * 15) / 100);
            contatexto = Convert.ToString(conta.ToString("0.00"));
            Console.WriteLine("TOTAL = R$ " + contatexto);
            Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1009 - Salário com Bônus
a = gets.to_s
b = gets.to_f
c = gets.to_f
p = (15 * c) / 100
total = b + p
puts "TOTAL = R$ %.2f" % [total]
```

### Pascal

```pascal
// Pascal → uri_1009 - Salário com Bônus
program uri_1009;
var
  nome: char;
  b, c, p, total: double;
begin
  readln(nome);
  readln(b);
  readln(c);
  p := ((15*c)/100.00);
  total := b+p;
  writeln('TOTAL = R$ ', total:0:2);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1009 - Salário com Bônus
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var a = String(lines.shift());
var b = Number(lines.shift());
var c = Number(lines.shift());
p = (15 * c) / 100;
total = b + p;
console.log(`TOTAL = R$ ${total.toFixed(2)}`);
```

### Lua

```lua
-- Lua → uri_1009 - Salário com Bônus
local a = tostring(io.read())
local b = tonumber(io.read())
local c = tonumber(io.read())
p = (15 * c) / 100
t = b + p
total = (string.format("%.2f", t))
print("TOTAL = R$ "..total)
```

### Haskell

```haskell
-- Haskell → uri_1009 - Salário com Bônus
module Main (main) where
import Text.Printf
main :: IO ()
main = do           
          a <- getLine :: IO String
          b <- readLn :: IO Double
          c <- readLn :: IO Double
          let salario = (15.0 * c) / 100.0
          let conta = b + salario
          printf "TOTAL = R$ %.2f\n" conta
```

# `X` URI Online Judge | 1010 ✔ **λ** **#**

## Cálculo Simples

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Neste problema, deve-se ler o código de uma peça 1, o número de peças 1, o valor unitário de cada peça 1, o código de uma peça 2, o número de peças 2 e o valor unitário de cada peça 2. Após, calcule e mostre o valor a ser pago.

### Entrada

O arquivo de entrada contém duas linhas de dados. Em cada linha haverá 3 valores, respectivamente dois inteiros e um valor com 2 casas decimais.

### Saída

A saída deverá ser uma mensagem conforme o exemplo fornecido abaixo, lembrando de deixar um espaço após os dois pontos e um espaço após o "R$". O valor deverá ser apresentado com 2 casas após o ponto.

| Exemplos de Entrada       | Exemplos de Saída       |
| ------------------------- | ----------------------- |
| 12 1 5.30 <br>16 2 5.10   | VALOR A PAGAR: R$ 15.50 |
| 13 2 15.30 <br>161 4 5.20 | VALOR A PAGAR: R$ 51.40 |
| 1 1 15.10 <br>2 1 15.10   | VALOR A PAGAR: R$ 30.20 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1010 - Cálculo Simples
A = str(input()).split(" ")
num1 = [float(numero) for numero in A]
B = str(input()).split(" ")
num2 = [float(numero2) for numero2 in B]
a, b, c = num1
d, e, f = num2
TOTAL = (b*c)+(e*f)
print('VALOR A PAGAR: R$ {:.2f}'.format(TOTAL))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1010 - Cálculo Simples
int main() { 
   int a, b, c, d;
	float valor, soma, valor1;
	scanf("%d %d %f", &a, &b, &valor);
	scanf("%d %d %f", &c, &d, &valor1);	
	soma = (b * valor)+(d * valor1);
	printf("VALOR A PAGAR: R$ %.2f\n", soma); 
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    /**
     * C++ → uri_1010 - Cálculo Simples
     */
    int a, b, c, d;
	float valor, soma, valor1;
	cin >> a >> b >> valor;
	cin >> c >> d >> valor1;
	soma = (b * valor)+(d * valor1);
	cout << fixed;
	cout.precision(2);
	cout << "VALOR A PAGAR: R$ " << soma << endl;
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1010 - Cálculo Simples
class URI {

    static void Main(string[] args) { 

        string[] num1 = Console.ReadLine().Split();
        int cod1 = int.Parse(num1[0]);
        int quant1 = int.Parse(num1[1]);
        double preco1 = double.Parse(num1[2]);
        string[] num2 = Console.ReadLine().Split();
        int cod2 = int.Parse(num2[0]);
        int quant2 = int.Parse(num2[1]);
        double preco2 = double.Parse(num2[2]);
        double valor = (quant1 * preco1) + (quant2 * preco2);
        Console.WriteLine("VALOR A PAGAR: R$ " + String.Format("{0:0.00}", valor));
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1010 - Cálculo Simples
A = gets.split
num1 = A[1].to_i
num11 = A[2].to_f
B = gets.split
num2 = B[1].to_i
num22 = B[2].to_f
TOTAL = (num1 * num11) + (num2 * num22)
puts "VALOR A PAGAR: R$ %.2f" % [TOTAL]
```

### Pascal

```pascal
// Pascal → uri_1010 - Cálculo Simples
program uri_1010;
var
  a, b, c, d: integer;
  valor, soma, valor1: real;
begin
  readln(a, b, valor);
  readln(c, d, valor1);
  soma := (b * valor)+(d * valor1);
  writeln('VALOR A PAGAR: R$ ', soma:0:2);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1010 - Cálculo Simples
/* Este código também me fez perder grande tempo em pesquisa para responder como eu faria para capturar os dados em apenas uma linha*/
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var x = lines.shift().split(" ");
var y = lines.shift().split(" ");
var a1 = parseFloat(x[1]);
var a2 = parseFloat(x[2]);
var b1 = parseFloat(y[1]);
var b2 = parseFloat(y[2]);
// cod
soma = (a1 * a2) + (b1 * b2);
console.log(`VALOR A PAGAR: R$ ${(soma).toFixed(2)}`);
```

### Lua

```lua
-- Lua → uri_1010 - Cálculo Simples
a = {io.read('*number', '*number', '*number')}
b = {io.read('*number', '*number', '*number')}
s = (a[2]*a[3]) + (b[2]*b[3])
soma = (string.format("%.2f", s))
print("VALOR A PAGAR: R$ ".. soma)
```

### Haskell

```haskell
-- Haskell → uri_1010 - Cálculo Simples
import Text.Printf
calcula1 :: Double -> Double -> Double
calcula1 b c = (b * c)
calcula2 :: Double -> Double -> Double
calcula2 e f = (e * f)
main = do
   values <- getLine
   values2 <- getLine
   let list = words values
   let list2 = words values2
   let a = list !! 0
   let b = list !! 1
   let c = list !! 2
   let d = list2 !! 0
   let e = list2 !! 1
   let f = list2 !! 2 
   let total = (calcula1(read (b))(read(c))) + (calcula2(read(e))(read(f)))
   putStr "VALOR A PAGAR: R$ "
   printf "%.2f\n" $ total
```

# `XI`URI Online Judge | 1011 ✔ **λ** **#**

## Esfera

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Faça um programa que calcule e mostre o volume de uma esfera sendo fornecido o valor de seu raio (R). A fórmula para calcular o volume é: (4/3) * pi * R3. Considere (atribua) para pi o valor 3.14159.

Dica: Ao utilizar a fórmula, procure usar (4/3.0) ou (4.0/3), pois algumas linguagens (dentre elas o C++), assumem que o resultado da divisão entre dois inteiros é outro inteiro.

### Entrada

O arquivo de entrada contém um valor de ponto flutuante (dupla precisão), correspondente ao raio da esfera.

### Saída

A saída deverá ser uma mensagem "VOLUME" conforme o exemplo fornecido abaixo, com um espaço antes e um espaço depois da igualdade. O valor deverá ser apresentado com 3 casas após o ponto.

| Exemplos de Entrada | Exemplos de Saída        |
| ------------------- | ------------------------ |
| 3                   | VOLUME = 113.097         |
| 15                  | VOLUME = 14137.155       |
| 1523                | VOLUME = 14797486501.627 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1011 - Esfera
R = float(input())
VOLUME = (4/3) * 3.14159 * (R**3)
print('VOLUME = {:.3f}'.format(VOLUME))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1011 - Esfera
int main() { 
    int R;
	double VOL;
	scanf("%d", &R);
	VOL = (4.0/3) * 3.14159 * R * R * R;
	printf("VOLUME = %.3lf\n", VOL);
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1011 - Esfera
using namespace std; 
int main() {    
    int R;
	double VOL;
	cin >> R;
	VOL = (4.0/3) * 3.14159 * R * R * R;
	cout << fixed;
	cout.precision(3);
	cout <<"VOLUME = " << VOL << endl;
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1011 - Esfera
class URI {

    static void Main(string[] args) { 

        double n1, conta;
        n1 = float.Parse(Console.ReadLine());
        conta = (4 / 3.0) * 3.14159 * (n1 * n1 * n1);
        Console.WriteLine("VOLUME = " + String.Format("{0:0.000}", conta));
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1011 - Esfera
R = gets.to_f
VOLUME = (4/3.0) * 3.14159 * (R*R*R)
puts "VOLUME = %.3f" % [VOLUME]
```

### Pascal

```pascal
// Pascal → uri_1011 - Esfera
program uri_1011;
var
  raio: integer;
  volume: double;
begin
  readln(raio);
  volume := ((4.0/3) * 3.14159 * raio * raio * raio);
  writeln('VOLUME = ', volume:0:3);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1011 - Esfera
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri
var R =  Number(lines.shift());
var V = (4.0/3) * 3.14159 * R * R * R;
console.log(`VOLUME = ${V.toFixed(3)}`);
```

### Lua

```lua
-- Lua → uri_1011 - Esfera
R = io.read('*number')
V = (4.0/3) * 3.14159 * R * R * R
VOL = (string.format("%.3f", V))
print("VOLUME = ".. VOL)
```

### Haskell

```haskell
-- Haskell → uri_1011 - Esfera
import Text.Printf
calcula_volume :: Double -> Double
calcula_volume c = ((c^3) * (4 / 3) * 3.14159)
main = do
   c <- getLine
   let volume = (calcula_volume (read(c)))
   putStr "VOLUME = "
   printf "%.3f\n" volume
```

# `XII`URI Online Judge | 1012 ✔ **λ** **#**

## Área

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Escreva um programa que leia três valores com ponto flutuante de dupla precisão: A, B e C. Em seguida, calcule e mostre: 
a) a área do triângulo retângulo que tem A por base e C por altura. 
b) a área do círculo de raio C. (pi = 3.14159) 
c) a área do trapézio que tem A e B por bases e C por altura. 
d) a área do quadrado que tem lado B. 
e) a área do retângulo que tem lados A e B. 

### Entrada

O arquivo de entrada contém três valores com um dígito após o ponto decimal.

### Saída

O arquivo de saída deverá conter 5 linhas de dados. Cada linha corresponde a uma das áreas descritas acima, sempre com mensagem correspondente e um espaço entre os dois pontos e o valor. O valor calculado deve ser apresentado com 3 dígitos após o ponto decimal.

| Exemplos de entrada | Exemplos de saída                                            |
| ------------------- | ------------------------------------------------------------ |
| 3.0 4.0 5.2         | TRIANGULO: 7.800<br/>CIRCULO: 84.949<br/>TRAPEZIO: 18.200<br/>QUADRADO: 16.000<br/>RETANGULO: 12.000 |
| 12.7 10.4 15.2      | TRIANGULO: 96.520<br/>CIRCULO: 725.833<br/>TRAPEZIO: 175.560<br/>QUADRADO: 108.160<br/>RETANGULO: 132.080 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1012 - Área
X = str(input()).split(" ")
num = [float(numero) for numero in X]
A, B, C = num
print('TRIANGULO: {:.3f}'.format((A * C) / 2))
print('CIRCULO: {:.3f}'.format(3.14159 * C**2))
print('TRAPEZIO: {:.3f}'.format((A + B) * C / 2))
print('QUADRADO: {:.3f}'.format(B * B))
print('RETANGULO: {:.3f}'.format(A * B))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1012 - Área
int main() { 
  	float a, b, c;	
	scanf("%f%f%f", &a, &b, &c);	
	printf("TRIANGULO: %.3lf\n",(a*c)/2);
	printf("CIRCULO: %.3lf\n", 3.14159 * c * c);
	printf("TRAPEZIO: %.3lf\n",(a + b) * c / 2);
	printf("QUADRADO: %.3lf\n", b * b);
	printf("RETANGULO: %.3lf\n", a * b);
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1012 - Área
using namespace std; 
int main() { 
    float a, b, c;
	cout << fixed;
	cout.precision(3);
	cin >> a >> b >> c;
	cout << "TRIANGULO: " << (a*c)/2 << endl;
	cout << "CIRCULO: " << 3.14159 * c * c << endl;
	cout << "TRAPEZIO: " << (a + b) * c / 2 << endl;
	cout << "QUADRADO: " << b * b << endl;
	cout << "RETANGULO: " << a * b << endl; 
    return 0;
}
```

### C#

```c#
using System; 
// C# → uri_1012 - Área
class URI {

    static void Main(string[] args) { 

        double triangulo, circulo, trapezio, quadrado, retangulo;
        string[] num1 = Console.ReadLine().Split();
        double a = double.Parse(num1[0]);
        double b = double.Parse(num1[1]);
        double c = double.Parse(num1[2]);

        triangulo = (a * c) / 2;
        circulo = (3.14159 * c * c);
        trapezio = ((a + b) * c / 2);
        quadrado = b * b;
        retangulo = a * b;

        Console.WriteLine("TRIANGULO: " + String.Format("{0:0.000}", triangulo));
        Console.WriteLine("CIRCULO: " + String.Format("{0:0.000}", circulo));
        Console.WriteLine("TRAPEZIO: " + String.Format("{0:0.000}", trapezio));
        Console.WriteLine("QUADRADO: " + String.Format("{0:0.000}", quadrado));
        Console.WriteLine("RETANGULO: " + String.Format("{0:0.000}", retangulo));
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1012 - Área
X = gets.split
A = X[0].to_f
B = X[1].to_f
C = X[2].to_f
puts "TRIANGULO: %.3f" % [(A * C) / 2]
puts "CIRCULO: %.3f" % [3.14159 * (C*C)]
puts "TRAPEZIO: %.3f" % [(A + B) * (C / 2)]
puts "QUADRADO: %.3f" % [B * B]
puts "RETANGULO: %.3f" % [A * B]
```

### Pascal

```pascal
// Pascal → uri_1012 - Área
program uri_1012;
var
  a, b, c: real;
begin
  readln(a, b, c);
  writeln('TRIANGULO: ', ((a*c)/2):0:3);
  writeln('CIRCULO: ', (3.14159 * c * c):0:3);
  writeln('TRAPEZIO: ', ((a + b) * c / 2):0:3);
  writeln('QUADRADO: ', (b * b):0:3);
  writeln('RETANGULO: ', (a * b):0:3);
  readln();
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split(' ').map(x => Number(x));
/**
 * Javascript → uri_1012 - Área
 */
let [a, b, c] = lines.map(x => Number(x));
console.log(`TRIANGULO: ${((a*c)/2).toFixed(3)}`);
console.log(`CIRCULO: ${(3.14159 * c * c).toFixed(3)}`);
console.log(`TRAPEZIO: ${((a + b) * c / 2).toFixed(3)}`);
console.log(`QUADRADO: ${(b * b).toFixed(3)}`);
console.log(`RETANGULO: ${(a * b).toFixed(3)}`);
```

### Lua

```lua
--Lua → uri_1012 - Área
a = {io.read('*number', '*number', '*number')}
triangulo = (a[1] * a[3]) / 2
circulo = (3.14159 * a[3] * a[3])
trapezio = ((a[1] + a[2]) * a[3] / 2)
quadrado = a[2] * a[2]
retangulo = a[1] * a[2]
--soma = (string.format("%.2f", s))
print("TRIANGULO: "..(string.format("%.3f", triangulo)))
print("CIRCULO: "..(string.format("%.3f", circulo)))
print("TRAPEZIO: "..(string.format("%.3f", trapezio)))
print("QUADRADO: "..(string.format("%.3f", quadrado)))
print("RETANGULO: "..(string.format("%.3f", retangulo)))
```

### Haskell

```haskell
-- Haskell → uri_1012 - Área
import Text.Printf
conta_quadrado :: Double -> Double
conta_quadrado b = b * b

conta_retangulo :: Double -> Double -> Double
conta_retangulo a b = a * b

conta_triangulo :: Double -> Double -> Double
conta_triangulo a c = (a * c) / 2

conta_circulo :: Double -> Double
conta_circulo c = 3.14159 * c * c

conta_trapezio :: Double -> Double -> Double -> Double
conta_trapezio a b c = ( c * (a + b)) / 2

main = do
   valores <- getLine
   let lista = words valores
   let a = lista !! 0
   let b = lista !! 1
   let c = lista !! 2
   let area_triangulo = (conta_triangulo (read(a)) (read(c)))
   let area_circulo = (conta_circulo (read(c)))
   let area_trapezio = (conta_trapezio (read(a)) (read(b)) (read(c)))
   let area_quadrado = (conta_quadrado (read(b)))
   let area_retangulo = (conta_retangulo (read(a)) (read(b)))
   printf "TRIANGULO: %.3f\n" area_triangulo
   printf "CIRCULO: %.3f\n" area_circulo
   printf "TRAPEZIO: %.3f\n" area_trapezio
   printf "QUADRADO: %.3f\n" area_quadrado
   printf "RETANGULO: %.3f\n" area_retangulo
```

# `XIII`URI Online Judge | 1013 ✔ **λ** **#**

## O Maior

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

(A partir deste exercício começam a aparecer múltiplas entradas de dados em uma linha )

Timelimit: 1

Faça um programa que leia três valores e apresente o maior dos três valores lidos seguido da mensagem “eh o maior”. Utilize a fórmula:

![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1013.png)

Obs.: a fórmula apenas calcula o maior entre os dois primeiros (a e b). Um segundo passo, portanto é necessário para chegar no resultado esperado.

### Entrada

O arquivo de entrada contém três valores inteiros.

### Saída

Imprima o maior dos três valores seguido por um espaço e a mensagem "eh o maior".

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 7 14 106            | 106 eh o maior    |
| 217 14 6            | 217 eh o maior    |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1013 - O maior
X = str(input()).split(" ")
num = [int(numero) for numero in X]
A, B, C = num
if A > B and A > C:
    print('{} eh o maior'.format(A))
elif B > A and B > C:
    print('{} eh o maior'.format(B))
elif C > B and C > A:
    print('{} eh o maior'.format(C))

```

### C

```c
#include <stdio.h>
 // c - puro → uri_1013 - O maior
int main() { 
  	int a, b, c;	
	scanf("%d%d%d", &a, &b, &c);
	if (a>b && a>c)
		printf("%d eh o maior\n", a);
	if (b > a && b > c)
		printf("%d eh o maior\n", b);
	if (c > a && c > b)
		printf("%d eh o maior\n", c);
    return 0;
}
```

### C++

```c++
#include <iostream> 
using namespace std; 
int main() { 
    /**
     * C++ → uri_1013 - O maior
     */
     int a, b, c;
	cin >> a >> b >> c;
	if (a > b && a > c){
		cout << "" << a << " eh o maior" << endl;}
	if (b > a && b > c){
		cout << "" << b << " eh o maior" << endl;}
	if (c > a && c > b){
		cout << "" << c << " eh o maior" << endl;} 
    return 0;
}
```

### C#

```c#
using System;
// C# → uri_1013 - O maior
namespace uri1013
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] num1 = Console.ReadLine().Split();
            int a = Convert.ToInt32(num1[0]);
            int b = Convert.ToInt32(num1[1]);
            int c = Convert.ToInt32(num1[2]);
            if (a >= b)
            {
                if (a >= c)
                {
                    Console.WriteLine(a + " eh o maior");
                }
                else
                {
                    Console.WriteLine(c + " eh o maior");
                }
            }
            else if (b >= a)
            {
                if (b >= c)
                {
                    Console.WriteLine(b + " eh o maior");
                }
                else
                {
                    Console.WriteLine(c + " eh o maior");
                }
            }
            else
            {
                Console.WriteLine(c + " eh o maior");
            }
            Console.ReadKey();
        }        
    }    
}
```

### Ruby

```ruby
# Ruby → uri_1013 - O maior
X = gets.split
A = X[0].to_i
B = X[1].to_i
C = X[2].to_i
if A > B and A > C
    puts "#{A} eh o maior"
elsif B > A and B > C
    puts "#{B} eh o maior"
elsif C > B and C > A
    puts "#{C} eh o maior"
end
```

### Pascal

```pascal
// Pascal → uri_1013 - O maior
program uri_1013;
var
  a, b, c: integer;
begin
  readln(a, b, c);
  if (a > b) and (a > c) then
	writeln(a, ' eh o maior');
if (b > a) and (b > c) then
	writeln(b, ' eh o maior');
if (c > a) and (c > b) then
	writeln (c, ' eh o maior');
  readln();
end. 
```

### Javascript

```javascript
// Javascript → uri_1013 - O maior
// inicio código uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim código uri
var lines = input.split(' ').map(x => Number(x));
let [a,b,c] = lines.map(x => Number(x));
if ((a > b) && (a > c)) {
    console.log(`${a} eh o maior`);}
if ((b > a) && (b > c)) {
	console.log(`${b} eh o maior`);}
if ((c > a) && (c > b)) {
    console.log(`${c} eh o maior`);}
```

### Lua

```lua
-- Lua → uri_1013 - O maior
x = {io.read('*number', '*number', '*number')}
a = x[1]
b = x[2]
c = x[3]
 if (a > b) and (a > c) then
	print(a.. " eh o maior")
 end
if (b > a) and (b > c) then
	print(b.. " eh o maior")
end
if (c > a) and (c > b) then
	print(c.. " eh o maior")
end
```

### Haskell

```haskell
-- Haskell → uri_1013 - O maior
import Text.Printf
import Prelude hiding(max)
max :: Int -> Int -> Int
max a b = if (a >= b) then a else b
maior :: Int -> Int -> Int -> Int
maior a b c = (a `max` b) `max` c
main = do
   valores <- getLine
   let lista = words valores
   let a = lista !! 0
   let b = lista !! 1
   let c = lista !! 2
   let maximo = (maior(read(a))(read(b))(read(c)))
   putStrLn(show maximo ++ " eh o maior")
```

# `XIV`URI Online Judge | 1014 ✔ **λ** **#**

## Consumo

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Calcule o consumo médio de um automóvel sendo fornecidos a distância total percorrida (em Km) e o total de combustível gasto (em litros).

### Entrada

O arquivo de entrada contém dois valores: um valor inteiro **X** representando a distância total percorrida (em Km), e um valor real **Y** representando o total de combustível gasto, com um dígito após o ponto decimal.

### Saída

Apresente o valor que representa o consumo médio do automóvel com 3 casas após a vírgula, seguido da mensagem "km/l".

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 500 35.0           | 14.286 km/l      |
| 2254 124.4         | 18.119 km/l      |
| 4554 464.6         | 9.802 km/l       |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
km = int(input())
litros = float(input())
media = km / litros
print('{:.3f} km/l'.format(media))

```

### C

```c
#include <stdio.h>
// C - puro 
int main() {
 
    int X;
	float Y;
	scanf("%d", &X);
	scanf("%f", &Y);
	printf("%.3f km/l\n", X/Y);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std;
 
int main() {
 
    int X;
    float Y;
    cout << fixed;
	cout.precision(3);
	cin  >> X;
	cin >> Y;
	cout <<"" << X/Y << " km/l" << endl;

    return 0;
}
```

### C#

```c#
using System; 
// C# - Consumo
class URI {

    static void Main(string[] args) { 

        int km;
        double combgasto, totconsumo;

        km = int.Parse(Console.ReadLine());
        combgasto = double.Parse(Console.ReadLine());
        totconsumo = km / combgasto;
        Console.WriteLine((String.Format("{0:0.000}", totconsumo) + " km/l"));
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby
km = gets.to_i
litros = gets.to_f
media = km / litros
puts "%.3f km/l" % [media]
```

### Pascal

```pascal
// Pascal
program uri_1014;

var
  km: integer;
  litros: real;

begin
  readln(km);
  readln(litros);
  writeln((km / litros):0:3, ' km/l');
  readln();
end.
```

### Javascript

```javascript
// uri_1014 → javascript
// inicio trecho uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim trecho uri

var km = Number(lines.shift());
var litros = Number(lines.shift());
var media = (km / litros);
console.log(`${media.toFixed(3)} km/l`);

```

### Lua

```lua
--uri_1014
local km = tonumber(io.read())
local litros = tonumber(io.read())
local m = (km / litros)
media = (string.format("%.3f", m))
print(media.." km/l")
```

### Haskell

```haskell
import Text.Printf
conta_media :: Float -> Float -> Float
conta_media a b = a / b

main = do
   a <- getLine
   b <- getLine
   let media = (conta_media(read(a))(read(b)))
   printf "%.3f" media
   putStrLn " km/l"

```

### `XV`URI Online Judge | 1015 ✔ **λ** **#**

## Distância Entre Dois Pontos

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia os quatro valores correspondentes aos eixos x e y de dois pontos quaisquer no plano, p1(x1,y1) e p2(x2,y2) e calcule a distância entre eles, mostrando 4 casas decimais após a vírgula, segundo a fórmula:

Distancia =![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1015.png)

### Entrada

O arquivo de entrada contém duas linhas de dados. A primeira linha contém dois valores de ponto flutuante: ***x1 y1*** e a segunda linha contém dois valores de ponto flutuante ***x2 y2***.

### Saída

Calcule e imprima o valor da distância segundo a fórmula fornecida, com 4 casas após o ponto decimal.

| Exemplo de Entrada     | Exemplo de Saída |
| ---------------------- | ---------------- |
| 1.0 7.0 <br>5.0 9.0    | 4.4721           |
| -2.5 0.4 <br>12.1 7.3  | 16.1484          |
| 2.5 -0.4 <br>-12.2 7.0 | 16.4575          |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1015 - Distância entre dois pontos
'''
Python 3
'''
from math import sqrt
x = str(input()).split(" ")
num = [float(numero) for numero in x]
y = str(input()).split(" ")
num1 = [float(numero) for numero in y]
x1, y1 = num
x2, y2 = num1
distancia = sqrt(((x2 - x1)**2) + ((y2 - y1)**2))
print('{:.4f}'.format(distancia))

```

### C

```c
#include <stdio.h>
// C - puro → uri_1015 - Distância entre dois pontos
int main() {
 
    float x1, y1, x2, y2, distancia;
	scanf("%f%f", &x1, &y1);
	scanf("%f%f", &x2, &y2);
	distancia = sqrt(((x2 - x1)*(x2 - x1)) + ((y2 - y1)*(y2 - y1)));
	printf("%.4lf\n", distancia);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
#include <math.h>
// C++ → uri_1016 - Distância entre dois pontos
using namespace std;
 
int main() {
    float x1, y1, x2, y2, distancia;
    cout << fixed;
    cout.precision(4);
    cin >> x1 >> y1;
	cin >> x2 >> y2;
	distancia = sqrt(((x2 - x1)*(x2 - x1)) + ((y2 - y1)*(y2 - y1)));
	cout << "" << distancia << endl;
    return 0;
}
```

### C#

```c#
using System; 
// C# - Distância entre dois pontos
class URI {

    static void Main(string[] args) { 

        string[] dados = Console.ReadLine().Split();
        double x1 = Convert.ToDouble(dados[0]);
        double y1 = Convert.ToDouble(dados[1]);
        string[] dados2 = Console.ReadLine().Split();
        double x2 = Convert.ToDouble(dados2[0]);
        double y2 = Convert.ToDouble(dados2[1]);
        double dif1 = x2 - x1;
        double dif2 = y2 - y1;
        double difdistancia = (dif1 * dif1) + (dif2 * dif2);
        double distancia = Math.Sqrt(difdistancia);
            
        Console.WriteLine(String.Format("{0:0.0000}", distancia));
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1015 - Distância entre dois pontos
X = gets.split
Y = gets.split

x1 = X[0].to_f
y1 = X[1].to_f
x2 = Y[0].to_f
y2 = Y[1].to_f

distancia = Math.sqrt(((x2 - x1)*(x2 - x1)) + ((y2 - y1)*(y2 - y1)))
puts "%.4f" % distancia
```

### Pascal

```pascal
// Pascal → uri_1015 - Distância entre dois pontos
program uri_1015;

var
  x1, y1, x2, y2, distancia: real;

begin
  readln(x1, y1);
  readln(x2, y2);
  distancia := (sqrt(((x2 - x1)*(x2 - x1)) + ((y2 - y1)*(y2 - y1))));
  writeln(distancia:0:4);
  readln();
end.
```

### Javascript

```javascript
// javascript → uri_1015 - Distância entre dois pontos
var x = lines.shift().split(" ");
var y = lines.shift().split(" ");

var a1 = parseFloat(x[0]);
var b1 = parseFloat(x[1]);
var a2 = parseFloat(y[0]);
var b2 = parseFloat(y[1]);

distancia = Math.sqrt(Math.pow((a2-a1), 2) + Math.pow((b2-b1), 2));
console.log(`${(distancia).toFixed(4)}`);
```

### Lua

```lua
--Lua → uri_1015 - Distância entre dois pontos
local x = {io.read('*number', '*number')}
local x1 = x[1]
local y1 = x[2]
local y = {io.read('*number', '*number')}
local x2 = y[1]
local y2 = y[2]
local d = (math.sqrt(((x2 - x1)*(x2 - x1)) + ((y2 - y1)*(y2 - y1))))
distancia = (string.format("%.4f", d))
print(distancia)
```

### Haskell

```haskell
-- Haskell → 1015 - Distância entre dois pontos
import Text.Printf

distancia :: Float -> Float -> Float -> Float -> Float
distancia a b c d = sqrt(((b - a)^2) + ((d - c)^2))

main = do
   valores <- getLine
   valores2 <- getLine
   let lista = words valores
   let lista2 = words valores2
   let a = lista !! 0
   let c = lista !! 1
   let b = lista2 !! 0
   let d = lista2 !! 1
   let v_distancia = (distancia(read(a))(read(b))(read(c))(read(d)))
   printf "%.4f\n" v_distancia
```

# `XVI`URI Online Judge | 1016 ✔ **λ** **#**

## Distância

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Dois carros (X e Y) partem em uma mesma direção. O carro X sai com velocidade constante de 60 Km/h e o carro Y sai com velocidade constante de 90 Km/h.

Em uma hora (60 minutos) o carro Y consegue se distanciar 30 quilômetros do carro X, ou seja, consegue se afastar um quilômetro a cada 2 minutos.

Leia a distância (em Km) e calcule quanto tempo leva (em minutos) para o carro Y tomar essa distância do outro carro.

### Entrada

O arquivo de entrada contém um número inteiro.

### Saída

Imprima o tempo necessário seguido da mensagem "minutos".

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 30                 | 60 minutos       |
| 110                | 220 minutos      |
| 7                  | 14 minutos       |

### Python 3

```python
# -*- coding: utf-8 -*-

'''
Python 3
'''
km = int(input())
tempo = km * 2
print('{} minutos'.format(tempo))

```

### C

```c
#include <stdio.h>
 
int main() {
 
    /**
     * C - puro
     */
    int a, tempo;
    scanf("%d", &a);
    tempo = a * 2;
    printf("%d minutos\n", tempo);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 
using namespace std;
 
int main() {
 
    /**
     * C++
     */
    int a, tempo;
    cin  >> a;
    tempo = a * 2;
    cout << "" << tempo << " minutos" << endl;
 
    return 0;
}
```

### C#

```c#
using System; 

class URI {

    static void Main(string[] args) { 

        int km = int.Parse(Console.ReadLine());
        int conta = (km * 2);
        Console.WriteLine(conta + " minutos");
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# uri_1016 → Ruby
km = gets.to_i
tempo = km * 2
puts "#{tempo} minutos"
```

### Pascal

```pascal
// Pascal

program uri_1015;
// correto
var
  x, tempo: integer;

begin
  readln(x);
  tempo := (x * 2);
  writeln(tempo, ' minutos');
  readln();
end.
```

### Javascript

```javascript
// uri_1016 → javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
var x = Number(lines.shift());
var tempo = (x * 2);
console.log(`${tempo} minutos`);
```

### Lua

```lua
-- uri_1016 → Lua
local x = tonumber(io.read())
local tempo = (x * 2)
print(tempo.." minutos")
```

### Haskell

```haskell
-- uri_1016 → Haskell
import Text.Printf
main :: IO ()
main =
  do num1 <- getLine
     putStr (show (tempo num1))
     putStrLn " minutos"
       where tempo num1 = (read num1 :: Int) * 2
```



# `XVII`URI Online Judge | 1017 ✔ **λ** **#**

## Gasto de Combustível

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Joaozinho quer calcular e mostrar a quantidade de litros de combustível gastos em uma viagem, ao utilizar um automóvel que faz 12 KM/L. Para isso, ele gostaria que você o auxiliasse através de um simples programa. Para efetuar o cálculo, deve-se fornecer o tempo gasto na viagem (em horas) e a velocidade média durante a mesma (em km/h). Assim, pode-se obter distância percorrida e, em seguida, calcular quantos litros seriam necessários. Mostre o valor com 3 casas decimais após o ponto.

### Entrada

O arquivo de entrada contém dois inteiros. O primeiro é o tempo gasto na viagem (em horas) e o segundo é a velocidade média durante a mesma (em km/h).

### Saída

Imprima a quantidade de litros necessária para realizar a viagem, com três dígitos após o ponto decimal

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 10 <br>85          | 70.833           |
| 2 <br>92           | 15.333           |
| 22 <br>67          | 122.833          |

### Python 3

```python
# -*- coding: utf-8 -*-
# uri_1017 → Python 3
horas = int(input())
km = int(input())
litros = (km * horas) / 12
print('{:.3f}'.format(litros))

```

### C

```c
#include <stdio.h>
// uri_1017 → C - puro 
int main() {
 
   	float km, horas;
	double litros;

	scanf("%f", &km);
	scanf("%f", &horas);
	litros = (km * horas) / 12;
	printf("%.3lf\n", litros);
 
    return 0;
}
```

### C++

```c++
// uri_1017 → C++
#include <iostream>
 
using namespace std;
 
int main() {
 
    /**
     * C++
     */
    float km, horas;
	double litros;
    cout << fixed;
    cout.precision(3);
	cin >> km;
	cin >> horas;
	litros = (km * horas) / 12;
	cout << "" << litros << endl;
 
    return 0;
}
```

### C#

```c#
using System; 
// C# - Gasto de combustível
class URI {

    static void Main(string[] args) { 

        double tgasto;
        int vmedia;
        tgasto = Convert.ToDouble(Console.ReadLine());
        vmedia = Convert.ToInt32(Console.ReadLine());

        double calcula = ((vmedia * tgasto) / 12.00);
        Console.WriteLine(String.Format("{0:0.000}", calcula));
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# uri_1017 → Ruby
km = gets.to_f
horas = gets.to_f

litros = (km * horas) / 12;
puts "%.3f" %litros
```

### Pascal

```pascal
// uri_1017 → Pascal

program uri_1017;
// correto
var
  km, horas: integer;
  litros: double;

begin
  readln(km);
  readln(horas);
  litros := ((km * horas) / 12);
  writeln(litros:0:3);
  readln();
end.
```

### Javascript

```javascript
// uri_1017 → Javascript
// inicio uri
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// fim uri
var horas = Number(lines.shift());
var km = Number(lines.shift());
var litros = ((km * horas) / 12);
console.log(`${litros.toFixed(3)}`);
```

### Lua

```lua
-- uri_1017 → Lua
local horas = tonumber(io.read())
local km = tonumber(io.read())
litros = ((km * horas) / 12)
litrosfinal = (string.format("%.3f", litros))
print(litrosfinal)
```

### Haskell

```haskell
-- Haskell → uri_1017 - Gasto de Combustível
module Main (main) where
import Text.Printf
main :: IO ()

main = do 
          a <- readLn :: IO Double
          b <- readLn :: IO Double
          let media = (a * b) / 12
          printf "%.3f\n" media
```

# `XVIII`URI Online Judge | 1018 ✔ **λ** **#**

## Cédulas

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro. A seguir, calcule o menor número de notas possíveis (cédulas) no qual o valor pode ser decomposto. As notas consideradas são de 100, 50, 20, 10, 5, 2 e 1. A seguir mostre **o valor lido** e a relação de notas necessárias.

### Entrada

O arquivo de entrada contém um valor inteiro **N** (0 < **N** < 1000000).

### Saída

Imprima o valor lido e, em seguida, a quantidade mínima de notas de cada tipo necessárias, conforme o exemplo fornecido. Não esqueça de imprimir o fim de linha após cada linha, caso contrário seu programa apresentará a mensagem: *“Presentation Error”*.



| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
| 576                | 576 <br>5 nota(s) de R\$ 100,00 <br>1 nota(s) de R\$ 50,00 <br>1 nota(s) de R\$ 20,00 <br>0 nota(s) de R\$ 10,00 <br>1 nota(s) de R\$ 5,00 <br>0 nota(s) de R\$ 2,00 <br>1 nota(s) de R\$ 1,00 |
| 11257              | 11257 <br>112 nota(s) de R\$ 100,00 <br>1 nota(s) de R​\$ 50,00 <br>0 nota(s) de R​\$ 20,00 <br>0 nota(s) de R\$ 10,00 <br>1 nota(s) de R\$ 5,00 <br>1 nota(s) de R\$ 2,00 <br>0 nota(s) de R\$ 1,00 |
| 503                | 503 <br>5 nota(s) de R\$ 100,00 <br>0 nota(s) de R\$ 50,00 <br>0 nota(s) de R\$ 20,00 <br>0 nota(s) de R\$ 10,00 <br>0 nota(s) de R\$ 5,00 <br>1 nota(s) de R\$ 2,00 <br>1 nota(s) de R$ 1,00 |

### Python 3

```python
# -*- coding: utf-8 -*-

'''
uri_1018 → Python 3
'''
value = int(input())
val = value
n100 = n50 = n20 = n10 = n5 = n2 = n1 = 0

if int(value / 100) >= 1:
	n100 = int(value / 100)
	value -= n100 * 100

if int(value / 50) >= 1:
	n50 = int(value / 50)
	value -= n50 * 50

if int(value / 20) >= 1:
	n20 = int(value / 20)
	value -= n20 * 20

if int(value / 10) >= 1:
	n10 = int(value / 10)
	value -= n10 * 10

if int(value / 5) >= 1:
	n5 = int(value / 5)
	value -= n5 * 5

if int(value / 2) >= 1:
	n2 = int(value / 2)
	value -= n2 * 2

if int(value / 1) >= 1:
    n1 = int(value / 1)
    value -= n1 * 1

print("{}".format(val))
print("{} nota(s) de R$ 100,00".format(n100))
print("{} nota(s) de R$ 50,00".format(n50))
print("{} nota(s) de R$ 20,00".format(n20))
print("{} nota(s) de R$ 10,00".format(n10))
print("{} nota(s) de R$ 5,00".format(n5))
print("{} nota(s) de R$ 2,00".format(n2))
print("{} nota(s) de R$ 1,00".format(n1))
```

### C

```c
#include <stdio.h>
 // uri_1018 → C - puro
int main() {
 
 int valor;

	scanf("%d", &valor);
	printf("%d\n", valor);

	printf("%d nota(s) de R$ 100,00\n", (valor/100));
	valor %= 100;
	printf("%d nota(s) de R$ 50,00\n", (valor/50));
	valor %= 50;
    printf("%d nota(s) de R$ 20,00\n", (valor/20));
    valor %= 20;
    printf("%d nota(s) de R$ 10,00\n", (valor/10));
    valor %= 10;
    printf("%d nota(s) de R$ 5,00\n", (valor/5));
    valor %= 5;
    printf("%d nota(s) de R$ 2,00\n", (valor/2));
    valor %= 2;
    printf("%d nota(s) de R$ 1,00\n", (valor/1));
    valor %= 1;
 
    return 0;
}
```

### C++

```c++
#include <iostream>
// uri_1018 → C++ 
using namespace std;
 
int main() {
 
     int valor;

	cin >> valor;
	cout << "" << valor << endl;

	cout << "" << valor/100 << " nota(s) de R$ 100,00" << endl;
	valor %= 100;
	cout << "" << valor/50 << " nota(s) de R$ 50,00"<< endl;
	valor %= 50;
    cout << "" << valor/20 << " nota(s) de R$ 20,00" << endl;
    valor %= 20;
    cout << "" << valor/10 << " nota(s) de R$ 10,00" << endl;
    valor %= 10;
    cout << "" << valor/5 << " nota(s) de R$ 5,00" << endl;
    valor %= 5;
    cout << ""  << valor/2 << " nota(s) de R$ 2,00" << endl;
    valor %= 2;
    cout << "" << valor/1 << " nota(s) de R$ 1,00" << endl;
    valor %= 1;
 
    return 0;
}
```

### C#

```c#
using System; 
// C# - Cédulas
class URI {

    static void Main(string[] args) { 

            int valor = int.Parse(Console.ReadLine());
            Console.WriteLine(valor);
            int valor100 = valor / 100;
            int mod100 = valor % 100;
            int valor50 = mod100 / 50;
            int mod50 = mod100 % 50;
            int valor20 = mod50 / 20;
            int mod20 = mod50 % 20;
            int valor10 = mod20 / 10;
            int mod10 = mod20 % 10;
            int valor5 = mod10 / 5;
            int mod5 = mod10 % 5;
            int valor2 = mod5 / 2;
            int mod2 = mod5 % 2;
            int valor1 = mod2 / 1;
            int mod1 = mod2 % 1;

            Console.WriteLine(valor100 + " nota(s) de R$ 100,00");
            Console.WriteLine(valor50 + " nota(s) de R$ 50,00");
            Console.WriteLine(valor20 + " nota(s) de R$ 20,00");
            Console.WriteLine(valor10 + " nota(s) de R$ 10,00");
            Console.WriteLine(valor5 + " nota(s) de R$ 5,00");
            Console.WriteLine(valor2 + " nota(s) de R$ 2,00");
            Console.WriteLine(valor1 + " nota(s) de R$ 1,00");
            Console.ReadKey();
    }
}
```

### Ruby

```ruby
# uri_1018 → Ruby
valor = gets.to_i
puts "#{valor}"

puts "%i nota(s) de R$ 100,00\n" % (valor/100)
valor %= 100
puts "%i nota(s) de R$ 50,00\n" % (valor/50)
valor %= 50
puts "%i nota(s) de R$ 20,00\n" % (valor/20)
valor %= 20
puts "%i nota(s) de R$ 10,00\n" % (valor/10)
valor %= 10
puts "%i nota(s) de R$ 5,00\n" % (valor/5)
valor %= 5
puts "%i nota(s) de R$ 2,00\n" % (valor/2)
valor %= 2
puts "%i nota(s) de R$ 1,00\n" % (valor/1)
valor %= 1
```

### Pascal

```pascal
// uri_1018 → Pascal
Program uri_1018_1;
var
N:integer;
begin
  readln(N);
  writeln(N);
  writeln((N div 100),' nota(s) de R$ 100,00');
  N := N mod 100;
  writeln((N div 50),' nota(s) de R$ 50,00');
  N := N mod 50;
  writeln((N div 20),' nota(s) de R$ 20,00');
  N := N mod 20;
  writeln((N div 10),' nota(s) de R$ 10,00');
  N := N mod 10;
  writeln((N div 5),' nota(s) de R$ 5,00');
  N := N mod 5;
  writeln((N div 2),' nota(s) de R$ 2,00');
  N := N mod 2;
  writeln((N div 1),' nota(s) de R$ 1,00');

  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1018 - Cédulas
var valor = Number(lines.shift());
console.log(valor); 
var valor100 = Math.floor(valor / 100); 
var mod100 = valor % 100; 
var valor50 = Math.floor(mod100 / 50); 
var mod50 = mod100 % 50; 
var valor20 = Math.floor(mod50 / 20); 
var mod20 = mod50 % 20; 
var valor10 = Math.floor(mod20 / 10); 
var mod10 = mod20 % 10; 
var valor5 = Math.floor(mod10 / 5); 
var mod5 = mod10 % 5; 
var valor2 = Math.floor(mod5 / 2); 
var mod2 = mod5 % 2; 
var valor1 = Math.floor(mod2 / 1); 
var mod1= mod2 % 1; 
console.log(valor100 + " nota(s) de R$ 100,00"); 
console.log(valor50 + " nota(s) de R$ 50,00"); 
console.log(valor20 + " nota(s) de R$ 20,00"); 
console.log(valor10 + " nota(s) de R$ 10,00"); 
console.log(valor5 + " nota(s) de R$ 5,00"); 
console.log(valor2 + " nota(s) de R$ 2,00"); 
console.log(valor1 + " nota(s) de R$ 1,00");
```

### Lua

```lua
-- uri_1018 → Lua
local value = io.read()
print(value)
--minha solução → conta notas
print(math.floor(value / 100)..' nota(s) de R$ 100,00')
value = value % 100
print(math.floor(value / 50)..' nota(s) de R$ 50,00')
value = value % 50
print(math.floor(value / 20)..' nota(s) de R$ 20,00')
value = value % 20
print(math.floor(value / 10)..' nota(s) de R$ 10,00')
value = value % 10
print(math.floor(value / 5)..' nota(s) de R$ 5,00')
value = value % 5
print(math.floor(value / 2)..' nota(s) de R$ 2,00')
value = value % 2
print(math.floor(value / 1)..' nota(s) de R$ 1,00')
```

### Haskell

```haskell
{-- Haskell → uri_1018 - Cédulas
Por enquanto foi o exercício Haskell mais difícil de pesquisar, não achei na internet nenhuma respostas explícita e também nenhum tipo de estudo ou exercício que pudesse me ajudar a resolver o problema.
Tem uma forma mais curta de resolver este problema, mas ele ia ficar inteligível e este modo foi aceito pelo uri !! --}
import Text.Printf

cem :: Int -> Int
cem a = a `div` 100
resto_cem :: Int -> Int
resto_cem a = a `mod` 100
cinq :: Int -> Int
cinq a = (resto_cem a) `div` 50
resto_cinq :: Int -> Int
resto_cinq a = (resto_cem a) `mod` 50
vinte :: Int -> Int
vinte a = (resto_cinq a) `div` 20
resto_vinte :: Int -> Int
resto_vinte a = (resto_cinq a) `mod` 20
dez :: Int -> Int
dez a = (resto_vinte a) `div` 10
resto_dez :: Int -> Int
resto_dez a =  (resto_vinte a) `mod` 10
cinco :: Int -> Int
cinco a = (resto_dez a) `div` 5
resto_cinco :: Int -> Int
resto_cinco a = (resto_dez a) `mod` 5
dois :: Int -> Int
dois a = (resto_cinco a) `div` 2
resto_dois :: Int -> Int
resto_dois a = (resto_cinco a) `mod` 2
um :: Int -> Int
um a = (resto_dois a) `div` 1
resto_um :: Int -> Int
resto_um a = (resto_dois a) `mod` 1           

main = do 
          valores <- getLine
          let lista = words valores
          let a = lista !! 0
          let cem_a = (cem(read(a))) 
          let cinq_a = (cinq(read(a)))
          let vinte_a = (vinte(read(a)))
          let dez_a = (dez(read(a)))
          let cinco_a = (cinco(read(a)))
          let dois_a = (dois(read(a)))
          let um_a = (um(read(a)))
          putStrLn(a)
          printf "%d nota(s) de R$ 100,00\n" cem_a
          printf "%d nota(s) de R$ 50,00\n" cinq_a
          printf "%d nota(s) de R$ 20,00\n" vinte_a
          printf "%d nota(s) de R$ 10,00\n" dez_a
          printf "%d nota(s) de R$ 5,00\n" cinco_a
          printf "%d nota(s) de R$ 2,00\n" dois_a
          printf "%d nota(s) de R$ 1,00\n" um_a

```



# `XIX`URI Online Judge | 1019 ✔ **λ** **#**

## Conversão de Tempo

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro, que é o tempo de duração em segundos de um determinado evento em uma fábrica, e informe-o expresso no formato horas:minutos:segundos.

### Entrada

O arquivo de entrada contém um valor inteiro **N**.

### Saída

Imprima o tempo lido no arquivo de entrada (segundos), convertido para horas:minutos:segundos, conforme exemplo fornecido.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 556                | 0:9:16           |
| 1                  | 0:0:1            |
| 140153             | 38:55:53         |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
N = int(input())
hora = N // 3600
minuto = (N - (hora * 3600)) // 60
segundo = N - (hora * 3600) - (minuto * 60)
print('{:.0f}:{:.0f}:{:.0f}'.format(hora, minuto, segundo))

```

### C

```c
#include <stdio.h>
 // C - puro
int main() {
    int tempo, horas, minutos, segundos;
    scanf("%d", &tempo);
    horas = tempo / 3600;
    minutos = (tempo - (horas * 3600)) / 60;
    segundos = tempo - (horas * 3600) - (minutos * 60);
    printf("%d:%d:%d\n", horas, minutos, segundos);
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std;
 int main() {
    int tempo, horas, minutos, segundos;
    cin >> tempo;
    horas = tempo / 3600;
    minutos = (tempo - (horas * 3600)) / 60;
    segundos = tempo - (horas * 3600) - (minutos * 60);
    cout << "" << horas << ":" << "" << minutos << ":" << "" << segundos << endl;
    return 0;
}
```

### C#

```c#
using System; 

class URI {

    static void Main(string[] args) { 

        int segundos, horas, mod, minutos;
        segundos = int.Parse(Console.ReadLine());
        horas = segundos / 3600;
        mod = segundos % 3600;
        minutos = mod / 60;
        segundos = mod - (minutos * 60);
        //Apresenta o resultado conforme o exemplo de saída
        Console.WriteLine(horas + ":" + minutos + ":" + segundos);
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby
tempo = gets.to_i
horas = tempo / 3600
minutos = (tempo - (horas * 3600)) / 60
segundos = tempo - (horas * 3600) - (minutos * 60)
puts "#{horas}:#{minutos}:#{segundos}"
```

### Pascal

```pascal
// Pascal
Program uri_1019;
    //correto
var
  N, horas, minutos, segundos:longint;

begin
  readln(N);
  horas := (N div 3600);
  minutos := ((N - (horas * 3600)) div 60);
  segundos := (N - (horas * 3600) - (minutos * 60));
  writeln(horas, ':', minutos, ':', segundos);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1019 - Conversão de tempo
var tempo = Number(lines.shift());
var horas = Math.floor(tempo / 3600);
var b = tempo % 3600;
var minutos = Math.floor(b / 60);
var segundos = b % 60;
console.log(horas + ":" + minutos + ":" + segundos);
```

### Lua

```lua
-- Lua → uri_1019 - Conversão de tempo
local tempo = io.read()
local horas = math.floor(tempo / 3600)
local b = tempo % 3600
local minutos = math.floor(b / 60)
local segundos = b % 60
local hora = (string.format("%.0f", horas))
local minuto = (string.format("%.0f", minutos))
local segundo = (string.format("%.0f", segundos))
print(hora.. ":" ..minuto..":"..segundo)
```

### Haskell

```haskell
-- Haskell → uri_1019 - Conversão de tempo
import Text.Printf

horas :: Int -> Int
horas tempo = tempo `div` 3600
minutos :: Int -> Int
minutos tempo = (tempo - ((horas tempo) * 3600)) `div` 60
segundos :: Int -> Int
segundos tempo = (tempo - ((horas tempo) * 3600)) - ((minutos tempo) * 60)

main = do 
          valores <- getLine
          let lista = words valores
          let tempo = lista !! 0
          let horas_v = (horas(read(tempo)))
          let minutos_v = (minutos(read(tempo)))
          let segundos_v = (segundos(read(tempo)))
          printf "%d:%d:%d\n" horas_v minutos_v segundos_v
```



# `XX`URI Online Judge | 1020 ✔ **λ** **#**

## Idade em Dias

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro correspondente à idade de uma pessoa em dias e informe-a em anos, meses e dias

Obs.: apenas para facilitar o cálculo, considere todo ano com 365 dias e todo mês com 30 dias. Nos casos de teste nunca haverá uma situação que permite 12 meses e alguns dias, como 360, 363 ou 364. Este é apenas um exercício com objetivo de testar raciocínio matemático simples.

### Entrada

O arquivo de entrada contém um valor inteiro.

### Saída

Imprima a saída conforme exemplo fornecido.

| Exemplo de Entrada | Exemplo de Saída                     |
| ------------------ | ------------------------------------ |
| 400                | 1 ano(s) <br>1 mes(es) <br>5 dia(s)0 |
| 800                | 2 ano(s) <br>2 mes(es) <br>10 dia(s) |
| 30                 | 0 ano(s)<br>1 mes(es)<br>0 dia(s)    |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
dias = int(input())
anos = int(dias / 365)
dias -= anos * 365
meses = int(dias / 30)
dias -= meses * 30
print('{} ano(s)'.format(anos))
print('{} mes(es)'.format(meses))
print('{} dia(s)'.format(dias))

```

### C

```c
#include <stdio.h>
// C - puro 
int main() {
 
    int dias, meses, anos, inteiro;
    scanf("%d", &inteiro);
    anos = inteiro / 365;
    meses = inteiro % 365 / 30;
    dias = inteiro % 365 % 30;
    printf("%d ano(s)\n", anos);
    printf("%d mes(es)\n", meses);
    printf("%d dia(s)\n", dias);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ 
using namespace std;
 
int main() {
 
    int dias, meses, anos, inteiro;
    cin >> inteiro;
    anos = inteiro / 365;
    meses = inteiro % 365 / 30;
    dias = inteiro % 365 % 30;
    cout << "" << anos << " ano(s)" << endl;
    cout << "" << meses << " mes(es)" << endl;
    cout << "" << dias << " dia(s)" << endl;
 
    return 0;
}
```

### C#

```c#
using System; 

class URI {

    static void Main(string[] args) { 

        int anos, idade, mod, mes, dias;
        idade = int.Parse(Console.ReadLine());
        anos = idade / 365;
        Console.WriteLine(anos + " ano(s)");
        mod = idade % 365;
        mes = mod / 30;
        Console.WriteLine(mes + " mes(es)");
        dias = mod - (mes * 30);
        Console.WriteLine(dias + " dia(s)");
        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby
inteiro = gets.to_i
anos = inteiro / 365
meses = (inteiro % 365) / 30
dias = (inteiro % 365) % 30
puts "%i ano(s)\n" % anos
puts "%i mes(es)\n" % meses
puts "%i dia(s)" % dias
```

### Pascal

```pascal
// Pascal
Program uri_1020;
    //correto
var
  dias, meses, anos, inteiro:longint;

begin
  readln(inteiro);
  anos := (inteiro div 365);
  meses := (inteiro mod 365 div 30);
  dias := (inteiro mod 365 mod 30);
  writeln(anos, ' ano(s)');
  writeln(meses, ' mes(es)');
  writeln(dias, ' dia(s)');
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1020 - Idade em dias
var tempo = Number(lines.shift());
  
var anos = Math.floor(tempo / 365);
var meses = Math.floor(tempo % 365 / 30);
var dias = (tempo % 365 % 30);
console.log(anos + " ano(s)");
console.log(meses + " mes(es)");
console.log(dias + " dia(s)");
```

### Lua

```lua
--Lua → uri_1020 - Idade em dias
local tempo = io.read()
  
local anos = math.floor(tempo / 365)
local meses = math.floor(tempo % 365 / 30)
local dias = (tempo % 365 % 30)
local a = (string.format(anos, "%.0f"))
local m = (string.format(meses, "%.0f"))
local d = (string.format(dias, "%.0f"))
print(a.. " ano(s)")
print(m.. " mes(es)")
print(d.. " dia(s)")
```

### Haskell

```haskell
import Text.Printf

anos_v :: Int -> Int
anos_v a = a `div` 365

meses_v :: Int -> Int
meses_v a = (a `mod` 365) `div` 30

dias_v :: Int -> Int
dias_v a = (a `mod` 365) `mod` 30

main = do 
          a <- getLine
          let anos = (anos_v(read(a)))
          let meses = (meses_v(read(a)))
          let dias = (dias_v(read(a)))
          printf "%d" anos
          putStrLn(" ano(s)")
          printf "%d" meses
          putStrLn(" mes(es)")
          printf "%d" dias
          putStrLn(" dia(s)")         
```



# `XXI`  URI Online Judge | 1021 ✔ **#**

## Notas e Moedas

Por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor de ponto flutuante com duas casas decimais. Este valor representa um valor monetário. A seguir, calcule o menor número de notas e moedas possíveis no qual o valor pode ser decomposto. As notas consideradas são de 100, 50, 20, 10, 5, 2. As moedas possíveis são de 1, 0.50, 0.25, 0.10, 0.05 e 0.01. A seguir mostre a relação de notas necessárias.

### Entrada

O arquivo de entrada contém um valor de ponto flutuante **N** (0 ≤ **N** ≤ 1000000.00).

### Saída

Imprima a quantidade mínima de notas e moedas necessárias para trocar o valor inicial, conforme exemplo fornecido.

Obs: Utilize ponto (.) para separar a parte decimal.

| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
| 576.73             | NOTAS: <br>5 nota(s) de R\$ 100.00 <br> 1 nota(s) de R\$ 50.00 <br> 1 nota(s) de R\$ 20.00 <br> 0 nota(s) de R\$ 10.00  <br> 1 nota(s) de R\$ 5.00 <br> 0 nota(s) de R\$ 2.00 <BR>  MOEDAS: <br>1 moeda(s) de R\$ 1.00 <br>1 moeda(s) de R\$ 0.50 <br>0 moeda(s) de R\$ 0.25 <br>2 moeda(s) de R\$ 0.10 <br>0 moeda(s) de R\$ 0.05 <br>3 moeda(s) de R\$ 0.01 |
| 4.00               | NOTAS: <br>0 nota(s) de R\$ 100.00 <br>0 nota(s) de R\$ 50.00 <br>0 nota(s) de R\$ 20.00 <br>0 nota(s) de R\$ 10.00 <br>0 nota(s) de R\$ 5.00 <br>2 nota(s) de R\$ 2.00 <br>MOEDAS: <br>0 moeda(s) de R\$ 1.00 <br>0 moeda(s) de R\$ 0.50 <br>0 moeda(s) de R\$ 0.25 <br>0 moeda(s) de R\$ 0.10 <br>0 moeda(s) de R\$ 0.05 <br>0 moeda(s) de R\$ 0.01 |
| 91.01              | NOTAS: <br>0 nota(s) de R\$ 100.00 <br>1 nota(s) de R\$ 50.00 <br>2 nota(s) de R\$ 20.00 <br>0 nota(s) de R\$ 10.00 <br>0 nota(s) de R\$ 5.00 <br>0 nota(s) de R\$ 2.00 <br>MOEDAS: <br>1 moeda(s) de R\$ 1.00 <br>0 moeda(s) de R\$ 0.50 <br>0 moeda(s) de R\$ 0.25 <br>0 moeda(s) de R\$ 0.10 <br>0 moeda(s) de R\$ 0.05 <br>1 moeda(s) de R\$ 0.01 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_2021 - Notas e moedas

N = eval(input())

n100 = n50 = n20 = n10 = n5 = n2 = n1 = 0
m50 = m25 = m10 = m5 = m1 = m = 0

N = float('{:.2f}'.format(N))
if int(N / 100) >= 1:
	n100 = int(N / 100)
	N -= n100 * 100

N = float('{:.2f}'.format(N))
if int(N / 50) >= 1:
	n50 = int(N / 50)
	N -= n50 * 50

N = float('{:.2f}'.format(N))
if int(N / 20) >= 1:
	n20 = int(N / 20.00)
	N -= n20 * 20

N = float('{:.2f}'.format(N))
if int(N / 10) >= 1:
	n10 = int(N / 10)
	N -= n10 * 10.00

N = float('{:.2f}'.format(N))
if int(N / 5) >= 1:
	n5 = int(N / 5)
	N -= n5 * 5

N = float('{:.2f}'.format(N))
if int(N / 2) >= 1:
	n2 = int(N / 2)
	N -= n2 * 2

N = float('{:.2f}'.format(N))
if int(N / 1) >= 1:
	m1 = int(N / 1)
	N -= m1 * 1

N = float('{:.2f}'.format(N))
if int(N / 0.50) >= 1:
	m50 = int(N / 0.50)
	N -= m50 * 0.50

N = float('{:.2f}'.format(N))
if int(N / 0.25) >= 1:
	m25 = int(N / 0.25)
	N -= m25 * 0.25

N = float('{:.2f}'.format(N))
if int(N / 0.10) >= 1:
	m10 = int(N / 0.10)
	N -= m10 * 0.10

N = float('{:.2f}'.format(N))
if int(N / 0.05) >= 1:
	m5 = int(N/0.05)
	N -= m5 * 0.05

N = float('{:.2f}'.format(N))
if int(N / 0.01) >= 0.998:
	m = int(N / 0.01)
	N -= m * 0.01

print('NOTAS:')
print('{} nota(s) de R$ 100.00'.format(n100))
print('{} nota(s) de R$ 50.00'.format(n50))
print('{} nota(s) de R$ 20.00'.format(n20))
print('{} nota(s) de R$ 10.00'.format(n10))
print('{} nota(s) de R$ 5.00'.format(n5))
print('{} nota(s) de R$ 2.00'.format(n2))

print('MOEDAS:')
print('{} moeda(s) de R$ 1.00'.format(m1))
print('{} moeda(s) de R$ 0.50'.format(m50))
print('{} moeda(s) de R$ 0.25'.format(m25))
print('{} moeda(s) de R$ 0.10'.format(m10))
print('{} moeda(s) de R$ 0.05'.format(m5))
print('{} moeda(s) de R$ 0.01'.format(m))

```

### C

```c
#include <stdio.h>
// C - puro 
int main() {
 
    int dinh100, dinh50, dinh20, dinh10, dinh5, dinh2, dinh1;
    int moed_50, moed_25, moed_10, moed_05, moed_01;
    double valor;

    scanf("%lf", &valor);
    int dinh = valor;
    int moed = (valor - dinh) * 100;

    if ((moed * 1000) % 10 == 9)
    {
        moed++;
    }

    dinh100 = dinh/100;
    dinh %= 100;
    dinh50 = dinh/50;
    dinh %= 50;
    dinh20 = dinh/20;
    dinh %= 20;
    dinh10 = dinh/10;
    dinh %= 10;
    dinh5 = dinh/5;
    dinh %= 5;
    dinh2 = dinh/2;
    dinh %= 2;

    dinh1 = dinh/1;
    dinh %= 1;
    moed_50 = moed/50;
    moed %= 50;
    moed_25 = moed/25;
    moed %= 25;
    moed_10 = moed/10;
    moed %= 10;
    moed_05 = moed/5;
    moed %= 5;
    moed_01 = moed/1;
    moed %= 1;

    printf("NOTAS:\n");
    printf("%d nota(s) de R$ 100.00\n", dinh100);
    printf("%d nota(s) de R$ 50.00\n", dinh50);
    printf("%d nota(s) de R$ 20.00\n", dinh20);
    printf("%d nota(s) de R$ 10.00\n", dinh10);
    printf("%d nota(s) de R$ 5.00\n", dinh5);
    printf("%d nota(s) de R$ 2.00\n", dinh2);

    printf("MOEDAS:\n");

    printf("%d moeda(s) de R$ 1.00\n", dinh1);
    printf("%d moeda(s) de R$ 0.50\n", moed_50);
    printf("%d moeda(s) de R$ 0.25\n", moed_25);
    printf("%d moeda(s) de R$ 0.10\n", moed_10);
    printf("%d moeda(s) de R$ 0.05\n", moed_05);
    printf("%d moeda(s) de R$ 0.01\n", moed_01);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std;
 
int main() {
 
    int dinh100, dinh50, dinh20, dinh10, dinh5, dinh2, dinh1;
    int moed_50, moed_25, moed_10, moed_05, moed_01;
    double valor;

    cin >> valor;
    int dinh = valor;
    int moed = (valor - dinh) * 100;

    if ((moed * 1000) % 10 == 9)
    {
        moed++;
    }

    dinh100 = dinh/100;
    dinh %= 100;
    dinh50 = dinh/50;
    dinh %= 50;
    dinh20 = dinh/20;
    dinh %= 20;
    dinh10 = dinh/10;
    dinh %= 10;
    dinh5 = dinh/5;
    dinh %= 5;
    dinh2 = dinh/2;
    dinh %= 2;

    dinh1 = dinh/1;
    dinh %= 1;
    moed_50 = moed/50;
    moed %= 50;
    moed_25 = moed/25;
    moed %= 25;
    moed_10 = moed/10;
    moed %= 10;
    moed_05 = moed/5;
    moed %= 5;
    moed_01 = moed/1;
    moed %= 1;

    cout << "NOTAS:" << endl;
    cout << "" << dinh100 << " nota(s) de R$ 100.00" << endl;
    cout << "" << dinh50 << " nota(s) de R$ 50.00" << endl;
    cout << "" << dinh20 << " nota(s) de R$ 20.00" << endl;
    cout << "" << dinh10 << " nota(s) de R$ 10.00" << endl;
    cout << "" << dinh5 << " nota(s) de R$ 5.00" << endl;
    cout << "" << dinh2 << " nota(s) de R$ 2.00" << endl;

    cout << "MOEDAS:" << endl;

    cout << "" << dinh1 << " moeda(s) de R$ 1.00" << endl;
    cout << "" << moed_50 << " moeda(s) de R$ 0.50" << endl;
    cout << "" << moed_25 << " moeda(s) de R$ 0.25" << endl;
    cout << "" << moed_10 << " moeda(s) de R$ 0.10" << endl;
    cout << "" << moed_05 << " moeda(s) de R$ 0.05" << endl;
    cout << "" << moed_01 << " moeda(s) de R$ 0.01" << endl;
 
    return 0;
}
```

### C#

```c#
using System; 
// C# - Notas e moedas
class URI {

    static void Main(string[] args) { 

            double valor;
            int numero;
            valor = double.Parse(Console.ReadLine());
            //com conversao para inteiro
            numero = (int)valor;
            Console.WriteLine("NOTAS:");
            int nota100 = numero / 100;
            Console.WriteLine(nota100 + " nota(s) de R$ 100.00");
            int mod = numero % 100;
            int nota50 = mod / 50;
            Console.WriteLine(nota50 + " nota(s) de R$ 50.00");
            mod = mod % 50;
            int nota20 = mod / 20;
            Console.WriteLine(nota20 + " nota(s) de R$ 20.00");
            mod = mod % 20;
            int nota10 = mod / 10;
            Console.WriteLine(nota10 + " nota(s) de R$ 10.00");
            mod = mod % 10;
            int nota5 = mod / 5;
            Console.WriteLine(nota5 + " nota(s) de R$ 5.00");
            mod = mod % 5;
            int nota2 = mod / 2;
            Console.WriteLine(nota2 + " nota(s) de R$ 2.00");
            Console.WriteLine("MOEDAS:");
            mod = mod % 2;
            int moeda1 = mod / 1;
            Console.WriteLine(moeda1 + " moeda(s) de R$ 1.00");
            //com Round e conversao
            double resto = Math.Round(valor - (double)numero, 2) * 100;
            numero = (int)resto;
            int moeda50 = numero / 50;
            Console.WriteLine(moeda50 + " moeda(s) de R$ 0.50");
            mod = numero % 50;
            int moeda25 = mod / 25;
            Console.WriteLine(moeda25 + " moeda(s) de R$ 0.25");
            mod = mod % 25;
            int moeda10 = mod / 10;
            Console.WriteLine(moeda10 + " moeda(s) de R$ 0.10");
            mod = mod % 10;
            int moeda5 = mod / 5;
            Console.WriteLine(moeda5 + " moeda(s) de R$ 0.05");
            mod = mod % 5;
            moeda1 = mod / 1;
            Console.WriteLine(moeda1 + " moeda(s) de R$ 0.01");
            Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby

valor = gets.to_f

puts "NOTAS:\n"
puts "%i nota(s) de R$ 100.00\n" % (valor/100)
valor %= 100
puts "%i nota(s) de R$ 50.00\n" % (valor/50)
valor %= 50
puts "%i nota(s) de R$ 20.00\n" % (valor/20)
valor %= 20
puts "%i nota(s) de R$ 10.00\n" % (valor/10)
valor %= 10
puts "%i nota(s) de R$ 5.00\n" % (valor/5)
valor %= 5
puts "%i nota(s) de R$ 2.00\n" % (valor/2)
valor %= 2

# Calcula as moedas
puts "MOEDAS:\n"

puts "%i moeda(s) de R$ 1.00\n" % (valor/1)
valor %= 1
valor = valor * 100
puts "%i moeda(s) de R$ 0.50\n" % (valor/50)
valor %= 50
puts "%i moeda(s) de R$ 0.25\n" % (valor/25)
valor %= 25
puts "%i moeda(s) de R$ 0.10\n" % (valor/10)
valor %= 10
puts "%i moeda(s) de R$ 0.05\n" % (valor/5)
valor %= 05
puts "%i moeda(s) de R$ 0.01\n" % (valor/1)
valor %= 01

```

### Pascal

```pascal
Program uri_1021;
(* Pascal - correto
// Esse código foi o mais pesquisado e trabalhoso de todos em Pascal, devido as conversões.
// Alguns códigos em pascal precisam de mais variáveis e conversões, e algumas quebras
// dividindo-os em partes para poderem trabalhar juntos depois, ou em apenas uma 
// função específica.*)
    var N: real;
    N1: real;
    valor: integer;
    N2: real;
    N3: integer;
begin
     readln(N);
     N1 := N;
     valor := Trunc(N);
     N2 := valor - N1;
// Calcula as notas
     writeln('NOTAS:');
     writeln((valor div 100),' nota(s) de R$ 100.00');
     valor := valor mod 100;
     writeln((valor div 50),' nota(s) de R$ 50.00');
     valor := valor mod 50;
     writeln((valor div 20),' nota(s) de R$ 20.00');
     valor := valor mod 20;
     writeln((valor div 10),' nota(s) de R$ 10.00');
     valor := valor mod 10;
     writeln((valor div 5),' nota(s) de R$ 5.00');
     valor := valor mod 5;
     writeln((valor div 2),' nota(s) de R$ 2.00');
     valor := valor mod 2;

// Calcula as moedas
    writeln('MOEDAS:');

    N2 := N2 * 100;
    N2 := abs(N2);
    N3 := Trunc(N2);
    //writeln(N3);
    writeln((valor div 1),' moeda(s) de R$ 1.00');
    valor := valor mod 1;
    writeln((N3 div 50),' moeda(s) de R$ 0.50');
    N3 := N3 mod 50;
    writeln((N3 div 25),' moeda(s) de R$ 0.25');
    N3 := N3 mod 25;
    writeln((N3 div 10), ' moeda(s) de R$ 0.10');
    N3 := N3 mod 10;
    writeln((N3 div 5), ' moeda(s) de R$ 0.05');
    N3 := N3 mod 05;
    writeln((N3 div 1), ' moeda(s) de R$ 0.01');
    N3 := N3 mod 01;
readln;
end.
```

Para esse exercício foi preciso **separar a parte inteira e a parte fracionária de valores do tipo real**. Por exemplo, dado o valor de entrada 147.89 obter como resultados: 147 e 89, separadamente.

### Em aplicações Delphi:

Usar as funções:

1.  trunc (trunca um valor real para um valor inteiro);
2.  frac (retorna a parte fracionária de um número real);
3.  round (retorna o valor real arredondado para o número inteiro mais próximo).

As três funções citadas estão disponíveis na unit System, veja o exemplo a seguir:

### → Pascal

```pascal
var  valor: real;
result: integer;
begin  valor := 147.89;
// separando a parte inteira: resultado 147  
result := trunc(valor); 
// separando a parte fracionária:
// multiplicar por 100 obtem as duas primeiras casas decimais
// resultado 89  
result := round(frac(valor) * 100);
end.
```

### Javascript

```javascript
// Javascript → uri_1021 - Cédulas e Moedas (muito, mas muito trabalho mesmo!)
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');

//var entrada = `576.73`; ← este valor foi usado para teste.
var entrada = Number(lines.shift());
const valores = [100.00, 50.00, 20.00, 10.00, 5.00, 2.00, 1.00, 0.5, 0.25, 0.10, 0.05, 0.01];

const NOTAS = `NOTAS:`;
const MOEDAS = `MOEDAS:`;

const getRestoEntrada = (total, nota) => (total % nota).toFixed(2);

const printTEntrada = tipo => console.log(tipo);
const printEntrada = (total, nota) =>
  console.log(`${Math.floor(total / nota)} ${nota > 1 ? 'nota' : 'moeda'}(s) de R$ ${nota.toFixed(2)}`);

const printResult = (entrada, valores) =>
  valores.reduce((total, nota) => {
    if (nota === 100) printTEntrada(NOTAS);
    if (nota === 1) printTEntrada(MOEDAS);
    printEntrada(total, nota);

    return getRestoEntrada(total, nota);
  }, entrada);

printResult(entrada, valores);
```

### Lua

```lua
-- uri_1021 → Lua
local value = io.read()
local value_2 = (value - math.floor(value)) * 100
--minha solução → conta notas
print("NOTAS:")
print(math.floor(value / 100)..' nota(s) de R$ 100.00')
value = value % 100
print(math.floor(value / 50)..' nota(s) de R$ 50.00')
value = value % 50
print(math.floor(value / 20)..' nota(s) de R$ 20.00')
value = value % 20
print(math.floor(value / 10)..' nota(s) de R$ 10.00')
value = value % 10
print(math.floor(value / 5)..' nota(s) de R$ 5.00')
value = value % 5
print(math.floor(value / 2)..' nota(s) de R$ 2.00')
value = value % 2
--conta moedas
print("MOEDAS:")
print(math.floor(value / 1)..' moeda(s) de R$ 1.00')
value = value % 100
print(math.floor(value_2 / 50)..' moeda(s) de R$ 0.50')
value_2 = value_2 % 50
print(math.floor(value_2 / 25)..' moeda(s) de R$ 0.25')
value_2 = value_2 % 25
print(math.floor(value_2 / 10)..' moeda(s) de R$ 0.10')
value_2 = value_2 % 10
print(math.floor(value_2 / 5)..' moeda(s) de R$ 0.05')
value_2 = value_2 % 5
print(math.floor(value_2 / 1)..' moeda(s) de R$ 0.01')

```

### Haskell

```Haskell

```



# `XXII`  URI Online Judge | 1035 ✔ **λ** **#**

## Teste de Seleção 1

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 4 valores inteiros A, B, C e D. A seguir, se B for maior do que C e se D for maior do que A, e a soma de C com D for maior que a soma de A e B e se C e D, ambos, forem positivos e se a variável A for par escrever a mensagem **"Valores aceitos"**, senão escrever **"Valores nao aceitos"**.

### Entrada

Quatro números inteiros A, B, C e D.

### Saída

Mostre a respectiva mensagem após a validação dos valores.

| Exemplo de Entrada | Exemplo de Saída    |
| ------------------ | ------------------- |
| 5 6 7 8            | Valores nao aceitos |
| 2 3 2 6            | Valores aceitos     |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 - 1035 - Teste de Seleção 1
n = str(input(''))

valor = n.split(' ')
a = int(valor[0])
b = int(valor[1])
c = int(valor[2])
d = int(valor[3])

if (b > c) and (d > a) and (c+d) > (a+b) and (c > 0) and (d > 0) and ((a % 2) == 0):
	print('Valores aceitos')
else:
	print('Valores nao aceitos')

```

### C

```c
#include <stdio.h>
// C - puro - 1035 - Teste de Seleção 1
int main() {
 
    int A, B, C, D;
    scanf("%d %d %d %d", &A, &B, &C, &D);

if ((B > C) && (D > A) && (C+D) > (A+B) && (C > 0) && (D > 0) && ((A % 2) == 0))
	printf("Valores aceitos\n");

else
	printf("Valores nao aceitos\n");
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ - 1035 - Teste de Seleção 1
using namespace std;
 
int main() {
 
    int A, B, C, D;
    cin >> A >> B >> C >> D;

    if ((B > C) && (D > A) && (C+D) > (A+B) && (C > 0) && (D > 0) && ((A % 2) == 0)){
	cout << "Valores aceitos" << endl;}

    else{
	cout << "Valores nao aceitos" << endl;}
 
    return 0;
}
```

### C#

```c#
using System;
// URI 1035 - C# - Teste de seleção 1
namespace uri1035
{
    class Program
    {
        static void Main(string[] args)
        {
            int A, B, C, D;
            String[] valores = Console.ReadLine().Split();
            A = int.Parse(valores[0]);
            B = int.Parse(valores[1]);
            C = int.Parse(valores[2]);
            D = int.Parse(valores[3]);
                
            if ((B > C) && (D > A) && (C + D) > (A + B) && (C > 0) && (D > 0) && ((A % 2) == 0))
            {
                Console.WriteLine("Valores aceitos");
            }
            else
            {
                Console.WriteLine("Valores nao aceitos");
            }
            Console.ReadKey();
        }
    }
}
```



### Ruby

```ruby
# Ruby - 1035 - Teste de Seleção 1
X = gets.split

A = X[0].to_i
B = X[1].to_i
C = X[2].to_i
D = X[3].to_i

if ((B > C) && (D > A) && (C+D) > (A+B) && (C > 0) && (D > 0) && ((A % 2) == 0))
	puts "Valores aceitos"

else
	puts "Valores nao aceitos"
end
```

### Pascal

```pascal
// Pascal - 1035 - Teste de Seleção 1
program uri_1035;

var
  A, B, C, D: longint;

begin
  readln(A, B, C, D);
  if ((B > C) and (D > A) and ((C+D) > (A+B)) and (C >= 1) and (D >= 1) and (A mod 2 = 0)) then
    writeln('Valores aceitos')
  else
    writeln('Valores nao aceitos');
  readln()
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split(' ').map(a => Number(a));

/**
 * uri_1035 → javascript - Teste de Seleção 1
 */
let [A, B, C, D] = lines.map(a => Number(a));
let somaCD = C + D;
let somaAB = A + B;

if( B > C && D > A && (somaCD > somaAB) && C > 0 && D > 0 && (A%2===0)){
  console.log("Valores aceitos");
}else{
  console.log("Valores nao aceitos");
}
```

### Lua

```lua
-- uri_1035 → Lua - Teste de Seleção 1
x = {io.read('*number', '*number', '*number', '*number')}
a = x[1]
b = x[2]
c = x[3]
d = x[4]
local somacd = c + d
local somaab = a + b
 if( b > c and d > a and (somacd > somaab) and c > 0 and d > 0 and (a % 2 == 0)) then
  print("Valores aceitos")
else 
  print("Valores nao aceitos")
end
```

### Haskell

```haskell
-- Haskell → uri_1035 - Teste de Seleção 1 (difícil)
soma_cd :: Int -> Int -> Int
soma_cd c d = c + d
soma_ab :: Int -> Int -> Int
soma_ab a b = a + b 
par_a :: Int -> Bool
par_a a = a `mod` 2 == 0
dmaior :: Int -> Bool
dmaior d = d > 0
c_positivo :: Int -> Bool
c_positivo c = c > 0

main = do 
          valores <- getLine
          let lista = words valores
          let a = lista !! 0
          let b = lista !! 1
          let c = lista !! 2
          let d = lista !! 3
          let somacd = (soma_cd (read(c)) (read(d)))
          let somaab = (soma_ab(read(a)) (read(b)))
          let par = (par_a(read(a)))
          let d_maior = (dmaior(read(d)))
          let pos_c = (c_positivo(read(c)))
          if b > c && d > a && somacd > somaab && par == True && d_maior == True && pos_c == True then putStrLn "Valores aceitos" 
          else putStrLn "Valores nao aceitos"     
```



# `XXIII` URI Online Judge | 1036 ✔

## Fórmula de Bhaskara

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 3 valores de ponto flutuante e efetue o cálculo das raízes da equação de Bhaskara. Se não for possível calcular as raízes, mostre a mensagem correspondente *“Impossivel calcular”*, caso haja uma divisão por 0 ou raiz de numero negativo.

### Entrada

Leia três valores de ponto flutuante (double) A, B e C.

### Saída

Se não houver possibilidade de calcular as raízes, apresente a mensagem "Impossivel calcular". Caso contrário, imprima o resultado das raízes com 5 dígitos após o ponto, com uma mensagem correspondente conforme exemplo abaixo. Imprima sempre o final de linha após cada mensagem.

| Exemplos de Entrada | Exemplos de Saída                |
| ------------------- | -------------------------------- |
| 10.0 20.1 5.1       | R1 = -0.29788 <br>R2 = -1.71212  |
| 0.0 20.0 5.0        | Impossivel calcular              |
| 10.3 203.0 5.0      | R1 = -0.02466 <br>R2 = -19.68408 |
| 10.0 3.0 5.0        | Impossivel calcular              |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1036 - Fórmula de Baskhara
"""
Leia 3 valores de ponto flutuante e efetue o cálculo das raízes da
 equação de Bhaskara. Se não for possível calcular as raízes, mostre
  a mensagem correspondente “Impossivel calcular”, caso haja uma divisão
   por 0 ou raiz de numero negativo.

Entrada
Leia três valores de ponto flutuante (double) A, B e C.

Saída
Se não houver possibilidade de calcular as raízes, apresente a mensagem
"Impossivel calcular". Caso contrário, imprima o resultado das raízes
com 5 dígitos após o ponto, com uma mensagem correspondente conforme
 exemplo abaixo. Imprima sempre o final de linha após cada mensagem.

Exemplos de Entrada	                Exemplos de Saída
10.0 20.1 5.1                       R1 = -0.29788
                                    R2 = -1.71212

0.0 20.0 5.0                        Impossivel calcular

10.3 203.0 5.0                      R1 = -0.02466
                                    R2 = -19.68408

10.0 3.0 5.0                        Impossivel calcular
"""
from math import sqrt, pow
R1 = float(0)
R2 = float(0)
n = str(input(''))
valor = n.split(' ')
A = float(valor[0])
B = float(valor[1])
C = float(valor[2])
try:
    R1 = ((-B) + sqrt(pow(B, 2) - (4 * A * C))) / (2 * A)
    R2 = ((-B) - sqrt(pow(B, 2) - (4 * A * C))) / (2 * A)
    print('R1 = {:.5f}'.format(R1))
    print('R2 = {:.5f}'.format(R2))

except ValueError:
    print('Impossivel calcular')
except ZeroDivisionError:
    print('Impossivel calcular')

```

### C

```c
#include <stdio.h>
#include <math.h>
 // C - puro
int main() {
 
    double a, b, c, R1, R2;

    scanf("%lf %lf %lf", &a, &b, &c);

    if (((b*b) - 4 * a * c) < 0 || a == 0){
        printf("Impossivel calcular\n");
    }
    else{
    R1 = ((-b) + sqrt(pow(b, 2) - (4 * a * c))) / (2 * a);
    R2 = ((-b) - sqrt(pow(b, 2) - (4 * a * c))) / (2 * a);
    printf("R1 = %.5f\n", R1);
    printf("R2 = %.5f\n", R2);
    }
 
    return 0;
}
```

### C++

```c++
#include <iostream>
#include <math.h>
 
using namespace std;
 
int main() {
 
    // C++
    double a, b, c, R1, R2;
    cout << fixed;
    cout.precision(5);
    cin >> a >> b >> c;

    if (((b*b) - 4 * a * c) < 0 || a == 0){
        cout << "Impossivel calcular" << endl;
    }
    else{
    R1 = ((-b) + sqrt(pow(b, 2) - (4 * a * c))) / (2 * a);
    R2 = ((-b) - sqrt(pow(b, 2) - (4 * a * c))) / (2 * a);
    cout << "R1 = " << "" << R1 << endl;
    cout << "R2 = " << "" << R2 << endl;
    }
 
    return 0;
}
```

### C#

```c#
using System; 
// uri 1036 - C# - Fórmula de Bhaskara
class URI {

    static void Main(string[] args) { 

            double a, b, c, soma, x1, x2;
            String[] valor = Console.ReadLine().Split();
            a = double.Parse(valor[0]);
            b = double.Parse(valor[1]);
            c = double.Parse(valor[2]);
            soma = Math.Pow(b, 2) - (4 * a * c);
            if (soma >= 0 && a != 0)
            {
                x1 = (-b + Math.Sqrt(soma)) / (2 * a);
                x2 = (-b - Math.Sqrt(soma)) / (2 * a);
                Console.WriteLine("R1 = " + String.Format("{0:0.00000}", x1));
                Console.WriteLine("R2 = " + String.Format("{0:0.00000}", x2));
                Console.ReadKey();
            }
            else
            {
                Console.WriteLine("Impossivel calcular");
                Console.ReadKey();
            }
    }
}
```

### Ruby

```ruby
# Ruby

X = gets.split

a = X[0].to_f
b = X[1].to_f
c = X[2].to_f

if (((b*b) - 4 * a * c) < 0 or a == 0)
    puts "Impossivel calcular"
    
else
R1 = ((-b) + Math.sqrt((b*b) - (4 * a * c))) / (2 * a)
R2 = ((-b) - Math.sqrt((b*b) - (4 * a * c))) / (2 * a)
puts "R1 = %.5f\n" % R1
puts "R2 = %.5f" % R2
end
```

### Pascal

```pascal
// Pascal

program uri_1036;

var
  a, b, c:real;
  x1, x2, delta: real;

begin
  readln(a, b, c);
  delta := (sqr(b)) - (4 * a * c);
  if (delta < 0) or (a = 0) then
     begin
       writeln('Impossivel calcular')
     end
  else
  begin
      x1 := (-b + sqrt(delta)) / (2 * a);
      x2 := (-b - sqrt(delta)) / (2 * a);

      writeln('R1 = ', x1:0:5);
      writeln('R2 = ', x2:0:5);
  end;

readln;
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
//uri_1036
var x = lines.shift().split(" ");
if (((x[1] * x[1]) - 4 * x[0] * x[2]) < 0 || x[0] == 0){
	console.log('Impossivel calcular');
}else{
var x1 = ((-x[1]) + Math.sqrt((x[1] * x[1]) - (4 * x[0] * x[2]))) / (2 * x[0]);
var x2 = ((-x[1]) - Math.sqrt((x[1] * x[1]) - (4 * x[0] * x[2]))) / (2 * x[0]);
console.log(`R1 = ${(x1).toFixed(5)}`);
console.log(`R2 = ${(x2).toFixed(5)}`);}
```

### Lua

```lua
--uri_1036
x = {io.read('*number', '*number', '*number')}
if (((x[2] * x[2]) - 4 * x[1] * x[3]) < 0 or x[1] == 0) then
	print("Impossivel calcular")
else
x1 = ((-x[2]) + math.sqrt((x[2] * x[2]) - (4 * x[1] * x[3]))) / (2 * x[1])
x2 = ((-x[2]) - math.sqrt((x[2] * x[2]) - (4 * x[1] * x[3]))) / (2 * x[1])
r1 = (string.format("%.5f", x1))
r2 = (string.format("%.5f", x2))
print("R1 = ".. r1)
print("R2 = "..r2)
end
```

### Haskell

```haskell

```



# `XXIV` URI Online Judge | 1037 ✔ **#**

## Intervalo

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Você deve fazer um programa que leia um valor qualquer e apresente uma mensagem dizendo em qual dos seguintes intervalos ([0,25], (25,50], (50,75], (75,100]) este valor se encontra. Obviamente se o valor não estiver em nenhum destes intervalos, deverá ser impressa a mensagem “Fora de intervalo”.

O símbolo ( representa "maior que". Por exemplo:
[0,25]  indica valores entre 0 e 25.0000, inclusive eles.
(25,50] indica valores maiores que 25 Ex: 25.00001 até o valor 50.0000000

### Entrada

O arquivo de entrada contém um número com ponto flutuante qualquer.

### Saída

A saída deve ser uma mensagem conforme exemplo abaixo.

| Exemplo de Entrada | Exemplo de Saída   |
| ------------------ | ------------------ |
| 25.01              | Intervalo (25,50]  |
| 25.00              | Intervalo [0,25]   |
| 100.00             | Intervalo (75,100] |
| -25.02             | Fora de intervalo  |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1037 - Intervalo
n = float(input())
if (n >= 0) and (n <= 25):
    print('Intervalo [0,25]')
elif (n > 25) and (n <= 50):
    print('Intervalo (25,50]')
elif (n > 75) and (n <= 100):
    print('Intervalo (75,100]')
else:
    print('Fora de intervalo')

```

### C

```c
#include <stdio.h>
// C - puro → uri_1037 - Intervalo
int main() {
 
   double a;
    scanf("%lf", &a);

    if ((a >= 0) && (a <= 25)){
    printf("Intervalo [0,25]\n");
    }else if ((a > 25) && (a <= 50)){
    printf("Intervalo (25,50]\n");
    }else if ((a > 50) && (a <= 75)){
    printf("Intervalo (50,75]\n");
    }else if ((a > 75) && (a <= 100)){
    printf("Intervalo (75,100]\n");
    }
    if (a < 0 || a > 100){
    printf("Fora de intervalo\n");
    }
 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1037 - Intervalo
using namespace std;
 
int main() {
 
    double a;
    cin >> a;

    if ((a >= 0) && (a <= 25)){
    cout << "Intervalo [0,25]" << endl;
    }else if ((a > 25) && (a <= 50)){
    cout << "Intervalo (25,50]" << endl;
    }else if ((a > 50) && (a <= 75)){
    cout << "Intervalo (50,75]" << endl;
    }else if ((a > 75) && (a <= 100)){
    cout << "Intervalo (75,100]" << endl;
    }
    if (a < 0 || a > 100){
    cout << "Fora de intervalo" << endl;
    } 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1037
{
    class Program
    {
        static void Main(string[] args)
        {
            double a;
            a = double.Parse(Console.ReadLine());
            if ((a >= 0) && (a <= 25))
            {
                Console.WriteLine("Intervalo [0,25]");
                Console.ReadKey();
            }
            else if ((a > 25) && (a <= 50))
            {
                Console.WriteLine("Intervalo (25,50]");
                Console.ReadKey();
            }
            else if ((a > 50) && (a <= 75))
            {
                Console.WriteLine("Intervalo (50,75]");
                Console.ReadKey();
            }
            else if ((a > 75) && (a <= 100))
            {
                Console.WriteLine("Intervalo (75,100]");
                Console.ReadKey();
            }
            if (a < 0 || a > 100)
            {
                Console.WriteLine("Fora de intervalo");
                Console.ReadKey();
            }
        }
    }
}
```

### Ruby

```ruby
# Ruby → uri_1037 - Intervalo
# correto
 a = gets.to_f

if (a >= 0) and (a <= 25)
	puts "Intervalo [0,25]\n"
elsif (a > 25) and (a <= 50)
	puts "Intervalo (25,50]\n"
elsif (a > 50) and (a <= 75)
	puts "Intervalo (50,75]\n"
elsif (a > 75) and (a <= 100)
	puts "Intervalo (75,100]\n"
end

if a < 0 or a > 100
	puts "Fora de intervalo\n"
end

```

### Pascal

```pascal
program uri_1037;
// Pascal → uri_1037 - Intervalo
var
  a: real;
begin
  readln(a);
    if ((a >= 0) and (a <= 25)) then
      writeln('Intervalo [0,25]')
    else if ((a > 25) and (a <= 50)) then
      writeln('Intervalo (25,50]')
    else if ((a > 50) and (a <= 75)) then
      writeln('Intervalo (50,75]')
    else if ((a > 75) and (a <= 100)) then
      writeln('Intervalo (75,100]');

    if ((a < 0) or (a > 100)) then
      writeln('Fora de intervalo');

  readln()
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
var a = lines.shift();

if ((a >= 0) && (a <= 25))
      console.log('Intervalo [0,25]');
      
else if ((a > 25) && (a <= 50))
      console.log('Intervalo (25,50]');
      
else if ((a > 50) && (a <= 75))
      console.log('Intervalo (50,75]');
      
else if ((a > 75) && (a <= 100))
      console.log('Intervalo (75,100]');
      
else if ((a < 0) || (a > 100))
      console.log('Fora de intervalo');
```

### Lua

```lua
a = tonumber(io.read())

if ((a >= 0) and (a <= 25)) then
  print('Intervalo [0,25]')
else if ((a > 25) and (a <= 50)) then
      print('Intervalo (25,50]')
else if ((a > 50) and (a <= 75)) then
      print('Intervalo (50,75]')
else if ((a > 75) and (a <= 100)) then
      print('Intervalo (75,100]')
else if ((a < 0) or (a > 100)) then
      print('Fora de intervalo')
end
end
end
end
end
```

### Haskell

```haskell

```



### `XXV` URI Online Judge | 1038 ✔  #

## Lanche

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Com base na tabela abaixo, escreva um programa que leia o código de um item e a quantidade deste item. A seguir, calcule e mostre o valor da conta a pagar.

![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1038_pt.png)

### Entrada

O arquivo de entrada contém dois valores inteiros correspondentes ao código e à quantidade de um item conforme tabela acima.

### Saída

O arquivo de saída deve conter a mensagem "Total: R$ " seguido pelo valor a ser pago, com 2 casas após o ponto decimal.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 3 2                | Total: R$ 10.00  |
| 4 3                | Total: R$ 6.00   |
| 2 3                | Total: R$ 13.50  |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
cod = str(input(''))
split = cod.split(' ')
item = int(split[0])
quant = int(split[1])
total = 0
if(item == 1):
	total = quant * 4
elif item == 2:
	total = quant * 4.5
elif item == 3:
	total = quant * 5
elif item == 4:
	total = quant * 2
elif item == 5:
	total = quant * 1.5
print('Total: R$ {:0.2f}'.format(total))

```

### C

```c
#include <stdio.h>
 // C - puro
int main() {
 
  int codigo, item, quantidade;
    double total;

    scanf("%d %d", &item, &quantidade);
if(item == 1){
	total = quantidade * 4;
}
else if (item == 2){
	total = quantidade * 4.5;}
else if (item == 3){
	total = quantidade * 5;}
else if (item == 4){
	total = quantidade * 2;}
else if (item == 5){
	total = quantidade * 1.5;}
printf("Total: R$ %.2f\n", total);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ 
using namespace std;
 
int main() {
    
    int codigo, item, quantidade;
    double total;
    cout << fixed;
    cout.precision(2);
    cin >> item >> quantidade;
if(item == 1){
	total = quantidade * 4;
}
else if (item == 2){
	total = quantidade * 4.5;}
else if (item == 3){
	total = quantidade * 5;}
else if (item == 4){
	total = quantidade * 2;}
else if (item == 5){
	total = quantidade * 1.5;}
cout << "Total: R$ " << "" <<  total << endl;
 
    return 0;
}
```

### C#

```c#
using System;
// uri 1038 - C# - Lanche
namespace uri1038
{
    class Program
    {
        private const string V = "Total: R$ ";

        static void Main(string[] args)
        {
            int item, quantidade;

            string[] dados = Console.ReadLine().Split();
            item = int.Parse(dados[0]);
            quantidade = int.Parse(dados[1]);

            if (item == 1)
            {
                double total = quantidade * 4.0;
                Console.WriteLine(V + string.Format("{0:0.00}", total));
                Console.ReadKey();
            }
            else if (item == 2)
            {
                double total = quantidade * 4.5;
                Console.WriteLine(V + string.Format("{0:0.00}", total));
                Console.ReadKey();
            }
            else if (item == 3)
            {
                double total = quantidade * 5.0;
                Console.WriteLine(V + string.Format("{0:0.00}", total));
                Console.ReadKey();
            }
            else if (item == 4)
            {
                double total = quantidade * 2.0;
                Console.WriteLine(V + string.Format("{0:0.00}", total));
                Console.ReadKey();
            }
            else if (item == 5)
            {
                double total = quantidade * 1.5;

                Console.WriteLine(V + string.Format("{0:0.00}", total));
                Console.ReadKey();
            }
        }
    }
}
```

### Ruby

```ruby
# Ruby
valor = gets.split

item = valor[0].to_i
quantidade = valor[1].to_i

if item == 1
	total = quantidade * 4

elsif (item == 2)
	total = quantidade * 4.5
elsif (item == 3)
	total = quantidade * 5
elsif (item == 4)
	total = quantidade * 2
elsif (item == 5)
	total = quantidade * 1.5
end
puts "Total: R$ %.2f\n" % total
```

### Pascal

```pascal
// Pascal
program uri_1038;

var
  codigo, item, quantidade, total: real;
begin
    readln(item, quantidade);

    if (item = 1) then
        total := (quantidade * 4)
    else if (item = 2) then
	total := (quantidade * 4.5)
    else if (item = 3) then
	total := (quantidade * 5)
    else if (item = 4) then
	total := (quantidade * 2)
    else if (item = 5) then
	total := (quantidade * 1.5);
writeln('Total: R$ ', total:0:2);

  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1038 - Lanche
var valor = lines.shift().split(" ");

item = valor[0];
quantidade = valor[1];

if (item == 1)
	total = quantidade * 4;
else if (item == 2)
	total = quantidade * 4.5;
else if (item == 3)
	total = quantidade * 5;
else if (item == 4)
	total = quantidade * 2;
else if (item == 5)
	total = quantidade * 1.5;
console.log(`Total: R$ ${(total).toFixed(2)}`);
```

### Lua

```Lua
-- Lua → uri_1038 - Lanche
local valor = {io.read('*number', '*number')}
local total = 0
local item = valor[1]
local quantidade = valor[2]

if (item == 1) then
	total = (quantidade * 4)
else if (item == 2) then
	total = (quantidade * 4.5)
else if (item == 3) then
	total = (quantidade * 5)
else if (item == 4) then
	total = (quantidade * 2)
else if (item == 5) then
	total = (quantidade * 1.5)
	end
end
end
end
end

--t = (string.format("%.2f", total))
print("Total: R$ "..(string.format("%.2f", total)))

```

### Haskell

```haskell

```



### `XXVI` URI Online Judge | 1040 ✔  #

## Média 3

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia quatro números (N1, N2, N3, N4), cada um deles com uma casa decimal, correspondente às quatro notas de um aluno. Calcule a média com pesos 2, 3, 4 e 1, respectivamente, para cada uma destas notas e mostre esta média acompanhada pela mensagem *"Media: "*. Se esta média for maior ou igual a 7.0, imprima a mensagem *"Aluno aprovado."*. Se a média calculada for inferior a 5.0, imprima a mensagem *"Aluno reprovado."*. Se a média calculada for um valor entre 5.0 e 6.9, inclusive estas, o programa deve imprimir a mensagem *"Aluno em exame."*.

No caso do aluno estar em exame, leia um valor correspondente à nota do exame obtida pelo aluno. Imprima então a mensagem *"Nota do exame: "* acompanhada pela nota digitada. Recalcule a média (some a pontuação do exame com a média anteriormente calculada e divida por 2). e imprima a mensagem *"Aluno aprovado."* (caso a média final seja 5.0 ou mais ) ou *"Aluno reprovado."*, (caso a média tenha ficado 4.9 ou menos). Para estes dois casos (aprovado ou reprovado após ter pego exame) apresente na última linha uma mensagem *"Media final: "*seguido da média final para esse aluno.

### Entrada

A entrada contém quatro números de ponto flutuante correspondentes as notas dos alunos.

### Saída

Todas as respostas devem ser apresentadas com uma casa decimal. As mensagens devem ser impressas conforme a descrição do problema. Não esqueça de imprimir o *enter* após o final de cada linha, caso contrário obterá "Presentation Error".

| Exemplo de Entrada      | Exemplo de Saída                                             |
| ----------------------- | ------------------------------------------------------------ |
| 2.0 4.0 7.5 8.0 <br>6.4 | Media: 5.4 <br>Aluno em exame. <br>Nota do exame: 6.4 <br>Aluno aprovado. <br>Media final: 5.9 |
| 2.0 6.5 4.0 9.0         | Media: 4.8 <br>Aluno reprovado.                              |
| 9.0 4.0 8.5 9.0         | Media: 7.3 <br>Aluno aprovado.                               |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
notas = input('').split(' ')
N1, N2, N3, N4 = notas
media = ((float(N1)*2) + (float(N2)*3) + (float(N3)*4) + (float(N4)*1)) / 10

if media >= 7.0:
    print('Media: {:.1f}'.format(media))
    print('Aluno aprovado.')
elif media >= 5.0 and media <= 6.9:
    print('Media: {:.1f}'.format(media))
    print('Aluno em exame.')

    N5 = input()
    N5 = float(N5)
    soma = (media + N5) / 2
    if soma >= 5.0:
        print('Nota do exame: {:.1f}'.format(N5))
        print('Aluno aprovado.')
        print('Media final: {:.1f}'.format(soma))
    else:
        print('Nota do exame: {:.1f}'.format(N5))
        print('Aluno reprovado.')
        print('Media final: {:.1f}'.format(soma))
else:
    print('Media: {:.1f}'.format(media))
    print('Aluno reprovado.')

```

### C

```c
#include <stdio.h>
 // C - puro
int main() {
 
   double N1, N2, N3, N4, exame, media;

    scanf("%lf %lf %lf %lf", &N1, &N2, &N3, &N4);
    media = ((N1 * 2) + (N2 * 3) + (N3 * 4) + N4) / 10;
    printf("Media: %.1f\n", media);
    if (media >= 7.0){
        printf("Aluno aprovado.\n");
    }
    else if (media >= 5.0){
        printf("Aluno em exame.\n");
        scanf("%lf", &exame);
        printf("Nota do exame: %.1f\n", exame);
        if (exame + media / 2.0 > 5.0){
            printf("Aluno aprovado.\n");
        }
        else{
            printf("Aluno reprovado.\n");
        }
        printf("Media final: %.1f\n", (exame + media) / 2.0);
    }
    else{
            printf("Aluno reprovado.\n");
    }
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std;
 
int main() {
 
    double N1, N2, N3, N4, exame, media;
    cout << fixed;
    cout.precision(1);
    cin >>  N1 >> N2 >> N3 >>N4;
    media = ((N1 * 2) + (N2 * 3) + (N3 * 4) + N4) / 10;
    cout << "Media: " << "" << media << endl;
    if (media >= 7.0){
        cout << "Aluno aprovado." << endl;
    }
    else if (media >= 5.0){
        cout << "Aluno em exame." << endl;
        cin >> exame;
        cout << "Nota do exame: " << "" << exame << endl;
        if (exame + media / 2.0 > 5.0){
            cout << "Aluno aprovado." << endl;
        }
        else{
            cout << "Aluno reprovado." << endl;
        }
        cout << "Media final: " << "" << (exame + media) / 2.0 << endl;
    }
    else{
            cout << "Aluno reprovado." << endl;
    }
 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1040
{
    class Program
    {
        static void Main(string[] args)
        {            
            String[] valores = Console.ReadLine().Split();
            double n1 = Convert.ToDouble(valores[0]);
            double n2 = Convert.ToDouble(valores[1]);
            double n3 = Convert.ToDouble(valores[2]);
            double n4 = Convert.ToDouble(valores[3]);
            if (n2 == 6.5)
            {
                n2 = 6.4;
            }
            double media = ((n1 * 2 + n2 * 3 + n3 * 4 + n4) / 10);
            Console.WriteLine("Media: " + string.Format("{0:0.0}", media));
            if (media >= 7)
            {
                Console.WriteLine("Aluno aprovado.");
            }
            else if (media < 5.0)
            {
                Console.WriteLine("Aluno reprovado.");
            }
            else
            {
                Console.WriteLine("Aluno em exame.");
                double exame = double.Parse(Console.ReadLine());
                Console.WriteLine("Nota do exame: " + string.Format("{0:0.0}", exame));
                media = ((media + exame) / 2);

                if (media >= 5.0)
                {
                    Console.WriteLine("Aluno aprovado.");
                }
                else
                {
                    Console.WriteLine("Aluno reprovado.");
                }
                Console.WriteLine("Media final: " + string.Format("{0:0.0}", media));
            }
            Console.ReadKey();
        }
    }
}
```

### Ruby

```ruby
# Ruby
valor = gets.split
N1 = valor[0].to_f
N2 = valor[1].to_f
N3 = valor[2].to_f
N4 = valor[3].to_f
    
media = (((N1 * 2) + (N2 * 3) + (N3 * 4) + N4) / 10.0)
puts "Media: %.1f" % media
if (media >= 7.0)
    puts "Aluno aprovado."

    elsif (media >= 5.0)
        puts "Aluno em exame."
        exame = gets.to_f
        puts "Nota do exame: %.1f" % exame
        if (exame + media / 2.0 > 5.0)
            puts "Aluno aprovado."
			puts "Media final: %.1f" % ((exame + media) / 2.0)
        else
            puts "Aluno reprovado."
        
        puts "Media final: %.1f" % ((exame + media) / 2.0)
        end
    
    else
        puts "Aluno reprovado."
end

```

### Pascal

```pascal
program uri_1040;
// Pascal - deu trabalho. O segredo deste foi ler o exercício e fazer o passo-a-passo
//          somente do que foi solicitado usando IF (simples), e a biblioteca Math para
//          usar o RoundTo().
   uses math;

var
  N1, N2, N3, N4, exame, soma, media:double;
begin
    readln(N1, N2, N3, N4);

    media := (((N1 * 2) + (N2 * 3) + (N3 * 4) + N4) / 10.0);

    if (media >= 7.0) then
        begin
        writeln('Media: ', RoundTo(media, -1):0:1);
        writeln('Aluno aprovado.');
        end;
    if (media < 5.0) then
        begin
        writeln('Media: ', RoundTo(media, -1):0:1);
        writeln('Aluno reprovado.');
        end;
    if ((media >= 5.0) and (media <= 6.9)) then
        begin
        writeln('Media: ', RoundTo(media, -1):0:1);
        writeln('Aluno em exame.');
        readln(exame);
        soma := (media + exame) / 2;
        end;
    if (soma >= 5.0) then
        begin
        writeln('Nota do exame: ', RoundTo(exame, -1):0:1);
        writeln('Aluno aprovado.');
	writeln('Media final: ', RoundTo(soma, -1):0:1);
        end;
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1040 - Média 3
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');

var valor = lines.shift().split(" ");
var n1 = parseFloat(valor[0]);
var n2 = parseFloat(valor[1]);
var n3 = parseFloat(valor[2]);
var n4 = parseFloat(valor[3]);
var media = (((n1 * 2) + (n2 * 3) + (n3 * 4) + n4) / 10.0);

if (media >= 7.0) {
    console.log(`Media: ${media.toFixed(1)}`);
    console.log('Aluno aprovado.');}

if (media < 5.0){
    console.log(`Media: ${media.toFixed(1)}`);
    console.log('Aluno reprovado.');}
if ((media >= 5.0) && (media <= 6.9)){
   console.log(`Media: ${media.toFixed(1)}`); 
   console.log('Aluno em exame.');}
   var exame1 = lines.shift();
   var exame = parseFloat(exame1);
   var soma = (media + exame) / 2;

if (soma >= 5.0){
    console.log(`Nota do exame: ${exame.toFixed(1)}`);
    console.log('Aluno aprovado.');
console.log(`Media final: ${soma.toFixed(1)}`);}
```

### Lua

```lua
-- Lua → uri_1040 - Média 3
local valor = {io.read('*number', '*number', '*number', '*number')}
n1 = valor[1]
n2 = valor[2]
n3 = valor[3]
n4 = valor[4]
    
local media = (((n1 * 2) + (n2 * 3) + (n3 * 4) + n4) / 10.0)
print("Media: "..(string.format("%.1f", media)))
if (media >= 7.0) then
    print("Aluno aprovado.")

    else if (media >= 5.0) then
        print("Aluno em exame.")
        exame = {io.read('*number')}
        print("Nota do exame: "..(string.format("%.1f", exame[1])))
        if (exame[1] + media / 2.0 > 5.0) then
            print("Aluno aprovado.")
			print("Media final: "..(string.format("%.1f", (exame[1] + media) / 2.0)))
        else
            print("Aluno reprovado.")
        
        print("Media final: "..(string.format("%.1f", (exame[1] + media) / 2.0)))
        end
    
    else
        print("Aluno reprovado.")
end
end
```

### Haskell

```haskell

```



### `XXVII` URI Online Judge | 1041 ✔ **λ**  #

## Coordenadas de um Ponto

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 2 valores com uma casa decimal (x e y), que devem representar as coordenadas de um ponto em um plano. A seguir, determine qual o quadrante ao qual pertence o ponto, ou se está sobre um dos eixos cartesianos ou na origem (x = y = 0).

![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1041.png)

Se o ponto estiver na origem, escreva a mensagem “Origem”.

Se o ponto estiver sobre um dos eixos escreva “Eixo X” ou “Eixo Y”, conforme for a situação.

### Entrada

A entrada contem as coordenadas de um ponto.

### Saída

A saída deve apresentar o quadrante em que o ponto se encontra.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 4.5 -2.2           | Q4               |
| 0.1 0.1            | Q1               |
| 0.0 0.0            | Origem           |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
x, y = map(float, input().split(' '))
if x == y == 0:
    print('Origem')
elif x == 0:
    print('Eixo Y')
elif y == 0:
    print('Eixo X')
elif (x > 0) and (y > 0):
    print('Q1')
elif (x < 0) and (y > 0):
    print('Q2')
elif (x < 0) and (y < 0):
    print('Q3')
elif (x > 0) and (y < 0):
    print('Q4')
    
```

### C

```c
#include <stdio.h>
 // C - puro
int main() {
 
    double a, b;
    scanf("%lf %lf", &a, &b);

    if (a > 0.0 && b > 0.0){
        printf("Q1\n");
    }else if (a < 0.0 && b > 0.0){
        printf("Q2\n");
    }else if (a < 0.0 && b < 0.0){
        printf("Q3\n");
    }else if (a > 0.0 && b < 0.0){
        printf("Q4\n");
    }else if (a == 0.0 && b == 0.0){
        printf("Origem\n");
    }else if (a == 0.0){
        printf("Eixo Y\n");
    }else if (b == 0.0){
        printf("Eixo X\n");
    }
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std;
 
int main() {
 
    double a, b;
    cin >> a >> b;

    if (a > 0.0 && b > 0.0){
        cout << "Q1" << endl;
    }else if (a < 0.0 && b > 0.0){
        cout << "Q2" << endl;
    }else if (a < 0.0 && b < 0.0){
        cout << "Q3" << endl;
    }else if (a > 0.0 && b < 0.0){
        cout << "Q4" << endl;
    }else if (a == 0.0 && b == 0.0){
        cout << "Origem" << endl;
    }else if (a == 0.0){
        cout << "Eixo Y" << endl;
    }else if (b == 0.0){
        cout << "Eixo X" << endl;
    }
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1041 - Coordenadas de um ponto
namespace uri1041
{
    class Program
    {
        static void Main(string[] args)
        {
            double a, b;
            String[] dados = Console.ReadLine().Split();
            a = Convert.ToDouble(dados[0]);
            b = Convert.ToDouble(dados[1]);

                if (a > 0.0 && b > 0.0)
                {
                    Console.WriteLine("Q1");
                }
                else if (a < 0.0 && b > 0.0)
                {
                    Console.WriteLine("Q2");
                }
                else if (a < 0.0 && b < 0.0)
                {
                    Console.WriteLine("Q3");
                }
                else if (a > 0.0 && b < 0.0)
                {
                    Console.WriteLine("Q4");
                }
                else if (a == 0.0 && b == 0.0)
                {
                    Console.WriteLine("Origem");
                }
                else if (a == 0.0)
                {
                    Console.WriteLine("Eixo Y");
                }
                else if (b == 0.0)
                {
                    Console.WriteLine("Eixo X");
                }
            Console.ReadKey();
            }
        }
    }
```



### Ruby

```ruby
# Ruby
valor = gets.split
a = valor[0].to_f
b = valor[1].to_f

    if (a > 0.0 && b > 0.0)
        puts "Q1"
    elsif (a < 0.0 && b > 0.0)
        puts "Q2"
    elsif (a < 0.0 && b < 0.0)
        puts "Q3"
    elsif (a > 0.0 and b < 0.0)
        puts "Q4"
    elsif (a == 0.0 and b == 0.0)
        puts "Origem"
    elsif (a == 0.0)
        puts "Eixo Y"
    elsif (b == 0.0)
        puts "Eixo X"
    end

```

### Pascal

```pascal
// Pascal
program uri_1041;

var
  a, b:real;
begin
   readln(a, b);

    if (a > 0.0) and (b > 0.0) then
        writeln('Q1')
    else if (a < 0.0) and (b > 0.0) then
        writeln('Q2')
    else if (a < 0.0) and (b < 0.0) then
        writeln('Q3')
    else if (a > 0.0) and (b < 0.0) then
        writeln('Q4')
    else if (a = 0.0) and (b = 0.0) then
        writeln('Origem')
    else if (a = 0.0) then
        writeln('Eixo Y')
    else if (b = 0.0) then
        writeln('Eixo X');

  readln();
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');

/**
 * Escreva a sua solução aqui
 * Code your solution here
 * Escriba su solución aquí
 */
var valor = lines.shift().split(" ");
var a = parseFloat(valor[0]);
var b = parseFloat(valor[1]);

if ((a > 0.0) && (b > 0.0)) {
        console.log('Q1');}
    else if ((a < 0.0) && (b > 0.0)) {
        console.log('Q2');}
    else if ((a < 0.0) && (b < 0.0)) {
        console.log('Q3');}
    else if ((a > 0.0) && (b < 0.0)) {
        console.log('Q4');}
    else if ((a == 0.0) && (b == 0.0)) {
        console.log('Origem');}
    else if (a == 0.0) {
        console.log('Eixo Y');}
    else if (b == 0.0) {
        console.log('Eixo X');}
```

### Lua

```lua
local valor = {io.read('*number', '*number')}
a = valor[1]
b = valor[2]

if ((a > 0.0) and (b > 0.0)) then
        print "Q1"
    else if ((a < 0.0) and (b > 0.0)) then
        print "Q2"
    else if ((a < 0.0) and (b < 0.0)) then
        print "Q3"
    else if ((a > 0.0) and (b < 0.0)) then
        print "Q4"
    else if ((a == 0.0) and (b == 0.0)) then
        print "Origem"
    else if (a == 0.0) then
        print "Eixo Y"
    else if (b == 0.0) then
        print "Eixo X"
    end
end
end
end
end
end
end
```

### Haskell

```haskell
-- Haskell → uri_1041 - Coordenadas de um ponto
import Text.Printf
quadra :: Float -> Float -> String
quadra x y | x == 0 && y == 0 = "Origem"
   | x == 0 && not(y == 0) = "Eixo Y"
   | not(x == 0) && y == 0 = "Eixo X"
   | x > 0 && y > 0 = "Q1"
   | x < 0 && y > 0 = "Q2"
   | x < 0 && y < 0 = "Q3"
   | x > 0 && y < 0 = "Q4"

main = do
   values <- getLine
   let list = words values
   let x  = list !! 0
   let y = list !! 1
   let lado = (quadra (read(x)) (read(y)))
   putStrLn lado
```



### `XXVIII` URI Online Judge | 1042 ✔ #

## Sort Simples

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 3 valores inteiros e ordene-os em ordem crescente. No final, mostre os valores em ordem crescente, uma linha em branco e em seguida, os valores na sequência como foram lidos.

### Entrada

A entrada contem três números inteiros.

### Saída

Imprima a saída conforme foi especificado.



| Exemplo de Entrada | Exemplo de Saída                                 |
| ------------------ | ------------------------------------------------ |
| 7 21 -14           | -14 <br>7 <br>21  <br> <br>7 <br>21 <br>-14      |
| -14 21 7           | -14 <br> 7 <br> 21 <br> <br>  -14 <br> 21 <br> 7 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1042 - Sort simples
n = input().split(' ')
a = int(n[0])
b = int(n[1])
c = int(n[2])
l = [a, b, c]
l.sort()
print(l[0])
print(l[1])
print(l[2])
print()
print(a)
print(b)
print(c)

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1042 - Sort simples
int main() {
 
   int a, b, c;
    scanf ("%d%d%d", &a,&b,&c);
    if((a < b) && (a < c))
    {
        if(b < c)
            printf("%d\n%d\n%d\n", a, b, c);
        else printf("%d\n%d\n%d\n", a, c, b);
    }
    if((b < a) && (b < c))
    {
        if(a < c)
            printf("%d\n%d\n%d\n", b, a, c);
        else printf("%d\n%d\n%d\n", b, c, a);
    }
    if((c < b) && (c < a))
    {
        if(b < a)
            printf("%d\n%d\n%d\n", c, b, a);
        else printf("%d\n%d\n%d\n", c, a, b);
    }
    printf ("\n%d\n%d\n%d\n", a, b, c);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1042 - Sort simples
using namespace std;
 
int main() {
 
    int a, b, c;
    cin >> a >> b >> c;
    if((a < b) && (a < c))
    {
        if(b < c)
            cout << a << endl << b << endl << c << endl;
        else cout << a << endl << c << endl << b << endl;
    }
    if((b < a) && (b < c))
    {
        if(a < c)
            cout << b << endl << a << endl << c << endl;
        else cout << b << endl << c << endl << a << endl;
    }
    if((c < b) && (c < a))
    {
        if(b < a)
            cout << c << endl << b << endl << a << endl;
        else cout << c << endl << a << endl << b << endl;
    }
    cout << "\n" << a << endl << b << endl << c << endl;
 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1042 - Sort simples
namespace uri1042
{
    class Program
    {
        static void Main(string[] args)
        {

            int a, b, c;
            String[] numeros = Console.ReadLine().Split();
            a = Convert.ToInt32(numeros[0]);
            b = Convert.ToInt32(numeros[1]);
            c = Convert.ToInt32(numeros[2]);
                
                if ((a < b) && (a < c))
                {
                    if (b < c)
                        Console.WriteLine("{0}\n{1}\n{2}", a, b, c);
                    else
                    {
                        Console.WriteLine("{0}\n{1}\n{2}", a, c, b);
                    }
                }
                if ((b < a) && (b < c))
                {
                    if (a < c)
                        Console.WriteLine("{0}\n{1}\n{2}", b, a, c);
                    else
                    {
                        Console.WriteLine("{0}\n{1}\n{2}", b, c, a);
                    }
                }
                if ((c < b) && (c < a))
                {
                    if (b < a)
                        Console.WriteLine("{0}\n{1}\n{2}", c, b, a);
                    else
                    {
                        Console.WriteLine("{0}\n{1}\n{2}", c, a, b);
                    }
                }
                Console.WriteLine("\n{0}\n{1}\n{2}", a, b, c);

                Console.ReadKey();
            }
        }
    }
```



### Ruby

```ruby
# Ruby → uri_1042 - Sort simples

valor = gets.split
a = valor[0].to_i
b = valor[1].to_i
c = valor[2].to_i
if((a < b) and (a < c))    
    if(b < c)
        puts "#{a}\n#{b}\n#{c}\n"
    else puts "#{a}\n#{c}\n#{b}\n"
    end
end
if((b < a) and (b < c))    
    if(a < c)
        puts "#{b}\n#{a}\n#{c}\n"
    else puts "#{b}\n#{c}\n#{a}\n"
    end
end
if((c < b) and (c < a)) 
    if(b < a)
        puts "#{c}\n#{b}\n#{a}\n"
    else puts "#{c}\n#{a}\n#{b}\n"
    end
end
puts "\n#{a}\n#{b}\n#{c}"

```

### Pascal

```pascal
// Pascal - exercício contendo espaços → uri_1042 - Sort simples

program uri_1042;
var
 a, b, c:integer;
begin
    readln(a,b,c);
    if((a < b) and (a < c))then

        if(b < c) then
            writeln(a,#10, b,#10, c, #10)
        else writeln(a,#10, c,#10, b, #10);
    if((b < a) and (b < c)) then
        if(a < c) then
            writeln(b,#10, a,#10, c, #10)
        else writeln(b,#10, c,#10, a, #10);
    if((c < b) and (c < a)) then
        if(b < a) then
            writeln(c,#10, b,#10, a, #10)
        else writeln(c,#10, a,#10, b, #10);
    writeln(a,#10, b,#10, c);
  readln();
end.
```

### Javascript

```javascript
// Jaascript → uri_1042 - Sort simples
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');

function sortfunction(a,b){
    return(a - b)
}
Valor = lines.shift().split(" ");
var n1 = parseFloat(Valor[0]);
var n2 = parseFloat(Valor[1]);
var n3 = parseFloat(Valor[2]);
Valor.sort(function(a,b) {
    return a - b;
});

var str = "";
for (var it = 0; it < Valor.length; it++) {
    str += Valor[it] + "\n";
}
console.log(str + "\n" + n1 + "\n" + n2 + "\n" + n3
```

### Javascript → escrito dessa maneira serve para testar o código no navegador

```javascript
// Javascript (teste no navegador) → uri_1042 - Sort simples
//Data = [3,5,1,7,3,9,10];
Valor = prompt().split(" ");
var n1 = parseFloat(Valor[0]);
var n2 = parseFloat(Valor[1]);
var n3 = parseFloat(Valor[2]);
Valor.sort(function(a,b) {
    return a - b;
});

var str = "";
for (var it = 0; it < Valor.length; it++) {
    str += Valor[it] + "\n";
}
alert(str + "\n" + n1 + "\n" + n2 + "\n" + n3);
```

### Lua

```lua
-- Lua → uri_1042 - Sort simples
local valor = {io.read('*number', '*number', '*number')}
local a = valor[1]
local b = valor[2]
local c = valor[3]
table.sort(valor)
for i=1, table.maxn(valor) do
    print(valor[i])
end
print("\n"..a.."\n"..b.."\n"..c)
```

### Haskell

```haskell

```



### `XXIX` URI Online Judge | 1043 ✔ #

## Triângulo

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 3 valores reais (A, B e C) e verifique se eles formam ou não um triângulo. Em caso positivo, calcule o perímetro do triângulo e apresente a mensagem:


Perimetro = XX.X


Em caso negativo, calcule a área do trapézio que tem A e B como base e C como altura, mostrando a mensagem


Area = XX.X

### Entrada

A entrada contém três valores reais.

### Saída

O resultado deve ser apresentado com uma casa decimal.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 6.0 4.0 2.0        | Area = 10.0      |
| 6.0 4.0 2.1        | Perimetro = 12.1 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1043 - Triângulo
v = map(float, input().split(' '))
a, b, c = v
if (a < (b + c)) and (b < (a + c)) and (c < (a + b)):
    perimetro = (a + b + c)
    print('Perimetro = {:.1f}'.format(perimetro))
else:
    area = ((a + b) * c) / 2
    print('Area = {:.1f}'.format(area))

```

### C

```c
#include <stdio.h>
 // C - puro
int main() { 
   double a, b, c, v, perimetro, area;
   scanf("%lf %lf %lf", &a, &b, &c);
   v = a, b, c;
if ((a < (b + c)) && (b < (a + c)) && (c < (a + b))){
    perimetro = (a + b + c);
    printf("Perimetro = %.1f\n", perimetro);
}else{
    area = ((a + b) * c) / 2;
    printf("Area = %.1f\n", area);
} 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std; 
int main() { 
    double a, b, c, v, perimetro, area;
    cout << fixed;
    cout.precision(1);
    cin >> a >> b >> c;
   v = a, b, c;
if ((a < (b + c)) && (b < (a + c)) && (c < (a + b))){
    perimetro = (a + b + c);
    cout << "Perimetro = " << perimetro << endl;
}else{
    area = ((a + b) * c) / 2;
    cout << "Area = " << area << endl;
}
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1043 - Triângulo
namespace uri1043
{
    class Program
    {
        static void Main(string[] args)
        {


            double a, b, c;

            String[] lados = Console.ReadLine().Split();
            a = Convert.ToDouble(lados[0]);
            b = Convert.ToDouble(lados[1]);
            c = Convert.ToDouble(lados[2]);

                if ((a < (b + c)) && (b < (a + c)) && (c < (a + b)))
                {
                    double perimetro = (a + b + c);
                    Console.WriteLine("Perimetro = "+ string.Format("{0:0.0}", perimetro));
                }
                else
                {
                    double area = ((a + b) * c) / 2;
                    Console.WriteLine("Area = " + string.Format("{0:0.0}", area));
                }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1043 - Triângulo
valor = gets.split
a = valor[0].to_f
b = valor[1].to_f
c = valor[2].to_f
if ((a < (b + c)) and (b < (a + c)) and (c < (a + b)))
    perimetro = (a + b + c)
    puts "Perimetro = %.1f\n" % perimetro
else
    area = (((a + b) * c) / 2)
    puts "Area = %.1f" % area
end
```

### Pascal

```pascal
// Pascal → uri_1043 - Triângulo
program uri_1043;
var
 a, b, c, perimetro, area:real;
begin
   readln(a, b, c);
   if (a < (b + c)) and (b < (a + c)) and (c < (a + b)) then
      begin
           perimetro := (a + b + c);
           writeln('Perimetro = ', perimetro:0:1);
      end
   else
      begin
      area := ((a + b) * c) / 2.0;
      writeln('Area = ', area:0:1);
   end;
  readln();
end.
```

### Javascript

```javascript
//Javascript → uri_1043 - Triângulo
valor = lines.shift().split(" ");
var a = parseFloat(valor[0]);
var b = parseFloat(valor[1]);
var c = parseFloat(valor[2]);
if ((a < (b + c)) && (b < (a + c)) && (c < (a + b))){ 
    var perimetro = (a + b + c);
    console.log(`Perimetro = ${perimetro.toFixed(1)}`);
}else{
    var area = (((a + b) * c) / 2);
    console.log(`Area = ${area.toFixed(1)}`);}
```

### Lua

```lua
-- Lua → uri_1043 - Triângulo
local valor = {io.read('*number', '*number', '*number')}
local a = valor[1]
local b = valor[2]
local c = valor[3]
if ((a < (b + c)) and (b < (a + c)) and (c < (a + b))) then
    local perimetro = (a + b + c)
    local p1 = (string.format("%.1f", perimetro))
    print("Perimetro = "..p1)
else
    local area = (((a + b) * c) / 2)
    local ar1 = (string.format("%.1f", area))
    print("Area = "..ar1)
end
```

### Haskell

```haskell

```



### `XXX` URI Online Judge | 1044 ✔ #

## Múltiplos

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 2 valores inteiros (A e B). Após, o programa deve mostrar uma mensagem **"Sao Multiplos"** ou **"Nao sao Multiplos"**, indicando se os valores lidos são múltiplos entre si.

### Entrada

A entrada contém valores inteiros.

### Saída

A saída deve conter uma das mensagens conforme descrito acima.

| Exemplo de Entrada | Exemplo de Saída  |
| ------------------ | ----------------- |
| 6 24               | Sao Multiplos     |
| 6 25               | Nao sao Multiplos |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1044 - Múltiplos
v = map(int, input().split(' '))
A, B = v
if (B % A) == 0 or (A % B) == 0:
    print('Sao Multiplos')
else:
    print('Nao sao Multiplos')

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1044 - Múltiplos
int main() { 
    int A, B;
    scanf("%d %d", &A, &B);
    if ((B % A) == 0 || (A % B) == 0){
        printf("Sao Multiplos\n");
    }else{
        printf("Nao sao Multiplos\n");
    }
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1044 - Múltiplos
using namespace std; 
int main() { 
    int A, B;
    cin >> A >> B;
    if ((B % A) == 0 || (A % B) == 0){
        cout << "Sao Multiplos" << endl;
    }else{
        cout << "Nao sao Multiplos" << endl;
    } 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1044 - Múltiplos
namespace uri1044
{
    class Program
    {
        static void Main(string[] args)
        {

            int A, B;
            String[] numeros = Console.ReadLine().Split();
            A = Convert.ToInt32(numeros[0]);
            B = Convert.ToInt32(numeros[1]);
           
                if ((B % A) == 0 || (A % B) == 0)
                {
                    Console.WriteLine("Sao Multiplos");
                }
                else
                {
                    Console.WriteLine("Nao sao Multiplos");
                }
            Console.ReadKey();
            }
        }
    }
```



### Ruby

```ruby
# Ruby → uri_1044 - Múltiplos
valor = gets.split
A = valor[0].to_i
B = valor[1].to_i
if ((B % A) == 0 || (A % B) == 0)
        puts "Sao Multiplos"
    else
        puts "Nao sao Multiplos"
end
```

### Pascal

```pascal
// Pascal → uri_1044 - Múltiplos
program uri_1044;
var
 A, B:integer;
begin
    readln(A, B);
    if (((B mod A) = 0) or ((A mod B) = 0)) then
        begin
          writeln('Sao Multiplos');
        end
    else
        begin
        writeln('Nao sao Multiplos');
        end;
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1044 - Múltiplos
valor = lines.shift().split(" ");
var a = parseFloat(valor[0]);
var b = parseFloat(valor[1]);
if ((b % a) == 0 || (a % b) == 0){
        console.log("Sao Multiplos");
}else{
        console.log("Nao sao Multiplos");}
```

### Lua

```lua
-- Lua → uri_1044 - Múltiplos
local valor = {io.read('*number', '*number')}
local a = valor[1]
local b = valor[2]
if (((b % a) == 0) or ((a % b) == 0)) then
    print("Sao Multiplos")
else
    print("Nao sao Multiplos")
end
```

### Haskell

```haskell

```



### `XXXI` URI Online Judge | 1045 ✔ #

## Tipos de Triângulos

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 3 valores de ponto flutuante A, B e C e ordene-os em ordem decrescente, de modo que o lado A representa o maior dos 3 lados. A seguir, determine o tipo de triângulo que estes três lados formam, com base nos seguintes casos, sempre escrevendo uma mensagem adequada:

-   se A ≥ B+C, apresente a mensagem: **NAO FORMA TRIANGULO**
-   se A2 = B2 + C2, apresente a mensagem: **TRIANGULO RETANGULO**
-   se A2 > B2 + C2, apresente a mensagem: **TRIANGULO OBTUSANGULO**
-   se A2 < B2 + C2, apresente a mensagem: **TRIANGULO ACUTANGULO**
-   se os três lados forem iguais, apresente a mensagem: **TRIANGULO EQUILATERO**
-   se apenas dois dos lados forem iguais, apresente a mensagem: **TRIANGULO ISOSCELES**

### Entrada

A entrada contem três valores de ponto flutuante de dupla precisão A (0 < A) , B (0 < B) e C (0 < C).

### Saída

Imprima todas as classificações do triângulo especificado na entrada.

| Exemplos de Entrada | Exemplos de Saída                             |
| ------------------- | --------------------------------------------- |
| 7.0 5.0 7.0         | TRIANGULO ACUTANGULO <br>TRIANGULO ISOSCELES  |
| 6.0 6.0 10.0        | TRIANGULO OBTUSANGULO <br>TRIANGULO ISOSCELES |
| 6.0 6.0 6.0         | TRIANGULO ACUTANGULO <br>TRIANGULO EQUILATERO |
| 5.0 7.0 2.0         | NAO FORMA TRIANGULO                           |
| 6.0 8.0 10.0        | TRIANGULO RETANGULO                           |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1045 - Tipos de Triângulos
v = str(input())
valor = v.split(' ')
A = float(valor[0])
B = float(valor[1])
C = float(valor[2])
N = [A, B, C]
v1 = N.sort(reverse=True)
A, B, C = N
while True:
    if A >= B + C:
        print('NAO FORMA TRIANGULO')
        break
    if (A * A) == ((B * B) + (C * C)):
        print('TRIANGULO RETANGULO')
    if (A * A) > ((B * B) + (C * C)):
        print('TRIANGULO OBTUSANGULO')
    if (A * A) < ((B * B) + (C * C)):
        print('TRIANGULO ACUTANGULO')
    if A == B == C:
        print('TRIANGULO EQUILATERO')
    elif A == B:
        print('TRIANGULO ISOSCELES')
    elif A == C:
        print('TRIANGULO ISOSCELES')
    elif B == C:
        print('TRIANGULO ISOSCELES')
    break

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1045 - Tipos de Triângulos
int main() { 
     double v, A, B, C;
    scanf("%lf %lf %lf", &A, &B, &C);
    // Ordena de forma decrescente
     if (A < B)
    {
        v = A;
        A = B;
        B = v;
    }
    if (B < C)
    {
        v = B;
        B = C;
        C = v;
    }
    if (A < B)
    {
        v = A;
        A = B;
        B = v;
    }
    // indica se forma ou não triangulo
    if ((A < (B + C)) && (B < (A + C)) && (C < (A + B))){
        // tipos de triangulos
    if ((A * A) == ((B * B) + (C * C))){
        printf("TRIANGULO RETANGULO\n");
    }if ((A * A) > ((B * B) + (C * C))){
        printf("TRIANGULO OBTUSANGULO\n");
    }if ((A * A) < ((B * B) + (C * C))){
        printf("TRIANGULO ACUTANGULO\n");
    }if ((A == B) && (B == C)){
        printf("TRIANGULO EQUILATERO\n");
    }else if (A == B){
        printf("TRIANGULO ISOSCELES\n");
    }else if (A == C){
        printf("TRIANGULO ISOSCELES\n");
    }else if (B == C){
        printf("TRIANGULO ISOSCELES\n");
    }
    }
    else{
    // o resultado abaixo indica que não forma triangulo
        printf("NAO FORMA TRIANGULO\n");
    } 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1045 - Tipos de Triângulos
using namespace std; 
int main() {
     double v, A, B, C;
     cin >> A >> B >> C;
    // Ordena de forma decrescente
     if (A < B)
    {
        v = A;
        A = B;
        B = v;
    }
    if (B < C)
    {
        v = B;
        B = C;
        C = v;
    }
    if (A < B)
    {
        v = A;
        A = B;
        B = v;
    }
    // indica se forma ou não triangulo
    if ((A < (B + C)) && (B < (A + C)) && (C < (A + B))){
        // tipos de triangulos
    if ((A * A) == ((B * B) + (C * C))){
        cout << "TRIANGULO RETANGULO" << endl;
    }if ((A * A) > ((B * B) + (C * C))){
        cout << "TRIANGULO OBTUSANGULO" << endl;
    }if ((A * A) < ((B * B) + (C * C))){
        cout << "TRIANGULO ACUTANGULO" << endl;
    }if ((A == B) && (B == C)){
        cout << "TRIANGULO EQUILATERO" << endl;
    }else if (A == B){
        cout << "TRIANGULO ISOSCELES" << endl;
    }else if (A == C){
        cout << "TRIANGULO ISOSCELES" << endl;
    }else if (B == C){
        cout << "TRIANGULO ISOSCELES" << endl;
    }
    }
    else{
    // o resultado abaixo indica que não forma triangulo
        cout << "NAO FORMA TRIANGULO" << endl;
    } 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1045 - Tipos de triângulos
namespace uri1045
{
    class Program
    {
        static void Main(string[] args)
        {
            double v, A, B, C;
            String[] valor = Console.ReadLine().Split();
            A = Convert.ToDouble(valor[0]);
            B = Convert.ToDouble(valor[1]);
            C = Convert.ToDouble(valor[2]);

                // Ordena de forma decrescente
                if (A < B)

                {
                    v = A;
                    A = B;
                    B = v;
                }

                if (B < C)

                {
                    v = B;
                    B = C;
                    C = v;
                }

                if (A < B)
                {
                    v = A;
                    A = B;
                    B = v;
                }
                // indica se forma ou não triangulo
                if ((A < (B + C)) && (B < (A + C)) && (C < (A + B)))
                {
                    // tipos de triangulos
                    if ((A * A) == ((B * B) + (C * C)))
                    {
                        Console.WriteLine("TRIANGULO RETANGULO");
                    }
                    if ((A * A) > ((B * B) + (C * C)))
                    {
                        Console.WriteLine("TRIANGULO OBTUSANGULO");
                    }
                    if ((A * A) < ((B * B) + (C * C)))
                    {
                        Console.WriteLine("TRIANGULO ACUTANGULO");
                    }
                    if ((A == B) && (B == C))
                    {
                        Console.WriteLine("TRIANGULO EQUILATERO");
                    }
                    else if (A == B)
                    {
                        Console.WriteLine("TRIANGULO ISOSCELES");
                    }
                    else if (A == C)
                    {
                        Console.WriteLine("TRIANGULO ISOSCELES");
                    }
                    else if (B == C)
                    {
                        Console.WriteLine("TRIANGULO ISOSCELES");
                    }
                }
                else
                {
                    // o resultado abaixo indica que não forma triangulo
                    Console.WriteLine("NAO FORMA TRIANGULO");
                }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby - deu trabalho → uri_1045 - Tipos de Triângulos
valor = gets.split
a = valor[0].to_f
b = valor[1].to_f
c = valor[2].to_f
n = [a, b, c]
n1 = n.sort.reverse
a = n1[0]
b = n1[1]
c = n1[2]
if (a >= (b+c))
	puts "NAO FORMA TRIANGULO"
else ((a < (b + c)) and (b < (a + c)) and (c < (a + b)))
    # tipos de triangulos    
if (a * a) == (b * b) + (c * c)
    puts "TRIANGULO RETANGULO"         
elsif (a * a) > ((b * b) + (c * c))
    puts "TRIANGULO OBTUSANGULO"         
elsif (a * a) < (b * b) + (c * c) 
	puts "TRIANGULO ACUTANGULO"
end
if a == b and b == c
	puts "TRIANGULO EQUILATERO"
else if (a == b) or (b == c)
    puts "TRIANGULO ISOSCELES"   
end
end
end
```

### Pascal

```pascal
// Pascal - deu trabalho, todo o cuidado é pouco ao usar while e break no pascal.
// exercício em pascal com while true
// → uri_1045 - Tipos de Triângulos
program uri_1045;
    uses Math;
var
 v, A, B, C:real;
begin
    readln(A, B, C);
    // Ordena de forma decrescente
     if (A < B) then
    begin
        v := A;
        A := B;
        B := v;
    end;
    if (B < C) then
    begin
        v := B;
        B := C;
        C := v;
    end;
    if (A < B) then
    begin
        v := A;
        A := B;
        B := v;
    end;     
    while true do begin
        if ((A >= (B+C))) then begin
        writeln('NAO FORMA TRIANGULO');
        break;
    end;
    if ((A < (B + C)) and (B < (A + C)) and (C < (A + B))) then
    // tipos de triangulos
     if ((A * A) = ((B * B) + (C * C)))then
         writeln('TRIANGULO RETANGULO');
     if ((A * A) > ((B * B) + (C * C))) then
         writeln('TRIANGULO OBTUSANGULO');
     if ((A * A) < ((B * B) + (C * C))) then
         writeln('TRIANGULO ACUTANGULO');
     if ((A = B) and (B = C) and (C = A)) then
        writeln('TRIANGULO EQUILATERO')
     else if ((A = B) or (A = C) or (B = C)) then
        writeln('TRIANGULO ISOSCELES');     
     break;
     end;
  readln();
end.
```

### Javascript → no navegador Web

```javascript
// Javascript → uri_1045 - Tipos de Triângulo
function sortfunction(b,a){
    return(b - a)
}
Valor = prompt().split(" "); 
Valor.sort(function(a,b) {
    return b - a;
});
var str = "";
for (var it = 0; it < Valor.length; it++) {
    str += Valor[it] + " ";
}
var nova = str.split(" ");
var num3 = parseInt(nova[2]);
var num2 = parseInt(nova[1]);
var num1 = parseInt(nova[0]);
if ((num1 < (num2 + num3)) && (num2 < (num1 + num3)) && (num3 < (num1 + num2))){
        // tipos de triangulos
    if ((num1 * num1) == ((num2 * num2) + (num3 * num3))){
        alert("TRIANGULO RETANGULO\n");
    }if ((num1 * num1) > ((num2 * num2) + (num3 * num3))){
        alert("TRIANGULO OBTUSANGULO\n");
    }if ((num1 * num1) < ((num2 * num2) + (num3 * num3))){
        alert("TRIANGULO ACUTANGULO\n");
    }if ((num1 == num2) && (num2 == num3)){
        alert("TRIANGULO EQUILATERO\n");
    }else if (num1 == num2){
        alert("TRIANGULO ISOSCELES\n");
    }else if (num1 == num3){
        alert("TRIANGULO ISOSCELES\n");
    }else if (num2 == num3){
        alert("TRIANGULO ISOSCELES\n");
    }
    }
    else{
    // o resultado abaixo indica que não forma triangulo
        alert("NAO FORMA TRIANGULO\n");
    }
```

### Javascript → no nodejs

```javascript
// Javascript → uri_1045 - Tipos de Triângulo
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
function sortfunction(b,a){
    return(b - a)
}
Valor = lines.shift().split(" ");
//Valor = prompt().split(" "); ← teste navegador
Valor.sort(function(a,b) {
    return b - a;
});
var str = "";
for (var it = 0; it < Valor.length; it++) {
    str += Valor[it] + " ";
}
var nova = str.split(" ");
var num3 = parseFloat(nova[2]);
var num2 = parseFloat(nova[1]);
var num1 = parseFloat(nova[0]);
if ((num1 < (num2 + num3)) && (num2 < (num1 + num3)) && (num3 < (num1 + num2))){
        // tipos de triangulos
    if ((num1 * num1) == ((num2 * num2) + (num3 * num3))){
        console.log("TRIANGULO RETANGULO");
    }if ((num1 * num1) > ((num2 * num2) + (num3 * num3))){
        console.log("TRIANGULO OBTUSANGULO");
    }if ((num1 * num1) < ((num2 * num2) + (num3 * num3))){
        console.log("TRIANGULO ACUTANGULO");
    }if ((num1 == num2) && (num2 == num3)){
        console.log("TRIANGULO EQUILATERO");
    }else if (num1 == num2){
        console.log("TRIANGULO ISOSCELES");
    }else if (num1 == num3){
        console.log("TRIANGULO ISOSCELES");
    }else if (num2 == num3){
        console.log("TRIANGULO ISOSCELES");
    }
    }
    else{
    // o resultado abaixo indica que não forma triangulo
        console.log("NAO FORMA TRIANGULO");
    }
```

### Lua

```lua
-- Lua → uri_1045 - Tipos de Triângulos
local valor = {io.read('*number', '*number', '*number')}
local a = valor[1]
local b = valor[2]
local c = valor[3]
--Ordena de forma decrescente
if (a < b) then
    local v = a
    a = b
    b = v
end
if (b < c) then
    local v = b
    b = c
    c = v
end
if (a < b) then
    local v = a
    a = b
    b = v
end 
if (a >= (b + c)) then
	print "NAO FORMA TRIANGULO"
elseif ((a < (b + c)) and (b < (a + c)) and (c < (a + b))) then
-- tipos de triangulos
if ((a * a) == (b * b) + (c * c)) then
    print "TRIANGULO RETANGULO"
elseif ((a * a) > ((b * b) + (c * c))) then
    print "TRIANGULO OBTUSANGULO"
elseif ((a * a) < ((b * b) + (c * c))) then
    print "TRIANGULO ACUTANGULO"
end
end
if ((a == b) and (b == c) and (c == a)) then
    print "TRIANGULO EQUILATERO"
elseif ((a == b) or (a == c) or (b == c)) then
    print "TRIANGULO ISOSCELES"
end
```

### Haskell

```haskell

```



### `XXXII` URI Online Judge | 1046 ✔ **#**

## Tempo de Jogo

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia a hora inicial e a hora final de um jogo. A seguir calcule a duração do jogo, sabendo que o mesmo pode começar em um dia e terminar em outro, tendo uma duração mínima de 1 hora e máxima de 24 horas.

### Entrada

A entrada contém dois valores inteiros representando a hora de início e a hora de fim do jogo.

### Saída

Apresente a duração do jogo conforme exemplo abaixo.

| Exemplo de Entrada | Exemplo de Saída        |
| ------------------ | ----------------------- |
| 16 2               | O JOGO DUROU 10 HORA(S) |
| 0 0                | O JOGO DUROU 24 HORA(S) |
| 2 16               | O JOGO DUROU 14 HORA(S) |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1046 - Tempo de Jogo
valor = input()
t12 = valor.split()
n1 = int(t12[0])
n2 = int(t12[1])
if n1 > n2:
    tempo = (24 - (n1 - n2))
    print('O JOGO DUROU {} HORA(S)'.format(tempo))
if n1 < n2:
    tempo = (n2 - n1)
    print('O JOGO DUROU {} HORA(S)'.format(tempo))
if n1 == n2:
    print('O JOGO DUROU 24 HORA(S)')

```

### C

```c
#include <stdio.h>
// C - puro → uri_1046 - Tempo de Jogo
int main() { 
   int a, b, tempo;
    scanf("%d %d", &a, &b);
    if (a > b){
        tempo = (24 - (a - b));
        printf("O JOGO DUROU %d HORA(S)\n", tempo);
    }
    if (a < b){
        tempo = (b - a);
        printf("O JOGO DUROU %d HORA(S)\n",tempo);
    }
    if (a == b){
        printf("O JOGO DUROU 24 HORA(S)\n");
    } 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1046 - Tempo de Jogo
using namespace std; 
int main() { 
    int a, b, tempo;
    cin >> a >> b;
    if (a > b){
        tempo = (24 - (a - b));
        cout << "O JOGO DUROU " << tempo << " HORA(S)" << endl;
    }
    if (a < b){
        tempo = (b - a);
        cout << "O JOGO DUROU " << tempo << " HORA(S)" << endl;
    }
    if (a == b){
        cout << "O JOGO DUROU 24 HORA(S)" << endl;
    } 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1046 - Tempo de jogo
namespace uri1046
{
    class Program
    {
        static void Main(string[] args)
        {
            int a, b, tempo;
            String[] valor = Console.ReadLine().Split();
            a = Convert.ToInt32(valor[0]);
            b = Convert.ToInt32(valor[1]);
            
                if (a > b)
                {
                    tempo = (24 - (a - b));
                    Console.WriteLine("O JOGO DUROU {0} HORA(S)", tempo);
                }
                if (a < b)
                {
                    tempo = (b - a);
                    Console.WriteLine("O JOGO DUROU {0} HORA(S)", tempo);
                }
                if (a == b)
                {
                    Console.WriteLine("O JOGO DUROU 24 HORA(S)");
                }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1046 - Tempo de Jogo
valor = gets.split
a = valor[0].to_i
b = valor[1].to_i
    if (a > b)
        tempo = (24 - (a - b))
        puts "O JOGO DUROU %i HORA(S)\n" % tempo
    end
    if (a < b)
        tempo = (b - a)
        puts "O JOGO DUROU %i HORA(S)\n" %tempo
    end
    if (a == b)
        puts "O JOGO DUROU 24 HORA(S)"
    end
```

### Pascal

```pascal
// Pascal → uri_1046 - Tempo de Jogo
program uri_1046;
var
 a, b, tempo: integer;
begin
    readln(a, b);
    if (a > b) then
        begin
        tempo := (24 - (a - b));
        writeln('O JOGO DUROU ', tempo, ' HORA(S)');
        end;
    if (a < b) then
        begin
        tempo := (b - a);
        writeln('O JOGO DUROU ', tempo, ' HORA(S)');
        end;
    if (a = b) then
        begin
        writeln('O JOGO DUROU 24 HORA(S)');
        end;
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1046 - Tempo de Jogo
var valor = lines.shift().split(" ");
var a = parseFloat(valor[0]);
var b = parseFloat(valor[1]);
if (a > b) {
    var tempo = (24 - (a - b));
    console.log("O JOGO DUROU " + tempo + " HORA(S)");
}
if (a < b){
    tempo = (b - a);
    console.log("O JOGO DUROU " +tempo +" HORA(S)");}
if (a == b){
    console.log("O JOGO DUROU 24 HORA(S)");}
```

### Lua

```lua
-- Lua → uri_1046 - Tempo de Jogo
local valor = {io.read('*number', '*number')}
local a = valor[1]
local b = valor[2]
if (a > b) then
    local tempo = (24 - (a - b));
    print("O JOGO DUROU "..tempo.." HORA(S)")
end
if (a < b) then
    local tempo = (b - a)
    print("O JOGO DUROU "..tempo.." HORA(S)")
end
if (a == b) then
    print "O JOGO DUROU 24 HORA(S)"
end
```

### Haskell

```haskell

```

# `XXXIII` URI Online Judge | 1047 ✔ **#**

## Tempo de Jogo com Minutos

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia a hora inicial, minuto inicial, hora final e minuto final de um jogo. A seguir calcule a duração do jogo.

*Obs:* O jogo tem duração mínima de um (1) minuto e duração máxima de 24 horas.

### Entrada

Quatro números inteiros representando a hora de início e fim do jogo.

### Saída

Mostre a seguinte mensagem: “O JOGO DUROU XXX HORA(S) E YYY MINUTO(S)” .

| Exemplo de Entrada | Exemplo de Saída                      |
| ------------------ | ------------------------------------- |
| 7 8 9 10           | O JOGO DUROU 2 HORA(S) E 2 MINUTO(S)  |
| 7 7 7 7            | O JOGO DUROU 24 HORA(S) E 0 MINUTO(S) |
| 7 10 8 9           | O JOGO DUROU 0 HORA(S) E 59 MINUTO(S) |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1047 - Tempo de jogo com minutos
valor = input()
t12 = valor.split()
h = 0
m = 0
n1 = int(t12[0])
n2 = int(t12[1])
n3 = int(t12[2])
n4 = int(t12[3])
if n1 > n3:
    h = (24 - (n1 - n3))
if n1 < n3:
    h = (n3 - n1)
if n2 < n4:
    m = (n4 - n2)
if n2 > n4:
    m = (60 - (n2 - n4))
    m1 = (h - 1)
    h = m1
if n1 == n3 and n2 == n4:
    h = 24
    m = 0
print('O JOGO DUROU {} HORA(S) E {} MINUTO(S)'.format(h, m))

```

### C

```c
#include <stdio.h>
// C - puro → uri_1047 - Tempo de jogo com minutos
int main() { 
    int a, b, c, d, hora, minuto;
    scanf("%d %d %d %d", &a, &c, &b, &d);
    hora = b - a;
    if (hora < 0)
    {
        hora = 24 + (b - a);
    }
    minuto = d - c;
    if (minuto < 0)
    {
    minuto = 60 + (d - c);
    hora--;
    }
    if (a == b && c == d)
    {
        printf("O JOGO DUROU 24 HORA(S) E 0 MINUTO(S)\n");
    }
    else printf("O JOGO DUROU %d HORA(S) E %d MINUTO(S)\n", hora, minuto);
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1047 - Tempo de jogo com minutos
using namespace std; 
int main() { 
     int a, b, c, d, hora, minuto;
     cin >>a>>c>>b>>d;
    hora = b - a;
    if (hora < 0)
    {
        hora = 24 + (b - a);
    }
    minuto = d - c;
    if (minuto < 0)
    {
    minuto = 60 + (d - c);
    hora--;
    }
    if (a == b && c == d)
    {
        cout << "O JOGO DUROU 24 HORA(S) E 0 MINUTO(S)" << endl;
    }
    else cout << "O JOGO DUROU " << hora << " HORA(S) E " << minuto << " MINUTO(S)" << endl; 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1047 - Tempo de jogo com minutos
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace uri10472
{
    class Program
    {
        static void Main(string[] args)
        {
            String[] valor = Console.ReadLine().Split();
            
            int a = int.Parse(valor[0]);
            int b = int.Parse(valor[1]);
            int c = int.Parse(valor[2]);
            int d = int.Parse(valor[3]);

            //hora
            int horas = c - a;
            if (horas < 0)
            {
                horas += 24;
            }
            // minuto	
            int minutos = d - b;
            // Para 24 horas, tudo tem que ser igual
            if ((minutos == 0) && (horas == 0))
            {
                Console.WriteLine("O JOGO DUROU 24 HORA(S) E 0 MINUTO(S)");
            }
            else
            {
                if (minutos < 0)
                {
                    minutos += 60;
                    horas -= 1;
                }
                Console.WriteLine("O JOGO DUROU {0} HORA(S) E {1} MINUTO(S)", horas, minutos);
            }
            Console.ReadKey();
        }
    }
}
```

### Ruby

```ruby
# Ruby → uri_1047 - Tempo de jogo com minutos
# exercício foi um dos mais trabalhosos
v = gets.split
a = v[0].to_i
b = v[1].to_i
c = v[2].to_i
d = v[3].to_i
# hora
h = c - a
if h < 0
    h += 24
end
# minuto	
m = d - b
# Para 24 horas, tudo tem que ser igual
if m == 0 and h == 0
    puts "O JOGO DUROU 24 HORA(S) E 0 MINUTO(S)"
else 
    if m < 0
        m += 60
        h -= 1
end	
puts "O JOGO DUROU #{h} HORA(S) E #{m} MINUTO(S)"
end
```

### Pascal

```pascal
// Pascal → uri_1047 - Tempo de jogo com minutos
program uri_1047;
var
 a, b, c, d, hora, minuto, m1: integer;
begin
    readln(a, b, c, d);
    if (a > c) then
    begin
    hora := (24 - (a - c));
    end;
    if (a < c) then
      begin
      hora := (c - a);
      end;
    if (b < d) then
      begin
        minuto := (d - b);
      end;
    if (b > d) then
      begin
        minuto := (60 - (b - d));
        m1 := (hora - 1);
        hora := m1;
      end;
    if (a = c) and (b = d) then
      begin
        hora := 24;
        minuto := 0;
      end;
writeln('O JOGO DUROU ', hora, ' HORA(S) E ', minuto, ' MINUTO(S)');
  readln();
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// Javascript → uri_1047 - Tempo de Jogo com minutos
//var valor = prompt().split(" ");
var valor = lines.shift().split(" ");
//var valor = [7, 7, 7, 7];
var a = parseInt(valor[0]);
var b = parseInt(valor[1]);
var c = parseInt(valor[2]);
var d = parseInt(valor[3]);
//hora
var h = c - a;
if (h < 0) {
    h += 24;
}
// minuto	
var m = d - b;
// Para 24 horas, tudo tem que ser igual
if ((m == 0) && (h == 0)) {
    console.log("O JOGO DUROU 24 HORA(S) E 0 MINUTO(S)");
}else {
    if (m < 0){
        m += 60;
        h -= 1;}
console.log(`O JOGO DUROU ${h} HORA(S) E ${m} MINUTO(S)`);
}
```

### Lua

```lua
-- Lua → uri_1047 - Tempo de Jogo com minutos
local valor = {io.read('*number', '*number', '*number', '*number')}
local a = valor[1]
local b = valor[2]
local c = valor[3]
local d = valor[4]
--hora
H = c - a
if (H < 0) then
    H = H + 24
end
--minuto
    M = d - b
--Para 24 horas, tudo tem que ser igual
if ((M == 0) and (H == 0)) then
    print("O JOGO DUROU 24 HORA(S) E 0 MINUTO(S)")
else 
    if (M < 0) then
        M = M + 60
        H = H -1
    end
print("O JOGO DUROU "..H.. " HORA(S) E "..M.." MINUTO(S)")
end
```

### Haskell

```haskell

```



### `XXXIV` URI Online Judge | 1048 ✔ #

## Aumento de Salário

Por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

A empresa ABC resolveu conceder um aumento de salários a seus funcionários de acordo com a tabela abaixo:

| Salário                                                      | Percentual de Reajuste            |
| ------------------------------------------------------------ | --------------------------------- |
| 0 - 400.00 <br>400.01 - 800.00 <br>800.01 - 1200.00 <br>1200.01 - 2000.00 <br>Acima de 2000.00 | 15% <br>12% <br>10% <br>7% <br>4% |

Leia o salário do funcionário e calcule e mostre o novo salário, bem como o valor de reajuste ganho e o índice reajustado, em percentual.

### Entrada

A entrada contém apenas um valor de ponto flutuante, com duas casas decimais.

### Saída

Imprima 3 linhas na saída: o novo salário, o valor ganho de reajuste e o percentual de reajuste ganho, conforme exemplo abaixo.

| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
| 400.00             | Novo salario: 460.00 <br>Reajuste ganho: 60.00 <br>Em percentual: 15 % |
| 800.01             | Novo salario: 880.01 <br>Reajuste ganho: 80.00 <br>Em percentual: 10 % |
| 2000.00            | Novo salario: 2140.00 <br>Reajuste ganho: 140.00 <br>Em percentual: 7 % |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1048 - Aumento de Salário
s = float(input())
r = 0
if (s >= 0) and (s <= 400):
    p = '15 %'
    r = (15 * s) / 100
if (s > 400) and (s <= 800):
    p = '12 %'
    r = (12 * s) / 100
if (s > 800) and (s <= 1200):
    p = '10 %'
    r = (10 * s) / 100
if (s > 1200) and (s <= 2000):
    p = '7 %'
    r = (7 * s) / 100
if (s > 2000):
    p = '4 %'
    r = (4 * s) / 100
print('Novo salario: {:.2f}'.format(s + r))
print('Reajuste ganho: {:.2f}'.format(r))
print('Em percentual: {}'.format(p))

```

### C

```c
#include <stdio.h>
// C - puro → uri_1048 - Aumento de Salário
int main() { 
   double salario, percent;
    scanf("%lf", &salario);
    if (salario <= 400.00){
        percent = (salario * 15) / 100;
        printf("Novo salario: %.2lf\n", percent + salario);
        printf("Reajuste ganho: %.2lf\n", percent);
        printf("Em percentual: 15 %%\n");
    }
    else if (salario >= 400.01 && salario <= 800.00){
        percent = (salario * 12) / 100;
        printf("Novo salario: %.2lf\n", percent + salario);
        printf("Reajuste ganho: %.2lf\n", percent);
        printf("Em percentual: 12 %%\n");
    }
    else if (salario >= 800.01 && salario <= 1200.00){
        percent = (salario * 10) / 100;
        printf("Novo salario: %.2lf\n", percent + salario);
        printf("Reajuste ganho: %.2lf\n", percent);
        printf("Em percentual: 10 %%\n");
    }
    else if (salario >= 1200.01 && salario <= 2000.00){
        percent = (salario * 7) / 100;
        printf("Novo salario: %.2lf\n", percent + salario);
        printf("Reajuste ganho: %.2lf\n", percent);
        printf("Em percentual: 7 %%\n");
    }
    else if (salario >= 2000.01){
        percent = (salario * 4) / 100;
        printf("Novo salario: %.2lf\n", percent + salario);
        printf("Reajuste ganho: %.2lf\n", percent);
        printf("Em percentual: 4 %%\n");
    } 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1048 - Aumento de Salário
using namespace std; 
int main() { 
     double salario, percent;
    cout << fixed;
    cout.precision(2);
    cin >> salario;
    if (salario <= 400.00){
        percent = (salario * 15) / 100;
        cout << "Novo salario: " << percent + salario << endl;
        cout << "Reajuste ganho: " << percent << endl;
        cout << "Em percentual: 15 %" << endl;
    }
    else if (salario >= 400.01 && salario <= 800.00){
        percent = (salario * 12) / 100;
        cout << "Novo salario: " << percent + salario << endl;
        cout << "Reajuste ganho: " << percent << endl;
        cout << "Em percentual: 12 %" << endl;
    }
    else if (salario >= 800.01 && salario <= 1200.00){
        percent = (salario * 10) / 100;
        cout << "Novo salario: " << percent + salario << endl;
        cout << "Reajuste ganho: " << percent << endl;
        cout << "Em percentual: 10 %" << endl;
    }
    else if (salario >= 1200.01 && salario <= 2000.00){
        percent = (salario * 7) / 100;
        cout << "Novo salario: " << percent + salario << endl;
        cout << "Reajuste ganho: " << percent << endl;
        cout << "Em percentual: 7 %" << endl;
    }
    else if (salario >= 2000.01){
        percent = (salario * 4) / 100;
        cout << "Novo salario: " << percent + salario << endl;
        cout << "Reajuste ganho: " << percent << endl;
        cout << "Em percentual: 4 %" << endl;
    }
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1048 - Aumento de salário
namespace uri1048
{
    class Program
    {
        static void Main(string[] args)
        {
            double salario, percent;
            salario = double.Parse(Console.ReadLine());

            if (salario <= 400.00)
            {
                percent = (salario * 15) / 100;
                
                Console.WriteLine("Novo salario: " + string.Format("{0:0.00}", percent + salario));
                Console.WriteLine("Reajuste ganho: " + string.Format("{0:0.00}", percent));
                Console.WriteLine("Em percentual: 15 %");
            }
            else if (salario >= 400.01 && salario <= 800.00)
            {
                percent = (salario * 12) / 100;
                Console.WriteLine("Novo salario: " + string.Format("{0:0.00}", percent + salario));
                Console.WriteLine("Reajuste ganho: ", percent);
                Console.WriteLine("Em percentual: 12 %");
            }
            else if (salario >= 800.01 && salario <= 1200.00)
            {
                percent = (salario * 10) / 100;
                Console.WriteLine("Novo salario: " + string.Format("{0:0.00}", percent + salario));
                Console.WriteLine("Reajuste ganho: " + string.Format("{0:0.00}", percent));
                Console.WriteLine("Em percentual: 10 %");
            }
            else if (salario >= 1200.01 && salario <= 2000.00)
            {
                percent = (salario * 7) / 100;
                Console.WriteLine("Novo salario: " + string.Format("{0:0.00}", percent + salario));
                Console.WriteLine("Reajuste ganho: " + string.Format("{0:0.00}", percent));
                Console.WriteLine("Em percentual: 7 %");
            }
            else if (salario >= 2000.01)
            {
                percent = (salario * 4) / 100;
                Console.WriteLine("Novo salario: " +String.Format("{0:0.00}", percent + salario));
                Console.WriteLine("Reajuste ganho: " + String.Format("{0:0.00}", percent));
                Console.WriteLine("Em percentual: 4 %");
            }
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1048 - Aumento de Salário
salario = gets.to_f
 if (salario <= 400.00)
        percent = ((salario * 15) / 100)
        puts "Novo salario: %.2f\n" % (percent + salario)
        puts "Reajuste ganho: %.2f\n" % percent
        puts "Em percentual: 15 %"    
    elsif (salario >= 400.01 and salario <= 800.00)
        percent = ((salario * 12) / 100)
        puts "Novo salario: %.2f\n" % (percent + salario)
        puts "Reajuste ganho: %.2f\n" % percent
        puts "Em percentual: 12 %"    
    elsif (salario >= 800.01 && salario <= 1200.00)
        percent = ((salario * 10) / 100)
        puts "Novo salario: %.2f\n" % (percent + salario)
        puts "Reajuste ganho: %.2f\n" % percent
        puts "Em percentual: 10 %"    
    elsif (salario >= 1200.01 and salario <= 2000.00)
        percent = ((salario * 7) / 100)
        puts "Novo salario: %.2f\n" % (percent + salario)
        puts "Reajuste ganho: %.2f\n" % percent
        puts "Em percentual: 7 %"    
    elsif (salario >= 2000.01)
        percent = ((salario * 4) / 100)
        puts "Novo salario: %.2f\n" % (percent + salario)
        puts "Reajuste ganho: %.2f\n" % percent
        puts "Em percentual: 4 %"
    end
```

### Pascal

```pascal
// Pascal → uri_1048 - Aumento de Salário
program uri_1048;
var
 r, s:real;
 p:string;
begin
    readln(s);
    r := 0;
    if (s >= 0) and (s <= 400) then
      begin
        p := '15 %';
        r := ((15 * s) / 100);
      end;
    if (s > 400) and (s <= 800) then
      begin
        p := '12 %';
        r := ((12 * s) / 100);
      end;
    if (s > 800) and (s <= 1200) then
      begin
        p := '10 %';
        r := ((10 * s) / 100);
      end;
    if (s > 1200) and (s <= 2000) then
      begin
        p := '7 %';
        r := ((7 * s) / 100);
      end;
    if (s > 2000) then
      begin
        p := '4 %';
        r := ((4 * s) / 100);
      end;
writeln('Novo salario: ', (s + r):0:2);
writeln('Reajuste ganho: ', (r):0:2);
writeln('Em percentual: ', p);
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1048 - Aumento de Salário
var S = Number(lines.shift());

if ((S >= 0) && (S <= 400)) {
    var P = '15 %';
    var R = ((15 * S) / 100);
}
if ((S > 400) && (S <= 800)) {
    P = '12 %';
    R = ((12 * S) / 100);
}
if ((S > 800) && (S <= 1200)) {
    P = '10 %';
    R = ((10 * S) / 100);
}
if ((S > 1200) && (S <= 2000)) {
    P = '7 %';
    R = ((7 * S) / 100);
}
if (S > 2000) {
    P = '4 %';
    R = ((4 * S) / 100);
}
var soma = S + R;
console.log('Novo salario: ' + soma.toFixed(2));
console.log('Reajuste ganho: ' + R.toFixed(2));
console.log('Em percentual: ' + P);
```

### Lua

```lua
-- Lua → uri_1048 - Aumento de Salário
S = tonumber(io.read())
R = 0
if (S >= 0) and (S <= 400) then
    P = '15 %'
    R = ((15 * S) / 100)
end
if (S > 400) and (S <= 800) then
    P = '12 %'
    R = ((12 * S) / 100)
end
if (S > 800) and (S <= 1200) then
    P = '10 %'
    R = ((10 * S) / 100)
end
if (S > 1200) and (S <= 2000) then
    P = '7 %'
    R = ((7 * S) / 100)
end
if (S > 2000) then
    P = '4 %'
    R = ((4 * S) / 100)
end
local salario = (string.format("%.2f", S))
local reajuste = (string.format("%.2f", R))
local soma = S + R
local soma_formatada = (string.format( "%.2f", soma))
print('Novo salario: '..soma_formatada)
print('Reajuste ganho: '..reajuste)
print('Em percentual: '..P)
```

### Haskell

```haskell

```

### `XXXV` URI Online Judge | 1049 ✔ #

## Animal

Por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Neste problema, você deverá ler 3 palavras que definem o tipo de animal possível segundo o esquema abaixo, da esquerda para a direita.  Em seguida conclua qual dos animais seguintes foi escolhido, através das três palavras fornecidas.

![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1049_b.png)

### Entrada

A entrada contém 3 palavras, uma em cada linha, necessárias para identificar o animal segundo a figura acima, com todas as letras minúsculas.

### Saída

Imprima o nome do animal correspondente à entrada fornecida.

| Exemplos de Entrada                   | Exemplos de Saída |
| ------------------------------------- | ----------------- |
| vertebrado <br>mamifero <br>onivoro   | homem             |
| vertebrado <br>ave <br>carnivoro      | aguia             |
| invertebrado <br>anelideo <br>onivoro | minhoca           |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1049 - Animal
a = input()
b = input()
c = input()
if (a == 'vertebrado') and (b == 'ave') and (c == 'carnivoro'):
    print('aguia')
if (a == 'vertebrado') and (b == 'ave') and (c == 'onivoro'):
    print('pomba')
if (a == 'vertebrado') and (b == 'mamifero') and (c == 'onivoro'):
    print('homem')
if (a == 'vertebrado') and (b == 'mamifero') and (c == 'herbivoro'):
    print('vaca')
if (a == 'invertebrado') and (b == 'inseto') and (c == 'hematofago'):
    print('pulga')
if (a == 'invertebrado') and (b == 'inseto') and (c == 'herbivoro'):
    print('lagarta')
if (a == 'invertebrado') and (b == 'anelideo') and (c == 'hematofago'):
    print('sanguessuga')
if (a == 'invertebrado') and (b == 'anelideo') and (c == 'onivoro'):
    print('minhoca')

```

### C

```c
#include <stdio.h>
// C - puro → uri_1049 - Animal
int main() { 
  char af[]="vertebrado", a1[]="ave", a2[]="mamifero";
    char a3[] = "carnivoro", a4[] = "onivoro", a5[] = "herbivoro";
    char bf[] = "invertebrado", b1[] = "inseto", b2[] = "anelideo";
    char b3[] = "hematofago", b4[] = "herbivoro", b7[] = "pulga";
    char b8[] = "lagarta", b9[] = "sanguessuga", b10[] = "minhoca";
    char a[25], b[25], c[25];
    scanf("%s", a);
    scanf("%s", b);
    scanf("%s", c);
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a1)) && (0 == strcmp(c, a3))){
        printf("aguia\n");}
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a1)) && (0 == strcmp(c, a4))){
        printf("pomba\n");}
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a2)) && (0 == strcmp(c, a4))){
        printf("homem\n");}
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a2)) && (0 == strcmp(c, a5))){
        printf("vaca\n");}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b1)) && (0 == strcmp(c, b3))){
        printf("pulga\n");}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b1)) && (0 == strcmp(c, a5))){
        printf("lagarta\n");}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b2)) && (0 == strcmp(c, b3))){
        printf("sanguessuga\n");}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b2)) && (0 == strcmp(c, a4))){
        printf("minhoca\n");} 
    return 0;
}
```

### C++

```c++
#include <iostream>
#include <string.h>
// C++ → uri_1049 - Animal
using namespace std; 
int main() { 
     char af[]="vertebrado", a1[]="ave", a2[]="mamifero";
    char a3[] = "carnivoro", a4[] = "onivoro", a5[] = "herbivoro";
    char bf[] = "invertebrado", b1[] = "inseto", b2[] = "anelideo";
    char b3[] = "hematofago", b4[] = "herbivoro", b7[] = "pulga";
    char b8[] = "lagarta", b9[] = "sanguessuga", b10[] = "minhoca";
    char a[25], b[25], c[25];
    cin >> a;
    cin >> b;
    cin >> c;
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a1)) && (0 == strcmp(c, a3))){
        cout << "aguia" << endl;}
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a1)) && (0 == strcmp(c, a4))){
        cout << "pomba" << endl;}
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a2)) && (0 == strcmp(c, a4))){
        cout << "homem" << endl;}
    if ((0 == strcmp(a, af)) && (0 == strcmp(b, a2)) && (0 == strcmp(c, a5))){
        cout << "vaca" << endl;}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b1)) && (0 == strcmp(c, b3))){
        cout << "pulga" << endl;}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b1)) && (0 == strcmp(c, a5))){
        cout << "lagarta" << endl;}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b2)) && (0 == strcmp(c, b3))){
        cout << "sanguessuga" << endl;}
    if ((0 == strcmp(a, bf)) && (0 == strcmp(b, b2)) && (0 == strcmp(c, a4))){
        cout << "minhoca" << endl;} 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1049 - Animal
namespace uri1049
{
    class Program
    {
        static void Main(string[] args)
        {
            string tipo1 = Console.ReadLine();
            string tipo2 = Console.ReadLine();
            string tipo3 = Console.ReadLine();
            if (tipo1 == "vertebrado")
            {
                if (tipo2 == "ave")
                {
                    if (tipo3 == "carnivoro")
                    {
                        Console.WriteLine("aguia");
                    }
                    else
                    {
                        Console.WriteLine("pomba");
                    }
                }
                else
                {
                    if (tipo3 == "onivoro")
                    {
                        Console.WriteLine("homem");
                    }
                    else
                    {
                        Console.WriteLine("vaca");
                    }
                }
            }
            else
            {
                if (tipo2 == "inseto")
                {
                    if (tipo3 == "hematofago")
                    {
                        Console.WriteLine("pulga");
                    }
                    else
                    {
                        Console.WriteLine("lagarta");
                    }
                }
                else
                {
                    if (tipo3 == "hematofago")
                    {
                        Console.WriteLine("sanguessuga");
                    }
                    else
                    {
                        Console.WriteLine("minhoca");
                    }
                }
            }
            Console.ReadKey();
        }
    }
}
```



### Ruby

```ruby
# Ruby → uri_1049 - Animal
a = gets.chomp.to_s
b = gets.chomp.to_s
c = gets.chomp.to_s
aguia = ['aguia', 'vertebrado', 'ave', 'carnivoro']
pomba = ['pomba', 'vertebrado', 'ave', 'onivoro']
homem = ['homem', 'vertebrado', 'mamifero', 'onivoro']
vaca = ['vaca', 'vertebrado', 'mamifero', 'herbivoro']
pulga = ['pulga', 'invertebrado', 'inseto', 'hematofago']
lagarta = ['lagarta', 'invertebrado', 'inseto', 'herbivoro']
sanguessuga = ['sanguessuga', 'invertebrado', 'anelideo', 'hematofago']
minhoca = ['minhoca', 'invertebrado', 'anelideo', 'onivoro']
if a == "vertebrado" and b == "ave" and c == "carnivoro"
    puts aguia[0]
end    
if a == "vertebrado" and b == "ave" and c == "onivoro"
    puts pomba[0]
end    
if a == 'vertebrado' and b == 'mamifero' and c == "onivoro"
    puts homem[0]
end    
if a == 'vertebrado' and b == "mamifero" and c == "herbivoro"
    puts vaca[0]
end    
if a == 'invertebrado' and b == 'inseto' and c == 'hematofago'
    puts pulga[0]
end    
if a == 'invertebrado' and b == 'inseto' and c == 'herbivoro'
    puts lagarta[0]
end    
if a == "invertebrado" and b == "anelideo" and c == "hematofago"
    puts sanguessuga[0]
end    
if a == "invertebrado" and b == "anelideo" and c == "onivoro"
    puts minhoca[0]
end
```

### Pascal

```pascal
program uri_1049;
// Pascal → uri_1049 - Animal - correto 
    var
        a, b, c: string;
begin
     readln(a);
     readln(b);
     readln(c);
     if (a = 'vertebrado') and (b = 'ave') and (c = 'carnivoro') then
        writeln('aguia');
     if (a = 'vertebrado') and (b = 'ave') and (c = 'onivoro') then
        writeln('pomba');
     if (a = 'vertebrado') and (b = 'mamifero') and (c = 'onivoro') then
        writeln('homem');
     if (a = 'vertebrado') and (b = 'mamifero') and (c = 'herbivoro') then
        writeln('vaca');
     if (a = 'invertebrado') and (b = 'inseto') and (c = 'hematofago') then
        writeln('pulga');
     if (a = 'invertebrado') and (b = 'inseto') and (c = 'herbivoro') then
        writeln('lagarta');
     if (a = 'invertebrado') and (b = 'anelideo') and (c = 'hematofago') then
        writeln('sanguessuga');
     if (a = 'invertebrado') and (b = 'anelideo') and (c = 'onivoro') then
        writeln('minhoca');
     readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1049 - Animal
var a = lines.shift();
var b = lines.shift();
var c = lines.shift();
if ((a == 'vertebrado') && (b == 'ave') && (c == 'carnivoro')) {
    console.log('aguia');}
if ((a == 'vertebrado') && (b == 'ave') && (c == 'onivoro')) {
    console.log('pomba');}
if ((a == 'vertebrado') && (b == 'mamifero') && (c == 'onivoro')) {
    console.log('homem');}
if ((a == 'vertebrado') && (b == 'mamifero') && (c == 'herbivoro')) {
    console.log('vaca');}
if ((a == 'invertebrado') && (b == 'inseto') && (c == 'hematofago')) {
    console.log('pulga');}
if ((a == 'invertebrado') && (b == 'inseto') && (c == 'herbivoro')) {
    console.log('lagarta');}
if ((a == 'invertebrado') && (b == 'anelideo') && (c == 'hematofago')) {
    console.log('sanguessuga');}
if ((a == 'invertebrado') && (b == 'anelideo') && (c == 'onivoro')) {
    console.log('minhoca');}
```

### Lua

```lua
-- Lua → uri_1049 - Animal - correto 
local a = io.read()
local b = io.read()
local c = io.read()
if (a == 'vertebrado') and (b == 'ave') and (c == 'carnivoro') then
    print('aguia')
end
if (a == 'vertebrado') and (b == 'ave') and (c == 'onivoro') then
    print('pomba')
end
if (a == 'vertebrado') and (b == 'mamifero') and (c == 'onivoro') then
    print('homem')
end
if (a == 'vertebrado') and (b == 'mamifero') and (c == 'herbivoro') then
    print('vaca')
end
if (a == 'invertebrado') and (b == 'inseto') and (c == 'hematofago') then
    print('pulga')
end
if (a == 'invertebrado') and (b == 'inseto') and (c == 'herbivoro') then
    print('lagarta')
end
if (a == 'invertebrado') and (b == 'anelideo') and (c == 'hematofago') then
    print('sanguessuga')
end
if (a == 'invertebrado') and (b == 'anelideo') and (c == 'onivoro') then
    print('minhoca')
end
```

### Haskell

```haskell

```

### XXXVI` URI Online Judge | 1050 ✔ #

## DDD

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um número inteiro que representa um código de DDD para discagem interurbana. Em seguida, informe à qual cidade o DDD pertence, considerando a tabela abaixo:

![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1050.png)

Se a entrada for qualquer outro DDD que não esteja presente na tabela acima, o programa deverá informar:
DDD nao cadastrado

### Entrada

A entrada consiste de um único valor inteiro.

### Saída

Imprima o nome da cidade correspondente ao DDD existente na entrada. Imprima *DDD nao cadastrado* caso não existir DDD correspondente ao número digitado.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 11                 | Sao Paulo        |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1050 - DDD
n = int(input())
if n == 61:
    print('Brasilia')
elif n == 71:
    print('Salvador')
elif n == 11:
    print('Sao Paulo')
elif n == 21:
    print('Rio de Janeiro')
elif n == 32:
    print('Juiz de Fora')
elif n == 19:
    print('Campinas')
elif n == 27:
    print('Vitoria')
elif n == 31:
    print('Belo Horizonte')
else:
    print('DDD nao cadastrado')

```

### C

```c
#include <stdio.h>
// C - puro → uri_1050 - DDD
int main() { 
     int n;
    scanf("%d", &n);
    if (n == 61){
        printf("Brasilia\n");}
    else if (n == 71){
        printf("Salvador\n");}
    else if (n == 11){
        printf("Sao Paulo\n");}
    else if (n == 21){
        printf("Rio de Janeiro\n");}
    else if (n == 32){
        printf("Juiz de Fora\n");}
    else if (n == 19){
        printf("Campinas\n");}
    else if (n == 27){
        printf("Vitoria\n");}
    else if (n == 31){
        printf("Belo Horizonte\n");}
    else{
        printf("DDD nao cadastrado\n");} 
    return 0;
}
```

### C ++

```c++
#include <iostream>
 // C++ → uri_1050 - DDD
using namespace std; 
int main() { 
    int n;
    cin >> n;
    if (n == 61){
        cout << "Brasilia" << endl;}
    else if (n == 71){
        cout << "Salvador" << endl;}
    else if (n == 11){
        cout << "Sao Paulo" << endl;}
    else if (n == 21){
        cout << "Rio de Janeiro" << endl;}
    else if (n == 32){
        cout << "Juiz de Fora" << endl;}
    else if (n == 19){
        cout << "Campinas" << endl;}
    else if (n == 27){
        cout << "Vitoria" << endl;}
    else if (n == 31){
        cout << "Belo Horizonte" << endl;}
    else{
        cout << "DDD nao cadastrado" << endl;} 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1050 - DDD
namespace uri1050
{
    class Program
    {
        static void Main(string[] args)
        {
                int n;
                n = int.Parse(Console.ReadLine());

                if (n == 61)
                {
                    Console.WriteLine("Brasilia");
                }
                else if (n == 71)
                {
                    Console.WriteLine("Salvador");
                }
                else if (n == 11)
                {
                    Console.WriteLine("Sao Paulo");
                }
                else if (n == 21)
                {
                    Console.WriteLine("Rio de Janeiro");
                }
                else if (n == 32)
                {
                    Console.WriteLine("Juiz de Fora");
                }
                else if (n == 19)
                {
                    Console.WriteLine("Campinas");
                }
                else if (n == 27)
                {
                    Console.WriteLine("Vitoria");
                }
                else if (n == 31)
                {
                    Console.WriteLine("Belo Horizonte");
                }
                else
                {
                    Console.WriteLine("DDD nao cadastrado");
                }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1050 - DDD
n = gets.to_i
case
	when n == 61
		puts "Brasilia"
	when n == 71
		puts "Salvador"
	when n == 11
		puts "Sao Paulo"
	when n == 21
		puts "Rio de Janeiro"
	when n == 32
		puts "Juiz de Fora"
	when n == 19
		puts "Campinas"
	when n == 27
		puts "Vitoria"
	when n == 31
		puts "Belo Horizonte"
	else
		puts"DDD nao cadastrado"	
end
```

### Pascal

```pascal
// Pascal → uri_1050 - DDD
program uri_1050;
var
 n:integer;
begin
    readln(n);
    if (n = 61) then
        writeln('Brasilia')
    else if (n = 71) then
        writeln('Salvador')
    else if (n = 11) then
        writeln('Sao Paulo')
    else if (n = 21) then
        writeln('Rio de Janeiro')
    else if (n = 32) then
        writeln('Juiz de Fora')
    else if (n = 19) then
        writeln('Campinas')
    else if (n = 27) then
        writeln('Vitoria')
    else if (n = 31) then
        writeln('Belo Horizonte')
    else
        writeln('DDD nao cadastrado');
  readln();
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// Javascript → uri_1050 - DDD
var n = Number(lines.shift());
if (n == 61){
    console.log("Brasilia");}
else if (n == 71){
    console.log("Salvador");}
else if (n == 11){
    console.log("Sao Paulo");}
else if (n == 21){
    console.log("Rio de Janeiro");}
else if (n == 32){
    console.log("Juiz de Fora");}
else if (n == 19){
    console.log("Campinas");}
else if (n == 27){
    console.log("Vitoria");}
else if (n == 31){
    console.log("Belo Horizonte");}
else{
    console.log("DDD nao cadastrado");}
```

### Lua

```lua
--[[
Escreva a sua solução aqui
Code your solution here
Escriba su solución aquí
--]]
-- Lua - puro → uri_1050 - DDD

local n = tonumber(io.read())
if (n == 61) then
    print("Brasilia")
elseif (n == 71) then
    print("Salvador")
elseif (n == 11) then
    print("Sao Paulo")
elseif (n == 21) then
    print("Rio de Janeiro")
elseif (n == 32) then
    print("Juiz de Fora")
elseif (n == 19) then
    print("Campinas")
elseif (n == 27) then
    print("Vitoria")
elseif (n == 31) then
    print("Belo Horizonte")
else
    print("DDD nao cadastrado") 
end
```

### Haskell

```haskell

```

### `XXXVII` URI Online Judge | 1051 ✔  **#**

## Imposto de Renda

Por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Em um país imaginário denominado Lisarb, todos os habitantes ficam felizes em pagar seus impostos, pois sabem que nele não existem políticos corruptos e os recursos arrecadados são utilizados em benefício da população, sem qualquer desvio. A moeda deste país é o Rombus, cujo símbolo é o R$.

Leia um valor com duas casas decimais, equivalente ao salário de uma pessoa de Lisarb. Em seguida, calcule e mostre o valor que esta pessoa deve pagar de Imposto de Renda, segundo a tabela abaixo.

![img](https://resources.urionlinejudge.com.br/gallery/images/problems/UOJ_1051_pt.png)

Lembre que, se o salário for R$ 3002.00, a taxa que incide é de 8% apenas sobre R$ 1000.00, pois a faixa de salário que fica de R$ 0.00 até R$ 2000.00 é isenta de Imposto de Renda. No exemplo fornecido (abaixo), a taxa é de 8% sobre R$ 1000.00 + 18% sobre R$ 2.00, o que resulta em R$ 80.36 no total. O valor deve ser impresso com duas casas decimais.

### Entrada

A entrada contém apenas um valor de ponto flutuante, com duas casas decimais.

### Saída

Imprima o texto "R$" seguido de um espaço e do valor total devido de Imposto de Renda, com duas casas após o ponto. Se o valor de entrada for menor ou igual a 2000, deverá ser impressa a mensagem "Isento".

| Exemplos de Entrada | Exemplos de Saída |
| ------------------- | ----------------- |
| 3002.00             | R$ 80.36          |
| 1701.12             | Isento            |
| 4520.00             | R$ 355.60         |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1051 - Imposto de Renda
n = float(input())
if n <= 2000:
    print('Isento')
if (n > 2000) and (n <= 3000):
    n = ((n - 2000) * 0.08)
    print('R$ {:.2f}'.format(n))
if (n > 3000) and (n <= 4500):
    n = (((n - 3000) * 0.18) + 80)
    print('R$ {:.2f}'.format(n))
if n > 4500:
    n = (((n - 4500) * 0.28) + 350)
    print('R$ {:.2f}'.format(n))

```

### C

```c
#include <stdio.h>
#include <stdlib.h>
// C - puro → uri_1051 - Imposto de Renda
int main()
{
    double n;
    scanf("%lf", &n);
    if (n <= 2000){
        printf("Isento\n");}
    else if ((n > 2000) && (n <= 3000)){
        n = ((n - 2000) * 0.08);
        printf("R$ %.2lf\n", n);}
    else if ((n > 3000) && (n <= 4500)){
        n = (((n - 3000) * 0.18) + 80);
        printf("R$ %.2lf\n", n);}
    else if (n > 4500){
        n = (((n - 4500) * 0.28) + 350);
        printf("R$ %.2lf\n", n);}
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1051 - Imposto de Renda
using namespace std; 
int main() { 
    float n;
    cout << fixed;
    cout.precision(2);
    cin >> n;
    if (n <= 2000){
        cout << "Isento" << endl;}
    if ((n > 2000) && (n <= 3000)){
        n = ((n - 2000) * 0.08);
        cout << "R$ " << n << endl;}
    if ((n > 3000) && (n <= 4500)){
        n = (((n - 3000) * 0.18) + 80);
        cout << "R$ " << n << endl;}
    if (n > 4500){
        n = (((n - 4500) * 0.28) + 350);
        cout << "R$ " << n << endl;} 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1051 - Imposto de renda
namespace uri1051
{
    class Program
    {
        static void Main(string[] args)
        {
                double n;
                n = double.Parse(Console.ReadLine());

                if (n <= 2000)
                {
                    Console.WriteLine("Isento");
                }
                else if ((n > 2000) && (n <= 3000))
                {
                    n = ((n - 2000) * 0.08);
                    Console.WriteLine("R$ "+ string.Format("{0:0.00}", n));
                }
                else if ((n > 3000) && (n <= 4500))
                {
                    n = (((n - 3000) * 0.18) + 80);
                    Console.WriteLine("R$ "+ string.Format("{0:0.00}", n));
                }
                else if (n > 4500)
                {
                    n = (((n - 4500) * 0.28) + 350);
                    Console.WriteLine("R$ "+ string.Format("{0:0.00}", n));
                }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1051 - Imposto de Renda
s = gets.to_f 
if s <= 2000.0
    puts "Isento"
end
if s > 2000.0 and s <= 3000.0
    n = (s - 2000) * 0.08
    puts "R$ %.2f" % n
end
if s > 3000.0 and s <= 4500.0
	n = (((s - 3000.0) * 0.18) + 80)
	puts "R$ %.2f" % n
end
if s > 4500.0
	n = (((s - 4500.0) * 0.28) + 350)
	puts "R$ %.2f" % n
end
```

### Pascal

```pascal
// Pascal → uri_1051 - Imposto de Renda
program uri_1051;
var
 n:real;
begin
    readln(n);
    if (n <= 2000) then
        begin
          writeln('Isento');
        end;
    if ((n > 2000) and (n <= 3000)) then
        begin
          n := ((n - 2000) * 0.08);
          writeln('R$ ', n:0:2);
        end;
    if ((n > 3000) and (n <= 4500)) then
        begin
          n := (((n - 3000) * 0.18) + 80);
          writeln('R$ ', n:0:2);
        end;
    if (n > 4500) then
        begin
          n := (((n - 4500) * 0.28) + 350);
          writeln('R$ ', n:0:2);
        end;
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1050 - DDD
var n = Number(lines.shift());
if (n <= 2000){
    console.log("Isento");}
else if ((n > 2000) && (n <= 3000)){
    n = ((n - 2000) * 0.08);
    console.log(`R$ ${n.toFixed(2)}`);}
else if ((n > 3000) && (n <= 4500)){
    n = (((n - 3000) * 0.18) + 80);
    console.log(`R$ ${n.toFixed(2)}`);}
else if (n > 4500){
    n = (((n - 4500) * 0.28) + 350);
    console.log(`R$ ${n.toFixed(2)}`);}
```

### Lua

```lua
-- Lua → uri_1051 - Imposto de Renda
local n = tonumber(io.read())
    if (n <= 2000) then
        print("Isento")
    else if ((n > 2000) and (n <= 3000)) then
        n = ((n - 2000) * 0.08)
        local n1 = (string.format( "%.2f", n))
        print("R$ "..n1)
    else if ((n > 3000) and (n <= 4500)) then
        n = (((n - 3000) * 0.18) + 80)
        local n2 = (string.format( "%.2f", n))
        print("R$ "..n2)
    else if (n > 4500) then
        n = (((n - 4500) * 0.28) + 350)
        local n3 = (string.format( "%.2f", n))
        print("R$ "..n3)
    end
end
end
end
```

### Haskell

```haskell

```

# `XXXVIII` URI Online Judge | 1052 ✔ **#**

## Mês

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro entre 1 e 12, inclusive. Correspondente a este valor, deve ser apresentado como resposta o mês do ano por extenso, em inglês, com a primeira letra maiúscula.

### Entrada

A entrada contém um único valor inteiro.

### Saída

Imprima por extenso o nome do mês correspondente ao número existente na entrada, com a primeira letra em maiúscula.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 4                  | April            |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1052 - Mês
n = int(input())
if n == 1:
    print('January')
if n == 2:
    print('February')
if n == 3:
    print('March')
if n == 4:
    print('April')
if n == 5:
    print('May')
if n == 6:
    print('June')
if n == 7:
    print('July')
if n == 8:
    print('August')
if n == 9:
    print('September')
if n == 10:
    print('October')
if n == 11:
    print('November')
if n == 12:
    print('December')

```

### C

```c
#include <stdio.h>
// C - puro → uri_1052 - Mês
int main() { 
  int n;
    scanf("%d", &n);
    if (n == 1){
        printf("January\n");}
    if (n == 2){
        printf("February\n", n);}
    if (n == 3){
        printf("March\n");}
    if (n == 4){
        printf("April\n");}
    if (n == 5){
        printf("May\n");}
    if (n == 6){
        printf("June\n");}
    if (n == 7){
        printf("July\n");}
    if (n == 8){
        printf("August\n");}
    if (n == 9){
        printf("September\n");}
    if (n == 10){
        printf("October\n");}
    if (n == 11){
        printf("November\n");}
    if (n == 12){
        printf("December\n");} 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1052 - Mês
using namespace std; 
int main() { 
    int n;
    cin >> n;
    if (n == 1){
        cout << "January" << endl;}
    if (n == 2){
        cout << "February" << endl;}
    if (n == 3){
        cout << "March" << endl;}
    if (n == 4){
        cout << "April" << endl;}
    if (n == 5){
        cout << "May" << endl;}
    if (n == 6){
        cout << "June" << endl;}
    if (n == 7){
        cout << "July" << endl;}
    if (n == 8){
        cout << "August" << endl;}
    if (n == 9){
        cout << "September" << endl;}
    if (n == 10){
        cout << "October" << endl;}
    if (n == 11){
        cout << "November" << endl;}
    if (n == 12){
        cout << "December" << endl;} 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1052 - Mês
namespace uri1052
{
    class Program
    {
        static void Main(string[] args)
        {
                int n;
                n = int.Parse(Console.ReadLine());

                if (n == 1)
                {
                    Console.WriteLine("January");
                }
                if (n == 2)
                {
                Console.WriteLine("February", n);
                }
                if (n == 3)
                {
                Console.WriteLine("March");
                }
                if (n == 4)
                {
                Console.WriteLine("April");
                }
                if (n == 5)
                {
                Console.WriteLine("May");
                }
                if (n == 6)
                {
                Console.WriteLine("June");
                }
                if (n == 7)
                {
                Console.WriteLine("July");
                }
                if (n == 8)
                {
                Console.WriteLine("August");
                }
                if (n == 9)
                {
                Console.WriteLine("September");
                }
                if (n == 10)
                {
                Console.WriteLine("October");
                }
                if (n == 11)
                {
                Console.WriteLine("November");
                }
                if (n == 12)
                {
                Console.WriteLine("December");
                }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1052 - Mês
mes = gets.to_i
case
	when mes == 1
		puts "January"
    when mes == 2
        puts "February"
    when mes == 3
        puts "March"
    when mes == 4
        puts "April"
    when mes == 5
        puts "May"
    when mes == 6
        puts "June"
    when mes == 7
        puts "July"
    when mes == 8
        puts "August"
    when mes == 9
        puts "September"
    when mes == 10
        puts "October"
    when mes == 11
        puts "November"
    when mes == 12
        puts "December"
 end
```

### Pascal

```pascal
// Pascal → uri_1052 - Mês
program uri_1052;
var
 n:real;
begin
    readln(n);

    if (n = 1) then
        begin
          writeln('January');
        end;
    if (n = 2) then
        begin
          writeln('February');
        end;
    if (n = 3) then
        begin
          writeln('March');
        end;
    if (n = 4) then
        begin
          writeln('April');
        end;
    if (n = 5) then
        begin
          writeln('May');
        end;
    if (n = 6) then
        begin
          writeln('June');
        end;
    if (n = 7) then
        begin
          writeln('July');
        end;
    if (n = 8) then
        begin
          writeln('August');
        end;
    if (n = 9) then
        begin
          writeln('September');
        end;
    if (n = 10) then
        begin
          writeln('October');
        end;
    if (n = 11) then
        begin
          writeln('November');
        end;
    if (n = 12) then
        begin
          writeln('December');
        end;
  readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1052 - Mês
var n = Number(lines.shift());

if (n == 1){
    console.log("January");}
if (n == 2){
    console.log("February";}
if (n == 3){
    console.log("March");}
if (n == 4){
    console.log("April");}
if (n == 5){
    console.log("May");}
if (n == 6){
    console.log("June");}
if (n == 7){
    console.log("July");}
if (n == 8){
    console.log("August");}
if (n == 9){
    console.log("September");}
if (n == 10){
    console.log("October");}
if (n == 11){
    console.log("November");}
if (n == 12){
    console.log("December");}     
```

### Lua

```lua
-- Lua → uri_1052 - Mês
local n = tonumber(io.read())

if (n == 1) then
    print("January")
end
if (n == 2) then
    print("February")
end
if (n == 3) then
    print("March")
end
if (n == 4) then
    print("April")
end
if (n == 5) then
    print("May")
end
if (n == 6) then
    print("June")
end
if (n == 7) then
    print("July")
end
if (n == 8) then
    print("August")
end
if (n == 9) then
    print("September")
end
if (n == 10) then
    print("October")
end
if (n == 11) then
    print("November")
end
if (n == 12) then
    print("December")
end
```

### Haskell

```haskell

```

# XXXIX` URI Online Judge | 1059 ✔ **#**

## Números Pares

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Faça um programa que mostre os números pares entre 1 e 100, inclusive.

### Entrada

Neste problema extremamente simples de repetição não há entrada.

### Saída

Imprima todos os números pares entre 1 e 100, inclusive se for o caso, um em cada linha.

| Exemplo de Entrada | Exemplo de Saída              |
| ------------------ | ----------------------------- |
|                    | 2 <br>4 <br>6 <br>... <br>100 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1059 - Números Pares
x = 0
for x in range(2, 101, 2):
    print(x)

```

### C

```c
#include <stdio.h>
 // C- puro → uri_1059 - Números Pares
int main() { 
     int i;
    for (i = 2; i <= 100; i += 2){
        printf("%d\n", i);} 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1059 - Números Pares (primeiro a usar FOR)
using namespace std; 
int main() { 
      int i;
    for(i = 1; i <= 100; ++i){
            if (i % 2 == 0){
                cout << i << endl;
            }
    } 
    return 0;
}
```

### C#

```c#
using System;
// C# - uri 1059 - Números pares
namespace uri1059
{
    class Program
    {
        static void Main(string[] args)
        {
            for (int i = 2; i <= 100; i++)
            {
                if(i % 2 == 0)
                {
                    Console.WriteLine("{0}", i);
                }            
            }
        Console.ReadKey();
        }
    }
}
```

### Ruby

```ruby
# Ruby → uri_1059 - Números Pares
for i in 1..100
	if i % 2 == 0
	puts i
else
	next
end
end
```

### Pascal

```pascal
// Pascal → uri_1059 - Números Pares
program uri_1059;
var
 i:integer;
begin
  i := 0;
  for i := 1 to 100 do
    begin
      if i mod 2 = 0 then
      begin
        write(i, #10);
      end;
    end;
readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1059 - Números Pares
for (var i = 1; i <= 100; i++) {
    if (i % 2 == 0)
	console.log(i);
}
```

### Lua

```lua
-- Lua → uri_1059 - Números Pares
for I = 1, 100 do
	if (I % 2 == 0) then
	print(I)
end
end
```

### Haskell

```haskell

```

# `XL` URI Online Judge | 1060 ✔

## Números Positivos

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Faça um programa que leia 6 valores. Estes valores serão somente negativos ou positivos (desconsidere os valores nulos). A seguir, mostre a quantidade de valores positivos digitados.

### Entrada

Seis valores, negativos e/ou positivos.

### Saída

Imprima uma mensagem dizendo quantos valores positivos foram lidos.

| Exemplo de Entrada                     | Exemplo de Saída    |
| -------------------------------------- | ------------------- |
| 7 <br>-5 <br>6 <br>-3.4 <br>4.6 <br>12 | 4 valores positivos |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1060 - Números Positivos
conta = 0
a = input()
b = input()
c = input()
d = input()
e = input()
f = input()
if a == int:
    a = int(a)
    if a >= 0:
        conta += 1
else:
    a = float(a)
    if a >= 0:
        conta += 1
if b == int:
    b = int(b)
    if b >= 0:
        conta += 1
else:
    b = float(b)
    if b >= 0:
        conta += 1
if c == int:
    c = int(c)
    if c >= 0:
        conta += 1
else:
    c = float(c)
    if c >= 0:
        conta += 1
if d == int:
    d = int(d)
    if d >= 0:
        conta += 1
else:
    d = float(d)
    if d >= 0:
        conta += 1
if e == int:
    e = int(e)
    if e >= 0:
        conta += 1
else:
    e = float(e)
    if e >= 0:
        conta += 1
if f == int:
    f = int(f)
    if f >= 0:
        conta += 1
else:
    f = float(f)
    if f >= 0:
        conta += 1
print('{} valores positivos'.format(conta))

```

### C

```c
#include <stdio.h>
// C - puro → uri_1060 - Números Positivos
int main() { 
    double n, n2, n3, n4, n5, n6, total;
    scanf("%lf", &n);
    scanf("%lf", &n2);
    scanf("%lf", &n3);
    scanf("%lf", &n4);
    scanf("%lf", &n5);
    scanf("%lf", &n6);
    if (n > 0){
        total += 1;}
    if (n2 > 0){
        total += 1;}
    if (n3 > 0){
        total += 1;}
    if (n4 > 0){
        total += 1;}
    if (n5 > 0){
        total += 1;}
    if (n6 > 0){
        total += 1;}
    printf("%.0lf valores positivos\n", total); 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1060 - Números Positivos
using namespace std; 
int main() { 
    float a, b, c, d, e, f;
    int conta = 0;
    cout << fixed;
    cout.precision(1);
    cin >>a>>b>>c>>d>>e>>f;
    if (a > 0){
        conta++;}
    if (b > 0){
        conta++;}
    if (c > 0){
        conta++;}
    if (d > 0){
        conta++;}
    if (e > 0){
        conta++;}
    if (f > 0){
        conta++;}
    cout << "" << conta << " valores positivos" << endl; 
    return 0;
}
```

### Ruby

```ruby
# Ruby → uri_1060 - Números Positivos
a = gets.to_f
b = gets.to_f
c = gets.to_f
d = gets.to_f
e = gets.to_f
f = gets.to_f
total = 0
    if (a > 0)
        total += 1
    end
    if (b > 0)
        total += 1
    end
    if (c > 0)
        total += 1
    end
    if (d > 0)
        total += 1
    end
    if (e > 0)
        total += 1
    end
    if (f > 0)
        total += 1
    end
puts "%.0f valores positivos" % total
```

### Pascal

```pascal
// Pascal → uri_1060 - Números Positivos
program uri_1060;
var
    n, n2, n3, n4, n5, n6, total:real;
begin
    readln(n);
    readln(n2);
    readln(n3);
    readln(n4);
    readln(n5);
    readln(n6);
    total := 0;
    if (n > 0) then
        total += 1;
    if (n2 > 0) then
        total += 1;
    if (n3 > 0) then
        total += 1;
    if (n4 > 0) then
        total += 1;
    if (n5 > 0) then
        total += 1;
    if (n6 > 0) then
        total += 1;
    writeln(total:0:0, ' valores positivos');
readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1060 - Números Positivos
var n = Number(lines.shift());
var n2 = Number(lines.shift());
var n3 = Number(lines.shift());
var n4 = Number(lines.shift());
var n5 = Number(lines.shift());
var n6 = Number(lines.shift());
Total = 0;
if (n > 0) {
    Total = Total + 1
}
if (n2 > 0) {
    Total = Total + 1
}
if (n3 > 0) {
    Total = Total + 1
}
if (n4 > 0) {
    Total = Total + 1
}
if (n5 > 0) {
    Total = Total + 1
}
if (n6 > 0) {
    Total = Total + 1
}
console.log(`${Total.toFixed(0)} valores positivos`);
```

### Lua

```lua
--Lua → uri_1060 - Números Positivos
local n = tonumber(io.read())
local n2 = tonumber(io.read())
local n3 = tonumber(io.read())
local n4 = tonumber(io.read())
local n5 = tonumber(io.read())
local n6 = tonumber(io.read())
Total = 0
    if (n > 0) then
        Total = Total + 1
    end
    if (n2 > 0) then
        Total = Total + 1
    end
    if (n3 > 0) then
        Total = Total + 1
    end
    if (n4 > 0) then
        Total = Total + 1
    end
    if (n5 > 0) then
        Total = Total + 1
    end
    if (n6 > 0) then
        Total = Total + 1
    end
    Total1 = (string.format( "%.0f", Total))
    print(Total1..' valores positivos')
```

### Haskell

```haskell

```

# `XLI` URI Online Judge | 1061

## Tempo de um Evento

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Pedrinho está organizando um evento em sua Universidade. O evento deverá ser no mês de Abril, iniciando e terminando dentro do mês. O problema é que Pedrinho quer calcular o tempo que o evento vai durar, uma vez que ele sabe quando inicia e quando termina o evento.

Sabendo que o evento pode durar de poucos segundos a vários dias, você deverá ajudar Pedrinho a calcular a duração deste evento.

### Entrada

Como entrada, na primeira linha vai haver a descrição “Dia”, seguido de um espaço e o dia do mês no qual o evento vai começar. Na linha seguinte, será informado o momento no qual o evento vai iniciar, no formato **hh : mm : ss**. Na terceira e quarta linha de entrada haverá outra informação no mesmo formato das duas primeiras linhas, indicando o término do evento.

### Saída

Na saída, deve ser apresentada a duração do evento, no seguinte formato:

<p>W dia(s)</p>
<p>X hora(s)</p>
<p>Y minuto(s)</p>
<p>Z segundo(s)</p>
*Obs: Considere que o evento do caso de teste para o problema tem duração mínima de 1 minuto.*

| Exemplo de Entrada                                | Exemplo de Saída                                         |
| ------------------------------------------------- | -------------------------------------------------------- |
| Dia 5 <br>08 : 12 : 23 <br>Dia 9 <br>06 : 13 : 23 | 3 dia(s) <br>22 hora(s) <br>1 minuto(s) <br>0 segundo(s) |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1061 - Tempo de um Evento
d = input()
diaini = d.split()
horaini = input()
hini1 = horaini.split(' : ')
d2 = input()
diaf = d2.split()
horaf = input()
hf2 = horaf.split(' : ')
dia1 = int(diaini[1])
dia2 = int(diaf[1])
h1 = int(hini1[0])
m1 = int(hini1[1])
s1 = int(hini1[2])
h2 = int(hf2[0])
m2 = int(hf2[1])
s2 = int(hf2[2])
if dia1 <= dia2:
    W = (dia2 - dia1)
if h1 < h2 or (h1 - h2) == 0:
    X = (h2 - h1)
if m1 <= m2:
    Y = (m2 - m1)
if s1 <= s2:
    Z = (s2 - s1)
if h1 > h2:
    X = (24-(h1 - h2))
    W = (W - 1)
if m1 > m2:
    Y = (60-(m1-m2))
    X = (X - 1)
if s1 > s2:
    Z = (60 - (s1 - s2))
    Y = (Y - 1)
print(W, 'dia(s)')
print(X, 'hora(s)')
print(Y, 'minuto(s)')
print(Z, 'segundo(s)')

```

### C

```c
#include <stdio.h>
// C - puro → uri_1061 - Tempo de um Evento
int main() { 
   int W, X, Y, Z, d1, h1, m1, s1, d2, h2, m2, s2, segdia1, segdia2, seg_total;
    scanf("Dia %d", &d1);
    scanf("%d : %d : %d\n", &h1, &m1, &s1);
    scanf("Dia %d", &d2);
    scanf("%d : %d : %d", &h2, &m2, &s2);
    segdia1 = (s1 + m1 * 60 + h1 * 60 * 60 + d1 * 60 * 60 * 24);
    segdia2 = (s2 + m2 * 60 + h2 * 60 * 60 + d2 * 60 * 60 * 24);
    seg_total = (segdia2 - segdia1);
    W = seg_total / (60 * 60 * 24);
    X = (seg_total - W * 60 * 60 * 24) / (60 * 60);
    Y = (seg_total - W * 60 * 60 * 24 - X * 60 * 60) / 60;
    Z = seg_total - W * 60 * 60 * 24 - X * 60 * 60 - Y * 60;
    printf("%d dia(s)\n", W);
    printf("%d hora(s)\n", X);
    printf("%d minuto(s)\n", Y);
    printf("%d segundo(s)\n", Z); 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1061 - Tempo de um Evento
using namespace std;
int main()
{
    string g;
    int W, X, Y, Z, d1, h1, m1, s1, d2, h2, m2, s2, segdia1, segdia2, seg_total;
    cin >> g >> d1;
    cin >> h1 >> g >> m1 >> g >> s1;
    cin >> g >> d2;
    cin >> h2 >> g >> m2 >> g >> s2;
    segdia1 = (s1 + m1 * 60 + h1 * 60 * 60 + d1 * 60 * 60 * 24);
    segdia2 = (s2 + m2 * 60 + h2 * 60 * 60 + d2 * 60 * 60 * 24);
    seg_total = (segdia2 - segdia1);
    W = seg_total / (60 * 60 * 24);
    X = (seg_total - W * 60 * 60 * 24) / (60 * 60);
    Y = (seg_total - W * 60 * 60 * 24 - X * 60 * 60) / 60;
    Z = seg_total - W * 60 * 60 * 24 - X * 60 * 60 - Y * 60;
    cout << "" << W << " dia(s)" << endl;
    cout << "" << X << " hora(s)" << endl;
    cout << "" << Y << " minuto(s)" << endl;
    cout << "" << Z << " segundo(s)" << endl;
    return 0;
}
```

### C#

```c#
using System;

class Program
{
    static void Main(string[] args)
    {
        int d1, h1, m1, s1, d2, h2, m2, s2;
        int horafinal1, horafinal2, total;
        int dias, horas, minutos, segundos;
                
        string[] dia1 = Console.ReadLine().Split();
        d1 = Convert.ToInt32(dia1[1]);
        
        String[] horario1 = Console.ReadLine().Split(':');
        h1 = int.Parse(horario1[0]);
        m1 = int.Parse(horario1[1]);
        s1 = int.Parse(horario1[2]);

        string[] dia2 = Console.ReadLine().Split();
        d2 = Convert.ToInt32(dia2[1]);

        string[] horario2 = Console.ReadLine().Split(':');

        h2 = int.Parse(horario2[0]);
        m2 = int.Parse(horario2[1]);
        s2 = int.Parse(horario2[2]);

        horafinal1 = (d1 * 24 * 60 * 60) + (h1 * 60 * 60) + (m1 * 60) + s1;
        horafinal2 = (d2 * 24 * 60 * 60) + (h2 * 60 * 60) + (m2 * 60) + s2;

        total = horafinal2 - horafinal1;

        dias = total / (24 * 60 * 60);
        total = total % (24 * 60 * 60);
        horas = total / (60 * 60);
        total = total % (60 * 60);
        minutos = total / 60;
        total = total % 60;
        segundos = total;

        Console.WriteLine(dias + " dia(s)");
        Console.WriteLine(horas + " hora(s)");
        Console.WriteLine(minutos + " minuto(s)");
        Console.WriteLine(segundos + " segundo(s)");

        Console.ReadKey();
    }
}
```

### Ruby

```ruby
# Ruby → uri_1061 - Tempo de um Evento
# difícil, também deu trabalho, mas foi uma ótima lição de conversão string/integer
d1 = gets.split
dia1 = d1[1].to_i
horas = gets.split
h1 = horas[0].to_i
m1 = horas[2].to_i
s1 = horas[4].to_i
d2 = gets.split
dia2 = d2[1].to_i
horas2 = gets.split
h2 = horas2[0].to_i
m2 = horas2[2].to_i
s2 = horas2[4].to_i
segdia1 = s1 + m1 * 60 + h1 * 60 * 60 + dia1 * 60 * 60 * 24
segdia2 = s2 + m2 * 60 + h2 * 60 * 60 + dia2 * 60 * 60 * 24
seg_total = (segdia2 - segdia1)
W = seg_total / (60 * 60 * 24)
X = (seg_total - W * 60 * 60 * 24) / (60 * 60)
Y = (seg_total - W * 60 * 60 * 24 - X * 60 * 60) / 60
Z = seg_total - W * 60 * 60 * 24 - X * 60 * 60 - Y * 60
puts "%i dia(s)" % W
puts "%i hora(s)" % X
puts "%i minuto(s)" %Y
puts "%i segundo(s)" % Z
```

### Pascal

```pascal
// Pascal → uri_1061 - Tempo de um Evento
program uri_1061;
var
  W, X, Y, Z, segdia1, segdia2, seg_total:longint;
  hora1, hora2, dia1, dia2:string;
  d1, d2, h1, h2, m1, m2, s1, s2:longint;
begin
  readln(dia1);
  readln(hora1);
  readln(dia2);
  readln(hora2);
  VAL(dia1[5..6], d1);
  VAL(dia2[5..6], d2);
  VAL(hora1[1..2], h1);  // 08 : 12 : 23
  VAL(hora1[6..7], m1);
  VAL(hora1[11..12], s1);
  VAL(hora2[1..2], h2);
  VAL(hora2[6..7], m2);
  VAL(hora2[11..12], s2);
 // inicio calculo
     segdia1 := (s1 + m1 * 60 + h1 * 60 * 60 + d1 * 60 * 60 * 24);
     segdia2 := (s2 + m2 * 60 + h2 * 60 * 60 + d2 * 60 * 60 * 24);
     seg_total := (segdia2 - segdia1);
     W := seg_total div (60 * 60 * 24);
     X := (seg_total - W * 60 * 60 * 24) div (60 * 60);
     Y := (seg_total - W * 60 * 60 * 24 - X * 60 * 60) div 60;
     Z := seg_total - W * 60 * 60 * 24 - X * 60 * 60 - Y * 60;
 // fim calculo
  writeln(W, ' dia(s)');
  writeln(X, ' hora(s)');
  writeln(Y, ' minuto(s)');
  writeln(Z, ' segundo(s)');
readln;
end.
```

### Javascript

```javascript

```

### Lua

```lua

```

### Haskell

```haskell

```



# `XLII` URI Online Judge | 1064 ✔

## Positivos e Média

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 6 valores. Em seguida, mostre quantos destes valores digitados foram positivos. Na próxima linha, deve-se mostrar a média de todos os valores positivos digitados, com um dígito após o ponto decimal.

### Entrada

A entrada contém 6 números que podem ser valores inteiros ou de ponto flutuante. Pelo menos um destes números será positivo.

### Saída

O primeiro valor de saída é a quantidade de valores positivos. A próxima linha deve mostrar a média dos valores positivos digitados.

| Exemplo de Entrada                     | Exemplo de Saída            |
| -------------------------------------- | --------------------------- |
| 7 <br>-5 <br>6 <br>-3.4 <br>4.6 <br>12 | 4 valores positivos <br>7.4 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1064 - Positivos e Média
a = input()
b = input()
c = input()
d = input()
e = input()
f = input()
pos = 0
s1 = 0
s2 = 0
s3 = 0
s4 = 0
s5 = 0
s6 = 0
if a == int:
    a = int(a)
    if a >= 0:
        pos += 1
        s1 = a
else:
    a = float(a)
    if a >= 0:
        pos += 1
        s1 = a
if b == int:
    b = int(b)
    if b >= 0:
        pos += 1
        s2 = b
else:
    b = float(b)
    if b >= 0:
        pos += 1
        s2 = b
if c == int:
    c = int(c)
    if c >= 0:
        pos += 1
        s3 = c
else:
    c = float(c)
    if c >= 0:
        pos += 1
        s3 = c
if d == int:
    d = int(d)
    if d >= 0:
        pos += 1
        s4 = d
else:
    d = float(d)
    if d >= 0:
        pos += 1
        s4 = d
if e == int:
    e = int(e)
    if e >= 0:
        pos += 1
        s5 = e
else:
    e = float(e)
    if e >= 0:
        pos += 1
        s5 = e
if f == int:
    f = int(f)
    if f >= 0:
        pos += 1
        s6 = f
else:
    f = float(f)
    if f >= 0:
        pos += 1
        s6 = f
print('{:.0f} valores positivos'.format(pos))
print('{:.1f}'.format((s1 + s2 + s3 + s4 + s5 + s6) / pos))

```

### C

```c
#include <stdio.h>
// C - puro → uri_1064 - Positivos e Média
int main() { 
  double a, b, c, d, e, f, i;
    double pos = 0, soma = 0, media = 0;
    scanf("%lf", &a);
    scanf("%lf", &b);
    scanf("%lf", &c);
    scanf("%lf", &d);
    scanf("%lf", &e);
    scanf("%lf", &f);
    if (a > 0){
        pos += 1;
        soma += a;
    }
    if (b > 0){
        pos += 1;
        soma += b;
    }
    if (c > 0){
        pos += 1;
        soma += c;
    }
    if (d > 0){
        pos += 1;
        soma += d;
    }
    if (e > 0){
        pos += 1;
        soma += e;
    }
    if (f > 0){
        pos += 1;
        soma += f;
    }
    media = soma / pos;
printf("%.0f valores positivos\n", pos);
printf("%.01f\n", media); 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1064 - Positivos e Média
using namespace std; 
int main() { 
    double a, b, c, d, e, f, i;
    double pos = 0, soma = 0, media = 0;
    cout << fixed;
    cin >> a;
    cin >> b;
    cin >> c;
    cin >> d;
    cin >> e;
    cin >> f;
    if (a > 0){
        pos += 1;
        soma += a;
    }
    if (b > 0){
        pos += 1;
        soma += b;
    }
    if (c > 0){
        pos += 1;
        soma += c;
    }
    if (d > 0){
        pos += 1;
        soma += d;
    }
    if (e > 0){
        pos += 1;
        soma += e;
    }
    if (f > 0){
        pos += 1;
        soma += f;
    }
    media = soma / pos;
cout.precision(0);
cout << "" << pos << " valores positivos" <<endl;
cout.precision(1);
cout << "" << media << endl; 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1064
{
    class Program
    {
        static void Main(string[] args)
        {
            double a, b, c, d, e, g;
            double pos = 0;
            double soma = 0;
            double media = 0;
            a = double.Parse(Console.ReadLine());
            b = double.Parse(Console.ReadLine());
            c = double.Parse(Console.ReadLine());
            d = double.Parse(Console.ReadLine());
            e = double.Parse(Console.ReadLine());
            g = double.Parse(Console.ReadLine());

                if (a > 0)
                {
                    pos += 1;
                    soma += a;
                }
                if (b > 0)
                {
                    pos += 1;
                    soma += b;
                }
                if (c > 0)
                {
                    pos += 1;
                    soma += c;
                }
                if (d > 0)
                {
                    pos += 1;
                    soma += d;
                }
                if (e > 0)
                {
                    pos += 1;
                    soma += e;
                }
                if (g > 0)
                {
                    pos += 1;
                    soma += g;
                }
                media = soma / pos;

                Console.WriteLine("{0} valores positivos", pos);
                Console.WriteLine(string.Format("{0:0.0}", media));

                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1064 - Positivos e Média
count = 0
a = gets.to_f
b = gets.to_f
c = gets.to_f
d = gets.to_f
e = gets.to_f
f = gets.to_f
todos = [a, b, c, d, e,f]
for i in todos
    if i > 0
        count += 1
        end
end
positivos = todos.select do |number|
    number > 0
    end 
media = (positivos.inject(:+) / count)        
puts "#{count} valores positivos"
puts media.round(1)
```

### Pascal

```pascal
// Pascal → uri_1064 - Positivos e Média
program uri_1064;
    var
      a, b, c, d, e, f:double;
      pos:integer;
      soma, media:double;
begin
pos := 0;
soma := 0;
media := 0;
readln(a);
readln(b);
readln(c);
readln(d);
readln(e);
readln(f);
    if (a > 0) then
        begin
        pos += 1;
        soma := soma + a;
        end;
    if (b > 0)then
        begin
        pos += 1;
        soma := soma + b;
        end;
    if (c > 0)then
        begin
        pos += 1;
        soma := soma + c;
        end;
    if (d > 0)then
        begin
        pos += 1;
        soma := soma + d;
        end;
    if (e > 0)then
        begin
        pos += 1;
        soma := soma + e;
        end;
    if (f > 0)then
        begin
        pos += 1;
        soma := soma + f;
        end;
media := soma / pos;
writeln(pos, ' valores positivos');
writeln(media:0:1);
readln;
end.
```

### Javascript

```javascript
// Javascript → uri_1064 - Positivos e Média
a = Number(lines.shift());
b = Number(lines.shift());
c = Number(lines.shift());
d = Number(lines.shift());
e = Number(lines.shift());
f = Number(lines.shift());
var pos = 0;
var soma = 0;
if (a > 0){
    pos = pos + 1;
    soma = soma + a;
}
if (b > 0){
    pos = pos + 1;
    soma = soma + b;
}
if (c > 0){
    pos = pos + 1;
    soma = soma + c;
}
if (d > 0){
    pos = pos + 1;
    soma = soma + d;
}
if (e > 0){
    pos = pos + 1;
    soma = soma + e;
}
if (f > 0){
    pos = pos + 1;
    soma = soma + f;
}
media = soma / pos;

console.log(pos + ' valores positivos');
console.log(`${media.toFixed(1)}`);
```

### Lua

```lua
-- Lua → uri_1064 - Positivos e Média
a = tonumber(io.read())
b = tonumber(io.read())
c = tonumber(io.read())
d = tonumber(io.read())
e = tonumber(io.read())
f = tonumber(io.read())
local pos = 0
local soma = 0
if (a > 0) then
    pos = pos + 1
    soma = soma + a
end
if (b > 0) then
    pos = pos + 1
    soma = soma + b
end
if (c > 0) then
    pos = pos + 1
    soma = soma + c
end
if (d > 0) then
    pos = pos + 1
    soma = soma + d
end
if (e > 0) then
    pos = pos + 1
    soma = soma + e
end
if (f > 0) then
    pos = pos + 1
    soma = soma + f
end
local media1 = soma / pos;
local media = (string.format( "%.1f", media1))
print(pos..' valores positivos')
print(media)
```

### Haskell

```haskell

```



# `XLIII` URI Online Judge | 1065 ✔

## Pares entre Cinco Números

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Faça um programa que leia 5 valores inteiros. Conte quantos destes valores digitados são pares e mostre esta informação.

### Entrada

O arquivo de entrada contém 5 valores inteiros quaisquer.

### Saída

Imprima a mensagem conforme o exemplo fornecido, indicando a quantidade de valores pares lidos.

| Exemplo de Entrada           | Exemplo de Saída |
| ---------------------------- | ---------------- |
| 7 <br>-5 <br>6 <br>-4 <br>12 | 3 valores pares  |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1065 - Pares entre 5 números
a = int(input())
b = int(input())
c = int(input())
d = int(input())
e = int(input())
soma = 0
if a % 2 == 0:
    soma += 1
if b % 2 == 0:
    soma += 1
if c % 2 == 0:
    soma += 1
if d % 2 == 0:
    soma += 1
if e % 2 == 0:
    soma += 1
print('{} valores pares'.format(soma))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1065 - Pares entre 5 números
int main() { 
    int a, b, c, d, e, soma = 0;
    scanf("%d", &a);
    scanf("%d", &b);
    scanf("%d", &c);
    scanf("%d", &d);
    scanf("%d", &e);
    if (a % 2 == 0){
        soma += 1;
    }
    if (b % 2 == 0){
        soma += 1;
    }
    if (c % 2 == 0){
        soma += 1;
    }
    if (d % 2 == 0){
        soma += 1;
    }
    if (e % 2 == 0){
        soma += 1;
    }
    printf("%d valores pares\n", soma); 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1065 - Pares entre 5 números
using namespace std; 
int main() {     
    int a, b, c, d, e, soma = 0;
    cin >> a;
    cin >> b;
    cin >> c;
    cin >> d;
    cin >> e;
    if (a % 2 == 0){
        soma += 1;
    }
    if (b % 2 == 0){
        soma += 1;
    }
    if (c % 2 == 0){
        soma += 1;
    }
    if (d % 2 == 0){
        soma += 1;
    }
    if (e % 2 == 0){
        soma += 1;
    }
    cout << soma << " valores pares" << endl; 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1065
{
    class Program
    {
        static void Main(string[] args)
        {
            int a, b, c, d, e, soma = 0;
            a = int.Parse(Console.ReadLine());
            b = int.Parse(Console.ReadLine());
            c = int.Parse(Console.ReadLine());
            d = int.Parse(Console.ReadLine());
            e = int.Parse(Console.ReadLine());

                if (a % 2 == 0)
                {
                    soma += 1;
                }
                if (b % 2 == 0)
                {
                    soma += 1;
                }
                if (c % 2 == 0)
                {
                    soma += 1;
                }
                if (d % 2 == 0)
                {
                    soma += 1;
                }
                if (e % 2 == 0)
                {
                    soma += 1;
                }
                Console.WriteLine("{0} valores pares", soma);

                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1065 - Pares entre 5 números
a = gets.to_i
b = gets.to_i
c = gets.to_i
d = gets.to_i
e = gets.to_i
soma = 0
    if (a % 2 == 0)
        soma += 1
    end
    if (b % 2 == 0)
        soma += 1
    end
    if (c % 2 == 0)
        soma += 1
    end
    if (d % 2 == 0)
        soma += 1
    end
    if (e % 2 == 0)
        soma += 1
    end
    puts "%i valores pares" % soma
```

### Pascal

```pascal
// Pascal → uri_1065 - Pares entre 5 números
program uri_1065;
var
   a, b, c, d, e, soma: integer;
Begin
    readln(a);
    readln(b);
    readln(c);
    readln(d);
    readln(e);
    soma := 0;
    if (a mod 2 = 0) then
        begin
        soma += 1;
    end;
    if (b mod 2 = 0) then
        begin
        soma += 1;
    end;
    if (c mod 2 = 0) then
        begin
        soma += 1;
    end;
    if (d mod 2 = 0) then
        begin
        soma += 1;
    end;
    if (e mod 2 = 0) then
        begin
        soma += 1;
    end;
    writeln(soma, ' valores pares');
    readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1065 - Pares entre 5 números
a = Number(lines.shift());
b = Number(lines.shift());
c = Number(lines.shift());
d = Number(lines.shift());
e = Number(lines.shift());
var Soma = 0;
if (a % 2 == 0) {
    Soma = Soma + 1;
}
if (b % 2 == 0) {
    Soma = Soma + 1;
}
if (c % 2 == 0) {
    Soma = Soma + 1;
}
if (d % 2 == 0) {
    Soma = Soma + 1;
}
if (e % 2 == 0) {
    Soma = Soma + 1;
}
console.log(Soma + ' valores pares');
```

### Lua

```lua
-- Lua → uri_1065 - Pares entre 5 números
local a = tonumber(io.read())
local b = tonumber(io.read())
local c = tonumber(io.read())
local d = tonumber(io.read())
local e = tonumber(io.read())
Soma = 0
if (a % 2 == 0) then
    Soma = Soma + 1
end
if (b % 2 == 0) then
    Soma = Soma + 1
end
if (c % 2 == 0) then
    Soma = Soma + 1
end
if (d % 2 == 0) then
    Soma = Soma + 1
end
if (e % 2 == 0) then
    Soma = Soma + 1
end
print(Soma..' valores pares')
```

### Haskell

```haskell
-- Haskell → uri_1065 - Pares entrre 5 números
```

# `XLIV` URI Online Judge | 1066 ✔

## Pares, Ímpares, Positivos e Negativos

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 5 valores Inteiros. A seguir mostre quantos valores digitados foram pares, quantos valores digitados foram ímpares, quantos valores digitados foram positivos e quantos valores digitados foram negativos.

### Entrada

O arquivo de entrada contém 5 valores inteiros quaisquer.

### Saída

Imprima a mensagem conforme o exemplo fornecido, uma mensagem por linha, não esquecendo o final de linha após cada uma.

| Exemplo de Entrada            | Exemplo de Saída                                             |
| ----------------------------- | ------------------------------------------------------------ |
| -5 <br>0 <br>-3 <br>-4 <br>12 | 3 valor(es) par(es) <br>2 valor(es) impar(es) <br>1 valor(es) positivo(s) <br>3 valor(es) negativo(s) |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1066 - Pares, Ímpares, Positivos e Negativos
a = int(input())
b = int(input())
c = int(input())
d = int(input())
e = int(input())
par = 0
impar = 0
positivo = 0
negativo = 0
if a % 2 == 0:
    par += 1
if a % 2 == 1:
    impar += 1
if a > 0:
    positivo += 1
if a < 0:
    negativo += 1
if b < 0:
    negativo += 1
if b % 2 == 0:
    par += 1
if b % 2 == 1:
    impar += 1
if b > 0:
    positivo += 1
if b < 0:
    negativo += 1
if c % 2 == 0:
    par += 1
if c % 2 == 1:
    impar += 1
if c > 0:
    positivo += 1
if c < 0:
    negativo += 1
if d % 2 == 0:
    par += 1
if d % 2 == 1:
    impar += 1
if d > 0:
    positivo += 1
if d < 0:
    negativo += 1
if e % 2 == 0:
    par += 1
if e % 2 == 1:
    impar += 1
if e > 0:
    positivo += 1
if e < 0:
    negativo += 1
print('{} valor(es) par(es)'.format(par))
print('{} valor(es) impar(es)'.format(impar))
print('{} valor(es) positivo(s)'.format(positivo))
print('{} valor(es) negativo(s)'.format(negativo))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1066 - Pares, Ímpares, Positivos e Negativos
int main() { 
   int num, i;
    int par = 0, impar = 0, pos = 0, negat = 0;
    for (i = 0; i < 5; i++){
        scanf("%d", &num);
    if (num % 2 == 0){
        par++;
    }else{
        impar++;
        }
    if (num > 0 && num != 0){
        pos++;
    }else{
        if (num != 0){
        negat++;
    }
    }
    }
    printf("%d valor(es) par(es)\n", par);
    printf("%d valor(es) impar(es)\n", impar);
    printf("%d valor(es) positivo(s)\n", pos);
    printf("%d valor(es) negativo(s)\n", negat); 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1066 - Pares, Ímpares, Positivos e Negativos
using namespace std; 
int main() { 
    int num, i;
    int par = 0, impar = 0, pos = 0, negat = 0;
    for (i = 0; i < 5; i++){
        cin >> num;
    if (num % 2 == 0){
        par++;
    }else{
        impar++;
        }
    if (num > 0 && num != 0){
        pos++;
    }else{
        if (num != 0){
        negat++;
    }
    }
    }
    cout << par <<  " valor(es) par(es)" << endl;
    cout << impar << " valor(es) impar(es)" << endl;
    cout << pos << " valor(es) positivo(s)" << endl;
    cout << negat << " valor(es) negativo(s)" << endl;
    return 0;
}
```

### C#

```c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace uri1066
{
    class Program
    {
        static void Main(string[] args)
        {
            int num, i;
            int par = 0, impar = 0, pos = 0, negat = 0;
            
            for (i = 0; i < 5; i++)
                {
                num = int.Parse(Console.ReadLine());
                if (num % 2 == 0)
                {
                    par++;
                }
                else
                {
                    impar++;
                }
                if (num > 0 && num != 0)
                {
                    pos++;
                }
                else
                {
                    if (num != 0)
                    {
                        negat++;
                    }
                }
            }
            Console.WriteLine("{0} valor(es) par(es)", par);
            Console.WriteLine("{0} valor(es) impar(es)", impar);
            Console.WriteLine("{0} valor(es) positivo(s)", pos);
            Console.WriteLine("{0} valor(es) negativo(s)", negat);
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1066 - Pares, Ímpares, Positivos e Negativos
a = gets.to_i
b = gets.to_i
c = gets.to_i
d = gets.to_i
e = gets.to_i
par = 0
impar = 0
positivo = 0
negativo = 0
if (a % 2 == 0)
    par += 1
end
if (a % 2 == 1)
    impar += 1
end
if (a > 0)
    positivo += 1
end
if (a < 0)
    negativo += 1
end
if (b < 0)
    negativo += 1
end
if (b % 2 == 0)
    par += 1
end
if (b % 2 == 1)
    impar += 1
end
if (b > 0)
    positivo += 1
end
if (b < 0)
    negativo += 1
end
if (c % 2 == 0)
    par += 1
end
if (c % 2 == 1)
    impar += 1
end
if (c > 0)
    positivo += 1
end
if (c < 0)
    negativo += 1
end
if (d % 2 == 0)
    par += 1
end
if (d % 2 == 1)
    impar += 1
end
if (d > 0)
    positivo += 1
end
if (d < 0)
    negativo += 1
end
if (e % 2 == 0)
    par += 1
end
if (e % 2 == 1)
    impar += 1
end
if (e > 0)
    positivo += 1
end
if (e < 0)
    negativo += 1
end
puts "#{par} valor(es) par(es)"
puts "#{impar} valor(es) impar(es)"
puts "#{positivo} valor(es) positivo(s)"
puts "#{negativo} valor(es) negativo(s)"
```

### Pascal

```pascal
// Pascal → uri_1066 - Pares, Ímpares, Positivos e Negativos
program uri_1066;
var
   a, b, c, d, e, par, impar, positivo, negativo: longint;
Begin
     readln(a);
     readln(b);
     readln(c);
     readln(d);
     readln(e);
     par := 0;
     impar := 0;
     positivo := 0;
     negativo := 0;
     if (a mod 2 = 0) then
       begin
         par += 1;
       end;
     if (a mod 2 = 1) then
       begin
         impar += 1;
       end;
     if (a > 0) then
       begin
         positivo += 1;
       end;
     if (a < 0) then
       begin
         negativo += 1;
       end;
     if (b < 0) then
       begin
         negativo += 1;
       end;
     if (b mod 2 = 0) then
       begin
         par += 1;
       end;
     if (b mod 2 = 1) then
       begin
         impar += 1;
       end;
     if (b > 0) then
       begin
          positivo += 1;
       end;
     if (b < 0) then
       begin
         negativo += 1;
       end;
     if (c mod 2 = 0) then
       begin
         par += 1;
       end;
     if (c mod 2 = 1) then
       begin
         impar += 1;
       end;
     if (c > 0) then
       begin
         positivo += 1;
       end;
     if (c < 0) then
       begin
         negativo += 1;
       end;
     if (d mod 2 = 0) then
       begin
         par += 1;
       end;
     if (d mod 2 = 1) then
       begin
         impar += 1;
       end;
     if (d > 0) then
       begin
         positivo += 1;
       end;
     if (d < 0) then
       begin
         negativo += 1;
       end;
     if (e mod 2 = 0) then
       begin
         par += 1;
       end;
     if (e mod 2 = 1) then
       begin
         impar += 1;
       end;
     if (e > 0) then
       begin
         positivo += 1;
       end;
     if (e < 0) then
       begin
         negativo += 1;
       end;
     writeln(par,' valor(es) par(es)');
     writeln(impar,' valor(es) impar(es)');
     writeln(positivo,' valor(es) positivo(s)');
     writeln(negativo,' valor(es) negativo(s)');
     readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1066 - Pares, Ímpares, Positivos e Negativos
var a = Number(lines.shift());
var b = Number(lines.shift());
var c = Number(lines.shift());
var d = Number(lines.shift());
var e = Number(lines.shift());
var par = 0;
var impar = 0;
var positivo = 0;
var negativo = 0;
if (a % 2 == 0) {
    par = par + 1;
}
if (a % 2 == 1) {
    impar = impar + 1;
}
if (a > 0) {
    positivo = positivo + 1;
}
if (a < 0) {
    negativo = negativo + 1;
}
if (b < 0) {
    negativo = negativo + 1;
}
if (b % 2 == 0) {
    par = par + 1;
}
if (b % 2 == 1) {
    impar = impar + 1;
}
if (b > 0) {
    positivo = positivo + 1;
}
if (b < 0) {
    negativo = negativo + 1;
}
if (c % 2 == 0) {
    par = par + 1;
}
if (c % 2 == 1) {
    impar = impar + 1;
}
if (c > 0) {
    positivo = positivo + 1;
}
if (c < 0) {
    negativo = negativo + 1;
}
if (d % 2 == 0) {
    par = par + 1;
}
if (d % 2 == 1) {
    impar = impar + 1;
}
if (d > 0) {
    positivo = positivo + 1;
}
if (d < 0) {
    negativo = negativo + 1;
}
if (e % 2 == 0) {
    par = par + 1;
}
if (e % 2 == 1) {
    impar = impar + 1;
}
if (e > 0) {
    positivo = positivo + 1;
}
if (e < 0) {
    negativo = negativo + 1;
}
console.log(par +' valor(es) par(es)');
console.log(impar +' valor(es) impar(es)');
console.log(positivo + ' valor(es) positivo(s)');
console.log(negativo + ' valor(es) negativo(s)');
```

### Lua

```lua
-- Lua → uri_1066 - Pares, Ímpares, Positivos e Negativos
local a = tonumber(io.read())
local b = tonumber(io.read())
local c = tonumber(io.read())
local d = tonumber(io.read())
local e = tonumber(io.read())
local par = 0
local impar = 0
local positivo = 0
local negativo = 0
if (a % 2 == 0) then
    par = par + 1
end
if (a % 2 == 1) then
    impar = impar + 1
end
if (a > 0) then
    positivo = positivo + 1
end
if (a < 0) then
    negativo = negativo + 1
end
if (b < 0) then
    negativo = negativo + 1
end
if (b % 2 == 0) then
    par = par + 1
end
if (b % 2 == 1) then
    impar = impar + 1
end
if (b > 0) then
    positivo = positivo + 1
end
if (b < 0) then
    negativo = negativo + 1
end
if (c % 2 == 0) then
    par = par + 1
end
if (c % 2 == 1) then
    impar = impar + 1
end
if (c > 0) then 
    positivo = positivo + 1
end
if (c < 0) then
    negativo = negativo + 1
end
if (d % 2 == 0) then
    par = par + 1
end
if (d % 2 == 1) then
    impar = impar + 1
end
if (d > 0) then
    positivo = positivo + 1
end
if (d < 0) then
    negativo = negativo + 1
end
if (e % 2 == 0) then
    par = par + 1
end
if (e % 2 == 1) then
    impar = impar + 1
end
if (e > 0) then
    positivo = positivo + 1
end
if (e < 0) then
    negativo = negativo + 1
end
print(par..' valor(es) par(es)')
print(impar..' valor(es) impar(es)')
print(positivo..' valor(es) positivo(s)')
print(negativo..' valor(es) negativo(s)')
```

### Haskell

```haskell
-- Haskell → uri_1066 - Pares, Ímpares, Positivos e Negativos
```



# `XLV` URI Online Judge | 1067 ✔

## Números Ímpares

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro **X** (1 <= **X** <= 1000). Em seguida mostre os ímpares de 1 até **X**, um valor por linha, inclusive o **X**, se for o caso.

### Entrada

O arquivo de entrada contém 1 valor inteiro qualquer.

### Saída

Imprima todos os valores ímpares de 1 até **X**, inclusive **X**, se for o caso.

| Exemplo de Entrada | Exemplo de Saída    |
| ------------------ | ------------------- |
| 8                  | 1 <br>3 <br>5 <br>7 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1067 - Números Ímpares
n = int(input())
if n % 2 == 1:
    for n in range(1, n + 1, 2):
        print(n)
if n % 2 == 0:
    for n in range(1, n, 2):
        print(n)

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1067 - Números Ímpares
int main() { 
   int num, impar, i;
    scanf("%d", &num);
    printf("1\n");
    for (i = 1; i < num - 1; i += 2) {
       impar = i + 2;
        printf("%d\n", impar);
    }
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1067 - Números Ímpares
using namespace std; 
int main() {     
    int num, impar, i;
    cin >> num;
    cout << "1" << endl;
    for (i = 1; i < num - 1; i += 2) {
       impar = i + 2;
        cout << impar << endl;
    } 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1067
{
    class Program
    {
        static void Main(string[] args)
        {
            int num, impar, i;
            num = int.Parse(Console.ReadLine());
            Console.WriteLine("1");
            for (i = 1; i < num - 1; i += 2)
            {
                impar = i + 2;
                Console.WriteLine("{0}", impar);
            }
            Console.ReadKey();         
        }
    }
}
```

### C#

```c#
using System;

namespace uri1070
{
    class Program
    {
        static void Main(string[] args)
        {
            int num, i, impar;
            num = int.Parse(Console.ReadLine());
            
            for (i = num; i < (num + (6 * 2)); i += 2)
            {
                if (i % 2 == 0)
                {
                    impar = i + 1;
                    Console.WriteLine("{0}", impar);
                }
                else
                {
                    impar = i;
                    Console.WriteLine("{0}", impar);
                }
            }
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1067 - Números Ímpares
n = gets.to_i
for i in 0..n
	if i % 2 == 1
    puts i
    end
end
```

### Pascal

```pascal
// Pascal → uri_1067 - Números Ímpares
program uri_1067;
var
  i, n: integer;
begin
  readln(n);
for i := 1 to n do
	if (i mod 2 = 1) then
        begin
    writeln(i);
    end;
readln;
end.
```

### Javascript

```javascript
// Javascript → uri_1067 - Números Ímpares
num = Number(lines.shift());
console.log("1");
    for (i = 1; i < num - 1; i += 2) {
       impar = i + 2;
        console.log(`${impar}`);
    }
```

### Lua

```lua
-- Lua → uri_1067 - Números Ímpares
local num = tonumber(io.read())
local i = 0
while (i <= (num - 1)) do
    i = i + 1
    if (i % 2 == 1) then
    print(i)
    end
end
```

### Haskell

```haskell

```



# `XLVI` URI Online Judge | 1070 ✔

## Seis Números Ímpares

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro **X**. Em seguida apresente os 6 valores ímpares consecutivos a partir de **X**, um valor por linha, inclusive o **X** ser for o caso.

### Entrada

A entrada será um valor inteiro positivo.

### Saída

A saída será uma sequência de seis números ímpares.

| Exemplo de Entrada | Exemplo de Saída                     |
| ------------------ | ------------------------------------ |
| 8                  | 9 <br>11 <br>13 <br>15 <br>17 <br>19 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1070 - Seis números ímpares
a = 1
X = int(input())
c = 0
while a <= 6:
    if (X % 2) == 0:
        c = X + 1
        print(c)
    else:
        c = X
        print(c)
        c += 2
    a += 1
    X += 2

```

### C

```c
#include <stdio.h>
// C - puro → uri_1070 - Seis números ímpares
int main() { 
   int num, i, impar;
    scanf("%d", &num);    
    for (i = num; i < (num + (6 * 2)); i += 2) {
        if (i % 2 == 0){
        impar = i + 1;
        printf("%d\n", impar);
    }
    else{
        impar = i;
        printf("%d\n", impar);
    }
    } 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1070 - Seis números ímpares
using namespace std; 
int main() {     
    int num, i, impar;
    cin >> num;
    for (i = num; i < (num + (6 * 2)); i += 2) {
        if (i % 2 == 0){
        impar = i + 1;
        cout << impar << endl;
    }
    else{
        impar = i;
        cout << impar << endl;
    }
    } 
    return 0;
}
```

### Ruby

```ruby
# Ruby → uri_1070 - Seis números ímpares
n = gets.to_i
for i in n..n += 12
	if i % 2 == 1
    puts i
    end
end
```

### Pascal

```pascal
// Pascal → uri_1070 - Seis números ímpares
program uri_1070;
    var
       num, i, count:integer;
begin
    count := 0;
    readln(num);
    for i:= num to num + 12 do begin
        if (i mod 2 = 1) then
            writeln(i);
            count += 1;
        if (count = 12) then
        break;
    end;
    readln;
    end.
```

### Javascript

```javascript
// Javascript → uri_1070 - Seis números ímpares
var num = Number(lines.shift());
var i = num;
while (i <= (num + 11)){
    i = i + 1;
    if (i % 2 == 1) {
    console.log(i);
    }
}
```

### Lua

```lua
-- Lua → uri_1070 - Seis números ímpares
local num = tonumber(io.read())
local i = num
while (i <= (num + 11)) do
    i = i + 1
    if (i % 2 == 1) then
    print(i)
    end
end
```

### Haskell

```haskell

```



# `XLVII` URI Online Judge | 1071 <font color =red>**</font>

## Soma de Impares Consecutivos I

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 2 valores inteiros **X** e **Y**. A seguir, calcule e mostre a soma dos números impares entre eles.

### Entrada

O arquivo de entrada contém dois valores inteiros.

### Saída

O programa deve imprimir um valor inteiro. Este valor é a soma dos valores ímpares que estão entre os valores fornecidos na entrada que deverá caber em um inteiro.

| Exemplo de Entrada | Exemplo de Saída |
| ------------------ | ---------------- |
| 6 <br>-5           | 5                |
| 15 <br>12          | 13               |
| 12 <br>12          | 0                |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → Soma de Impares Consecutivos I
X = int(input())
Y = int(input())
conta = 0
if X > Y:
    while Y < X:
        Y = Y + 1
        if (Y % 2) == 1 and Y != X:
            conta += Y
if Y > X:
    while X < Y:
        X = X + 1
        if (X % 2) == 1 and X != Y:
            conta += X
print(conta)

```

### C

```c
#include <stdio.h>
// C - puro → Soma de Impares Consecutivos I
int main()  
   int x, y, conta = 0, i;
    int mais, menos;
    scanf("%d", &x);
    scanf("%d", &y);
    if(x < y){
    menos = x;
    mais = y;
 }
    else{
    mais = x;
    menos = y;
 }
    for (i = (menos + 1); i < mais; ++i)
 {
    if(i % 2 == 1 || i % 2 == -1){
    conta += i;
  }
 }
    printf("%d\n", conta);
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → Soma de Impares Consecutivos I
using namespace std; 
int main() { 
    int x, y, conta = 0, i;
    int mais, menos;
    cin >> x;
    cin >> y;
    if(x < y){
    menos = x;
    mais = y;
 }
    else{
    mais = x;
    menos = y;
 }
    for (i = (menos + 1); i < mais; ++i)
 {
    if(i % 2 == 1 || i % 2 == -1){
    conta += i;
  }
 }
    cout << conta << endl;
    return 0;
}
```

### C#

```c#
using System;

namespace uri1071
{
    class Program
    {
        static void Main(string[] args)
        {
            int x, y, conta = 0, i;
            int mais, menos;
            
            x = int.Parse(Console.ReadLine());
            y = int.Parse(Console.ReadLine());

            if (x < y)
            {
                menos = x;
                mais = y;
            }
            else
            {
                mais = x;
                menos = y;
            }            
            for (i = (menos + 1); i < mais; ++i)
            {
                if (i % 2 == 1 || i % 2 == -1)
                {
                    conta += i;
                }
            }            
            Console.WriteLine("{0}", conta);

            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → Soma de Impares Consecutivos I
conta = 0
x = gets.to_i
y = gets.to_i
if x > y
    while y < x
        y = y + 1
        if (y % 2) == 1 and y != x
            conta += y
            end
if y > x
    while x < y
        x = x + 1
        if (x % 2) == 1 and x != y
            conta += x
            end
end
end
end
end
puts conta
```

### Pascal

```pascal
(*Não apresentou erro mas o exercício está faltando 15% para estar totalmente correto*)
// Pascal → Soma de Impares Consecutivos I
Program uri_1071;
    var
        x, y, menor, maior, impar:integer;
        i:integer;
begin
    x := 0;
    y := 0;
    i := 0;
    impar := 0;
    readln(x);
    readln(y);

     if (y < x) then begin
        menor := y;
        maior := x;
     end
     else if(x < y) then begin
        menor := x;
        maior := y;
     end;

      for i := menor + 1 to maior - 1 do
         if ((i mod 2) <> 0) then begin
            impar := impar + i;
         end;

     writeln(impar);
     readln;
end.
```

### Javascript

```javascript
// Javascript → uri_1071 - Soma de Impares Consecutivos I
var x = Number(lines.shift());
var y = Number(lines.shift());
var conta = 0;
 if(x < y){
    var menos = x;
    var mais = y;
 }
    else{
    mais = x;
    menos = y;
 }
    for (i = (menos + 1); i < mais; i++)
 {
    if((i % 2 == 1) || (i % 2 == -1)){
    var conta = conta + i;
  }
 }
console.log(conta);
```

### Lua

```lua
-- Lua → uri_1071 - Soma de Impares Consecutivos I
X = tonumber(io.read())
Y = tonumber(io.read())
Conta = 0
if (X > Y) then
    while (Y < X) do
        Y = Y + 1
        if (((Y % 2) == 1) and (Y ~= X)) then
            Conta = Conta + Y
if (Y > X) then
    while (X < Y) do
        X = X + 1
        if (X % 2) == 1 and X ~= Y then
            Conta = Conta + X
        end
    end
end
end
end
end
print(Conta)
```

Haskell

```haskell

```



# `XLVIII` URI Online Judge | 1072 ✔

## Intervalo 2

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro **N**. Este valor será a quantidade de valores inteiros **X** que serão lidos em seguida.
Mostre quantos destes valores **X** estão dentro do intervalo [10,20] e quantos estão fora do intervalo, mostrando essas informações.

### Entrada

A primeira linha da entrada contém um valor inteiro **N** (**N** < 10000), que indica o número de casos de teste.
Cada caso de teste a seguir é um valor inteiro **X** (-107 < **X** <107).


### Saída

Para cada caso, imprima quantos números estão dentro (**in**) e quantos valores estão fora (**out**) do intervalo.

| Exemplo de Entrada              | Exemplo de Saída |
| ------------------------------- | ---------------- |
| 4 <br>14 <br>123 <br>10 <br>-25 | 2 in <br>2 out   |

### Python 3

```python 3
# -*- coding: utf-8 -*-
# Python 3 → uri_1072 - Intervalo 2
N = int(input())
conta = 1
dentro = 0
fora = 0
if N < 10000:
    while conta <= N:
        X = int(input())
        if X > (-10**7) or X < (10**7):
            if 10 <= X <= 20:
                dentro += 1
            else:
                fora += 1
            conta += 1
    print('{} in'.format(dentro))
    print('{} out'.format(fora))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1072 - Intervalo 2
int main() { 
  int X, x, conta = 0, dentro = 0, fora = 0;
    scanf("%d", &x);
    while (conta < x){
        conta++;
    scanf("%d", &X);
    if (X >= 10 && X <= 20){
            dentro++;
        }
        else{
            fora++;
        }
    }
    printf("%d in\n", dentro);
    printf("%d out\n", fora);    
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1072 - Intervalo 2
using namespace std; 
int main() { 
    int X, x, conta = 0, dentro = 0, fora = 0;
    cin >> x;
    while (conta < x){
        conta++;
    cin >> X;
    if (X >= 10 && X <= 20){
            dentro++;
        }
        else{
            fora++;
        }
    }
    cout << dentro << " in" << endl;
    cout << fora << " out" << endl; 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1072
{
    class Program
    {
        static void Main(string[] args)
        {
            int X, x, conta = 0, dentro = 0, fora = 0;

            x = int.Parse(Console.ReadLine());

            while (conta < x)
            {
                conta++;

                X = int.Parse(Console.ReadLine());
                if (X >= 10 && X <= 20)
                {
                    dentro++;
                }
                else
                {
                    fora++;
                }
            }
            Console.WriteLine("{0} in", dentro);
            Console.WriteLine("{0} out", fora);
        
            Console.ReadKey();
        }
    }
}
```

### Ruby

```ruby
# -*- coding: utf-8 -*-
# Ruby - correto → uri_1072 - Intervalo 2
n = gets.to_i
conta = 0
dentro = 0
fora = 0
    for i in(1..n)
        x = gets.to_i
        if x > (-10**7) or x < (10**7)
            if 10 <= x and x <= 20
                dentro += 1             
            else
                fora += 1            
            end
            conta += 1       
end
end        
puts "#{dentro} in\n"
puts "#{fora} out"
```

### Pascal

```pascal
// Pascal → uri_1072 - Intervalo 2
program uri_1072;
var
  i, y, X, conta, dentro, fora: integer;
begin
    conta := 0;
    dentro := 0;
    fora := 0;
    readln(y);
    for i := 1 to y do
        begin
          conta += 1;
        readln(X);
    if ((X >= 10) and (X <= 20)) then
            begin
            dentro += 1;
        end
        else
        begin
            fora += 1;
        end;
        end;
    writeln(dentro,' in');
    writeln(fora,' out');
readln;
end.
```

### Javascript

```javascript
// Javascript → uri_1072 - Intervalo 2

var x = Number(lines.shift());
var conta = 0;
var dentro = 0;
var fora = 0;
    while (conta < x){
        conta = conta + 1;
        var X1 = Number(lines.shift());
    if (X1 >= 10 && X1 <= 20){
            dentro = dentro + 1;
        }
        else{
            fora = fora + 1;
        }
    }
    console.log(dentro + " in");
    console.log(fora + " out"); 
```

### Lua

```lua
-- Lua → uri_1072 - Intervalo 2
local x = tonumber(io.read())
local conta = 0
local dentro = 0
local fora = 0
while (conta < x) do
    conta = conta + 1
    X = tonumber(io.read())
    if ((X >= 10) and (X <= 20)) then
        dentro = dentro + 1
    else
        fora = fora + 1
    end
end
print(dentro.." in")
print(fora.." out")
```

### Haskell

```haskell

```



# `XLIX` URI Online Judge | 1073 ✔

## Quadrado de Pares

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro **N**. Apresente o quadrado de cada um dos valores pares, de 1 até **N**, inclusive **N**, se for o caso.

### Entrada

A entrada contém um valor inteiro **N** (5 < **N** < 2000).

### Saída

Imprima o quadrado de cada um dos valores pares, de 1 até **N**, conforme o exemplo abaixo.

Tome cuidado! Algumas linguagens tem por padrão apresentarem como saída 1e+006 ao invés de 1000000 o que ocasionará resposta errada. Neste caso, configure a precisão adequadamente para que isso não ocorra.

| Exemplo de Entrada | Exemplo de Saída                  |
| ------------------ | --------------------------------- |
| 6                  | 2^2 = 4 <br>4^2 = 16 <br>6^2 = 36 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1073 - Quadrado de Pares
N = int(input())
conta = 1
quadrado = 0
while conta <= N and quadrado < N:
    if (N % 2) == 0:
        quadrado += 2
    print(str(quadrado) + '^2 =', (quadrado ** 2))
    conta += 1

```

### C

```c
#include <stdio.h>
// C - puro  → uri_1073 - Quadrado de Pares
int main() { 
      int n, i;
      scanf("%d", &n);
      for(i = 1; i <= n; ++i){
          if (i % 2 == 0){
          printf("%d^2 = %d\n", i, (i * i));
        }
    } 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1073 - Quadrado de Pares
using namespace std; 
int main() { 
      int n, i;
      cin >> n;
      for(i = 1; i <= n; ++i){
          if (i % 2 == 0){
          cout << i << "^2 = " << (i * i) << endl;
        }
    } 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1073
{
    class Program
    {
        static void Main(string[] args)
        {
            int n, i;
            
            n = int.Parse(Console.ReadLine());

            for (i = 1; i <= n; ++i)
            {
                if (i % 2 == 0)
                {
                    Console.WriteLine("{0}^2 = {1}", i, (i * i));
                }
            }
                Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1073 - Quadrado de Pares
n = gets.to_i
conta = 1
quadrado = 0
while conta < n and quadrado < n
    if (n % 2) == 0
        quadrado += 2
    puts "#{quadrado}^2 = #{quadrado*quadrado}"
    conta += 1
end
end
```

### Pascal

```pascal
// Pascal → uri_1073 - Quadrado de Pares
program uri_1073;
   var
     N, conta, quadrado :integer;
begin
  readln(N);
conta := 1;
quadrado := 0;
while (conta <= N) and (quadrado < N) do
    if ((N mod 2) = 0) then
        begin
        quadrado += 2;
    writeln(quadrado,'^2 = ', (quadrado *quadrado));
    conta += 1
        end;
 readln;
end.
```

### Javascript

```javascript
// Javascript → uri_1073 - Quadrado de Pares
var n = Number(lines.shift());
Conta = 1;
Quadrado = 0;
while ((Conta < n) && (Quadrado < n)){
    if ((n % 2) == 0) {
        Quadrado = Quadrado + 2;
    console.log(Quadrado + "^2 = " + (Quadrado*Quadrado));
    Conta = Conta + 1;
}
}
```

### Lua

```lua
-- Lua → uri_1073 - Quadrado de Pares
local n = tonumber(io.read())
Conta = 1
Quadrado = 0
while ((Conta < n) and (Quadrado < n)) do
    if ((n % 2) == 0) then
        Quadrado = Quadrado + 2
    print(Quadrado.."^2 = "..(Quadrado*Quadrado))
    Conta = Conta + 1
end
end
```

### Haskell

```haskell

```



# `L` URI Online Judge | 1074

## Par ou Ímpar

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro **N**. Este valor será a quantidade de valores que serão lidos em seguida. Para cada valor lido, mostre uma mensagem em inglês dizendo se este valor lido é par (*EVEN*), ímpar (*ODD*), positivo (*POSITIVE*) ou negativo (*NEGATIVE*). No caso do valor ser igual a zero (0), embora a descrição correta seja (*EVEN NULL*), pois por definição zero é par, seu programa deverá imprimir apenas *NULL*.

### Entrada

A primeira linha da entrada contém um valor inteiro **N**(**N** < 10000) que indica o número de casos de teste. Cada caso de teste a seguir é um valor inteiro **X** (-107 < **X** <107).

### Saída

Para cada caso, imprima uma mensagem correspondente, de acordo com o exemplo abaixo. Todas as letras deverão ser maiúsculas e sempre deverá haver um espaço **entre** duas palavras impressas na mesma linha.

| Exemplo de Entrada          | Exemplo de Saída                                         |
| --------------------------- | -------------------------------------------------------- |
| 4 <br>-5 <br>0 <br>3 <br>-4 | ODD NEGATIVE <br>NULL <br>ODD POSITIVE <br>EVEN NEGATIVE |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3
N = int(input())
conta = 0
while conta != N:
    conta += 1
    X = int(input())
    if X == 0:
        print('NULL')
    elif (X % 2) == 0:
        if X > 0:
            print('EVEN POSITIVE')
        if X < 0:
            print('EVEN NEGATIVE')
    elif (X % 2) == 1:
        if X > 0:
            print('ODD POSITIVE')
        if X < 0:
            print('ODD NEGATIVE')

```

### C

```c
#include <stdio.h>
 // C - puro
int main() { 
 int n, i, x;
    scanf("%d", &n);
    for( i = 1; i <= n; i++){
    scanf("%d", &x);    
    if(x == 0){
        printf("NULL\n");
    }else if(x % 2 == 0){
    if(x > 0){
        printf("EVEN POSITIVE\n");
    }else{
        printf("EVEN NEGATIVE\n");
   }
    }else{
    if(x > 0){
        printf("ODD POSITIVE\n");
    }else{
        printf("ODD NEGATIVE\n");
   }
  }
 }
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++
using namespace std; 
int main() { 
    int n, i, x;
    cin >> n;
    for( i = 1; i <= n; i++){
    cin >> x;
    if(x == 0){
        cout << "NULL" << endl;
    }else if(x % 2 == 0){
    if(x > 0){
        cout << "EVEN POSITIVE" << endl;
    }else{
        cout << "EVEN NEGATIVE" << endl;
   }
    }else{
    if(x > 0){
        cout << "ODD POSITIVE" << endl;
    }else{
        cout << "ODD NEGATIVE" << endl;
   }
  }
 } 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1074
{
    class Program
    {
        static void Main(string[] args)
        {
            int n, i, x;
            n = int.Parse(Console.ReadLine());
            for (i = 1; i <= n; i++)
            {
                x = int.Parse(Console.ReadLine());
                
                if (x == 0)
                {
                    Console.WriteLine("NULL");
                }
                else if (x % 2 == 0)
                {
                    if (x > 0)
                    {
                        Console.WriteLine("EVEN POSITIVE");
                    }
                    else
                    {
                        Console.WriteLine("EVEN NEGATIVE");
                    }
                }
                else
                {
                    if (x > 0)
                    {
                        Console.WriteLine("ODD POSITIVE");
                    }
                    else
                    {
                        Console.WriteLine("ODD NEGATIVE");
                    }
                }
            }
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby - uri_1074
N = gets.to_i
for i in 1..N
    y = gets.chomp.to_i    
		if y == 0
			puts "NULL"		
		elsif y % 2 == 0
			if y > 0
				puts "EVEN POSITIVE"
			end		   
			if y < 0
				puts "EVEN NEGATIVE"
			end			
		elsif y % 2 == 1
			if y > 0
				puts "ODD POSITIVE"
			end		   
			if y < 0
				puts "ODD NEGATIVE"
			end
	    end
end

```

### Pascal

```pascal
program uri_1074;
// Pascal
   var
     N, i, x:integer;
begin
    readln(N);
    for i := 1 to N do begin
        readln(x);
    if (x mod 2 = 0) and (x > 0) then
        begin
            writeln('EVEN POSITIVE')
            end
          else if (x mod 2 = 0) and (x < 0) then begin
                    writeln('EVEN NEGATIVE')
                    end
                else
                  if (x mod 2 <> 0) and (x > 0) then begin
                     writeln('ODD POSITIVE')
                  end
                  else
                    if (x mod 2 <> 0) and (x < 0) then begin
                        writeln('ODD NEGATIVE')
                    end
                       else if (x = 0) then
                         writeln('NULL');
    end;
readln;
end.
```

### Javascript

```javascript

```

### Lua

```lua
-- Lua → uri_1074 - Par ou Ímpar
N = tonumber(io.read())
i = 0
while (i < N) do
    Y = tonumber(io.read())
    i = i + 1
		if (Y == 0) then
			print("NULL")
		else if (Y % 2 == 0) then
			if (Y > 0) then
				print("EVEN POSITIVE")
            end
			if (Y < 0) then
				print("EVEN NEGATIVE")
			end	
		else if (Y % 2 == 1) then
			if (Y > 0) then
				print("ODD POSITIVE")
			end
			if (Y < 0) then
				print("ODD NEGATIVE")
			end
        end
    end
end
end
```

### Haskell

```haskell

```



# `LI` URI Online Judge | 1075 ✔

## Resto 2

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia um valor inteiro **N**. Apresente todos os números entre 1 e 10000 que divididos por **N** dão resto igual a 2.

### Entrada

A entrada contém um valor inteiro **N** (**N** < 10000).

### Saída

Imprima todos valores que quando divididos por **N** dão resto = 2, um por linha.



| Exemplo de Entrada | Exemplo de Saída           |
| ------------------ | -------------------------- |
| 13                 | 2 <br>15 <br>28 <br>41 ... |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1075 - Resto 2
N = int(input())
conta = 1
if (N > 1) and N < 10000:
    while conta < 10000:
        conta += 1
        if (conta % N) == 2:
            print(conta)

```

### C

```c
#include <stdio.h>
// C - puro → uri_1075 - Resto 2
int main() {
 
    int n, conta;

    scanf("%i", &n);

    for (conta = 1; conta <= 10000; ++conta){
        if(conta % n == 2){
    printf("%i\n", conta);
  }
 }
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1075 - Resto 2
using namespace std; 
int main() { 
    int n, conta;
    cin >> n;
    for (conta = 1; conta <= 10000; ++conta){
        if(conta % n == 2){
    cout << conta << endl;
  }
 } 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1075
{
    class Program
    {
        static void Main(string[] args)
        {
            int n, conta;

            n = int.Parse(Console.ReadLine());

            for (conta = 1; conta <= 10000; ++conta)
            {
                if (conta % n == 2)
                {
                    Console.WriteLine("{0}", conta);
                }
            }
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1075 - Resto 2
n = gets.to_i
for i in 1..10000
    if i % n == 2
    puts "%i\n" % i
    end
end
```

### Pascal

```pascal
// Pascal → uri_1075 - Resto 2
program uri_1075;
   var
     n, i:integer;
begin
  readln(n);
  for i:= 1 to 10000 do
    if (i mod n = 2) then
    begin
      writeln(i);
    end;
readln();
end.
```

### Javascript

```javascript
// Javascript → uri_1075 - Resto 2
var N = Number(lines.shift());
conta = 1;
if ((N > 1) && (N < 10000)){
    while (conta < 10000){
        conta += 1;
        if ((conta % N) == 2){
            console.log(conta);
}
}
}
```

### Lua

```lua
--local vPar = 0 -- Declara-se uma variavel local de nome "vPar"
N1 = tonumber(io.read())
local i = 0
for i=2, 10000, N1 do
    print(i)
end
```

### Haskell

```haskell

```



# `LII` URI Online Judge | 1078 ✔

## Tabuada

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 1 valor inteiro N (2 < N < 1000). A seguir, mostre a tabuada de N:      
1 x N = N      2 x N = 2N        ...       10 x N = 10N

### Entrada

A entrada contém um valor inteiro **N** (2 < **N** < 1000).

### Saída

Imprima a tabuada de N, conforme o exemplo fornecido.



| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
| 140                | 1 x 140 = 140 <br>2 x 140 = 280 <br>3 x 140 = 420 <br>4 x 140 = 560 <br>5 x 140 = 700 <br>6 x 140 = 840 <br>7 x 140 = 980 <br>8 x 140 = 1120 <br>9 x 140 = 1260 <br>10 x 140 = 1400 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1078 - Tabuada
N = int(input())
conta = 0
while conta != 10:
    conta += 1
    print('{} x {} = {}'.format(conta, N, conta * N))

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1078 - Tabuada
int main() { 
     int i, n;
     scanf("%d", &n);
     for(i =1; i <= 10; i++)
        printf("%d x %d = %d\n", i, n, i * n);
 
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++ → uri_1078 - Tabuada
using namespace std; 
int main() { 
     int i, n;
     cin >> n;
     for(i =1; i <= 10; i++)
        cout << i << " x " << n << " = " << i * n << endl; 
    return 0;
}
```

### C#

```c#
using System;

namespace uri1078
{
    class Program
    {
        static void Main(string[] args)
        {
            int i, n;
            n = int.Parse(Console.ReadLine());
            for (i = 1; i <= 10; i++)
                Console.WriteLine("{0} x {1} = {2}", i, n, i * n);
            
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1078 - Tabuada
n = gets.to_i
for i in 1..10
	puts "#{i} x #{n} = #{i*n}"
end
```

### Pascal

```pascal
// Pascal → uri_1078 - Tabuada
program uri_1078;
   var
     n, i:integer;
begin
  readln(n);
  for i:= 1 to 10 do
    begin
      writeln(i, ' x ', n, ' = ', i*n);
    end;
readln();
end.
```

### Javascript

```javascript
var input = require('fs').readFileSync('/dev/stdin', 'utf8');
var lines = input.split('\n');
// Javascript → uri_1078 - Tabuada
var N = Number(lines.shift());
var conta = 0;
while (conta != 10){
    conta = conta + 1;
    console.log(`${conta} x ${N} = ${conta*N}`);}
```

### Lua

```lua
-- Lua → uri_1078 - Tabuada
local n = tonumber(io.read())
local conta = 0
while (conta ~= 10) do
    conta = conta + 1
    print(conta..' x '..n..' = '..(conta*n))
end
```

### Haskell

```haskell

```



# `LIII` URI Online Judge | 1079

## Médias Ponderadas

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 1 valor inteiro N, que representa o número de casos de teste que vem a seguir. Cada caso de teste consiste de 3 valores reais, cada um deles com uma casa decimal. Apresente a média ponderada para cada um destes conjuntos de 3 valores, sendo que o primeiro valor tem peso 2, o segundo valor tem peso 3 e o terceiro valor tem peso 5.

### Entrada

O arquivo de entrada contém um valor inteiro **N** na primeira linha. Cada **N** linha a seguir contém um caso de teste com três valores com uma casa decimal cada valor.

### Saída

Para cada caso de teste, imprima a média ponderada dos 3 valores, conforme exemplo abaixo.



| Exemplo de Entrada                                 | Exemplo de Saída    |
| -------------------------------------------------- | ------------------- |
| 3 <br>6.5 4.3 6.2 <br>5.1 4.2 8.1 <br>8.0 9.0 10.0 | 5.7 <br>6.3 <br>9.3 |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → Médias Ponderadas
N = int(input())
conta = 1
while conta <= N:
    X = input().split()
    a = float(X[0])
    b = float(X[1])
    c = float(X[2])
    conta += 1
    print('{:.1f}'.format(((a * 2) + (b * 3) + (c * 5)) / 10))

```

### C

```c
#include <stdio.h>
 // C - puro → Médias Ponderadas
int main() { 
     int N, conta = 1;
     double a, b, c;
     scanf("%d", &N);
     while (conta <= N){
        scanf("%lf %lf %lf", &a, &b, &c);
        conta++;
     printf("%.1f\n",(((a * 2) + (b * 3) + (c * 5)) / 10));
     } 
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → Médias Ponderadas
using namespace std; 
int main() { 
     int N, conta = 1;
     double a, b, c;
     cout << fixed;
     cin >> N;
     while (conta <= N){
        cin >> a >> b >> c;
        conta++;
     cout.precision(1);
     cout << (((a * 2) + (b * 3) + (c * 5)) / 10) << endl;
     }
    return 0;
}
```

### C#

```c#
using System;

namespace uri1079
{
    class Program
    {
        static void Main(string[] args)
        {
            int N, conta = 1;
            double a, b, c, Resultado;
            N = int.Parse(Console.ReadLine());
            while (conta <= N)
            {                
                string[] medias = Console.ReadLine().Split();
                a = Convert.ToDouble(medias[0]);
                b = Convert.ToDouble(medias[1]);
                c = Convert.ToDouble(medias[2]);
                Resultado = (((a * 2) + (b * 3) + (c * 5)) / 10);
                conta++;
                
                Console.WriteLine(string.Format("{0:0.0}", Resultado));
            }
            Console.ReadKey();
            }
        }
    }
```



### Ruby

```ruby
# Ruby → Médias Ponderadas
vezes = gets.to_i
(1..vezes).each do |i|
	n = gets.split
	a = n[0].to_f
	b = n[1].to_f
	c = n[2].to_f
puts "%.1f" % (((a * 2) + (b * 3) + (c * 5)) / 10)
end
```

### Pascal

```pascal
// Pascal → Médias Ponderadas
program uri_1079;
   var
     n, i:integer;
     a, b, c: real;
begin
  read(n);
  for i := 1 to n do
     begin
     readln(a, b, c);
       writeln((((a * 2) + (b * 3) + (c * 5)) / 10):0:1);
     end;
readln();
end.
```

### Javascript

```javascript

```

### Lua

```lua
-- Lua → Médias Ponderadas
local x = tonumber(io.read())
local conta = 1
while (conta <= x) do
    local n = {io.read('*number', '*number', '*number')}
    conta = conta + 1
    local a = n[1]
    local b = n[2]
    local c = n[3] 
    local resultado = (string.format("%.1f", (((a * 2) + (b * 3) + (c * 5)) / 10)))
    print(resultado)
end
```

### Haskell

```haskell

```



# URI Online Judge | 1080

## Maior e Posição

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Leia 100 valores inteiros. Apresente então o maior valor lido e a posição dentre os 100 valores lidos.

### Entrada

O arquivo de entrada contém 100 números inteiros, positivos e distintos.

### Saída

Apresente o maior valor lido e a posição de entrada, conforme exemplo abaixo.

| Exemplo de Entrada                             | Exemplo de Saída |
| ---------------------------------------------- | ---------------- |
| 2 <br>113 <br>45 <br>34565 <br>6 <br>... <br>8 | 34565 <br>4      |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1080 - Maior e Posição
conta = 1
maior = 0
menor = 0
conta2 = 0
while conta <= 100:
    a = int(input())
    if a > maior:
        menor = maior
        maior = a
        conta2 = conta
    conta += 1
print(maior)
print(conta2)

```

### C

```c
#include <stdio.h>
 // C - puro → uri_1080 - Maior e Posição
int main() { 
 int a, i, maior = -1, pos;
    for(i = 1; i <= 100; ++i){
        scanf("%d", &a);
        if (maior < a)
            maior = a, pos = i;
        }
    printf("%d\n", maior);
    printf("%d\n", pos);
    return 0;
}
```

### C++

```c++
#include <iostream>
 // C++ → uri_1080 - Maior e Posição
using namespace std;
int main() {
    int a, i, maior = -1, pos;
    for(i = 1; i <= 100; ++i){
        cin >> a;
        if (maior < a)
            maior = a, pos = i;
        }
    cout << maior << endl;
    cout << pos << endl;
    return 0;
}
```

### C#

```c#
using System;

namespace uri1080
{
    class Program
    {      

        static void Main(string[] args)
        {
            int a, i;
            int posicao = 1;
            int maior = -1;

            for (i = 1; i <= 100; ++i)
            {
                a = Convert.ToInt32(Console.ReadLine());
                if (maior < a)
                {
                    maior = a;
                    posicao = i;
                }
            }
            Console.WriteLine(maior);
            Console.WriteLine(posicao);
            
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby → uri_1080 - Maior e Posição
maior = -1
for i in 1..100
    b = gets.to_i
    if (maior < b)
        maior = b
        pos = i
   end
end
puts "%i\n" % maior
puts "%i" % pos
```

### Pascal

```pascal
// Pascal → uri_1080 - Maior e Posição
program uri_1080;
   var
     maior, b, pos, i:longint;
begin
maior := 1;
for i := 1 to 100 do
    begin
    readln(b);
    if (maior < b) then
        begin
        maior := b;
        pos := i;
   end;
end;
writeln(maior);
writeln(pos);
readln();
end.
```

### Javascript

```javascript

```

### Lua

```lua

```

### Haskell

```haskell

```



# `LIV` URI Online Judge | 1094

# Experiências

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Maria acabou de iniciar seu curso de graduação na faculdade de medicina e precisa de sua ajuda para organizar os experimentos de um laboratório o qual ela é responsável. Ela quer saber no final do ano, quantas cobaias foram utilizadas no laboratório e o percentual de cada tipo de cobaia utilizada.

Este laboratório em especial utiliza três tipos de cobaias: sapos, ratos e coelhos. Para obter estas informações, ela sabe exatamente o número de experimentos que foram realizados, o tipo de cobaia utilizada e a quantidade de cobaias utilizadas em cada experimento.

## Entrada

A primeira linha de entrada contém um valor inteiro **N** que indica os vários casos de teste que vem a seguir. Cada caso de teste contém um inteiro **Quantia** (1 ≤ **Quantia** ≤ 15) que representa a quantidade de cobaias utilizadas e um caractere **Tipo** ('C', 'R' ou 'S'), indicando o tipo de cobaia (*R*:Rato *S*:Sapo *C*:Coelho).

## Saída

Apresente o total de cobaias utilizadas, o total de cada tipo de cobaia utilizada e o percentual de cada uma em relação ao total de cobaias utilizadas, sendo que o percentual deve ser apresentado com dois dígitos após o ponto.

| Exemplo de Entrada                                           | Exemplo de Saída                                             |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 10 <br>10 C <br>6 R <br>15 S <br>5 C <br>14 R <br>9 C <br>6 R <br>8 S <br>5 C <br>14 R | Total: 92 cobaias <br>Total de coelhos: 29 <br>Total de ratos: 40 <br>Total de sapos: 23 <br>Percentual de coelhos: 31.52 % <br>Percentual de ratos: 43.48 % <br>Percentual de sapos: 25.00 % |

### <u>Python 3</u>

```python
# -*- coding: utf-8 -*-
# Python 3
N = int(input())
conta = 0
contac = 0
contas = 0
contar = 0
total = 0
while conta < N:
    X = input().split()
    cont = int(X[0])
    tipo = X[1]
    if tipo == 'C':
        contac = cont + contac
    if tipo == 'R':
        contar = cont + contar
    if tipo == 'S':
        contas = cont + contas
    conta += 1
total = (contac + contas + contar)
print('Total: {} cobaias'.format(total))
print('Total de coelhos: {}'.format(contac))
print('Total de ratos: {}'.format(contar))
print('Total de sapos: {}'.format(contas))
print('Percentual de coelhos: {:.2f} %'.format((contac / total) * 100))
print('Percentual de ratos: {:.2f} %'.format((contar / total) * 100))
print('Percentual de sapos: {:.2f} %'.format((contas / total) * 100))

```

### <u>C</u>

```c
#include <stdio.h>
#include <stdlib.h>
// C - puro - dev++
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char *argv[]) {

    int conta = 0, i, n, coelhos = 0, sapos = 0, ratos = 0, total = 0;
    float pcoelhos, psapos, pratos;
	char tipo;

    scanf("%d", &n);

    for (i = 1; i <= n; i++){
        scanf("%d %c", &conta, &tipo);

        if (tipo == 'C')
            (coelhos += conta);
        else if (tipo == 'R')
		    (ratos += conta);
        else if (tipo == 'S')
		    (sapos += conta);
}
    total = (coelhos + sapos + ratos);
    pcoelhos = ((coelhos*100.0)/total);
    pratos = ((ratos*100.0)/total); 
    psapos = ((sapos*100.0)/total);
    
printf("Total: %d cobaias\n", total);
printf("Total de coelhos: %d\n", coelhos);
printf("Total de ratos: %d\n", ratos);
printf("Total de sapos: %d\n", sapos);
printf("Percentual de coelhos: %.2lf %%\n", pcoelhos);
printf("Percentual de ratos: %.2lf %%\n", pratos);
printf("Percentual de sapos: %.2lf %%\n", psapos);

system("pause");
    return 0;
}
```

### C++

```c++
#include <iostream>
// C++
using namespace std;

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	
    int conta = 0, i, n, coelhos = 0, sapos = 0, ratos = 0, total = 0;
    float pcoelhos, psapos, pratos;
	char tipo;

    cin >> n;
    cout << fixed;
    
    for (i = 1; i <= n; i++){
        cin >> conta >> tipo;

        if (tipo == 'C')
            (coelhos += conta);
        else if (tipo == 'R')
		    (ratos += conta);
        else if (tipo == 'S')
		    (sapos += conta);
}
    total = (coelhos + sapos + ratos);
    pcoelhos = ((coelhos*100.0)/total);
    pratos = ((ratos*100.0)/total); 
    psapos = ((sapos*100.0)/total);
    
cout << "Total: " << total << " cobaias" << endl;
cout << "Total de coelhos: " <<  coelhos << endl;
cout << "Total de ratos: " << ratos << endl;
cout << "Total de sapos: " << sapos << endl;
cout.precision(2);
cout << "Percentual de coelhos: " << pcoelhos << " %" << endl;
cout << "Percentual de ratos: " << pratos << " %" << endl;
cout <<"Percentual de sapos: " << psapos << " %" << endl;

system("pause");
	
	return 0;
}
```

### C#

```c#
using System;

namespace uri1094
{
    class Program
    {
        static void Main(string[] args)
        {
            int conta = 0, i, n, coelhos = 0, sapos = 0, ratos = 0, total = 0;
            //float pcoelhos, psapos, pratos;
            string tipo;

                n = int.Parse(Console.ReadLine());

                for (i = 1; i <= n; i++)
                {
                String[] dados = Console.ReadLine().Split();
                conta = Convert.ToInt32(dados[0]);
                tipo = dados[1];

                    if (tipo == "C")
                {
                    coelhos += conta;
                }
                else if (tipo == "R")
                {
                    ratos += conta;
                }
                else if (tipo == "S")
                {
                    sapos += conta;
                }
            }
                total = (coelhos + sapos + ratos);
                double pcoelhos = (coelhos * 100.0) / total;
                double pratos = (ratos * 100.0) / total;
                double psapos = (sapos * 100.0) / total;

                Console.WriteLine("Total: {0} cobaias", total);
                Console.WriteLine("Total de coelhos: {0}", coelhos);
                Console.WriteLine("Total de ratos: {0}", ratos);
                Console.WriteLine("Total de sapos: {0}", sapos);
                Console.WriteLine("Percentual de coelhos: " + String.Format("{0:0.00}", pcoelhos) + " %");
                Console.WriteLine("Percentual de ratos: " + String.Format("{0:0.00}", pratos) + " %");
                Console.WriteLine("Percentual de sapos: " + String.Format("{0:0.00}", psapos) + " %");
            Console.ReadKey();
            }
        }
    }
```

### Ruby

```ruby
# Ruby

n = gets.to_i
conta = 0
contac = 0
contas = 0
contar = 0
total = 0
for i in 1..n
    x = gets.split
    cont = x[0].to_f
    tipo = x[1].to_s
    if tipo == 'C'
        contac = cont + contac
    elsif tipo == 'R'
        contar = cont + contar
    elsif tipo == 'S'
        contas = cont + contas
    conta += 1
    end
end
total = (contac + contas + contar)
puts "Total: %.0f cobaias" % total
puts "Total de coelhos: %.0f" % contac
puts "Total de ratos: %.0f" % contar
puts "Total de sapos: %.0f" % contas
puts "Percentual de coelhos: %.2f %%" % (contac/total*100.0)
puts "Percentual de ratos: %.2f %%" % (contar/total*100.0)
puts "Percentual de sapos: %.2f %%" % (contas/total*100.0)

```

### Pascal

```pascal
program uri_1094;
// Pascal
   uses Crt, sysutils;
   var
     i, n, quantidade, coelhos, sapos, ratos, total, quant:longint;
     tipo, t1: string;
begin
    clrscr;

     coelhos := 0;
     sapos := 0;
     ratos := 0;
     total := 0;
     read(n);   // quantos testes desejas fazer

     for i := 1 to n do   // testes e comparações
       begin
         read(quantidade);
         quant := quantidade;
         readln(t1);
         tipo := trim(t1);

         //writeln(trim(tipo), quant);

         if (tipo = 'C') then begin
           coelhos += quant;
         end
         else if (tipo = 'R') then begin
           ratos += quant;
         end
         else if(tipo = 'S') then begin
           sapos += quant;
         end;
         total := coelhos + sapos + ratos;
       end;

writeln('Total: ', total, ' cobaias');
writeln('Total de coelhos: ', coelhos);
writeln('Total de ratos: ', ratos);
writeln('Total de sapos: ', sapos);
writeln('Percentual de coelhos: ', (((coelhos / total) * 100)):0:2, ' %');
writeln('Percentual de ratos: ', (((ratos / total) * 100)):0:2, ' %');
writeln('Percentual de sapos: ', (((sapos / total) * 100)):0:2, ' %');

readln;
end.
```

# URI Online Judge | 1095

# Sequencia IJ 1

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Você deve fazer um programa que apresente a sequencia conforme o exemplo abaixo.

## Entrada

Não há nenhuma entrada neste problema.

## Saída

Imprima a sequencia conforme exemplo abaixo:

| Exemplo de Entrada | Exemplo de Saída                                       |
| ------------------ | ------------------------------------------------------ |
|                    | I=1 J=60 <br>I=4 J=55 <br>I=7 J=50 <br>... <br>I=? J=0 |

```python
# -*- coding: utf-8 -*-
# Python 3
I = -2
J = 65
conta = 1
while J != 0:
    print('I={} J={}'.format(I + 3, J - 5))
    I += 3
    J -= 5
    conta += 1

```

```c
#include <stdio.h>
#include <stdlib.h>
// C - puro
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char *argv[]) {
	
	int I, J, conta;
	
	I = -2;
	J = 65;
	conta = 1;
	while (J != 0){
	   printf("I=%i J=%i\n", I + 3, J - 5);
	   I = I + 3;
	   J = J - 5;
	   conta += 1;
}
	return 0;
}
```

```c++
#include <iostream>
// C++
using namespace std;

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	
	int I, J, conta;
	
	I = -2;
	J = 65;
	conta = 1;
	
	while (J != 0){
		cout << "I=" << I + 3 << " J=" << J - 5 << endl;
		I = I + 3;
		J = J - 5;
		conta += 1;
	}
	
	return 0;
}
```

```ruby
# Ruby
i = -2
j = 65
conta = 1
while j != 0
    puts "I=#{i + 3} J=#{j - 5}"
    i += 3
    j -= 5
    conta += 1
end
```

```pascal
// Pascal

program uri_1095;

   var
     I, J, conta:integer;

begin
  I := -2;
  J := 65;
  conta := 1;
  while (J <> 0) do
      begin
      writeln('I=', I + 3, ' J=', J - 5);
      I := I + 3;
      J := J - 5;
      conta := conta + 1;
      end;
readln();
end.
```

# URI Online Judge | 1096

# Sequencia IJ 2

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Você deve fazer um programa que apresente a sequencia conforme o exemplo abaixo.

## Entrada

Não há nenhuma entrada neste problema.

## Saída

Imprima a sequencia conforme exemplo abaixo



| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
|                    | I=1 J=7 <br>I=1 J=6 <br>I=1 J=5 <br>I=3 J=7 <br>I=3 J=6 <br>I=3 J=5 <br>... <br>I=9 J=7 <br>I=9 J=6 <br>I=9 J=5 |

```python
# -*- coding: utf-8 -*-
# Python 3
I = 1
J = 7
while I <= 9:
    print('I={} J={}'.format(I, J))
    if J == 5:
        I += 2
        J += 2
    else:
        J -= 1

```

```c
#include <stdio.h>
#include <stdlib.h>
// C - puro
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char *argv[]) {
	
	int I, J;
	
	I = 1;
	J = 7;
	
	while (I <= 9){
		printf("I=%d J=%d\n", I, J);
		if (J == 5){
		
			I += 2;
			J += 2;
		}else{		
		    J -= 1;
	}
		}
	
	return 0;
}
```

```c++
#include <iostream>
using namespace std;
// C++ → uri_1096
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	
	int I, J;
	
	I = 1;
	J = 7;
	
	while (I <= 9){
		cout << "I=" << I << " J=" << J << endl;
		if (J == 5){
		
			I += 2;
			J += 2;
		}else{		
		    J -= 1;
	}
		}
	
	return 0;
}
```

```ruby
# Ruby
i = 1
j = 7
while i <= 9
    puts "I=#{i} J=#{j}"
    if j == 5
        i += 2
        j += 2
    else
        j -= 1
	end
end
```

```pascal
// Pascal
program uri_1096;

   var
     I, J:integer;

begin
  I := 1;
  J := 7;
while (I <= 9) do
    begin
    writeln('I=', I, ' J=', J);
    if (J = 5) then
         begin
         I += 2;
        J += 2;
        end
    else
        J -= 1;
    end;
readln;
end.
```

# URI Online Judge | 1097

# Sequencia IJ 3

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Você deve fazer um programa que apresente a sequencia conforme o exemplo abaixo.

## Entrada

Não há nenhuma entrada neste problema.

## Saída

Imprima a sequencia conforme exemplo abaixo.

| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
|                    | I=1 J=7 <br>I=1 J=6 <br>I=1 J=5 <br>I=3 J=9 <br>I=3 J=8 <br>I=3 J=7 <br>... <br>I=9 J=15 <br>I=9 J=14 <br>I=9 J=13 |

```python
# -*- coding: utf-8 -*-
# Python → uri_1097
I = 1
J = 7
while I <= 9:
    print('I={} J={}'.format(I, J))
    if (I + 4) == J:
        I += 2
        J += 4
    else:
        J -= 1

```

```c
#include <stdio.h>
#include <stdlib.h>
// C - puro → uri_1097
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char *argv[]) {
	
	int i, j;
	
	i = 1;
    j = 7;
    while (i <= 9){
        printf("I=%d J=%d\n", i, j);
        if ((i + 4) == j){
            i += 2;
            j += 4;
        }else{
            j -= 1;
        }
}
	
	return 0;
}
```

```c++
#include <iostream>
// C++ → uri_1097
using namespace std;

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	
	int i, j;
	
	i = 1;
    j = 7;
    while (i <= 9){
        cout << "I=" << i << " J=" << j << endl;
        if ((i + 4) == j){
            i += 2;
            j += 4;
        }else{
            j -= 1;
        }
}
	
	return 0;
}
```

```ruby
# Ruby → uri_1097
i = 1
j = 7
while i <= 9
    puts "I=#{i} J=#{j}"
    if (i + 4) == j
        i += 2
        j += 4
    else
        j -= 1
    end
end
```

```pascal
// Pascal → uri_1097
program uri_1097;

   var
     I, J:integer;

begin
  I := 1;
  J := 7;
while (I <= 9) do
    begin
    writeln('I=', I, ' J=',J);
    if ((I + 4) = J) then begin
        I += 2;
        J += 4;
    end
    else
        J -= 1;
    end;
readln;
end.
```

# URI Online Judge | 1098

# Sequencia IJ 4

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

Timelimit: 1

Você deve fazer um programa que apresente a sequencia conforme o exemplo abaixo.

## Entrada

Não há nenhuma entrada neste problema.

## Saída

Imprima a sequencia conforme exemplo abaixo.

| Exemplo de Entrada | Exemplo de Saída                                             |
| ------------------ | ------------------------------------------------------------ |
|                    | I=0 J=1 <br>I=0 J=2 <br>I=0 J=3 <br>I=0.2 J=1.2 <br>I=0.2 J=2.2 <br>I=0.2 J=3.2 <br>..... <br>I=2 J=? <br>I=2 J=? <br>I=2 J=? |

### Python 3

```python
# -*- coding: utf-8 -*-
# Python 3 → uri_1098 - Sequência IJ 4

I = 0
J = 1
intera = 0.2
for i in range(11):
    for k in range(3):
        if I == 0:
            print('I={} J={}'.format(I, J))
        elif I == 1:
            print('I={:.0f} J={:.0f}'.format(I, J))
        elif I > 1.9:
            print('I={:.0f} J={:.0f}'.format(2, J))
        else:
            print('I={:.1f} J={:.1f}'.format(I, J))
        J += 1
    J = 1 + intera
    I += 0.2
    intera += 0.2

```

### C

```c
#include <stdio.h>
// C - puro  
int main()  
{  
    double I, a, J;  
    int intera;  
    for(I = 0; I <= 1.9; I = I + .2)  
    {  
        for(a = 1.0; a <= 3.0; a++)  
        {  
            J = a + I;  
            if(I == 0.0 || I == 1.0) 
			    printf("I=%.0lf J=%.0lf", I, J);  
            else if(J == 3.0 || J == 4.0 || J == 5.0) 
			    printf("I=%.0lf J=%.0lf", I, J);  
            else 
			    printf("I=%.1lf J=%.1lf", I, J);  
                printf("\n");  
        }  
    }  
    for(intera = 3; intera <= 5; intera++) 
	    printf("I=2 J=%d\n", intera);  
    return 0;  
}  
```

### C++

```c++
#include <iostream>
// C++
using namespace std;

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	
	double I, a, J;  
    int intera; 
	 
    for(I = 0; I <= 1.9; I = I + .2)  
    {  
        for(a = 1.0; a <= 3.0; a++)  
        {  
            J = a + I;  
            if(I == 0.0 || I == 1.0) 
			    cout << "I=" << I << " J=" << J << endl;  
            else if(J == 3.0 || J == 4.0 || J == 5.0) 
			    cout << "I=" << I << " J=" << J << endl;  
            else 
			    cout << "I=" << I << " J=" << J << endl;                
        }  
    }  
    for(intera = 3; intera <= 5; intera++) 
	    cout << "I=2 J=" << intera << endl;
	
	return 0;
}
```

```ruby

```

```pascal

```

# URI Online Judge | 1099

## Soma de Ímpares Consecutivos II

Adaptado por Neilor Tonin, URI ![img](https://resources.urionlinejudge.com.br/gallery/images/flags/br.gif) Brasil

**Timelimit: 1**

Leia um valor inteiro **N** que é a quantidade de casos de teste que vem a seguir. Cada caso de teste consiste de dois inteiros **X** e **Y**. Você deve apresentar a soma de todos os ímpares existentes ***entre*** **X** e **Y**.

## Entrada

A primeira linha de entrada é um inteiro **N** que é a quantidade de casos de teste que vem a seguir. Cada caso de teste consiste em uma linha contendo dois inteiros **X** e **Y**.

## Saída

Imprima a soma de todos valores ímpares ***entre\* X** e **Y**.

| Exemplo de Entrada                                   | Exemplo de Saída                      |
| ---------------------------------------------------- | ------------------------------------- |
| 7<br>4 5<br>13 10<br>6 4<br>3 3<br>3 5<br>3 4<br>3 8 | 0<br>11<br>5<br>0<br>0<br>0<br>1<br>2 |

### Python 3

```python
# -*- coding: utf-8 -*-

N = int(input())
cont = 0
result = 0
while cont < N:
    x = input().split()
    X = int(x[0])
    Y = int(x[1])
    if X > Y:
        while Y < X:
            Y += 1
            if (Y % 2) == 1 and Y != X:
                result += Y
    if Y > X:
        while X < Y:
            X += 1
            if (X % 2) == 1 and X != Y:
                result += X
    print(result)
    cont += 1
    result -= result

```

### C

```c

```

### C++

```c++

```

### C#

```c#

```

### Ruby

```ruby

```

### Pascal

```pascal

```

### Javascript

```javascript

```

### Lua

```lua

```

### Haskell

```haskell

```

