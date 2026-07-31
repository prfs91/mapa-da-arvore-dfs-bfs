# Análise de Percursos em Árvores (DFS & BFS) 🌳🔍

[![Language: EN](https://img.shields.io/badge/Language-EN-lightgrey?style=flat-square&logo=gengo&logoColor=white)](README.md) [![Language: PT-PT](https://img.shields.io/badge/Language-PT--PT-lightgrey?style=flat-square&logo=gengo&logoColor=white)](README.pt-pt.md)

[![Python](https://img.shields.io/badge/Python-3.10--3.11-blue?style=for-the-badge&logo=python&logoColor=white)](https://python.org) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge&logo=mit&logoColor=white)](https://opensource.org)

Uma implementação educacional e técnica de algoritmos de percurso em grafos aplicados a estruturas de árvores. Este projeto analisa e visualiza as diferenças comportamentais e estruturais entre a **Busca em Profundidade (DFS)** e a **Busca em Largura (BFS)** utilizando módulos customizados em Python e ambientes interativos do Jupyter Notebook.

*Nota: Este projeto foi originalmente desenvolvido como um ativo de laboratório colaborativo para a **disciplina optativa de Mineração de Dados**, integrante da matriz curricular do curso de **Bacharelado em Engenharia de Computação** da **Universidade Federal do Pará (UFPA) - Campus Tucuruí** (Período Letivo: 23/03 a 23/07 de 2026). Embora as restrições de avaliação institucional exigissem que a estrutura original do repositório e o código-fonte principal permanecessem inalterados em português (Brasil) durante o semestre letivo ativo, este repositório está passando atualmente por um ciclo ativo e independente de modernização pós-curricular para transicionar a documentação, recursos e futuras atualizações de código para o inglês, visando implantação internacional e visibilidade de portfólio.*

## 🎯 Objetivos Principais
- **Modelagem de Dados:** Implementar estruturas abstratas de árvores utilizando listas de adjacência.
- **Análise Algorítmica:** Avaliar a eficiência, comportamento de caminhos e mecânicas de memória do DFS versus BFS.
- **Visualização de Dados:** Utilizar redes de grafos para gerar e exportar caminhos visuais dinâmicos passo a passo das execuções de busca.

## 🏗️ Destaques Técnicos e Engenharia Aplicada
A implementação demonstra fundamentos sólidos em engenharia de software e lógica computacional, destacando práticas profissionais aplicáveis a pipelines de dados do mundo real:
- **Arquitetura Desacoplada:** Separação clara de responsabilidades entre o motor de processamento lógico core (`algoritmos_de_busca.py`) e o ambiente de testes interativo (`analise_comparativa_dfs_bfs.ipynb`).
- **Provisionamento Automatizado de Ambiente:** Bloco de proteção em tempo de execução utilizando tratamento de exceções nativo do Python (`try/except`) para gerenciar automaticamente a instalação de pacotes (`networkx` e `matplotlib`) em novos ambientes.
- **Otimização de Complexidade de Tempo:** Utilização de estruturas de dados especializadas (`collections.deque`) garantindo custo computacional estável de O(1) durante as mutações de índice na fila do BFS, evitando operações custosas em arrays comuns.
- **Portabilidade de Host Cross-Platform:** Abstrações dinâmicas de roteamento de arquivos do sistema operacional (`os.path.abspath`), evitando caminhos estáticos para garantir execução fluida em ambientes heterogêneos (Unix/Windows).
- **Pipelines de Dados de Alta Resolução:** Motor de extração automatizada de logs analíticos gerando visualizações de alta fidelidade (exportações em 300 DPI estilizadas com métricas customizadas de alinhamento `monospace`).
- **Padrão de Ponto de Entrada de Produção:** Implementação estruturada do paradigma `if __name__ == "__main__"`, protegendo namespaces globais e permitindo testes unitários locais isolados sem efeitos colaterais na importação do módulo.

## 📊 Conceitos Core Implementados

### 1. Busca em Profundidade (DFS)
* **Estratégia:** Exploração Vertical Exaustiva.
* **Comportamento:** Prioriza descer até os nós folha (o ponto mais profundo de um ramo) antes de invocar blocos de *backtracking* na pilha de memória para explorar caminhos adjacentes.
* **Contexto Técnico:** Implementado de forma recursiva com estados base explícitos (`if visitados is None`) para demonstrar propagação de chamadas de pilha e rastreamento de estado. Complexidade de Tempo: \(\mathcal{O}(V + E)\).

### 2. Busca em Largura (BFS)
* **Estratégia:** Exploração Horizontal por Camadas.
* **Comportamento:** Explora todos os nós camada por camada (nível por nível) antes de descer na hierarquia da árvore.
* **Contexto Técnico:** Implementado utilizando mecânicas de fila de alta performance (`popleft()`), servindo como benchmark computacional para encontrar o caminho mais curto em termos de níveis da árvore. Complexidade de Tempo: \(\mathcal{O}(V + E)\).

## 📸 Visualização Técnica

O framework mapeia dinamicamente topologias estruturais e exporta automaticamente os resultados das análises dos caminhos de busca em gráficos de rede visuais:

![Modelled Tree Graph Map](output/figures/mapa_da_arvore_modelada.png)

*O motor verifica automaticamente os ambientes, gerencia camadas visuais dinâmicas condicionais (#e74c3c para alvos ativos, #2ecc71 para caminhos bem-sucedidos e #3498db para topologias inativas) e exporta logs como configurações de mapeamento vetorial bruto.*

## 📂 Arquitetura do Projeto

```text
├── output/figures/              # Gráficos de alta resolução e saídas visuais automáticas
├── .gitignore                   # Exclusões de arquivos otimizadas para ambientes Python
├── LICENSE                      # Licença Open Source MIT
├── README.md                    # Documentação Principal (Inglês)
├── README.pt-br.md              # Documentação Localizada (Português - Brasil)
├── README.pt-pt.md              # Documentação Localizada (Português - Portugal)
├── algoritmos_de_busca.py       # Motores lógicos desacoplados e wrappers de mapeamento visual
└── analise_comparativa_dfs_bfs.ipynb  # Ambiente de testes interativo e executor de pipelines
```

## 🛠️ Stack Tecnológica e Dependências
- **Core:** Python 3 (Conceitos de POO, convenções de nomenclatura snake_case aderentes ao guia de estilo PEP 8 e lógica condicional ternária aninhada para renderização de gráficos inline).
- **Arquitetura de Redes:** `NetworkX` (para construção lógica de grafos direcionados, parsing de nós e gerenciamento de layouts topológicos).
- **Motor de Visualização de Dados:** `Matplotlib` (para rastreamento de subplots multipainel utilizando padrões de loop concorrentes com `zip()`, renderização gráfica e blocos de exportação de interface).

## 🚀 Como Executar Localmente

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/prfs91/mapa-da-arvore-dfs-bfs.git
   cd mapa-da-arvore-dfs-bfs
   ```

2. **Execute a Análise Interativa:**
   Certifique-se de ter o Jupyter instalado (ou utilize o VS Code / Google Colab) e execute o notebook `analise_comparativa_dfs_bfs.ipynb`. O pipeline gerenciará nativamente a verificação e instalação automática das dependências (`networkx` e `matplotlib`), caso seja necessário.

## 👩‍💻 Autoria e Contexto Acadêmico
Desenvolvido cooperativamente pelo **Grupo 03** para a disciplina optativa de Mineração de Dados (UFPA):
- **Pamella Roberta** - [@prfs91](https://github.com/prfs91)
- Manuela Ferreira
- Rafaela Pinto
- Gabriel Batista

Professor Orientador: **Dr. Iago Medeiros**

---
*Buscando ativamente oportunidades remotas em desenvolvimento de software, projetos sob demanda (freelance) ou estágios. Conecte-se comigo no [LinkedIn](https://www.linkedin.com/in/robertaferreira91/).*
