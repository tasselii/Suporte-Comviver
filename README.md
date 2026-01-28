# Fluxo de Atendimento – Suporte ao Cliente

```mermaid
flowchart LR
    A[Cliente] -->|Abre chamado| B[Suporte]
    B -->|Registra| C[Identificar Chamado]

    C --> D{Modulo}

    D --> D1[DLG]
    D --> D2[TRBR]
    D --> D3[PRO]
    D --> D4[THR SQL]
    D --> D5[Parana Moveis]
    D --> D6[Guarulhos]
    D --> D7[DC Paulista]
    D --> D8[Asperbras]
    D --> D9[Bonolat]

    D -->|Definido| E[Desenvolvimento]
    E --> F{Precisa apoio?}

    F -->|Nao| G[Correcao]
    F -->|Sim| H[Consultoria]

    H --> H1[Financeiro]
    H --> H2[Logistica]
    H --> H3[Manufatura]

    H1 --> G
    H2 --> G
    H3 --> G

    G --> I[Suporte]
    I --> J[Cliente]
    J --> K[Finalizado]
