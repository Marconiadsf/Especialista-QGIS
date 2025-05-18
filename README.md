<img src=/capa2.jpeg alt="Imagem de capa" width="600px" height="200px">

## 🚀 Especialista-QGIS: GIS Inteligente para Todos

**Missão:** Democratizar o poder do Geoprocessamento (GIS) para profissionais que trabalham com dados espaciais, com foco em agentes públicos, geólogos, engenheiros e especialistas em gestão de riscos urbanos.

**Contexto:** Projeto desenvolvido para o Desafio Alura: Imersão IA.

---

## 🧠 Agentes Inteligentes QGIS via Interface Conversacional

**Objetivo Principal:** Desenvolver um sistema de **agentes inteligentes especializados** que integram o QGIS a uma **interface de linguagem natural**, permitindo que usuários sem conhecimento em programação realizem tarefas espaciais através de conversas intuitivas com um assistente virtual.

**Arquitetura:** Monolítica, baseada em **Google AI Studio**, **Google Colab** e **Python**. Planejamento futuro para integração como **plugin nativo no QGIS**.

---

## 🌍 GIS para Salvar Vidas: Tecnologia a Serviço da Segurança Urbana

Acreditamos que o acesso facilitado a ferramentas de geoprocessamento pode ser crucial na proteção de vidas e na construção de cidades mais resilientes.

**A Urgência:** Tragédias causadas por eventos climáticos extremos demandam respostas rápidas e precisas. A informação geográfica oportuna pode ser a chave para mitigar riscos e otimizar ações de resposta.

**Nossa Solução:** O Especialista-QGIS visa democratizar o GIS, oferecendo aos profissionais a capacidade de gerar mapas temáticos e relatórios de forma ágil, precisa e econômica, sem a dependência de softwares proprietários.

**Imagine:**

* **Mapas de risco em tempo real:** Identificação dinâmica de áreas vulneráveis a deslizamentos e enchentes.
* **Otimização de rotas de emergência:** Planejamento eficiente para resgates e evacuações.
* **Comunicação clara de riscos:** Ferramentas visuais para informar a população de forma eficaz.

**Benefícios:**

* **Agilidade na produção:** Criação rápida de mapas e relatórios essenciais.
* **Redução de custos:** Eliminação da necessidade de licenças de software onerosas.
* **Potencial para salvar vidas:** Respostas mais rápidas e eficientes em situações de risco urbano (enchentes, deslizamentos, acidentes).
* **Empoderamento profissional:** Autonomia, produtividade e precisão para diversas áreas (gestão de riscos, mineração, logística, urbanismo, etc.).

---

Com este projeto, buscamos transformar a maneira como profissionais interagem com dados espaciais, colocando o poder do GIS nas mãos de quem realmente faz a diferença.
---

## ⚙️ Funcionamento Geral do Sistema

O sistema é composto por seis agentes cooperativos, cada um responsável por uma parte essencial do fluxo de trabalho:

### 🗣️ 1. **Agente Intérprete (Planejador Conversacional)**

* Recebe a solicitação em linguagem natural.
* Interpreta termos técnicos ou leigos.
* Gera um **plano de ação estruturado** e apresenta para validação do usuário.

### 📋 2. **Agente de Requisitos (Contextualizador)**

* Analisa o plano.
* Identifica informações faltantes.
* Realiza diagnósticos (plugins instalados, arquivos existentes etc.).
* Envia as informações ao próximo agente.

### 💻 3. **Agente Programador (Gerador de Código)**

* Gera código Python compatível com o QGIS.
* Adiciona verificações de ambiente e comentários.
* Prepara o código para ser validado.

### ✅ 4. **Agente de Qualidade (QA)**

* Revisa o código gerado.
* Verifica segurança, boas práticas e erros lógicos.
* Sugere correções ou tenta corrigi-las automaticamente.
* Informa o usuário se há riscos em seguir com o código como está.

### ⚠️ 5. **Agente Executor (em desenvolvimento)**

