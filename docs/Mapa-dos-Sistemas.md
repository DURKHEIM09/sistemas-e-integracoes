# Mapa dos sistemas

[Voltar à apresentação](../README.md) · [Ver os fluxos](./Fluxos-dos-Sistemas-e-Integracoes.md)

## Função antes da ferramenta

| Sistema | Papel no ambiente documentado | Relação demonstrada nos registros |
| --- | --- | --- |
| Linux | Sistema operacional do servidor e gestão dos serviços nativos. | Mantém Docker, acesso SSH e serviços de monitoramento. |
| Docker / Compose | Execução e organização de aplicações em contêineres. | Há implantações documentadas de n8n, Zabbix e Camofox; Grafana compartilha a implantação de monitoramento. |
| n8n | Automação de fluxos entre ferramentas. | É usado em integrações específicas, como relatórios do Factorio e transporte de demandas entre agentes. |
| Hermes Agent | Runtime de terceiros para execução do assistente e suas ferramentas. | A personalização Durkh 509 é documentada separadamente da instalação do software. |
| Obsidian | Interface Windows para editar e navegar nos documentos Markdown originais. | Acesso por compartilhamento de arquivos; um componente próprio de atualização acompanha metadados por SSH. |
| Zabbix | Monitoramento por uma stack em Compose e agente nativo do host. | Há integração de apresentação em uma Discord Activity e registros de manutenção. |
| Grafana | Visualização de métricas e dashboards. | O backend Zabbix é a fonte de métricas documentada; o serviço compartilha a implantação com ele. |
| Netdata | Monitoramento adicional como serviço nativo. | Complementa Zabbix/Grafana; não foi demonstrado um datasource Netdata → Grafana. |
| Camofox Browser | Navegação automatizada para agentes. | Há um registro de implantação em contêiner com testes de navegação e snapshot. A existência de plugins upstream não comprova ativação local. |

**Docker não hospeda todos os componentes.** O Hermes mantém seu runtime nativo; Obsidian é um aplicativo no Windows; Netdata e o agente de monitoramento são serviços nativos.

## Sistemas de terceiros e projetos próprios

As aplicações acima são usadas ou integradas. Minha implementação está na organização do ambiente, nos fluxos, na documentação e nos componentes próprios dos projetos.

Para entender a identidade do assistente, veja [Hermes/Durkh 509](https://github.com/DURKHEIM09/hermes-durkh-509). Para o painel, veja [Hermes Control](https://github.com/DURKHEIM09/hermes-control). O catálogo aqui explica a relação, sem copiar código ou instruções desses repositórios.

## Acesso humano

O Discord se tornou a interface principal de interação com o assistente. Algumas aplicações também têm apresentação integrada por Activities. Isso não transforma o Discord em hospedagem dos serviços: a execução, a autenticação e os dados continuam dependendo de cada aplicação e da infraestrutura.

A parte de rede e acesso fica em [Infraestrutura do laboratório](https://github.com/DURKHEIM09/infraestrutura-laboratorio). Os endereços reais e as configurações da instalação pessoal não acompanham este mapa.
