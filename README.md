# QA Web - Renner

![Status](https://img.shields.io/badge/status-em%20andamento-yellow)
![Tipo](https://img.shields.io/badge/tipo-teste%20manual-blue)
![Escopo](https://img.shields.io/badge/escopo-educacional-lightgrey)

## 📌 Sobre o projeto

Este repositório reúne a documentação de testes manuais realizados no site da **Renner**, com foco na validação das principais funcionalidades do e-commerce sob a perspectiva de Qualidade de Software (QA).

O objetivo é demonstrar habilidades em planejamento, elaboração de casos de teste, execução de testes, documentação de evidências e reporte de bugs, utilizando boas práticas da área de Quality Assurance — simulando o dia a dia de um(a) QA júnior atuando em um time de e-commerce.

> **Observação:** Este projeto possui caráter exclusivamente educacional e de portfólio.

---

## 🎯 Objetivo

Realizar testes funcionais manuais nas principais funcionalidades do e-commerce da Renner, documentando:

- Plano de testes
- Casos de teste 
- Evidências de execução
- Bugs encontrados (quando aplicável), com severidade e prioridade classificadas

Este projeto busca refletir um processo de QA real: planejar antes de testar, documentar de forma rastreável, e comunicar problemas de forma clara e acionável para um time de desenvolvimento.

---

## 📋 Escopo

As funcionalidades avaliadas incluem:

- Cadastro e Login
- Busca de produtos
- Filtros e ordenação
- Página de produto
- Carrinho de compras
- Simulação de frete (CEP)
- Fluxo de checkout (sem conclusão da compra)

### Fora do escopo

Este projeto **não contempla**:

- Finalização de compras reais
- Processamento de pagamentos
- Testes de carga ou performance
- Testes de segurança (Pentest)
- Automação de testes
- APIs ou sistemas internos da Renner

> A decisão de manter o projeto 100% manual (sem automação ou testes de carga) é intencional: o site é um ambiente de produção real de terceiros, e testes automatizados/carga exigiriam autorização explícita da empresa, o que está fora do escopo de um projeto de portfólio.

---

## 📊 Progresso dos Módulos Testados

| Módulo | Casos de Teste | Status | Bugs Encontrados |
|---|:---:|:---:|:---:|
| Cadastro e Login | 0 | 🔲 Não iniciado | - |
| Busca de Produtos | 0 | 🔲 Não iniciado | - |
| Filtros e Ordenação | 0 | 🔲 Não iniciado | - |
| Página de Produto | 0 | 🔲 Não iniciado | - |
| Carrinho de Compras | 0 | 🔲 Não iniciado | - |
| Simulação de Frete (CEP) | 0 | 🔲 Não iniciado | - |
| Checkout (até pagamento) | 0 | 🔲 Não iniciado | - |

**Legenda:** 🔲 Não iniciado · 🟡 Em andamento · ✅ Concluído · ⚠️ Concluído com bugs

> Esta tabela é atualizada conforme a execução avança. Cada módulo concluído deve linkar para seu arquivo de casos de teste correspondente em `/test-cases`.

---

## 🖥️ Ambiente de Testes

| Item                | Detalhes                |
| ------------------- | ------------------------ |
| Sistema Operacional | Windows 11               |
| Navegador Principal | Google Chrome (última versão estável) |
| Navegador Secundário| Mozilla Firefox (testes pontuais) |
| Tipo de Teste       | Testes Manuais Funcionais e Exploratórios |
| Ambiente            | Produção (Site Público — www.renner.com.br) |
| Resoluções testadas | Desktop (1920x1080) e Mobile (simulado via DevTools) |

---

## 🛠️ Ferramentas Utilizadas

| Ferramenta | Finalidade |
|---|---|
| Markdown | Documentação de casos de teste e bugs |
| Git & GitHub | Versionamento e portfólio público |
| Google Chrome + DevTools | Execução dos testes e inspeção de elementos/console |
| Ferramenta de captura de tela | Evidências visuais dos testes e bugs |

---

## 🔍 Metodologia

1. **Planejamento** — definição de escopo, riscos e critérios em `test-plan.md`
2. **Elaboração dos casos de teste** — cenários escritos em Gherkin, cobrindo caminho feliz, caminhos alternativos e casos de borda
3. **Execução manual** — navegação real no site, seguindo os cenários definidos
4. **Registro de evidências** — prints das telas relevantes, salvos em `/evidencias`
5. **Reporte de bugs** — sempre que um cenário falha, é gerado um relatório padronizado em `/bug-reports`, com severidade e prioridade
6. **Atualização de progresso** — a tabela de progresso é atualizada a cada módulo concluído

---

## 📂 Estrutura do Repositório

```text
qa-web-renner/
│
├── README.md
│
├── bug-reports/
│   └── bug.md
│
├── documentacao/
│   ├── Plano_de_Testes.md
│   ├── Resultado_dos_Testes.md
│   └── Cenarios_e_Casos_de_Teste/
│       ├── cadastro-login.md
│       ├── busca-e-filtros.md
│       ├── pagina-produto.md
│       ├── carrinho.md
│       ├── frete-e-cep.md
│       └── checkout.md
│
└── metricas/
```

---

## 🚦 Critérios de Severidade e Prioridade

| Severidade | Critério |
|---|---|
| **S1 — Crítico** | Bloqueia fluxo principal (ex: impossível adicionar item ao carrinho) |
| **S2 — Alto** | Funcionalidade não funciona como esperado, mas há workaround |
| **S3 — Médio** | Comportamento inconsistente, sem bloquear o uso |
| **S4 — Baixo** | Problema visual/cosmético, sem impacto funcional |

| Prioridade | Significado |
|---|---|
| **P0 — Urgente** | Bug crítico e reproduzível, com alto impacto |
| **P1 — Alta** | Impacta usuários de forma relevante |
| **P2 — Média** | Importante, mas pode esperar |
| **P3 — Baixa** | Backlog, sem prazo definido |

---

## 🧭 Como Navegar Neste Repositório

- Comece pelo [`documentacao/test-plan.md`](./test-plan.md) para entender escopo e estratégia
- Veja os casos de teste em [`documentacao/Cenarios_e_Casos_de_Teste/`](./test-cases), organizados por funcionalidade
- Bugs encontrados durante a execução ficam documentados em `bug-reports/`, seguindo o template padrão
- Evidências (prints) referenciadas nos casos de teste e bugs ficam em `evidencias/`

---

## ⚖️ Disclaimer

Este projeto foi desenvolvido **exclusivamente para fins educacionais e de demonstração de habilidades em QA**.

Todos os testes foram realizados utilizando apenas funcionalidades públicas do site, sem exploração de vulnerabilidades, sem utilização de dados sensíveis e sem qualquer tentativa de comprometer a disponibilidade ou a segurança da aplicação.

Nenhuma compra foi concluída, nenhuma transação financeira foi realizada e nenhum dado pessoal de terceiros foi utilizado durante a execução dos testes.

A marca **Renner** pertence aos seus respectivos proprietários. Este repositório não possui qualquer vínculo oficial com a empresa.

---

## 👨‍💻 Autor

**Miguel Luis**
Quality Assurance (QA) Júnior

- Testes Manuais
- Testes de API (Postman, Newman)
- Documentação de Testes
- Reporte de Bugs
- Planejamento de Testes
- ISTQB CTFL Certified

📎 LinkedIn: [linkedin.com/in/miguel-luisatf](https://www.linkedin.com/in/miguel-luisatf/)
