# SPEC — Mini CRM (vivo)

## Objetivo
Um Mini-CRM para cadastrar e acompanhar leads/contatos e o status do funil.

## MVP (primeira versão)
- Cadastrar Lead
- Listar Leads
- Atualizar status do Lead (NEW, CONTACTED, QUALIFIED, WON, LOST)

## Regras de negócio (iniciais)
- Nome é obrigatório
- Email (se informado) deve ser válido
- Status começa como NEW

## Decisões
- ADR-0001: Arquitetura (monólito modular)

## Próximos passos
- [ ] Bootstrap do projeto Spring Boot (verde)
- [ ] Criar ADR-0001
- [ ] Subir pipeline de CI (GitHub Actions)
- [ ] Implementar “Cadastrar Lead” end-to-end
