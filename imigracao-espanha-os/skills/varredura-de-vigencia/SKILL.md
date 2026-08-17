---
name: varredura-de-vigencia
description: "GATE 1 — reabre BOE consolidado + hoja/formulário/gerador vivos e registra a data. Frentes 👤💼⚖️. Travas T2,T3,T4,T5. Espanha — LO 4/2000 + RD 1155/2024/RD 316/2026. Zero número operacional hardcoded; URL oficial + data. Use em: vigência, atualizou, RD 1155, RD 316/2026, PEMA, taxa, hoja."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# VARREDURA DE VIGENCIA

> **Camada C1** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-espanha-os` · Régua: `context/anexo-travas-espanha.md` (10 travas)

## Papel
GATE 1 — reabre BOE consolidado + hoja/formulário/gerador vivos e registra a data

## Anexos
`context/anexo-travas-espanha.md`, `context/anexo-loex-rd1155.md`

## Travas aplicáveis
- **T2:** Regulamento vigente é o **RD 1155/2024** consolidado com o **RD 316/2026**. RD 557/2011 está derrogado. Hoja não vence BOE.
- **T3:** Rota encerrada não vira produto: golden visa (arts. 63–67 Ley 14/2013 sem conteúdo), LMD (novos pedidos/citas fechados) e EX-31/EX-32 (janelas até 30/06/2026).
- **T4:** Data de **formalização** do asilo decide o regime. Desde 12/06/2026 = PEMA; reposición incompatível e não interrompe prazo judicial.
- **T5:** Não existe alzada universal. Autor do ato + notificação integral governam via e dies a quo. Consulta de estado ≠ resolução. Caixa eletrônica pode produzir efeito sem leitura.

## Disclaimer (uma linha)
Não substitui profissional habilitado e colegiado na Espanha (abogado/procurador) nem garante concessão de visto, autorização, TIE ou nacionalidade. BOE e páginas oficiais vencem a memória do modelo.


## Como rodar o GATE 1

Para **cada** afirmação operacional (taxa, formulário, hoja, limiar, cota, prazo de processamento):

1. Abrir o **BOE consolidado** do diploma (ELI).
2. Abrir a **hoja / modelo / gerador** vivo do órgão.
3. Registrar **URL + data/hora** da consulta.
4. Classificar: `CONFIRMADO` · `TRANSICAO` · `CONFLITO` · `NAO-PROVADO`.
5. `TRANSICAO` e `CONFLITO` **nunca** viram resposta categórica. Em conflito hoja × BOE, **BOE vence** (ex.: Hoja 32 × art. 130.2).

### Gatilhos obrigatórios deste gate
RD 1155/2024 · RD 316/2026 · PEMA 12/06/2026 · GECCO/ordem anual · hojas EX · gerador 790 · investidor/LMD/EX-31–32 · notificação individual.

### ⛔ Recusar de memória
RD 557/2011 como vigente · golden visa aberto · LMD aberta · EX-31/32 como regularização nova · reposición no PEMA · valor de taxa/IPREM/SMI.


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
