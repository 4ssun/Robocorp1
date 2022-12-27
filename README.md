**ROBOCORP**

Introduzindo o Robocorp, ele é uma solução de RPA de código aberto. Tendo isso em mente, nós sabemos como a automação de processos vem sendo *muuito* utilizada em empresas de médio e grande porte, tudo para economizar tempo em algumas tarefas repetitivas e mapeadas.
Pensando nisso, qual o diferencial do Robocorp de outros concorrentes como a gigante Uipath?

 - Curva de aprendizado curta;
 - Grande ecossistema de libraries disponíveis;
 - Baseado em Python;
 - Extensão própria no editor Visual Studio Code;
 - Suporte para Max, Linux e Windows.
# Este diretório

Nesse repertorio github estão os arquivos que foram criados no meu robô para obter o certificado level 1 do Robocorp.


## O que devo ter em mente?

O robô que criamos juntamente do robocorp possui um corpo. Imagine em três partes:

 - **Cabeça**
 - **Tronco**
 - **Pernas**
 
 Mas eles estão dispostos com outros nomes que são:
 - ***Settings***
 -   ***Tasks***
 - ***Keywords***

E após nosso robô belíssimo ser construído, deve ser orquestrado e para isso, utilizamos o próprio laboratório de controle de robôs do Robocorp, disponível em seu painel de controle de usuário. Lá, conseguimos acompanhar como está o andamento da tarefa, com os status: New, Pending, Processing, Failed, Done, Total e Exceptions.
## Falando mais sobre o corpo

Settings é literalmente a cabeça do robô, onde iremos importar as bibliotecas que serão necessárias durante seu desenvolvimento e inclusive podemos incluir uma documentação nesta etapa.

Tasks será a chamada a de funções que irão ser empenhadas na etapa de Keywords que falaremos em alguns segundos. Tasks funciona como quando criamos uma função em Python e precisamos chamá-la.

Podemos dividir a compreensão de Keywords em duas partes:

 - Nomeamos a função que será chamada em Tasks.
 - Desenvolvemos abaixo o que aquela função fará.
 
 Exemplo:
 ***Log in***

->Input Text  username  'maria'

->Input Password  password  'thoushallnotpass'

Submit Form

Wait Until Page Contains Element  'id:sales-form'

Conseguiram identificar uns comandinhos conhecidos em Python? Wait Until lembra o quê? Exatamente: **Selenium**. O nome da função sendo Log in, as tarefas da função sendo:

 - Input Text
 - Input Password
 - Submit Form
 - Wait until Page Contains Element

E após as tarefas vêm seus respectivos parâmetros. Além disso, vale salientar que o Robocorp precisa de uma identação igual ao Python, uma barra tab ou duas batidas na barra de espaço é suficiente.

