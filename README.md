# 🚀 Nelore — Consultoria em Transformação Digital

🔗 **Acesse o Aplicativo Online (GitHub Pages):** [Clique aqui para abrir o App](https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/)

## 👥 Especialistas Responsáveis (Autores)
- **Nome do Aluno(a) 1 Matheus Pereira
- **Unidade Curricular:** Exploração Digital e Fundamentos Tecnológicos (Objetos de Conhecimento 05 e 06)

---

## 🎯 1. O Problema Empresarial e Objetivo do Aplicativo
Pequenas e médias empresas sabem que precisam se modernizar, mas não sabem por onde começar. Os sintomas costumam ser os mesmos: um computador do escritório fazendo papel de servidor, backup manual em HD externo, planilhas soltas circulando pelo WhatsApp, vendas que não conversam com o financeiro, equipes perdendo horas com copiar e colar e senhas compartilhadas em post-it. O **Nelore** é um **Diagnóstico 360º de Maturidade Digital** (Opção B da ERS). Em cerca de 5 minutos, a empresa responde 12 perguntas distribuídas em 4 pilares. O app calcula o **Índice de Maturidade Digital (0 a 100%)**, classifica a empresa em um estágio (**Iniciante, Em Transição, Conectada ou Líder Digital**) e emite um **Laudo Técnico** com plano de boas práticas priorizado por urgência e prazo (0–30, 30–90 e 90–180 dias).

## 🏛 2. Os 4 Pilares de Boas Práticas Aplicados no Diagnóstico
- **☁ Infraestrutura e Migração para a Nuvem:** avalia onde rodam os sistemas, a rotina de backup e as práticas de continuidade. Recomenda a Regra de Backup 3-2-1 com cópia imutável, redundância de link (dual-WAN), monitoramento e FinOps. Um simulador indica o modelo de nuvem mais aderente (**SaaS, PaaS ou IaaS**) conforme porte, setor e legado, e gera um roteiro seguro de migração em 5 etapas.
- **🔄 Sistemas Empresariais (ERP/CRM) e Fluxo de Dados:** mede o grau de integração entre áreas, os indicadores de gestão e o percentual de retrabalho com dados. Recomenda a fonte única de verdade (Single Source of Truth), a integração CRM ↔ ERP via API/iPaaS e dashboards gerenciais, além de uma recomendação específica para cada setor (Varejo, Indústria, Saúde, Agronegócio etc.).
- **🤖 IA Generativa e Automação No-Code:** avalia o uso de IA e o nível de automação, e estima as **horas/mês liberáveis** com IA e No-Code. Recomenda pilotos controlados, biblioteca de prompts, automação do “top 3” de gargalos (Make, Zapier, Power Automate, n8n) e sempre **Human-in-the-Loop**.
- **🛡 Governança, Ética e Segurança Digital (LGPD):** verifica gestão de senhas, MFA, tratamento de dados de clientes em IAs e controles da LGPD (Encarregado, ROPA, plano de incidentes). Recomenda MFA em todas as contas, menor privilégio, política de uso ético de IA e anonimização, e cita a base legal (arts. 11, 14, 37 e 41 da LGPD; Resoluções CD/ANPD nº 2/2022 e nº 15/2024).

## 🛠 3. IAs Generativas e Ferramentas Utilizadas
| Ferramenta / IA | Como foi utilizada no projeto |
| :--- | :--- |
| **Claude (Anthropic) via Claude Code** | Estruturação das regras de negócio, pesos do diagnóstico, motor de recomendações e geração do código HTML/CSS/JS. |
| **TailwindCSS & Chart.js (CDN)** | Estilização executiva responsiva e geração dos gráficos dinâmicos (radar no painel e barras no laudo). |
| **Lucide Icons (CDN)** | Ícones da interface. |
| **GitHub & GitHub Pages** | Versionamento de código e publicação em nuvem estática (PaaS/CDN). |

## 🧠 4. Diário de Construção: Como Construímos e Refinamos o App
1. **Concepção e Engenharia de Prompt:** partimos do Prompt Mestre da ERS, escolhemos a Opção B (Diagnóstico 360º) e pedimos à IA que atuasse como engenheira de software sênior e consultora de transformação digital. Para dar profundidade técnica, incorporamos elementos das outras opções: o simulador SaaS/PaaS/IaaS (Opção A) e a calculadora de horas economizadas com automação (Opção C).
2. **Ajustes e Refinamentos Técnicos:** depois do primeiro teste, refinamos as recomendações para diferenciar quando usar SaaS, PaaS ou IaaS. Também adicionamos regras por setor e porte (critério SEBRAE), base legal da LGPD nas recomendações e priorização por urgência e prazo. Na parte técnica, corrigimos um conflito de nomes de classe CSS com o Tailwind e uma animação de contagem que podia exibir valores negativos, além de formatar o laudo para impressão em A4 (`window.print()`).
3. **Principal Aprendizado:** Com este projeto pude ter uma visão mais ampla e exemplificada através de inumeros recursos graficos que o site gera.

---

### ⚙️ Funcionalidades (checklist da ERS)
- **RF01:** identificação do cliente (nome, setor e nº de colaboradores, com porte calculado automaticamente).
- **RF02:** 12 controles interativos (8 de múltipla escolha, 2 sliders e 2 checklists), 3 por pilar.
- **RF03:** motor de score em JavaScript, recalculado a cada clique, sem recarregar a página.
- **RF04:** gráfico radar (empresa × meta de 80%) e gráfico de barras no laudo, com Chart.js.
- **RF05:** laudo com mais de 50 regras de boas práticas, personalizado por respostas, setor e porte.
- **RF06:** botão “Carregar Caso Exemplo”, que alterna entre 3 empresas fictícias, e botão “Imprimir / Exportar Laudo em PDF”.
- **RNF01–RNF04:** arquivo único `index.html`, layout responsivo, aviso Privacy by Design no rodapé e este README.
