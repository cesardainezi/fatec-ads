#### [[ISO030 - Sistemas Operacionais| ◀ Voltar: ISO030 - Sistemas Operacionais]]
#### [[Machado & Maia - Arquitetura de Sistemas Operacionais - 4ª ed.pdf#page=14|▶ Livro: Machado & Maia, Arquitetura de Sistemas Operacionais]]

# Resumo (gerado por IA)

## 1. Introdução

> Um **sistema operacional** é um conjunto de rotinas que gerencia os recursos do computador, atuando como intermediário entre o usuário e o hardware. Ele controla o uso do processador, da memória e dos dispositivos de entrada e saída, garantindo eficiência, segurança e facilidade de uso ao abstrair a complexidade do hardware, sendo acionado de forma não linear em resposta a eventos do sistema.

--- 

## 2. Funções Básicas

> O sistema operacional é responsável por gerenciar e coordenar os recursos de hardware e software do computador, garantindo seu uso eficiente e seguro. Entre suas principais funções estão o **gerenciamento do processador**, controlando a execução e o escalonamento dos processos; o **gerenciamento de memória**, alocando e liberando espaço conforme a necessidade dos programas; o **gerenciamento de dispositivos de entrada e saída**, por meio de drivers e mecanismos de comunicação com o hardware; e o **gerenciamento de arquivos**, organizando o armazenamento, acesso e proteção dos dados. Além disso, o sistema operacional fornece uma **interface de interação com o usuário**, seja gráfica ou por linha de comando, e mecanismos de **proteção e segurança**, assegurando a integridade do sistema e o isolamento entre processos.

--- 

## 3. Máquina de Camadas

> A organização em **máquina de camadas** consiste em estruturar o sistema operacional em níveis hierárquicos, nos quais cada camada utiliza apenas os serviços da camada imediatamente inferior e fornece serviços à camada superior. Essa abordagem permite ocultar os detalhes de implementação do hardware por meio de abstrações progressivas, tornando o sistema mais organizado, modular e compreensível. Entre suas principais vantagens estão a **facilidade de desenvolvimento, manutenção e depuração**, já que alterações em uma camada tendem a afetar minimamente as demais. Como desvantagem, o modelo pode introduzir **sobrecarga e perda de desempenho**, devido à necessidade de atravessar múltiplas camadas para acessar determinados recursos.


--- 

## 4. Histórico

