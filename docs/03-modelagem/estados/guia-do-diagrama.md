# Guia dos Diagramas de Estados

## 1. O que representa
Representa os estados possíveis de um objeto e os eventos ou condições que provocam mudanças entre eles ao longo de seu ciclo de vida.

## 2. Por que é importante no projeto
Ajuda a definir o comportamento de pedidos, ordens de produção, compras e expedições, evitando transições incompatíveis com as regras operacionais.

## 3. Exemplo no nosso sistema
Uma OP com insuficiência de insumos aguarda reposição. Quando os insumos estão disponíveis, pode iniciar a produção e, após o registro da conclusão, passa ao estado concluído.

## 4. Base para elaboração
Escopo e requisitos, casos de uso e regras de negócio. Quando o catálogo oficial de estados e transições não está definido, o desenho é identificado como proposta para validação do grupo.
