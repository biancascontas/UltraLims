# Relatório de Correção da Suíte

Nome: Bianca Rocha Bernardo
Data: 07/10/2026

---

## 1. Problemas encontrados

Liste o que estava errado. Um item por problema, com o arquivo e a linha aproximada.

| # | Arquivo | Problema | Por que isso é um problema |
|---|---------|----------|----------------------------|
| 1 |Laudo    |linha  15 | Não faz nada  (redundante) |
| 2 |Laudo    |linha  16 | Sempre passa               |

## 2. O que você mudou

Um parágrafo curto por alteração. Diga o que fez e por que essa é a correção certa, não apenas o que faz o teste passar.

Retirei as linhas 15 e 16 por entender que a primeira não faz nada e a segunda obriga o teste a passar sem validar corretamente se o laudo está liberado. A minha correção foi para validar a tela aberta afim de verificar o laudo e confirmar o "liberado" na listagem.

## 3. Resultado do teste de estabilidade

Saída de `npm run estabilidade`:

```
(![Print do teste](./img.png)
![alt text](image-1.png)

  (Run Finished)


       Spec                                              Tests  Passing  Failing  Pending  Skipped
  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ √  amostra.cy.js                            00:02        1        1        -        -        - │
  ├────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ √  laudo.cy.js                              00:03        1        1        -        -        - │
  ├────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ √  login.cy.js                              00:01        1        1        -        -        - │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘
    √  All specs passed!                        00:06        3        3        -        -        -

    PS C:\Users\Bianca\Downloads\qa-junior-cypress\qa-junior-cypress\cypress> npm run estabilidade

    > ultra-lims-desafio-qa@1.0.0 estabilidade
    > node scripts/estabilidade.js

    Execucao 1 de 10... passou
    Execucao 2 de 10... passou
    Execucao 3 de 10... passou
    Execucao 4 de 10... passou
    Execucao 5 de 10... passou
    Execucao 6 de 10... passou
    Execucao 7 de 10... passou
    Execucao 8 de 10... passou
    Execucao 9 de 10... passou
    Execucao 10 de 10... passou

    ----------------------------------------
    Execucoes que passaram: 10 de 10
    ----------------------------------------
)
```

## 4. O que você deixaria para depois

O que você percebeu mas escolheu não resolver agora, e por quê. Priorizar faz parte do trabalho.
O login usa credenciais fixas diretamente no teste, isso pode ser ruim para segurança ou manutenção porque pode vazar no git ou ficar visivel no repositório, também pode usar um login e senha real da produção. Verificaria esse ponto com meu superior para entender melhor. 
---

*Fim do relatório. Não adicione outras seções.*
