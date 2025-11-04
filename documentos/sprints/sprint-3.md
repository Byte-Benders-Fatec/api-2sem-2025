# Sprint 3 — 03/11/2025 a 23/11/2025

**Meta da Sprint:**  
Implementar funcionalidades de **roteirização, alertas em tempo real (acidentes e clima)** e **modo offline**, para visualização das propriedades salvas.

---

## 🧩 Capacidade da equipe (estimativa)
- Capacidade estimada: **21 SP**

---

## 📋 Stories selecionadas (Sprint Backlog)

| ID | Rank | User Story | Estimativa (SP) |
|----|------|-------------|-----------------|
| 7  | Alta | Como usuário, quero gerar um certificado digital para comprovar a posse da minha propriedade. | 3 |
| 8  | Alta | Como usuário, quero traçar rotas até uma propriedade para chegar ao destino com praticidade. | 6 |
| 9  | Alta | Como usuário, quero receber alertas de acidentes na rota para ajustar meu trajeto. | 3 |
| 10 | Alta | Como usuário, quero visualizar alertas climáticos para planejar melhor minha viagem. | 3 |
| 11 | Baixa | Como usuário, quero acessar o aplicativo sem internet para consultar minhas propriedades salvas. | 6 |

**Total estimado:** **18 SP** (Sprint intensa, focada em integração de APIs externas e experiência do usuário)

---

## ✅ Critérios de Sucesso / Aceitação

**Story 8 — Roteirização até a propriedade**  
- Usuário seleciona uma propriedade e o app exibe a rota traçada até o destino.  
- Integração com API de rotas (Google Maps Directions API ou similar).  

**Story 9 — Alertas de acidentes na rota**  
- Notificações em tempo real quando há incidentes próximos à rota traçada.  
- Permitir replanejamento ou sugestão de rota alternativa.  

**Story 10 — Alertas climáticos**  
- Exibição de informações meteorológicas (chuva, tempestade, etc.) ao visualizar ou planejar rotas.  
- Alertas visuais e/ou sonoros conforme condição climática.  

**Story 11 — Acesso offline**  
- Usuário pode consultar propriedades e certificados mesmo sem conexão.  
- Dados essenciais armazenados localmente via cache (SQLite ou AsyncStorage).  

---

## 🧾 Definition of Done (DoD)

- Código submetido via **Pull Request** e revisado.  
- **Testes manuais e de integração** executados com sucesso.  
- **Documentação** de novas APIs, fluxos e limitações técnicas.  
- Aplicativo funcional no emulador Android, com demonstração de rotas e alertas.  
- Protótipo validado e apresentado na *Sprint Review*.  

---

## 🎯 Entregáveis / Demonstração

- **Data da Review:** 24/11/2025  
- **Demonstração esperada:**  
  - Traçar e visualizar rotas no mapa.  
  - Receber alertas em tempo real de acidentes e clima.  
  - Consultar propriedades sem internet.  
- **Artefatos:**  
  - Código atualizado no GitHub (branch principal)  
  - Vídeo ou APK de demonstração funcional  

---

📌 **Resumo da Sprint 3:**  
Esta sprint consolida a **fase avançada do projeto**, trazendo inteligência de rota, notificações em tempo real e suporte offline — recursos fundamentais para tornar o sistema completo e aplicável em cenários reais. A equipe focará em **melhorar a experiência do usuário** e garantir **resiliência do sistema**, conectando o uso prático do mapa com funcionalidades úteis no dia a dia.
