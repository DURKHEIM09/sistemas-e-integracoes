# Sistemas e integrações do meu laboratório

Sou o Lucas. Este repositório reúne como organizo as ferramentas que dão suporte aos meus projetos pessoais de IA, automação e documentação.

O interesse aqui é mostrar o papel de cada sistema e como as partes se conectam. O código dos projetos próprios fica nos repositórios correspondentes; os sistemas de terceiros continuam com seus autores.

Minha referência para escolher a arquitetura é o uso real: custo, usabilidade e manutenção precisam fazer sentido. Gosto de experimentar estruturas complexas, mas no dia a dia uma integração simples pode resolver melhor.

## O que está documentado

- **Execução:** Linux, Docker e Docker Compose para hospedar os serviços.
- **Automação:** n8n para fluxos que precisam conectar etapas e sistemas.
- **Agentes:** Hermes como base do assistente; Durkh 509 como minha personalização.
- **Documentação:** Markdown e Obsidian para manter o contexto dos projetos.
- **Observabilidade:** Zabbix, Grafana e Netdata com funções complementares.
- **Navegação automatizada:** implantação documentada de Camofox Browser.

A lista descreve o uso registrado na minha documentação. O foco é a integração entre ferramentas e os projetos que construí a partir delas.

## Por onde começar

| Documento | O que você encontra |
| --- | --- |
| [Mapa dos sistemas](./docs/Mapa-dos-Sistemas.md) | Funções, relações e limites de cada ferramenta. |
| [Fluxos e integrações](./docs/Fluxos-dos-Sistemas-e-Integracoes.md) | Como automação, agentes, documentação e métricas se conectam. |
| [Roteiro de implementação](./docs/Roteiro-dos-Sistemas-e-Integracoes.md) | Uma sequência para montar uma integração pequena e ampliá-la. |
| [Estado e limites](./docs/Estado-e-Limites-dos-Sistemas.md) | O que foi registrado, o que depende de validação e o que não acompanha esta publicação. |

## Projetos relacionados

| Repositório | Relação |
| --- | --- |
| [Infraestrutura do laboratório](https://github.com/DURKHEIM09/infraestrutura-laboratorio) | Rede, acesso e ambiente que sustentam os sistemas. |
| [Hermes e Durkh 509](https://github.com/DURKHEIM09/hermes-durkh-509) | Minha experiência com o assistente e a coordenação de agentes. |
| [Neuro-Link e Obsidian](https://github.com/DURKHEIM09/neuro-link-obsidian) | Estrutura documental, metodologia e modelos públicos. |
| [Hermes Control](https://github.com/DURKHEIM09/hermes-control) | Painel próprio para reunir informações e ações; em desenvolvimento pausado. |
| [Factorio — Durkh Coop](https://github.com/DURKHEIM09/factorio-durkh-coop) | Exemplo de automação e IA integradas a um jogo. |

Esta é uma apresentação documental preparada em **19/11/2026**, a partir dos registros existentes. Não houve nova consulta aos serviços para afirmar disponibilidade atual.
