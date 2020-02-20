# OZchallenge - Summer Edition

## Contextualização

A DevOZ possui hoje um sistema para controle de permissão de execução de seu sistema principal, o OZmap, chamado ISIS Manager.  
O ISIS Manager, como o nome já diz, é uma implementação antiga, tendo como principal funcionalidade armazenras dados enviados pelos OZmaps e realizar autenticação de clientes registrados.  
O objetivo do desafio é uma implementação moderna de um software para agir como OZmap Manager, incluindo as funcionalidades atuais e alguns adendos que servirão para melhorar o fluxo de venda / suporte da empresa.

## Entrega
O desafio prevê uma série de entregas semanais, toda sexta-feira, para permitir ao cliente (DevOZ) acompanhamento do desenvolvimento do sistema.  
Terá início na sexta-feira 21/02/2020 e tem a data de término agendada para 27/03/2020.  
Os competidores serão divididos em duplas, montadas por sorteio.
Nesta data, além da entrega do código fonte cada equipe deve realizar uma apresentação de até 10 minutos sobre o software desenvolvido.  

## Definição das funcionalidades
A implementação deve prever no mínimo as seguintes funcionalidades:

### Serviços básicos
* Sistema Web 

* Interface responsiva

* Autenticação (Login / Senha, Token, Social Media ([google no mínimo](https://github.com/jaredhanson/passport-google)))

* Controle de acesso  
Usuários sem autenticação não devem ter acesso a informações sensitivas.

### Serviços externos (APIs externas)

* <strong>Autenticação</strong>  
Pelo menos uma vez ao dia, cada OZmap envia uma requisição ao manager informando estado atual da rede, e recebe uma resposta se está permitido a continuar a execução.  
A implementação deve seguir o modelo atual do manager.

### Serviços pela interface

* <strong>Informações de máquinas</strong>  
Deve armazenar e exibir informações que permitam acesso a máquina dos clientes, tais como:
  * Host
  * Porta
  * User
  * Password
  * Identificador

* <strong>Informações de clientes</strong>  
Deve armazenar, exibir e exportar informações básicas dos clients, que são enviados a cada pedido de autenticação, incluindo número de caixas, clientes e a versão atual sendo executada.

* <strong>Manter dados históricos</strong>  
Armazenar informações históricas (enviadas a cada autenticação) e que permitam monitorar o uso / engajamento do OZmap (definir estratégia de forma que considere o uso do cliente, sem considerar as ações feitas por integrações e softwares de monitoramento).

* <strong>Reinicialização de serviços</strong>  
De forma fácil e intuitiva, permitir que um serviço sendo executado na máquina de um cliente seja reiniciado.

* <strong>Envio de notificações</strong>  
Deve ser possível enviar uma mensagem a um ou mais OZmaps.
A mensagem deve possuir um tipo e um nível de urgência, ambos configuráveis, para melhor apresentação da mensagem.

#### As funcionalidades abaixo não são obrigatórias, mas a modelagem do banco e estruturação do software devem ao mínimo possibilitar uma implementação futura.

### Serviços de integração
* <strong>Identificação de plano</strong>  
Identificar no ERP o plano do cliente e disponibilizar ao OZmap quais módulos o cliente tem acesso.

* <strong>Identificação de mudança de faixa</strong>  
Alguns clientes possuem um modelo de contrato envolvendo faixas de clientes. O sistema deve identificar mudança de faixa e notificar os adminstradores por email.

* <strong>Identificação de inadimplência</strong>  
Identificar inadimplência no ERP.

* <strong>Criação / remoção de máquinas</strong>  
Poder criar e remover máquinas automaticamente de acordo com uma compra no site / inadimplência prolongada.

## Tecnologias
* Única restrição de tecnologia para implementação do sistema:  
Não pode ser feito uso de ExtJS.  
Qualquer outra biblioteca / framework JS está liberado.

* Não reinvente a roda. Faça uso de tecnlogias e bibliotecas existentes.

* Siga sempre o [principio KISS](https://pt.wikipedia.org/wiki/Princ%C3%ADpio_KISS).

## Critérios de Avaliação
* UX
* Completa implementação das funcionalidades obrigatórias
* Implementação das funcionalidades de integração
* Bom uso do git (commits concisos, boas mensagens de commit, etc)
* Boas práticas de programação (nomes de variáveis, tamanho de funções, perfomance)
* Código bem organizado e com uma boa arquitetura
* Uso de bibliotecas para auxiliar o desenvolvimento  

Será considerado vencedora a equipe que acumular um maior número de pontos considerando os critérios dispostos neste documento e uma avaliação geral da apresentação final.  
Caso nenhuma equipe apresente um resultado superior ao ISIS Manager atualmente implementado, não haverá vencedor.


## Premiação
Um total de R$500.00 a ser dividido entre os membros da equipe.

Boa sorte!

Equipe DevOZ	
