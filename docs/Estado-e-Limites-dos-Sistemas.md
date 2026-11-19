# Estado e limites dos sistemas

[Voltar à apresentação](../README.md) · [Roteiro de referência](./Roteiro-dos-Sistemas-e-Integracoes.md)

## Base desta publicação

Preparação editorial em **19/11/2026**, usando as fichas dos sistemas e os registros de implantação existentes. Nenhum serviço foi consultado ou reiniciado para preparar este repositório.

| Conjunto | O que os documentos sustentam | Limite da afirmação |
| --- | --- | --- |
| Linux, Docker e Hermes | Organização dos componentes nos seus caminhos nativos e relações com os projetos. | Não é uma auditoria atual de versões, saúde ou permissões. |
| n8n | Implantação em Compose e histórico de atualização de outubro de 2026. | O histórico não comprova disponibilidade hoje nem execução de todos os fluxos. |
| Zabbix e Grafana | Implantação integrada e manutenção registrada em 18/10/2026, com verificações históricas de saúde. | A publicação não repetiu os testes nem exportou a stack privada. |
| Netdata | Serviço nativo complementar de monitoramento. | Não foi demonstrada uma integração de datasource com Grafana. |
| Camofox | Implantação em contêiner e testes históricos de navegação em 18/10/2026. | A versão da árvore de código e a da imagem executada eram diferentes; a presença de um recurso upstream não comprova uso local. |
| Obsidian | Interface sobre os originais e atualização de metadados documentada em novembro de 2026. | O registro de 19/11 informa recuperação do cadastro com lentidão de leitura remanescente. A integração depende de rede e servidor disponíveis. |

Datas e resultados históricos são preservados para explicar a evolução. Uma alteração de versão, rede ou aplicação exige validação no ambiente afetado.

## O que acompanha o repositório

- Visão das ferramentas e de suas responsabilidades.
- Diagramas das relações documentadas.
- Roteiro de referência para uma integração pequena.
- Links para os projetos com código e exemplos públicos.

## O que permanece fora

Credenciais, sessões, arquivos de ambiente, endereços e identificadores reais, bases persistentes, configurações operacionais completas e documentos particulares.

Este pacote também não inclui o código do plugin de atualização do Obsidian nem o mecanismo privado de recuperação de conhecimento. O repositório [Neuro-Link e Obsidian](https://github.com/DURKHEIM09/neuro-link-obsidian) publica metodologia e modelos.

## Autoria e escopo

As ferramentas de terceiros preservam seus autores e licenças. Este repositório apresenta minha organização e experiência de integração em projetos pessoais.

O roteiro é uma síntese explicativa. Ele não substitui as instruções oficiais de cada software e não promete reproduzir toda a instalação pessoal com um comando.
