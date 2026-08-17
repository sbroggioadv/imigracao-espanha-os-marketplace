---
name: razoes-humanitarias
description: "hipótese fechada do art. 128, prova, conflito Hoja 32 versus art. 130.2 e pós-concessão. Frentes 👤💼⚖️. Travas T2,T5,T8. Espanha — LO 4/2000 + RD 1155/2024/RD 316/2026. Zero número operacional hardcoded; URL oficial + data. Use em: razões humanitárias, Hoja 32, art. 128."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# RAZOES HUMANITARIAS

> **Camada C7** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-espanha-os` · Régua: `context/anexo-travas-espanha.md` (10 travas)

## Papel
hipótese fechada do art. 128, prova, conflito Hoja 32 versus art. 130.2 e pós-concessão

## Anexos
`context/anexo-protecao-pema.md`, `context/anexo-arraigo-humanitario.md`

## Travas aplicáveis
- **T2:** Regulamento vigente é o **RD 1155/2024** consolidado com o **RD 316/2026**. RD 557/2011 está derrogado. Hoja não vence BOE.
- **T5:** Não existe alzada universal. Autor do ato + notificação integral governam via e dies a quo. Consulta de estado ≠ resolução. Caixa eletrônica pode produzir efeito sem leitura.
- **T8:** Apostila não traduz nem prova verdade material. Tradução juramentada BR não tem aceitação universal. Taxa/checklist/formulário = fonte viva do dia.

## Disclaimer (uma linha)
Não substitui profissional habilitado e colegiado na Espanha (abogado/procurador) nem garante concessão de visto, autorização, TIE ou nacionalidade. BOE e páginas oficiais vencem a memória do modelo.


## Como operar esta skill

1. Confirmar **frente** e se os gates já rodaram nesta sessão; se não, chamar `varredura-de-vigencia` e/ou `trava-de-representacao`.
2. Pedir os **fatos mínimos**: nacionalidade (origem?), onde está, objetivo, status/título, datas de protocolo/formalização/notificação.
3. **Classificar o regime** (comum / UE-família / UGE / arraigo / proteção / longa duração / nacionalidade) **antes** do checklist.
4. Mapear **finalidade → dispositivo (LOEX / RD 1155/2024 / especial) → hoja viva → órgão/canal → legitimado**.
5. Montar entrega na profundidade da frente:
   - 👤 checklist e decisões honestas, sem minuta de mandato ES
   - 💼 escopo vendável, contrato e o que **não** vender
   - ⚖️ matriz norma→requisito→prova→remédio, com referral ao abogado colegiado se faltar habilitação
6. Toda afirmação operacional: **URL oficial + data**. Sem fonte atual → `NAO-PROVADO`.
7. Antes de fechar entrega normativa: `validador-imigratorio-es` (e `suprema-corte-imigratoria-es` se ⚖️).


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
