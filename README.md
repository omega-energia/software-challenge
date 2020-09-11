<p align="center">
    <img src="https://github.com/omega-energia/software-challenge/blob/master/challenge-66.png" width="800">
</p>

# Software Challenge

## Descrição

Esse desafio faz parte do processo seletivo da Omega Energia para a vaga de Software Developer e com ele poderemos avaliar melhor seu perfil em relação a vaga. O desafio consiste em duas partes: uma aplicação Front-end e uma solução Back-end. A descrição com os requisitos delas estão respectivamente [aqui](./Frontend.md) e [aqui](./Backend.md).

## Cenário

A empresa Green Co. possui um milhão de clientes. Na casa desses clientes, a empresa instalou um equipamento no modem de internet para aferir medições de consumo. De hora em hora este equipamento pega o valor em megabyte de quanto foi consumido de dados naquela hora. Logo em seguida, o equipamento envia uma requisição POST HTTP para [https://omegaenergia.com.br/dados/medicao](https://omegaenergia.com.br/dados/medicao) com as seguintes informações:

- CPF do cliente
- megabyte consumido
- hora do consumo
- data do consumo

Por motivos técnicos em alguns modems, pode haver casos em que nosso equipamento não consegue aferir a medição de dados de uma determinada hora. Quando isso acontece, o equipamento tenta aferir novamente aquele horário problemático 24 horas depois e em seguida envia a requisição para o servidor. Em caso de falha novamente, o equipamento tentará de 24 em 24 horas.

Mensalmente a empresa Green Co. agrega todas as informações de consumo e cria uma fatura para o cliente. Essa fatura contém a quantidade de dados consumida, assim como o valor em reais de quanto o consumir precisa pagar.

## Instruções para entrega do projeto

- Desenvolva e use Git para versionamento do código
- Cria um repositório **privado** em um dos três serviços de hospedagem de código: GitHub, BitBucket ou Gitlab
- Adicione no seu repositório como membro o usuário [@vinimdocarmo](https://github.com/vinimdocarmo)
- Envie o documento com a solução Back-end para vinicius.carmo@omegaenergia.com.br
- Qualquer dúvida sobre esse projeto podem ser perguntadas por email em vinicius.carmo@omegaenergia.com.br
