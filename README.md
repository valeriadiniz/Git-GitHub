
# Introdução ao Git e ao GitHub

- 1-controle de versão 
- 2-armazenamento em nuvem
- 3-trabalho em equipe
- 4-melhoria de código e reconhecimento

### windows/                   unix
#### -cd /                      -cd
#### -dir /                     -ls
#### -mkdir /                   -mkdir
#### -del/rmdir /               -rm -rf
#### -cls                      -clear (or ctrl l)
#### (archive/repositories)    
#### -tab for autocomplete       
#### -echo hello > hello.txt   (create archive)

### SHA - Secure Hash Algorithm(algoritmo de hash seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA). É uma forma curta de representar um arquivo

#### exemplo: openssl sha1 texto.txt

### BLOBS -> bolha contém: tipo, tamanho, \0 e contúdo

#### "echo 'conteudo' | git hash-object --stdin" e "echo -e 'blob *\0conteudo' | openssl sha1 retornam a mesma chave" aha1 do arquivo

### TREES -> árvores

#### armazena e aponta para blobs diferentes e outras árvores dferentes, e também guarda o nome do arquivo. Tem sha1 conectados com as árvores, mudando um arquivo altera toda a estrutura

### COMMITS ->  objeto que aponta para árvore, parente(último commit), autor, mensagem(exemplo "first commit") e timestamp(data e hora que foi criado) também possui seu sha1 

### Traked - git tem ciência deles (reconhecimento) sendo eles: unmodified, modiefied e staged(arquivos que estão se preparando p/fazer parte de outro tipo de agrupamento)

### Untracked - git tem ciência deles (reconhecimento)

### Ambiente de desenvolvimento
- Working Directory
- Staging Area
- Local Repository 

### Servidor (Neste caso github)
- Remote Repository

