# 📋 Processo de Revisão de Código

**Projeto:** Genius Finance – Equipe 2  
**Objetivo:** Formalizar critérios, responsabilidades e boas práticas para revisões de código durante o desenvolvimento.

---

## 👥 1. Quem revisa?

- Cada *Pull Request* (PR) deve ser revisado por **pelo menos 1 pessoa**.
- O revisor ideal é alguém **familiarizado com a parte do sistema afetada**.
- Revisores adicionais podem ser envolvidos conforme a **complexidade da mudança**.

---

## 🔄 2. Como escolher o revisor?

- Adotamos um **sistema de rodízio com prioridade por familiaridade**:
  - A cada sprint, é definida uma **lista rotativa** de revisores.
  - Quem tiver mais domínio sobre o código alterado será priorizado.

---

## ✅ 3. Critérios de Avaliação

### 🧾 Legibilidade
- Nomes de variáveis e funções **descritivos**.
- **Funções pequenas**, com responsabilidades bem definidas.
- Comentários apenas **quando necessários**.
- Formatação **consistente** (ex: uso de ESLint, Prettier).

### 🧱 Boas Práticas
- Uso adequado de **camadas** (Controller, Service, Repository).
- Evitar **duplicação de código** (DRY).
- Aplicação dos princípios **SOLID**.
- Respeito à **arquitetura proposta**.

### 🧪 Testes
- Presença de **testes unitários** e/ou **de integração**.
- Verificar **cobertura e clareza** dos testes.
- Testes **automatizados e reprodutíveis**.
- Inclusão de **casos de falha e borda**.

### 🔐 Segurança
- Validação e sanitização de **dados de entrada**.
- Tratamento adequado de **exceções e erros**.
- Proteção contra **SQL Injection**, **XSS**, etc.
- Evitar exposição de **informações sensíveis**.

### ⚙️ Performance
- Evitar **laços desnecessários** ou **cálculos repetitivos**.
- Uso de **estruturas de dados apropriadas**.
- Redução de **chamadas redundantes** a APIs ou bancos de dados.
- Garantia de **desempenho adequado** da aplicação.

---

## 💬 4. Padrão de Comentários

- **Prefira perguntas construtivas**:
  - Ex: “Você considerou usar X?” ou “O que acha de aplicar Y aqui?”
- **Evite julgamentos** e mantenha um tom respeitoso.
- **Valorize pontos positivos** sempre que possível.
- Trate a revisão como **colaboração, não correção**.
- Emojis podem ser usados **com equilíbrio**.

---

## ✅ 5. Aprovação de Pull Request

Um PR será aprovado quando:

- Todos os **critérios de revisão** forem verificados.
- Feedbacks forem **resolvidos ou justificadamente recusados**.
- O PR **passar nos testes automatizados** com cobertura adequada.

---

Este documento orienta as revisões até o fim do projeto. Alterações futuras devem ser feitas com consenso do time.