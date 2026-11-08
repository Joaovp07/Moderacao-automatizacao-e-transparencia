# PIST — Plataforma Integrada de Solicitações e Transparência: automação auditável de pedidos administrativos municipais com acompanhamento cidadão


## Integrantes

* Bruno Rodrigues | dev-rodrigues-bruno | Gestão | 48101541  
* Caio Dal Pizzol Fonseca | caio-fonseca | Cibersegurança e Gestão | 47923121
* Denner de Paula Coutinho | denner-coutinho | Engenharia de Dados e Gestão | 48094030
* João Vitor Pires Ribeiro | Joaovp07 | Ciência de Dados e Gestão | 47792591
* Nicollas Guedes Da Silva Santos | Nicollas-Guedes | Engenharia de Dados e Cloud | 48131334

**Dossiê:** 5 - Moderação automatizada e transparência 

**Recorte:** digitalização e automação, por regras auditáveis e com decisão final sempre humana, das solicitações administrativas de uma prefeitura, permitindo ao cidadão abrir e acompanhar o pedido online e à população consultar indicadores agregados de desempenho em um painel público. A implantação começa por um piloto em um único serviço municipal.

---

## 1. Análise do Problema

### 1.1 Quem é afetado, onde e quanto
- **Volume e dados estatísticos:** 84% dos brasileiros (156 milhões) acessam a internet, mas 18,6 milhões de Pessoas com Deficiência (8,9% da população acima de 2 anos) encontram barreiras severas: apenas 2,8% dos sites brasileiros e 10% dos portais públicos são plenamente acessíveis.
- **Danos da moderação enviesada:** Casos análogos demonstrados na literatura (como o caso HireVue/Intuit com transcrição automática inadequada para candidatos surdos, ou vieses raciais/de gênero observados em modelos generativos que preferem nomes brancos em 85% dos casos).

### 1.2 Causas Tecnológicas
1. **Modelos de Caixa-Preta (*Black Box*):** Falta de explicabilidade (XAI) na tomada de decisão sobre remoções ou restrições de alcance.
2. **Dados Históricos Enviesados:** Treinamento em dados sem tratamento (*re-weighting*), que perpetua exclusões históricas e dialetais.
3. **Ausência de Acessibilidade Nativa:** Falta de conformidade com os princípios POUR da WCAG desde a etapa de requisitos.

### 1.3 O que já existe e por que não basta
- Classificadores nativos sob segredo industrial e relatórios genéricos de transparência que não cumprem o devido processo digital exigido por normas globais (como o EU AI Act e a NYC Local Law 144).

---

## 2. Proposta Tecnológica

### 2.1 A solução do ponto de vista do usuário
- Painel transparente de notificação com justificativa clara (XAI), leitor de tela integrado, transcrição acessível e canal direto para recurso humano.

### 2.2 Arquitetura e Ciclo de Vida do Software
- Mapeamento das etapas de requisitos, coleta, modelagem, testes e implantação, garantindo *Fairness-aware Learning*, auditoria de subgrupos e testes com leitor de tela.

### 2.3 O trabalho de cada área
- **Engenharia de Software:** Arquitetura semântica, suporte a teclado/leitores de tela (WCAG Nível AA) e integração de XAI.
- **Análise de Dados:** Limpeza de datasets, auditoria de amostras (*re-weighting*) e monitoramento contínuo de métricas por subgrupo.

### 2.4 O que a tecnologia não resolve
- Decisão final em casos ambíguos, validação ética e julgamento contextual, que permanecem sob supervisão humana direta.

---

## 3. Análise Ética e Regulatória

### 3.1 Matriz de Riscos (Mínimo 5)
- Análise de riscos de viés, opacidade, falhas de acessibilidade, vazamento de dados e falta de revisão humana.

### 3.2 Decisão e Justificativa
- **Decisão:** Implantar com controles.
- **Justificativa:** (Até 10 linhas, com base nos princípios do Código de Ética da ACM e Recomendação da UNESCO).

### 3.3 Controles antes de entrar em produção
- Abrangendo os 6 eixos: transparência, revisão humana, minimização de dados, segurança, teste de viés e canal de contestação.

### 3.4 LGPD
- Tratamento de dados sob a base legal do legítimo interesse ou cumprimento de obrigação legal, observando a minimização e direitos dos titulares.

### 3.5 Comunicado Público
- Texto conciso (até 600 caracteres) destacando compromisso ético e governança.

---

## 4. Acessibilidade e Inclusão Digital

### 4.1 Quem pode ficar de fora
- Pessoas cegas ou com baixa visão, surdas, com deficiência motora, cognitiva ou de fala.

### 4.2 Requisitos Concretos de Acessibilidade
- **Visual:** *Alt text* em mídias, contraste mínimo de 4,5:1 (WCAG Nível AA), suporte a leitor de tela (NVDA/TalkBack).
- **Auditiva:** Legendas e transcrições em vídeo/áudio.
- **Motora:** Navegação 100% funcional por teclado (tecla Tab/Enter), sem necessidade de precisão de mouse.
- **Cognitiva e Fala:** Linguagem simples, padrões previsíveis e comandos alternativos ao toque/voz.
- **Enquadramento Legal:** Conformidade rigorosa com a LBI (Lei 13.146/2015, Art. 63) e eMAG.

---

## 5. Sustentabilidade

### 5.1 Impacto ambiental da solução (TI Verde)
- Emprego de modelos compactos (*SLMs*), filtragem em camadas e servidores em data centers renováveis.

### 5.2 Sustentabilidade do projeto
- Manutenção por equipe multidisciplinar, suporte à saúde mental dos moderadores humanos e governança aberta.

---

## 6. Impacto Esperado, 7. Quadro de Decisões, 8. Capítulos Individuais e 9. Referências
- Inclusão das referências
