# Sprint 2 — 06/10/2025 a 26/10/2025

**Meta da Sprint:** Entregar a gestão e visualização de propriedades — listagem, exibição no mapa, registro preciso via Plus Code e geração de certificado digital.

---

## 🧩 Capacidade da equipe (estimativa)
- Capacidade estimada: **16 SP** (mesma referência usada na Sprint 1)

---

## 📋 Stories selecionadas (Sprint Backlog)

| ID | Rank | User Story | Estimativa (SP)|
|----|------|------------|-----------------|
| 4  | Alta | Como usuário, quero visualizar minhas propriedades em uma lista para acessá-las de forma organizada. | 3 |
| 5  | Alta | Como usuário, quero ver minhas propriedades no mapa para acompanhar sua localização. | 6 |
| 6  | Alta | Como usuário, quero adicionar o Plus Code da minha propriedade para registrá-la com precisão. | 4 |
| 7  | Média | Como usuário, quero gerar um certificado digital para comprovar a posse da minha propriedade. | 3 |

**Total estimado:** **16 SP** (encaixa na capacidade estimada — sprint sem folga, planejamento cuidadoso necessário)

---

## ✅ Critérios de Sucesso / Aceitação

**Story 4 — Listagem de propriedades**
- Endpoint `/properties` retorna lista com campos mínimos (id, nome, coordenadas, PlusCode).  
- Frontend exibe lista ordenável (por nome/data) e abre detalhe ao clicar.  
- Teste: criar 3 propriedades de exemplo e confirmar listagem e navegação.

**Story 5 — Propriedades no mapa**
- Marcadores aparecem no mapa para todas as propriedades com coordenadas válidas.  
- Ao tocar num marcador, abre um *callout* com nome e botão “Ver detalhes”.  
- Performance: mapa deve carregar até 50 marcadores sem travar (teste em dispositivo real).

**Story 6 — Cadastro do Plus Code**
- Formulário permite inserir Plus Code, valida formato e converte para coordenadas.  
- Backend salva Plus Code e coordenadas associadas à propriedade.  
- Fluxo: usuário cadastra Plus Code → app mostra marcação no mapa imediata.

**Story 7 — Geração de certificado PDF**
- Backend (ou frontend) gera PDF com dados da propriedade, proprietário e código único.  
- Usuário pode baixar/compartilhar o PDF no Android.  
- PDF contém assinatura/identificador para validação (mínimo: selo/texto com data e id).

---

## 🧾 Definition of Done (DoD)

- Código com **Pull Request** criado e descrição completa.  
- **Revisão de código** aprovada por pelo menos um revisor.  
- **Testes manuais** executados e validados.  
- **Documentação** atualizada (endpoints, telas ou instruções).  
- Build Android funcional em ambiente de teste e validado na *Sprint Review*.

---

## 🎯 Entregáveis / Demonstração

- **Data da Review:** 27/10/2025  
- **Demonstração esperada:**  
  - Listagem e mapa de propriedades funcionando.  
  - Cadastro de Plus Code com validação.  
  - Geração e visualização de certificado em PDF.  
- **Artefatos:**  
  - PRs no GitHub  
  - Endpoints documentados no README/API  
  - Build APK ou execução no emulador Android

---

📌 **Resumo da Sprint 2:**  
A equipe focará em consolidar o núcleo do sistema de propriedades, adicionando funcionalidades práticas e visuais que conectam o backend (dados reais) ao mapa e à geração de certificados. Essa entrega fecha o ciclo de “gerenciamento de propriedades” e prepara o terreno para a Sprint 3 (roteirização e alertas em tempo real).