[[Machado & Maia - Arquitetura de Sistemas Operacionais - 4ª ed.pdf#page=17|Vide livro]]

--- 

## 5. Tipos de Sistemas Operacionais

> Os **sistemas operacionais** podem ser classificados de acordo com a forma de execução dos programas, o número de usuários, o tipo de processamento e a arquitetura de hardware.  

> Quanto à **execução de programas**, destacam-se os sistemas **monoprogramáveis (monotarefa)**, que executam apenas um programa por vez, e os **multiprogramáveis (multitarefa)**, que permitem a execução concorrente de vários programas. Estes últimos subdividem-se em **batch**, nos quais os programas são executados em sequência sem interação com o usuário; **tempo compartilhado**, onde cada processo recebe uma fatia de tempo de CPU, dando a impressão de simultaneidade; e **tempo real**, nos quais a correção do sistema depende do atendimento a prazos rígidos, com forte controle por prioridades.  

> Quanto ao **número de usuários**, os sistemas podem ser **monousuário** ou **multiusuário**, permitindo acesso simultâneo de vários usuários ao mesmo sistema.  

> Em relação à **arquitetura de processamento**, existem sistemas **monoprocessados** e **multiprocessados**, sendo estes últimos capazes de utilizar vários processadores de forma cooperativa, com memória compartilhada (fortemente acoplados) ou distribuída (fracamente acoplados).  

> Por fim, há classificações baseadas no **ambiente de aplicação**, como sistemas **distribuídos**, **embarcados** e **móveis**, desenvolvidos para atender requisitos específicos de desempenho, consumo de energia, confiabilidade e conectividade.

--- 

## 6. Exercícios

**1. Como seria utilizar um computador sem um sistema operacional? Quais são suas duas principais funções?**
> _O acesso seria pouco prático e arriscado, pois o usuário precisaria manipular diretamente o hardware do computador, o que demandaria de profundo conhecimento sobre a máquina. Quanto às funções de um sistema operacional, as duas principais são: **facilitação de acesso aos recursos** – o usuário se torna capaz de realizar tarefas computacionalmente complexas com poucos comandos; **compartilhamento de recursos de forma organizada e protegida** – o sistema administra os recursos para o usuário, utilizando à medida que for necessário. Isto impede o acesso direto ao hardware o que reduz o risco de danificação por mau uso._

**2. Quais as principais dificuldades que um programador teria no desenvolvimento de uma aplicação em um ambiente sem um sistema operacional?**
> _Uma aplicação seria programada diretamente no hardware, o que demandaria conhecimentos sobre o funcionamento elementar de cada componente. Além disso, o programador teria que implementar em sua aplicação uma série de rotinas que o sistema operacional já executa, como gerenciamento de memória._

**3. Explique o conceito de máquina virtual. Qual a grande vantagem em utilizar este conceito?**
> _Máquina virtual é uma abstração do computador fornecida pelo sistema operacional ao usuário e às aplicações. A grande vantagem é permitir que programas sejam desenvolvidos e executados sem a necessidade de conhecer detalhes dos componentes de hardware, proporcionando maior segurança, simplicidade e isolamento._

**4. Defina o conceito de uma máquina de camadas.**
>_Uma máquina de camadas é um modelo organizacional do computador em níveis hierárquicos, do mais baixo ao mais alto. No nível mais baixo encontram-se os componentes de hardware, enquanto que no nível mais alto estão o sistema operacional e as aplicações. Este conceito permite que cada camada utilize os serviços da camada inferior sem a necessidade de conhecer sua implementação._

**5. Quais os tipos de sistemas operacionais existentes?**
> _Os sistemas operacionais podem ser classificados em:_
> - _**Monoprogramáveis** (ou monotarefa): permitem a execução de apenas um programa por vez, utilizando todos os recursos do sistema._
> - _**Multiprogramáveis** (ou multitarefa): permitem a execução concorrente de vários programas, organizando o uso dos recursos por meio de técnicas como processamento batch, tempo compartilhado e tempo real._
> - _**Sistemas com múltiplos processadores**: utilizam mais de um processador para executar programas, possibilitando paralelismo real e maior desempenho._

**6. Por que dizemos que existe uma subutilização de recursos em sistemas monoprogramáveis?** 
> _Dizemos que existe uma subutilização dos recursos porque apenas um programa é mantido em memória. Desta forma, quando o programa realiza operações de entrada e saída, a unidade de processamento permanece ociosa, sendo assim, subutilizada._

**7. Qual a grande diferença entre sistemas monoprogramáveis e sistemas multiprogramáveis?**

> Um sistema monoprogramável mantém um único programa em execução por vez, de forma que, durante operações de entrada e saída, a unidade de processamento permanece ociosa. Em sistemas multiprogramáveis, ocorre a execução concorrente de vários programas, diminuindo a subutilização de recursos e possibilitando o maior aproveitamento da UCP.

**8. Quais as vantagens dos sistemas multiprogramáveis?**

> A principal vantagem dos sistemas multiprogramáveis é o melhor aproveitamento dos recursos do sistema, o que efetivamente diminui os custos de execução em função à. Este tipo de sistema também permite a redução do tempo médio de execução das aplicações, já que uma aplicação não precisa esperar outra encerrar para começar a utilizar recursos.

**9. Um sistema monousuário pode ser um sistema multiprogramável? Dê um exemplo.**

> Sim. Um exemplo é um sistema operacional para computadores pessoais e estações de trabalho, onde há um único usuário interagindo.1

**10. Quais os tipos de sistemas multiprogramáveis?**

> _Resposta_

**11. O que caracteriza o processamento batch? Quais aplicações podem ser processadas neste tipo de ambiente?**

> _Resposta_

**12. Como funcionam os sistemas de tempo compartilhado? Quais as vantagens em utilizá-los?**

> _Resposta_

**13. Qual a grande diferença entre sistemas de tempo compartilhado e tempo real? Quais aplicações são indicadas para sistemas de tempo real?**

> _Resposta_

**14. O que são sistemas com múltiplos processadores e quais as vantagens em utilizá-los?**

> _Resposta_

**15. Qual a grande diferença entre sistemas fortemente acoplados e fracamente acoplados?**

> _Resposta_

**16. O que é um sistema SMP? Qual a diferença para um sistema assimétrico?**

> _Resposta_

**17. O que é um sistema fracamente acoplado? Qual a diferença entre sistemas operacionais de rede e sistemas operacionais distribuídos?**

> _Resposta_

**18. Quais os benefícios de um sistema com múltiplos processadores em um computador pessoal?**

> _Resposta_

**19. Qual seria o tipo de sistema operacional recomendável para uso como servidor de aplicações em um ambiente corporativo?**

> _Resposta_

**20. Qual seria o tipo de sistema operacional recomendável para executar uma aplicação que manipula grande volume de dados e necessita de um baixo tempo de processamento?**

> _Resposta_

