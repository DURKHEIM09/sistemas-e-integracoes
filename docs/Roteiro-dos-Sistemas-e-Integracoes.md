# Roteiro dos sistemas e integrações

[Voltar à apresentação](../README.md) · [Estado e limites](./Estado-e-Limites-dos-Sistemas.md)

Este é um roteiro de referência derivado da organização documentada. O repositório não traz uma instalação completa da stack. As versões e as opções de instalação precisam ser escolhidas no ambiente de quem for reproduzir.

## 1. Escolher uma entrega pequena

Comece por um resultado observável: por exemplo, receber uma solicitação, executar um relatório e salvar a saída. Defina a entrada, o resultado esperado e como identificar uma falha.

Não é necessário instalar todo o catálogo para testar um fluxo.

## 2. Separar as responsabilidades

Descreva o fluxo antes de configurá-lo:

| Parte | Decisão necessária | Resultado esperado |
| --- | --- | --- |
| Interface | De onde chega o pedido? | Uma entrada clara e identificável. |
| Coordenação | Uma chamada direta basta ou há etapas para o n8n organizar? | Um caminho de execução definido. |
| Execução | Qual script, API ou ferramenta faz o trabalho? | Uma tarefa delimitada e verificável. |
| Dados | Onde ficam entrada, saída e estado? | Artefatos acessíveis aos componentes autorizados. |
| Documentação | Onde se registra a configuração e sua operação? | Uma fonte de referência para retomar o trabalho. |

O n8n é útil quando o fluxo pede integração de etapas. Uma rotina simples pode continuar como script ou chamada de API.

## 3. Preparar o ambiente de execução

Use o tipo de instalação que o sistema requer: contêiner quando a implantação usa Compose; runtime nativo quando esse é o desenho suportado. Separe aplicação, estado persistente e configuração.

Defina as permissões de acesso e o armazenamento de credenciais no seu próprio ambiente. Não copie configurações pessoais de outro laboratório. A visão da base está em [Infraestrutura do laboratório](https://github.com/DURKHEIM09/infraestrutura-laboratorio).

## 4. Implementar um único caminho completo

Configure a entrada, execute uma tarefa pequena e confira o resultado. Se usar n8n, mantenha as credenciais no armazenamento apropriado e documente os nós pelo papel que cumprem no fluxo.

Antes de ampliar, confirme:

- A entrada chegou ao componente esperado.
- A tarefa produziu o artefato previsto.
- Um erro fica visível e permite descobrir em qual etapa aconteceu.
- Repetir um pedido tem um comportamento conhecido, sem duplicação acidental de efeitos.

Esses são critérios propostos para uma nova implementação; não são uma declaração de que toda integração do laboratório já os atende.

## 5. Acrescentar observabilidade conforme a necessidade

Comece verificando a aplicação e os recursos dos quais ela depende. Zabbix e Grafana têm uma integração documentada neste laboratório; Netdata tem papel complementar. Instalar os três não é requisito para executar uma automação.

Registre quais sinais ajudam a tomar uma decisão: falha de execução, indisponibilidade, falta de espaço ou consumo anormal. Um dashboard deve responder a uma pergunta concreta.

## 6. Documentar e manter

Mantenha uma nota com função, dependências, instalação, operação, validação e limites. Registre a versão realmente executada e a data da conferência.

Na manutenção, preserve os dados e um caminho de retorno. A documentação histórica da stack de monitoramento inclui procedimentos de backup e rollback; este pacote não entrega essas rotinas nem comprova uma restauração feita por quem o adotar.

Para exemplos com implementação pública, consulte [Hermes Control](https://github.com/DURKHEIM09/hermes-control) e [Factorio — Durkh Coop](https://github.com/DURKHEIM09/factorio-durkh-coop). Para os modelos documentais, veja [Neuro-Link e Obsidian](https://github.com/DURKHEIM09/neuro-link-obsidian).
