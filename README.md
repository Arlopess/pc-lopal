# pc-lopal
Repositório para armazenar códigos da aula.


# Desafio 1

## `1.0.0.`

## O que significa cada número dessa versão?

**R**= O primeiro número indica mudanças grandes que quebram a compatibilidade, o segundo traz novas funções compatíveis, e o terceiro corrige erros pequenos. Cada um tem um nome específico 1.(Maior / Major), 0.(Menor / Minor) e 0.(Correção / Patch)

## Quem decide como esse número muda e com base em quê?

**R**= 1.- Muda quando uma versão muda por completo.

  

**R**= 0.- Muda quando novas funções entram no programa.

  

**R**= 0.- Muda apenas para consertar erros, falhas ou bugs.


# Desafio 2

## `dependencies` e `devDependencies`

## Qual a diferença entre os dois grupos?

**dependencies**

* São os pacotes vitais para o projeto rodar.

* O sistema instala esses arquivos no servidor de produção.

* Exemplos comuns: frameworks como Express ou bibliotecas de interface como React.

  

**devDependencies**

* São ferramentas de apoio para programar.

* O sistema ignora estes pacotes ao colocar o site no ar.

* Exemplos comuns: ferramentas de teste como Jest ou formatadores de código como ESLint.

## Como você decide em qual grupo colocar uma biblioteca?

**R**= Se você quer decidir entre qual dos dois usar. Faça-se uma pergunta "Se eu remover essa biblioteca, o meu usuário final ainda consegue usar o aplicativo no servidor?"

  

Se a resposta for **SIM**, ele é de desenvolvimento **`devDependencies`**

  

Agora se a resposta for **NÃo**, ele é de prodção **`dependencies`**

# Desafio 3

## `^1.0.0`; `~1.0.0`

## O que cada símbolo permite atualizar?

**R**=

* ^- Permite atualizar apenas versões `minor` e `patch`

* ~- Permite atualizar apenas versões `patch`

## O que acontece quando não existe nenhum símbolo?

**R**= : Fixa a versão exata, permitindo apenas a instalação daquela específica.


# Desafio 4


## `CommonJS` e `ES Modules`

## Qual a diferença entre os dois?

**R**= CommonJS (CJS) usa `require()` e `module.exports` de forma síncrona e dinâmica no Node.js. ES Modules (ESM) usa `import` e `export` de forma estônica, assíncrona e é o padrão oficial do ecossistema JavaScript moderno para navegadores e servidores.

## Como cada um surgiu?

**R**=

* O Surgimento do CommonJS (2009)O problema inicial: No começo, o JavaScript não tinha nativamente uma forma de dividir o código em arquivos separados. Tudo ficava no escopo global.

* A solução: O projeto foi idealizado inicialmente sob o nome ServerJS por desenvolvedores focados em criar aplicações fora do navegador.

* Adoção pelo Node.js: Em 2009, o Node.js adotou essa especificação como padrão nativo, popularizando as funções require() e module.exports.

* Característica principal: É síncrono e ideal para o disco rígido do servidor, onde ler um arquivo de forma imediata não causa travamentos visuais.]

## Como é a sintaxe de importação e exportação em cada um?

**R**= O CommonJS usa a função `require()` para importar e o objeto `module.exports` para exportar. Já o ES Modules (ESM) utiliza as palavras-chave `import` e `export`. O CommonJS é o padrão histórico do Node.js, enquanto o ES Modules é o padrão oficial do JavaScript moderno para navegadores e servidores.