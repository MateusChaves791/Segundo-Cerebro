# Modelo de e-mails de casos KT (para a Raisa, Volkswagen)

Base: 16 das 38 threads com a Raisa, lidas até agora. Padrão confirmado nelas. Atualizar conforme ler o restante.

## O que é fixo (o processo não muda)
- Assunto: `KT [número] | DN 1417 | VEÍCULO PARADO | [modelo] | [chassi]`, ou `FORMULÁRIO DO CRM [números] DN-1417 CHASSIS [chassi]`.
- Saudação curta: "Bom dia Raisa," ou "Boa tarde Raisa,".
- Estrutura: primeiro o status do caso, depois o pedido ou a cobrança, depois o fechamento.
- Pedido sempre com "por gentileza" e a ação de quem deve fazer (cotar, cancelar, acompanhar, abrir IPPR).
- Fechamento: "Atenciosamente," e a assinatura padrão de Supervisor | Peças, Servopa Volkswagen Pinheirinho.
- Tabela do formulário do CRM, com as colunas: Caso Salesforce DN | Pedido | Linha | Peça | Veículo Imobilizado? | Data Imobilização | Reparo em Garantia? | Reparo no DN? | Locação | Observação | Chassi.
- Cópia para a equipe conforme a função: Eva (funilaria), Chayene (pedidos e cancelamentos), Amanda (NF, IPPR e acompanhamento de faturamento).

## O que muda (dados do caso)
- Número do KT ou do CRM, chassi, modelo.
- Código da peça, número do pedido e linha.
- Valor, fornecedor da rede, frete, CNPJ do fornecedor quando for cotação.
- Status: faturado, pendente, sem previsão, em garantia, em cancelamento.
- Data de previsão de entrega ou NF.

## Tipos de mensagem que aparecem
1. **Abertura do caso:** envio do formulário com a tabela e as peças por linha.
2. **Cotação na rede:** item, fornecedor, valor e frete, pedindo análise ou aprovação.
3. **Cobrança de pendência:** o item ainda não alocado ou não faturado, com a previsão do fornecedor.
4. **Confirmação de fechamento:** "não há mais pendências" e a data prevista de entrega.
5. **Pedido de ação interna:** cancelamento de item, IPPR de ação D quando o item chegar, acompanhamento de faturamento.

## Exemplos reais (dados trocados)
- Cobrança: "Temos retorno da escala do caso para KT? Segue pendente o item abaixo: [item]. O fornecedor informou entrega na semana [X]. Item ainda não alocado no pedido."
- Fechamento: "Não há mais pendências, previsão de entrega do veículo para [data]. Agradeço o apoio!"
- Cotação: "Tivemos retorno na rede sobre o item: [item] - [fornecedor] (R$ [valor] + frete [UF]). Pode por gentileza analisar?"

## Regras de qualidade
- Não usar nome de cliente nem dado pessoal no e-mail.
- Citar só o número do caso, o item e a data, para a Raisa localizar rápido.
- Antes de enviar, conferir se o chassi e o KT batem com o assunto.
