# Proposta para Fomentar o Aprendizado Contínuo em Sistemas Conversacionais

## **Introdução**

O crescente domínio das interfaces conversacionais em diversos setores de mercado tem sido notável. Esses sistemas não só apoiam colaboradores de diferentes departamentos, mas também têm o potencial de revolucionar a experiência do consumidor. Entre suas inúmeras aplicações, os robôs conversacionais, ou chatbots, visam essencialmente auxiliar as pessoas na resolução de problemas e na execução eficiente de tarefas do dia a dia.

## **Desafios dos Sistemas Conversacionais**

Além das vantagens oferecidas pelos sistemas conversacionais, há desafios significativos que precisam ser enfrentados para garantir sua eficácia e relevância contínuas. Um desses desafios é o constante ajuste e aprimoramento dos modelos de conversação em resposta às mudanças nas preferências do usuário, no contexto e nas expectativas. Outro desafio crítico é o gerenciamento do *concept drift*, que se refere à evolução gradual das características e padrões nas interações humanas ao longo do tempo. O *concept drift* pode levar à deterioração do desempenho do sistema se não for devidamente reconhecido e tratado.

## **Concept Drift**

O *concept drift* é uma preocupação central nos sistemas conversacionais. Ele ocorre quando as relações entre as entradas e saídas do sistema mudam ao longo do tempo, devido a mudanças nas preferências dos usuários, nas tendências sociais, nas políticas da empresa ou em outros fatores contextuais. Essas mudanças contínuas na distribuição dos dados podem tornar os modelos de conversação obsoletos, afetando negativamente a qualidade das interações.

## **Solução Proposta**

### **Diagrama de Blocos**

<img width="1504" alt="Relationship Diagram 1" src="https://github.com/ragazziluis/sistema-conversacional/assets/110607385/555fca5e-f1f1-426c-99c1-023c66074011">

### **Descrição Textual do Diagrama de Blocos do Sistema Conversacional**

O diagrama de blocos ilustra o fluxo de informações em um sistema conversacional:

**1. Conversa com Chatbot:**

- Descrição: Registrar interações entre o usuário e o sistema, abrangendo perguntas feitas pelo usuário e as respostas fornecidas pelo sistema.
- Método: Monitorar ativamente as conversas em tempo real, capturando e armazenando dados relevantes para análise subsequente.

**2. Análise de Sentimento:**

- Descrição: Avaliar a satisfação e a resposta emocional do usuário, bem como identificar mudanças nas preferências ao longo do tempo.
- Método: Empregar técnicas de análise de sentimento para compreender a reação emocional do usuário em relação às respostas fornecidas pelo sistema, permitindo uma adaptação mais precisa e contextualizada.

**3. Retorno de Resposta ao Usuário:**

- Descrição: O modelo, após finalizar a análise de sentimento, retorna uma resposta para a interface de usuário.
- Método: Retornar resposta e oferecer como opcional ao usuário a oportunidade de realizar um feedback.

Repare que, após o modelo retornar uma resposta ao usuário, o mesmo terá a oportunidade de fazer a devolutiva de um feedback para o sistema, fazendo com que o sistema identifique um concept drift. O diagrama dessa parte da solução será da seguinte forma:

### **Descrição Textual do Diagrama de Blocos do Sistema Conversacional com Identificação de Concept Drift**

<img width="2480" alt="Relationship Diagram 2" src="https://github.com/ragazziluis/sistema-conversacional/assets/110607385/9be28dc0-5904-4ea0-9f48-619d00f451ff">

**Feedback do Usuário:**

- O sistema coleta feedback do usuário sobre a resposta gerada.
- O feedback pode ser positivo (satisfeito com a resposta) ou negativo (insatisfeito com a resposta).
- O feedback é utilizado para melhorar o desempenho do sistema ao longo do tempo.

**Processamento do Feedback:**

- O feedback do usuário é analisado para determinar se a resposta foi satisfatória ou não.
- Se a resposta foi satisfatória, o modelo é atualizado para fortalecer a geração de respostas semelhantes.
- Se a resposta foi insatisfatória, o modelo é atualizado para evitar a geração de respostas semelhantes no futuro.

## **Conclusão**

Esta proposta visa abordar o problema da falta de atualização de modelos em sistemas conversacionais, permitindo que eles se adaptem continuamente às mudanças nos dados de entrada. Embora a implementação de tal solução exija esforço significativo em termos de desenvolvimento de algoritmos de detecção de *concept drift*, reamostragem de dados e treinamento incremental, os benefícios resultantes em termos de qualidade das interações e satisfação do usuário podem justificar esse esforço.

## **Referências Bibliográficas**

1. Gama, J., Sebastião, R., & Rodrigues, P. (2004). Issues in Incremental Learning. In AAAI-2004 Workshop on. Link
2. Widmer, G., & Kubat, M. (1996). Learning in the Presence of Concept Drift and Hidden Contexts. Machine Learning, 23(1), 69–101. Link
3. Tsymbal, A. (2004). The problem of concept drift: definitions and related work. Technical report, Trinity College Dublin, Ireland. Link
