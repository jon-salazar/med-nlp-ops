# med-nlp-ops

## Tema central

Deploy de modelo NLP em produção com pipeline CI/CD, monitoramento e otimização de latência.

## Contexto

Este projeto simula o cenário de um hospital de referência que precisa automatizar a triagem de laudos médicos em texto para classificação de urgência:

- **normal**
- **atenção**
- **urgente**

O núcleo da solução é um classificador de texto (NLP) leve, disponibilizado por meio de uma **API REST** empacotada em **container Docker**.

## Objetivo do projeto

Garantir que o ciclo de vida do modelo seja operacionalizável de ponta a ponta, com foco em:

1. **CI/CD com GitHub Actions**  
   Automação de build, testes e entrega da aplicação/modelo.

2. **Orquestração básica de retreino com Airflow**  
   Execução agendada e rastreável de fluxos de atualização do modelo.

3. **Monitoramento essencial com Prometheus + Grafana**  
   Coleta e visualização de métricas de saúde da API e desempenho do modelo.

4. **Otimização de latência**  
   Redução de tempo de resposta para viabilizar uso em ambiente clínico.

## Escopo funcional esperado

- Serviço de inferência para classificação de urgência de laudos médicos.
- Pipeline de integração e entrega contínua para mudanças de código e modelo.
- Rotina inicial de retreino/versionamento orquestrada.
- Observabilidade mínima para disponibilidade e performance.
- Práticas de operação voltadas à confiabilidade e baixa latência.