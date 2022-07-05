# DOCKER - Full Cycle

## Container
> Um processo com subprocessos que são isolados emulando um sistema operacional.

- Namespace: isolamento de processos.
- CGroups: isolamento e controle de recusos computacionais dos processos.
- Overlay File System(OFS): Sistema de arquivos em camadas que usa um arquivo base que só pode ser lido e toda mudança ou adição de arquivos é adicionado em um outro diretóio e então as mundanças são mergeadas e utilizadas. 
  - utiliza a bibliotecas e arquivos do sistema operacionail e só agrega os arquivos necessários.

# Images
> Duas formas de gerar uma imagem, através do build de um Dockerfile ou por um commit em um container já existente rodando, que por sua vez, cria uma nova versão com as alterações do container anterior.

### Dockerfile
> Arquivo declarativo para construir imagens    

    FROM: imageName
    RUN: <comandos> apt-get install
    EXPOSE: 8080 (expor portas para acesso)
- imagens imutáveis com uma camada de leitura e escrita.
- todo build de um Dockerfile gera uma nova imagem.

  