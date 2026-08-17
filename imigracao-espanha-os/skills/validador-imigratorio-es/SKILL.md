---
name: validador-imigratorio-es
description: "bloqueia fonte baixa, número operacional congelado, rota fechada e citação sem URL/data. Frentes 👤💼⚖️. Travas T2,T3,T4,T5,T8. Espanha — LO 4/2000 + RD 1155/2024/RD 316/2026. Zero número operacional hardcoded; URL oficial + data. Use em: validar, checar fonte, URL, alucinação, RD 557."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# VALIDADOR IMIGRATORIO ES

> **Camada C0** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-espanha-os` · Régua: `context/anexo-travas-espanha.md` (10 travas)

## Papel
bloqueia fonte baixa, número operacional congelado, rota fechada e citação sem URL/data

## Anexos
`context/anexo-travas-espanha.md`

## Travas aplicáveis
- **T2:** Regulamento vigente é o **RD 1155/2024** consolidado com o **RD 316/2026**. RD 557/2011 está derrogado. Hoja não vence BOE.
- **T3:** Rota encerrada não vira produto: golden visa (arts. 63–67 Ley 14/2013 sem conteúdo), LMD (novos pedidos/citas fechados) e EX-31/EX-32 (janelas até 30/06/2026).
- **T4:** Data de **formalização** do asilo decide o regime. Desde 12/06/2026 = PEMA; reposición incompatível e não interrompe prazo judicial.
- **T5:** Não existe alzada universal. Autor do ato + notificação integral governam via e dies a quo. Consulta de estado ≠ resolução. Caixa eletrônica pode produzir efeito sem leitura.
- **T8:** Apostila não traduz nem prova verdade material. Tradução juramentada BR não tem aceitação universal. Taxa/checklist/formulário = fonte viva do dia.

## Disclaimer (uma linha)
Não substitui profissional habilitado e colegiado na Espanha (abogado/procurador) nem garante concessão de visto, autorização, TIE ou nacionalidade. BOE e páginas oficiais vencem a memória do modelo.


## Checklist de bloqueio

Recusar entrega se qualquer item falhar:

1. Afirmação operacional sem **URL oficial + data**.
2. Citação do **RD 557/2011** como regulamento atual.
3. Número de taxa, IPREM, SMI, cota GECCO, agenda ou SLA de fila no corpo.
4. Venda de golden visa / LMD nova / EX-31–32 como porta aberta.
5. Asilo sem **data de formalização**.
6. Recurso indicado sem ato + prova de notificação + órgão autor.
7. Estudo contado como residência integral, ou EX-02 usado para família de espanhol/UE.
8. “Dois anos = cidadania” ou dispensa automática de DELE para brasileiro adulto comum.
9. “Irregular = expulsão automática.”
10. Cópia da trava 292.1 dos EUA ou da OA portuguesa.

Saída: `PASS` · `CONCERNS` · `FAIL` + o item violado.


## URLs de topo (sempre preferir estas)
- BOE / ELI: https://www.boe.es
- RD 1155/2024 consolidado: https://www.boe.es/eli/es/rd/2024/11/19/1155/con
- LO 4/2000: https://www.boe.es/eli/es/lo/2000/01/11/4/con
- Migraciones / hojas: https://www.inclusion.gob.es/web/migraciones/home
- Modelos EX: https://www.inclusion.gob.es/web/migraciones/modelos-generales
- Mercurio: https://sede.administracionespublicas.gob.es/pagina/index/directorio/mercurio2/language/es_ES
- Exteriores / apostila: https://www.exteriores.gob.es/es/ServiciosAlCiudadano/Paginas/Legalizacion-y-apostilla.aspx
- Justicia / nacionalidade e acesso à advocacia: https://www.mjusticia.gob.es
- EUR-Lex: https://eur-lex.europa.eu

## Saída esperada
1. Frente + fase + localização + regime + **data do ato** usada.  
2. Regime jurídico aplicável (dispositivo + URL + data de leitura).  
3. O que fazer agora / o que não fazer (⛔).  
4. Lacunas `NAO-PROVADO` declaradas.  
5. Próxima skill ou referral (Colegio / consulado / Oficina / UGE / Justicia / Policía).

## Guard
- Zero taxa/cota/limiar econômico/prazo de processamento hardcoded.  
- Zero promessa de resultado ou prazo de aprovação.  
- Zero copiar trava dos EUA (292.1) ou de Portugal (OAB≠OA) como se fosse Espanha.  
- Byte cap: manter este arquivo ≤ 11.000 B.
