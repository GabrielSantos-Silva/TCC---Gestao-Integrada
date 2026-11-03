# Diagramas de Atividades — Gestão Integrada

**Revisão:** 03/11/2026  
**Status:** documentação-base para revisão do grupo.

## 1. Objetivo
Documentar os fluxos operacionais principais, destacando sequência de atividades, decisões e responsabilidades.

## 2. Arquivos
| Arquivo | Processo | Referências |
|---|---|---|
| `atividade-pedido-producao.mmd` | Pedido, OP, reserva de produto acabado e cálculo da produção restante | UC06–UC09; RF12–RF20; RN02–RN05, RN09–RN10; PD12 |
| `atividade-compras-recebimento.mmd` | Compra e recebimento de insumos | UC04–UC05; RF09–RF10; RN06 |
| `atividade-conclusao-producao.mmd` | Início e conclusão da produção | UC08–UC09; RF17–RF20; RN05, RN07–RN08 |
| `atividade-expedicao.mmd` | Expedição e saída de produtos acabados | UC10; RF21–RF22; RN11 |

## 3. Convenções
Os arquivos usam `flowchart` do Mermaid para representar atividades, decisões e caminhos alternativos. As raias/responsabilidades são simplificadas e não definem perfis de acesso.

## 4. Regras refletidas
- Todo pedido gera exatamente uma OP, inclusive quando a quantidade a produzir for zero.
- A OP de um pedido reúne seus produtos; não é criada uma OP por item.
- Quantidade a produzir = quantidade solicitada − quantidade reservada de produto acabado.
- A reserva não reduz o estoque físico; o saldo disponível considera reservas ativas.
- Compra registrada não gera entrada em estoque; a entrada ocorre no recebimento efetivo.
- Insuficiência de insumos não impede criar a OP, mas impede iniciar a produção.
- Consumo de insumos e entrada de produtos acabados ocorrem na conclusão da OP.
- Expedição gera saída correspondente do estoque de produtos acabados.

## 5. Pendências
Detalhes técnicos e concorrência das reservas (PD12), liberação/consumo de reservas em cancelamento e expedição, recebimentos parciais, divergências, cancelamentos, estornos e exceções durante a produção. As raias também devem ser validadas com o grupo.

Os diagramas não acrescentam aprovação automática de compras, envio de pedidos a fornecedores, transporte ou confirmação de entrega.
