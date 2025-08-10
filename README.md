# Guia Rápido: Usando Git e Executando o Projeto da Aula 01
Olá, turma! Este guia foi criado para ajudar vocês a baixar, compilar e executar os exemplos de código da nossa disciplina de Linguagem de Programação. Vamos usar o Git, uma ferramenta essencial para qualquer desenvolvedor.

## O que é Git e por que usá-lo?
* Git é um sistema de controle de versão. Pense nele como um "histórico superpoderoso" para seus projetos de código. Ele permite que você:
* Salve "fotos" (chamadas commits) do seu projeto ao longo do tempo.
* Volte para versões antigas se algo der errado.
* Trabalhe em equipe de forma organizada.
* Baixe e atualize facilmente projetos que estão na internet (como no GitHub, GitLab, etc.).

Nesta disciplina, usaremos o Git para que vocês possam baixar os códigos das aulas e receber atualizações de forma simples.

## Parte 1: Configuração Inicial do Git (Apenas uma vez!)
Antes de tudo, você precisa ter o Git instalado no seu computador. Se ainda não tiver, baixe em git-scm.com.
Depois de instalar, abra o terminal (ou Git Bash no Windows) e configure seu nome e e-mail. Isso é importante para identificar quem está fazendo as alterações nos projetos.

### Configure seu nome de usuário (use seu nome real)
```bash
git config --global user.name "Seu Nome Completo"
```
### Configure seu e-mail (use o mesmo e-mail do seu GitHub, se tiver)
```bash
git config --global user.email "seu.email@exemplo.com"
```
Você só precisa fazer isso uma vez na vida em cada computador que usar.

## Parte 2: Baixando (Clonando) o Projeto do Repositório
* "Clonar" é o termo que o Git usa para "baixar uma cópia completa de um projeto". Você fará isso para obter os arquivos da nossa aula.
* Abra o terminal.
* Navegue até a pasta onde você quer salvar os projetos da disciplina. Use o comando cd (change directory).

### Exemplo: para ir para a pasta "Documentos"
```bash
cd Documentos
```
Clone o repositório usando o link fornecido pelo professor.

### Substitua a URL abaixo pela URL do repositório da disciplina
```bash
git clone https://github.com/frfreire/linguagem-programacao-flex.git
```
Pronto! O Git vai baixar uma nova pasta chamada linguagem-programacao-flex com todos os arquivos do projeto dentro dela.

## Parte 3: Compilando e Executando o Projeto Java
Agora que você tem os arquivos, vamos compilar e executar nossa calculadora de exemplo.

Acesse a pasta do projeto que você acabou de clonar.
```bash
cd linguagem-programacao-flex
```
Liste os arquivos para ter certeza de que o Exemplo01.java está lá.

No Windows: 
```bash
dir
```
No macOS/Linux: 
```bash
ls
```
Compile o arquivo .java. O compilador do Java (javac) vai ler seu código-fonte e transformá-lo em bytecode (um arquivo .class), que a Máquina Virtual Java (JVM) consegue entender.
```java
javac Exemplo01.java
```
Se tudo der certo, nenhum erro aparecerá, e um novo arquivo chamado Exemplo01.class será criado na pasta.
Execute o programa! Agora, use o comando java para que a JVM execute o bytecode.

### Note que não usamos a extensão .class aqui
```java
java Exemplo01
```
O programa da calculadora iniciará no seu terminal, e você poderá interagir com ele.

**Dica Extra:** Mantendo seu Projeto Atualizado
Se o professor adicionar novos exemplos ou corrigir algum código, você não precisa baixar tudo de novo. Basta "puxar" (pull) as atualizações.
Abra o terminal e navegue até a pasta do projeto (linguagem-programacao-flex).
Execute o comando:
```bash
git pull
```
O Git buscará automaticamente as novidades e as adicionará à sua pasta local. Simples assim!

Se tiverem qualquer dúvida, não hesitem em perguntar!
