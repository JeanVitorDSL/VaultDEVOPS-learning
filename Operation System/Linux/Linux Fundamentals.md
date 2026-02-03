
---

# ***O que é o Kernel Linux?***

Kernel linux é a base, como se fosse o motor de um carro, ele é igual em todas as distribuições linux, usando de comparativo temos os mais famosos sendo o _Linux Mint, Linux Ubuntu e o Linux Debian_ que, tem o mesmo mortor (Kernel) mudando somente "configurações adicionais", para atingir seus públicos específicos e ganhar seu espaço no mundo linux, nesse sentido dos carros o motor sendo o mesmo muda unicamente a carroceria e suas tecnologias dentro do veículo. 

O kernel linux é oque inicia e da o bot no computador, é que os softwares e sistemas visuais interagem para comunicar com o hardware. Ele descide quem usa a **CPU, memória, disco, rede** e o que é permitido ou negado pelo sistema. O kernel **não** executa aplicações, ele que coordena a execução.

Existem dois mundos dentro de um sistema operacional, usando o linux como base podemos explicar esses dois mundo sendo eles o 
	 **Kernel vs User Spcace**

O kernel SEMPRE ira receber System call dos softwares para que possam ser usados o hardware. Um programa **não pode acessar hardware diretamente**, por isso ele sempre vai fazer uma **system call** para o kernel.

Exemplo mental da linha de ações.

ls → syscall → kernel → disco → kernel → ls → tela

#### O kernel funciona como uma API

O kernel é uma APi estável exposta via:

- System Calls (Read, write, fork, exec)
- /proc (informações dinâmicas)
- /sys (controle do sistema)
Tydi que o docker, Kubernetes e systemd fazem:

	É chamar funcionalidades do Kernel
nada realmente mágico. 


Kernel em si trabalha com processos, sendo a lógica básica do kernel.

Um container ou serviço, software e etc criam processos, esses processos tem um:

- PID
- Espaço de memória 
- Permiss~pes
- Estado (Running, Sleeping, Zombie)

Containers = Processos + isolamento (kernel puro)

Gerenciamento de CPU (Scheduler)

O kernel decide qual processo roda do sistema, quanto tempo e em qual core, resolvendo a  concorrência, fairness e prioridades


---
O que é o GNU?
Filosofia do linux?
Distribuições do linux.

