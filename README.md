Desafio DIO: Resumo sobre AWS Step Functions


Este repositório foi criado para documentar minhas anotações, práticas e insights adquiridos durante o desafio de projeto sobre **AWS Step Functions** na plataforma [Digital Innovation One (DIO)](https://www.dio.me/). O objetivo aqui é consolidar o aprendizado sobre workflows automatizados na nuvem e enriquecer meu portfólio de desenvolvimento e arquitetura de sistemas.

O que é o AWS Step Functions?

O AWS Step Functions é um serviço de orquestração sem servidor (serverless) que permite combinar serviços da AWS, como funções Lambda, para criar aplicações complexas e fluxos de trabalho automatizados. 

Meus principais aprendizados sobre o serviço:
Ele funciona como uma máquina de estados finitos.
Facilita o tratamento de erros e tentativas (retries) automáticas em chamadas de APIs.
É configurado usando a Amazon States Language (ASL), baseada em JSON.

Principais Componentes (Estados)

Durante as aulas, mapeei os principais tipos de estados utilizados para controlar o fluxo de execução:

| Tipo de Estado | Descrição do que faz |
| :--- | :--- |
| **Task (Tarefa)** | Executa uma unidade de trabalho, como invocar uma função AWS Lambda. |
| **Choice (Escolha)** | Adiciona ramificações condicionais à lógica (equivalente a um `if/else`). |
| **Parallel (Paralelo)** | Executa múltiplas ramificações de tarefas simultaneamente. |
| **Wait (Espera)** | Atrasa a execução do fluxo por um tempo determinado. |
| **Fail/Succeed** | Interrompe a execução indicando falha ou sucesso do fluxo. |

Casos de Uso no Mundo Real

Anotações sobre onde aplicar o AWS Step Functions em projetos reais:
1. **Processamento de Dados:** Orquestrar pipelines de dados complexos, extraindo e transformando informações de bancos de dados.
2. **E-commerce:** Gerenciar o fluxo de um pedido, desde a verificação do pagamento, baixa no estoque até o envio do e-mail de confirmação.
3. **[Adicione outro caso de uso que você achou interessante na aula]**
