# Fluxo-Publicacao-da-Tarefa


    
  ```mermaid
graph TD
    A[Pega atividade e cria branch] -->|Desenvolve e comita| B(Cria PRs) 
    B --> C[Escolha um Ambiente]
    C -->|completa PR da branch| D[sprint_superapp_63]
    C -->|completa PR da branch| E[homolog]
    C -->|completa PR da branch| F[main] --> G[É executado o pipeline] --> H[Solicitar aprovação da release] --> 
    I[Publica no staging] --> J[Verifica se ta tudo certo na staging]-->L[Executa o SWAP]


```
