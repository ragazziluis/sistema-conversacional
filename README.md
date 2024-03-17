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

