# A ideia básica se baseia em uma ferramenta genérica de processamento de streams. 

Este projeto visa tornar a gestão de processos na área de Tecnologia da Informação fácil de se realizar.
Auxilia a criação de processos otimizadores que potencializem a execução de trabalho da sua equipe de TI.
É utilizado o conceito básico de Macro-processo, Processo, Tarefa e Atividade.

A implementação será dividida em módulos para contemplar uma aplicação baseada em micro-serviços.
Serão utilizadas técnicas, ferramentas e metodologias focadas nas ferramentas que apoiam a gestão do software com facilidade como: __Docker, Jenkins, Java 8, orientação a objetos, restful api, monitoramento, Spring boot, etc.__

__Macro-processo:__ O usuário criará seus macro-processos o qual é o conjunto de regras de negócio definido o mais abstrato possível que englobe uma área do negócio que faça sentido sozinho.

__Processo:__ O usuário definirá em cada __macro-processo__ o conjunto de __processos__ que estão envolvidos no procedimento.

__Tarefa:__ Uma tarefa é uma operação descrita, ou seja, a descrição e definição do que deve acontecer.

__Atividade:__ A atividade por sua vez é a tarefa executada, assim sendo, a execução, de fato, da tarefa.

## Processamento de streams
O processamento de streams é a forma de trabalhar desta ferramenta. Sempre pensando em funções, ou seja, para uma entrada sempre terá a mesma saída. O usuário pode definir suas funções e definir o encadeamento entre cada uma das funções. Ao final, todas as funções terão transformado sua entrada na saída desejada.

__Deverá ser criado um mecanismo de registro de funções para uso nas tarefas.__

## Micro-serviços
### Em cada micro-serviço serão feitos o Cadastro, Alteração e Remoção dos modelos
- Macro-processo: A informação mais gerencial e onde é iniciado o processo, onde se olha o status geral do processo.
- Processo: O rastreamento, monitoramento, logging, e ordem da execução das tarefas.
- Tarefa: A definição dos contratos de interação do micro-serviço: Entrada e Saída.
- Atividade: A execução da função especificamente.

## Aplicação móvel
Será criada uma aplicação móvel Android nativa que gerencia as requisições e executa as atividades.
A ideia é que a aplicação móvel apenas dispare a solicitação e o trabalho pesado seja feito entre os micro-serviços.
Estes por sua vez devem saber sua ordem no processo, o que esperar do próximo micro-serviço e o que fazer caso algum micro-serviço se comporte de forma não esperada.

Vamos fazê-la juntos!
