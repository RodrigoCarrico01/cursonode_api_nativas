# PORTUGUÊS

## Curso NodeJS - APIs Nativas 

*Este repositório contém códigos práticos utilizados no quarto módulo do curso de Node.js, focado em demonstrar o uso de módulos nativos da plataforma. Cada secção cobre funcionalidades essenciais como **manipulação de buffers**, **processamento paralelo**, **eventos**, **erros**, **sistema de ficheiros** e muito mais.*

## Conteúdo
> Buffer
> Child Process
> Console
> Gestão de Erros
> Eventos
> HTTP Server
> Path
> Sistema de Ficheiros (FS)

### 1. Buffer
**Localização**: `buffer/buffer.js`
*O módulo **Buffer** é utilizado para trabalhar com fluxos de dados binários. No exemplo fornecido, temos:*
- Criação de buffers a partir de strings.
- Conversão de buffers para diferentes formatos de texto.
- Validação se um objeto é um buffer.

#### Como usar:
``` node buffer/buffer.js ```
*Deverá mostrar o conteúdo do buffer em diferentes formatos de codificação.*

### 2. Child Process
**Localização**: `childProcess/childProcess.js`
*Este código demonstra como executar processos em segundo plano (child processes) usando o módulo **child_process**:*
- O exemplo executa o comando `ls` no ambiente UNIX.
- Captura a saída (stdout) e os erros (stderr) do processo.

#### Como usar:
```node childProcess/childProcess.js```
*Deverá listar o conteúdo de vários diretórios conforme especificado no comando.*

### 3. Console
**Localização**: `console/console.js`
*Demonstra o uso de diferentes métodos do objeto global **console**:*
- `console.log` e `console.error` para mensagens gerais e erros.
- `console.table` para visualizar arrays e objetos de forma tabular.
- `console.count` e `console.countReset` para contar chamadas de funções.
- `console.time` e `console.timeEnd` para medir o tempo de execução.

#### Como usar:
```node console/console.js```
*Isto irá exibir tabelas, contagens e tempos de execução no terminal.*

### 4.1 Gestão de Error 
**Localização**: `error/error.js`
*Este exemplo mostra como capturar e tratar erros em funções aninhadas usando `try...catch.`*

#### Como usar:
```node error/error.js```
*Isto irá gerar uma mensagem de erro personalizada e permitir que o programa continue após o erro.*

### 4.2 Gestão de Erros | Event
**Localização**: `error/errorEvent.js`
*Demonstra o uso de eventos para detetar e tratar erros personalizados usando o módulo **events**.*

#### Como usar:
```node error/errorEvent.js```
*Quando um tipo de dado inválido é passado, o programa irá disparar um evento de erro e exibir uma mensagem correspondente.*

### 5. Eventos
**Localização**: `events/events.js`
*Demonstra a criação de eventos personalizados com o módulo **events**:*
- Criação de assinantes (subscribers) que respondem a eventos específicos.
- Emissão de eventos (publishers) para acionar os assinantes.

#### Como usar:
```node events/events.js```
*Deverá exibir mensagens conforme os eventos seguranca e encerrar são emitidos.*

### 6. HTTP Server
**Localização**: `http/index.js`
*Cria um servidor HTTP simples utilizando o módulo **http**:*
- Retorna uma página HTML ao cliente.
- Abre automaticamente o navegador apontando para o servidor.

#### Como usar:
```node http/index.js```
*O servidor será iniciado em http://127.0.0.1:3000/ e abrirá automaticamente o navegador.*

### 7. Path
**Localização**: `path/path.js`
*Demonstra o uso do módulo **path** para manipulação de caminhos de ficheiros:*
- `basename`: obtém o nome do ficheiro.
- `normalize`: normaliza o caminho, removendo redundâncias.
- `join e resolve`: constrói caminhos absolutos e relativos.
- `extname`: obtém a extensão do ficheiro.

#### Como usar:
```node path/path.js```
*Deverá mostrar no terminal diferentes manipulações de caminhos de ficheiros.*

### 8.1 Sistema de Ficheiros(FS) |  Async Read
**Localização**: `fs/asyncRead.js`
*Esta secção contém vários exemplos de manipulação de ficheiros utilizando o módulo **fs**.*
- Lê um ficheiro de forma assíncrona utilizando **async/await.**

#### Como usar:
```node fs/asyncRead.js```
*Deverá exibir o conteúdo de fs/texto.txt no terminal.*

### 8.2 Sistema de Ficheiros(FS) | Html
**Localização**: `fs/html.js`
- Lê um ficheiro HTML e retorna-o via servidor `HTTP`.

#### Como usar:
```node fs/html.js```
*Aceda ao servidor em http://127.0.0.1:3000/ para visualizar o conteúdo HTML.*

### 8.3 Sistema de Ficheiros(FS) | create dir structure
**Localização**: `fs/mkdir.js`
- Cria uma estrutura de diretórios recursiva automaticamente.

#### Como usar:
```node fs/mkdir.js```
*Deverá criar os diretórios especificados dentro de fs/projeto/assets/.*

### 8.4 Sistema de Ficheiros(FS) | write file (promise)
**Localização**: `fs/promiseWriteFile.js`
- Demonstra a criação de ficheiros usando Promises.

#### Como usar:
```node fs/promiseWriteFile.js```
*Deverá criar um ficheiro chamado `fs/promiseArquivo.txt`*

### 8.5 Sistema de Ficheiros(FS) | read dir
**Localização**: `fs/readDir.js`
- Lista todos os ficheiros no diretório atual utilizando uma função de callback.

#### Como usar:
```node fs/readDir.js```
*Deverá exibir os ficheiros do diretório onde o script foi executado.*

### 8.6 Sistema de Ficheiros(FS) | read file :)
**Localização**: `fs/readFile.js`
- Demonstra a leitura de ficheiros usando métodos de bloqueio (sync) e não bloqueio (async).

#### Como usar:
```node fs/readFile.js```
*Deverá exibir o conteúdo de `fs/texto.txt` no terminal.*

### 8.7 Sistema de Ficheiros(FS) | Write file (util)
**Localização**: `fs/utilWriteFile.js`
- Cria ficheiros utilizando o módulo util para promisificar funções.

#### Como usar:
```node fs/utilWriteFile.js```
*Deverá criar o ficheiro `fs/utilArquivo.txt`.*

### 8.8 Sistema de Ficheiros(FS) | write file
**Localização**: `fs/writeFile.js`
- Cria ficheiros de forma simples utilizando writeFile do módulo fs.

#### Como usar: 
```node fs/writeFile.js```
*Deverá criar o ficheiro `fs/arquivo.txt`.*

