# Atividade2Parte1

## 1. O que é JSON e por que ele se tornou tão popular

**JSON é um formato mais leve para troca de dados entre aplicativos.**
Ele é formado por textos e utiliza uma estrutura de chave e valor, parecidos com os objetos do JS.

Exemplo de JSON:
```json
{
  "nome": "Julia",
  "idade": 25,
  "Curso": "TSI"
}
```

### Por que é tão popular?
**A simplicidade:** fácil de ler e entender tanto por pessoas e maquinas.
**Compatibilidade:** pode ser usado em muitas linguagens de programação.
**É padrão na web:** quando um site se comunica com um servidor, geralmente usa JSON.
**É versátil:** pode ser pela internet, salvo em arquivos ou armazenados em bancos de dados.


## 2. Diferença entre JSON.stringify() e JSON.parse()

**JSON.stringify(): converte um objeto JS em uma string JSON.**
**JSON.parse(): faz o oposto, converte uma string JSON em um objeto JS.**

**Exemplo:**
```js
const pessoa = {nome: "Ana", idade: 23};

const jsonString = JSON.stringify(pessoa);

const objeto = JSON.parse(jsonString);
```
### Quando usar cada uma:
Use Use JSON.stringify(): quando for enviar dados ou salvar em algum lugar.
Use JSON.parse(): ao receber dados JSON e precisar trabalhar com eles no seu código.


## 3. Manipulação de strings em JavaScript

Frase de exemplo:
```js
const frase = "JavaScript é baseado em ECMA Script";
```

**a) Verificar se contém a palavra "Script"**
```js
console.log(frase.includes("Script"));
```

**b) Remover a palavra "JavaScript" e gerar uma nova string**
```js
const novaFrase = frase.replace("JavaScript ", "");
```

**c) Substituir "baseada" por "tem origem"**
```js
const fraseModificada = frase.replace("baseada", "tem origem");
```

## 4. Vantagem de usar Template Strings

As templates strings (usando crases `) facilitam criação de strings mais complexas assim dizendo:
**permitem inserir variáveis diretamente no texto.**
**aceitam quebras de linhas naturalmente.**

### Como era antes:
```js
const nome = "João";
const idade = 20;
const frase = "Meu nome é " + nome + " e tenho " + idade + " anos.";
```

### Como é agora:
```js
const nome = "João";
const idade = 20;
const frase = `Meu nome é ${nome} e tenho ${idade} anos.`;
```

### As vantagens é:
O código vai ficar mais limpo e fácil de entender.
Não precisa ficar fechando e abrindo aspas o tempo todo.
