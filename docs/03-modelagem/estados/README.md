# Diagramas de Estados — Gestão Integrada

**Revisão:** 03/11/2026  
**Status:** documentação-base para revisão do grupo.

## 1. Objetivo
Representar ciclos de vida dos objetos operacionais e distinguir transições documentadas daquelas que ainda dependem de decisão do grupo.

## 2. Arquivos
| Arquivo | Objeto | Situação |
|---|---|---|
| `estado-ordem-producao.mmd` | Ordem de Produção | Proposta baseada em RF17–RF20 e RN05, RN07–RN09; catálogo completo ainda precisa de validação. |
| `estado-pedido.mmd` | Pedido | Proposta; catálogo de estados pendente. |
| `estado-compra-recebimento.mmd` | Compra e recebimento | Proposta; recebimentos parciais e estados detalhados não definidos. |
| `estado-expedicao.mmd` | Expedição | Proposta; estados, cancelamentos e devoluções não definidos. |

## 3. Convenções
Os arquivos usam `stateDiagram-v2` do Mermaid. `[*]` representa estado inicial/final; setas representam transições e seus rótulos indicam eventos ou condições. Estados propostos não são decisões aprovadas.

## 4. Comportamentos documentados para a OP
- Pode ter origem em pedido ou ser criada manualmente (RN09).
- Pode ser criada mesmo com insuficiência, mas aguarda reposição e não pode iniciar (RN04–RN05).
- Pode iniciar quando todos os insumos necessários estiverem disponíveis.
- Consumo de insumos e entrada de produtos acabados são registrados na conclusão (RN07–RN08).

## 5. Pendências
Catálogo completo da OP; estados e cancelamentos de pedidos; recebimentos parciais/divergentes; estados de expedição, devolução e cancelamento; estornos e consistência das movimentações. Estes diagramas não criam requisitos de aprovação, entrega, devolução ou recebimento parcial.
