# smartexplorer

Solana program that responds to normal queries for block and tx details, automatically assign labels to some transactions, create graphs and analysis, create alerts based on activity on chain, include p2p network and scrapes social media for solana transactions, projects and related things.

```mermaid
flowchart TB
    website-frontend-->connect-wallet
    website-frontend-->r[burn-token]
    r[burn-token]-->request
    request-->solana-program
    solana-program-->response

    classDef red fill:#ff4d4d,stroke:#b8fb0,stroke-width:1px;
    class r red
```
