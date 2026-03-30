# ADR-0001 — Arquitetura inicial do Mini-CRM (monólito modular)

## Contexto
Queremos evoluir rápido com qualidade (CI sempre verde), mantendo regras de negócio claras e testáveis.
O projeto será pequeno/médio no começo, mas deve permitir modularização e refactoring contínuo.

## Decisão
Adotar um **monólito modular** com separação em módulos/pacotes:
- `domain`: modelo e regras de negócio (sem dependência de Spring)
- `application`: casos de uso e portas (interfaces)
- `infra`: implementações (persistência, integrações)
- `api`: controllers e DTOs

## Consequências
- (+) Regras de negócio ficam testáveis sem framework
- (+) Mudanças em infra não contaminam o domínio
- (+) Evolui para microserviços apenas se um dia fizer sentido
- (-) Exige disciplina de organização e limites entre módulos