* **Este agente ainda não foi implementado**, pois o front-end no QGIS não ficou pronto a tempo para o desafio.
* A função de execução, temporariamente, é assumida diretamente pelo usuário ou repassada ao próximo agente.

### 🔁 6. **Agente Corretor (Reparador)**

* Recebe logs de erros ou mensagens de falha.
* Analisa a causa do problema.
* Tenta gerar uma nova versão corrigida do código.
* Reenvia para o QA e mantém histórico de tentativas.

---

## 🔁 Fluxo de Operação dos Agentes

<a href=/fluxograma.png>
  <img src=/fluxograma.png alt="Fluxograma do sistema de agentes - Clique para ampliar" height="300" >
</a>



---


## 🚀 Como Começar

Explore e experimente o Especialista-QGIS de forma rápida e fácil:

* **🔗 Testar no Google Colab:** [Abrir o Notebook no Google Colab](coloque_o_link_real_aqui) - Execute e modifique o código diretamente no seu navegador.
* **📁 Documentação:** Consulte a documentação detalhada no [Repositório](coloque_o_link_do_repositorio_aqui) para entender a fundo o projeto.
* **🧠 Código Principal:** Mergulhe no coração do sistema e explore o código fonte.

---

## 💡 Casos de Uso

O projeto tem aplicação direta em:

* **Órgãos públicos** e prefeituras que utilizam QGIS na análise de risco urbano.
* **Profissionais técnicos** que desejam automatizar tarefas repetitivas com linguagem natural.
* **Mapeamento de áreas de risco, impacto ambiental, acessibilidade urbana e saneamento.**

---

## 🚧 Estado Atual

* ✔️ Agentes Intérprete, Requisitos, Programador, QA concluídos.
* ⏳ Agente Executor em desenvolvimento (aguardando front-end no QGIS).
* 🚧 Agente reparador: Precisa de reparos (o.O)
* 🛠️ Projeto funcional via Google Colab, com geração de código pronta para testes manuais no QGIS.

---

## 📌 Próximos Passos

* Desenvolver o plugin frontend no QGIS.
* Integrar todos os agentes em um pipeline automático.
* Melhorar o controle de contexto e refinamento iterativo com logs de feedback real.
* Corrigir o codigo do agente reparador
* Melhorar a função call_agent, e estabelecer um padrao de input/output dos agentes
* Refinar a interação entre os agentes para atender o fluxograma ideal.
* Criar/Conectar ferramentas "tools" ausentes como Google Maps, Conversão de Unidades, APIs de Dados Geográficos, etc
* Criar um sistema mais eficaz de controle de versao dos codigos reparados pelo Agente Reparador (quando funcionar) e controle de sessao/memória dos agentes.
* Estabelecer como o agente executor deve se somunicar com o computador cliente durante a execucao (debug)
* Não foi possível usar outros modelos (erros, não disponíveis ou sem créditos/uso livre) nos agentes de código. Futuramente tentar outros... 

---
## 🧠 Tecnologias Utilizadas

O Especialista-QGIS é construído com as seguintes tecnologias:

* 🐍 **Python:** A linguagem de programação principal para a lógica e os agentes inteligentes.
* ☁️ **Google Colab:** Plataforma para desenvolvimento e execução do projeto na nuvem.
* 🤖 **Google AI Studio (ADK):** Ferramentas para a criação e interação com modelos de linguagem.
* 🗺️ **QGIS:** Software de Sistema de Informação Geográfica para a integração e aplicação das funcionalidades.
* ✨ Código gerado com o auxílio do Gemini: [https://gemini.google.com/share/159a7bcbd25e](https://gemini.google.com/share/159a7bcbd25e)

---

## 📜 Licença

Este projeto é distribuído sob a **MIT License**. Consulte o arquivo `LICENSE` no repositório para obter mais informações sobre os termos e condições de uso.

---

## ✉️ Contato

* **Desenvolvedor:** Marconiadsf
* **Discord:** marconi2744
* **LinkedIn:** [https://www.linkedin.com/in/engenheirodeminas/](https://www.linkedin.com/in/engenheirodeminas/)

🐍 Participante do **Desafio Alura 2025**
