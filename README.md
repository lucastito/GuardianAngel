# Anjo da Guarda

Projeto acadêmico de automação residencial para detectar situações de risco e enviar alertas a pessoas responsáveis.

## Visão geral

O protótipo combina sensores conectados a um Arduino, uma aplicação desktop em Java e um aplicativo Android. O fluxo pretendido é:

1. sensores de presença e incêndio produzem leituras;
2. o Arduino envia os eventos pela porta serial;
3. a aplicação Java interpreta os eventos;
4. alertas podem ser encaminhados por SMS, e-mail ou servidor;
5. o aplicativo Android consulta o servidor e apresenta notificações.

## Componentes

- `arduino/`: código dos sensores, buzzer e indicadores.
- `Java/Anjo_da_Guarda/`: aplicação desktop, comunicação serial e mecanismos de alerta.
- `Android/AnjoDaGuardaAppFinalVersion/`: aplicativo Android legado.
- `Bibliotecas/`: dependências usadas no ambiente original, incluindo RXTX e clientes HTTP.
- `documentação/`: diagramas e materiais de apresentação.

## Hardware utilizado

- Arduino;
- sensor de presença por infravermelho passivo;
- sensor de incêndio ligado a uma entrada analógica;
- buzzer e diodos emissores de luz;
- computador conectado por porta serial.

## Estado do projeto

Este é um protótipo histórico, desenvolvido com bibliotecas e versões antigas de Java e Android. Serviços externos, endereços e APIs utilizados originalmente podem não estar mais disponíveis. A execução atual exige reconstruir o ambiente, revisar portas seriais e substituir as integrações legadas.

## Aviso de segurança

O código histórico contém configurações e credenciais inseridas diretamente nos fontes. Elas não devem ser reutilizadas e precisam ser consideradas comprometidas. Antes de qualquer execução ou reaproveitamento:

- revogue e substitua credenciais antigas;
- mova segredos para variáveis de ambiente ou um cofre de segredos;
- remova dados pessoais e endereços fixos;
- atualize dependências;
- utilize conexões seguras;
- não exponha o protótipo diretamente à internet.

O projeto não deve ser usado como sistema real de segurança ou emergência sem uma revisão completa de hardware, software, privacidade e confiabilidade.

