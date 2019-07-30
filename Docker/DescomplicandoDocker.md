# [Descomplicando Docker](https://www.linuxtips.io/descomplicando-docker)

<br> [x] Day 1
<br> [ ] Day 2
<br> [ ] Day 3
<br> [ ] Day 4
<br> [ ] Final
<br> [ ] Aula ao vivo

##

# Day one 

<br>Container = isolamento (que pode ser lógico - processos, usuários, rede etc ou  Físico - CPU, memória etc dedicados por exemplo)
<br>Na parte lógica temos namespaces e na física temos os Cgroups.
<br>Então containers são uma forma de fazer isolamentos.
<br>Antes do Docker já existiam formas de executar containers.
<br>Quando se tem uma imagem de container existem várias camadas (dessa mesma imagem), porém SOMENTE na última camada se pode escrever(read n' write).
<br>Não se faz a alteração no original, neste mesmo momento em que precisa alterar algo, se criar uma cópia da origial (última camada) onde são feitas as alterações. Isso garante que os containers estejam rodando a mesma imagem onde apenas a última camada (onde foi feita a alteração) execute as alterações.
<br>As camadas abaixo são chamadas de Read only.  
<br>Quando se mexe com VM cada uma já tem seu Kernell, sistema operacional etc. Já no container usa o Kernell do host (Linux) para que tenha o melhor gerenciamento de recursos.
<br>Dentro do Kernell do Linux existem diverssos módulos para manter a saúde e para que os containers consigam se comunicar entre si.
<br>No Kernell tem os módulos namespaces, Cgroups,Netlink etc. Alguns tipos de namespaces são pid ( que faz isolamento de processos) e netnamespace (que faz isolamento de rede).

<br>Como instalar o docker?
<br>[Seguir a documentação](https://docs.docker.com/install/)
<br> Client - CLI
<br> Server - gerencia os containers