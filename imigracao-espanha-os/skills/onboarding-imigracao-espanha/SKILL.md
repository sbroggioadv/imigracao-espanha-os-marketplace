---
name: onboarding-imigracao-espanha
description: "primeira interação por botões; coleta frente, nacionalidade, localização, status, objetivo e urgência sem concluir mérito. Frentes 👤💼⚖️. Travas T4,T5,T6,T7,T10. Espanha — LO 4/2000 + RD 1155/2024/RD 316/2026. Zero número operacional hardcoded; URL oficial + data. Use em: /start-imigracao-espanha, configurar, primeira vez, onboarding."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# ONBOARDING IMIGRACAO ESPANHA

> **Camada C0** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-espanha-os` · Régua: `context/anexo-travas-espanha.md` (10 travas)

## Papel
primeira interação por botões; coleta frente, nacionalidade, localização, status, objetivo e urgência sem concluir mérito

## Anexos
`context/anexo-travas-espanha.md`

## Travas aplicáveis
- **T4:** Data de **formalização** do asilo decide o regime. Desde 12/06/2026 = PEMA; reposición incompatível e não interrompe prazo judicial.
- **T5:** Não existe alzada universal. Autor do ato + notificação integral governam via e dies a quo. Consulta de estado ≠ resolução. Caixa eletrônica pode produzir efeito sem leitura.
- **T6:** Classificar status/regime antes do checklist: estancia ≠ residência; longa duração nacional ≠ UE ≠ permanente familiar UE; cinco arraigos atuais ≠ catálogo antigo; EX-02 ≠ EX-24 ≠ EX-19.
- **T7:** Dois anos para brasileiro **de origem** é limiar (CC art. 22.1), não cidadania automática. DELE em regra permanece. LMD fechada. EC 131/2023: sem perda automática da nacionalidade BR.
- **T10:** Irregularidade é infração grave, não expulsão automática (LO 4/2000 art. 57.1 — proporcionalidade). Preferente ≠ ordinário. Internação depende de juiz.

## Disclaimer (uma linha)
Não substitui profissional habilitado e colegiado na Espanha (abogado/procurador) nem garante concessão de visto, autorização, TIE ou nacionalidade. BOE e páginas oficiais vencem a memória do modelo.


## Fluxo (botões AskUserQuestion)

1. **Frente:** 👤 Imigrante · 💼 Comercial · ⚖️ Advogado · Só estudar o plugin.
2. **Objetivo:** entrar/trabalhar · estudar · não lucrativa/remote · família · nacionalidade · já tenho processo · não sei.
3. **Onde está agora:** Brasil · Espanha com título · Espanha sem título / irregular · outro.
4. **Nacionalidade:** brasileiro de origem · brasileiro naturalizado · UE · outro.
5. **Urgência:** pensando · prazo de notificação · expediente de expulsão · asilo · não sei.
6. **Datas:** tem protocolo/formalização/notificação com data? (texto livre se sim).

### ⛔ Se houver expediente de expulsão ou irregularidade
Não minimizar. Abrir `irregularidade-sancao-e-expulsao` **antes** de vender rota bonita.

### ⛔ Se o objetivo for golden visa / lei dos netos / EX-31–32
Aplicar **T3**: porta nova fechada. Só legado com prova de data/cita tempestiva.

### ⛔ Se o objetivo for asilo
Pedir **data de formalização** antes de qualquer fluxo (T4).

Grave o perfil localmente e devolva ao `imigracao-espanha-master`.


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
