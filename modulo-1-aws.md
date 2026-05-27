# Módulo 1
## Modelo Cliente-Servidor
O **client** faz o pedido para o server e ele valida se o pedido é legítimo ou não, e a partir desse pedido, o servidor retorna, ou não, uma resposta.

* **Client** - Quem faz a solicitação de informações ou dados.
* **Server** - Quem recebe, processa e devolve os dados.

## Computação em nuvem
É a entrega sob demanda de recursos de TI pela internet com preços de **pagamento conforme o uso**.

> **NOTAS IMPORTANTES**
> 1. *Sob demanda:* O usuário pode aumentar ou diminuir o uso de recursos de acordo com a necessidade.
> 2. *Pela internet:* O usuário acessa esses recursos por meio de serviços baseados na Web.

### Tipos de Implantação na nuvem
* **Nuvem (Cloud-Native):** Existe a flexibilidade de migrar os recursos existentes para a nuvem, projetar e criar novas aplicações no ambiente de nuvem, ou o uso de ambos.
    
* **On-premises (Local):** Exige a compra antecipada dos equipamentos físicos para hospedagem de sistemas da empresa, e como o servidor fica mais próximo, consequentemente resulta numa comunicação de rede mais rápida.
    
* **Híbrida:** Consiste na utilização da implantação on-premises e nuvem, onde se deixa o on-premises devido a preferências de manutenção ou requisitos regulatórios e a nuvem para processamento e análise avançada de dados.

## Principais Serviços Abordados

    
* **Amazon SQS (Simple Queue Service):**
É um serviço de fila de mensagens. Serve para o desacoplamento e comunicação entre diferentes partes de um sistema.
* **Amazon S3 (Simple Storage Service):** 
Serve para o armazenamento de objetos.
* **Amazon EC2 (Elastic Compute Cloud):**
Serve para computação escalável.

## Benefícios da Nuvem

* **Capacidade de pagar conforme o uso:** Permite trocar despesas fixas por despesas variáveis. Não é necessário investimento antecipado em espaço físico, hardware, pessoal ou manutenção. A cobrança mensal varia estritamente conforme o uso dos recursos.
* **Economias de escala massivas:** Como a AWS lida com uma demanda gigantesca de hardware globalmente, isso se reflete em custos significativamente mais baixos para os clientes.
* **Parar de adivinhar a capacidade:** Elimina a necessidade de prever a capacidade de infraestrutura antecipadamente. Você pode alocar apenas os recursos necessários e aumentá-los ou diminuí-los em minutos, com base na demanda real.
* **Aumento de velocidade e agilidade:** A AWS oferece um catálogo extenso de serviços e toda a flexibilidade para experimentá-los. É possível criar ambientes de testes rapidamente e, caso o experimento falhe, basta desativar os recursos para interromper os custos.
* **Parar de gastar dinheiro mantendo data centers:** Elimina não apenas o custo fixo de construir um *data center*, mas também os altos custos contínuos de manutenção dessa infraestrutura física.
* **Globalização em minutos:** Não é necessário construir um *data center* em cada país para operar globalmente. Com a nuvem, você pode implantar as suas aplicações em qualquer região do mundo em questão de minutos.

## Infraestrutura global da AWS

A AWS tem vários _data centers_ distribuídos ao redor do globo. Caso venha a ocorrer algum tipo de desastre, seja ele natural ou tecnológico, essa separação geográfica garante que as aplicações não fiquem indisponíveis todas ao mesmo tempo, conquistando a alta **disponibilidade** e a **tolerância a falhas**.

> **NOTAS IMPORTANTES**
> 1. *Alta disponibilidade:* Consiste em garantir que suas aplicações permaneçam acessíveis com tempo de inatividade mínimo.
> 2. *Tolerância a falhas:* Tem foco em projetar um sistema que continue operando, mesmo em caso de falha de múltiplos componentes.

A AWS foca em construir resiliência em cada camada para que nenhuma falha única derrube todo o sistema. A alta disponibilidade e tolerância a falhas é parte do motivo pelo qual a AWS opera em várias regiões em torno do globo.

### Zonas de Disponibilidade (AZs)

Dentro de cada região, existem as Zonas de Disponibilidade (Availability Zones - AZs).

* Múltiplas AZs (três ou mais) operam dentro de uma mesma região para garantir a redundância.
* Elas são construídas fisicamente separadas (a quilômetros de distância umas das outras). Dessa forma, se um desastre atingir uma AZ, não acarretará a queda das demais, preservando a conectividade e o funcionamento da aplicação.

## Modelo de Responsabilidade Compartilhada da AWS

A segurança e a conformidade são responsabilidades divididas entre a AWS e o cliente.

* **AWS (Segurança DA Nuvem):** A AWS é responsável por proteger a infraestrutura global que executa os serviços oferecidos na nuvem. Isso inclui a manutenção física dos *data centers*, a infraestrutura de rede, os hardwares físicos e os softwares de virtualização.

* **Cliente (Segurança NA Nuvem):** O cliente é responsável por tudo o que ele coloca, configura ou constrói dentro da nuvem. Isso inclui o gerenciamento dos seus próprios dados, a criptografia, a configuração de acessos, as regras de firewall e as atualizações do sistema operacional de suas máquinas virtuais.


### LINKS AWS

> **O que é a computação em nuvem:**
>
>https://aws.amazon.com/pt/what-is-cloud-computing/?nc1=f_cc
>
> **Modelo de responsabilidade compartilhada:**
>
>https://aws.amazon.com/pt/compliance/shared-responsibility-model/
>
> **Regiões e zonas de disponibilidade:**
>
>https://aws.amazon.com/pt/about-aws/global-infrastructure/regions_az/