> **AVISO:** O conteúdo deste documento foi organizado e estruturado com o auxílio de uma Inteligência Artificial. No entanto, todo o conhecimento, insights e anotações aqui presentes são de autoria própria, refletindo minha compreensão e aprendizado durante as aulas do módulo.

# Laboratório de Workflows Automatizados com AWS Step Functions

### 1. Objetivo do Desafio

Consolidar o aprendizado sobre workflows automatizados com AWS Step Functions por meio da criação de um repositório organizado, contendo anotações e insights adquiridos durante a prática. Este documento serve como material de apoio para estudos e futuras implementações.

### 2. O que são AWS Step Functions? (Resumo)

AWS Step Functions é um serviço de orquestração visual que permite automatizar processos e sequenciar serviços da AWS e de terceiros. A ferramenta funciona para coordenar múltiplos passos em um fluxo de trabalho (workflow), desde uma simples verificação de dados até o gerenciamento de atividades complexas, como o desligamento programado de recursos.

### 3. Resumo da Implementação Prática

O laboratório consistiu na construção de um workflow simples, utilizando um template pronto da AWS. O objetivo era verificar um input em formato JSON. A máquina de estados (State Machine) foi configurada para tomar uma decisão com base no valor do campo `"year"`. Caso o valor fosse `2024`, o fluxo seguiria um caminho; caso contrário, seguiria um caminho alternativo, demonstrando a capacidade de criar lógicas condicionais dentro da automação.

### 4. Anotações e Insights Adquiridos

A seguir, os principais aprendizados e observações obtidas durante a prática com a ferramenta:

* **Interface Visual e Intuitiva:** A plataforma se destaca pela simplicidade de uso. A construção dos workflows é baseada em um sistema de "arrastar e soltar" (*drag-and-drop*) com componentes visuais ("bloquinhos"). Essa abordagem é muito intuitiva e remete a outras ferramentas de automação visual, como os construtores de chatbot da ManyChat. Embora o código seja gerado e possa ser visualizado, toda a programação principal é feita de forma visual.

* **Ampla Capacidade de Integração:** Ficou claro que a ferramenta é extremamente versátil. É possível, por exemplo, integrar uma API Gateway para que o workflow seja iniciado por uma chamada externa, realizando validações com base nos dados recebidos.

* **Diversidade de Aplicações:** As possibilidades de automação são vastas. Alguns exemplos práticos incluem:
    * Invocar uma função **AWS Lambda** para executar uma tarefa específica.
    * Interagir com uma API para validação ou envio de dados.
    * Gerenciar o ciclo de vida de máquinas virtuais (EC2), ligando ou desligando-as em horários pré-definidos para otimização de custos.

* **Monitoramento e Logs Detalhados:** Todo o histórico de execução do workflow fica disponível para consulta. Isso é fundamental para o monitoramento e, principalmente, para a depuração de problemas. Em caso de erro, é possível verificar o log detalhado de cada passo para identificar a causa raiz da falha.
