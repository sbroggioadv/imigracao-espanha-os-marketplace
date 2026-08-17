---
name: suprema-corte-imigratoria-es
description: "QA adversarial R1–R4: fonte, literalidade, vigência, gap e não contradição com as 10 travas. Frentes ⚖️. Travas T1-T10. Espanha — LO 4/2000 + RD 1155/2024/RD 316/2026. Zero número operacional hardcoded; URL oficial + data. Use em: auditoria, revisão final, antes de protocolar, R1 R2 R3 R4, corte imigratoria."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# SUPREMA CORTE IMIGRATORIA ES

> **Camada C0** · Frentes: ⚖️ advogado  
> Plugin: `imigracao-espanha-os` · Régua: `context/anexo-travas-espanha.md` (10 travas)

## Papel
QA adversarial R1–R4: fonte, literalidade, vigência, gap e não contradição com as 10 travas

## Anexos
`context/anexo-travas-espanha.md`

## Travas aplicáveis
- **T1:** Representação administrativa (Ley 39/2015 art. 5 + RD 1155/2024 art. 197.4) ≠ abogacía (Ley 34/2006 + RD 135/2021). OAB sozinha não é título espanhol nem Colegio.
- **T2:** Regulamento vigente é o **RD 1155/2024** consolidado com o **RD 316/2026**. RD 557/2011 está derrogado. Hoja não vence BOE.
- **T3:** Rota encerrada não vira produto: golden visa (arts. 63–67 Ley 14/2013 sem conteúdo), LMD (novos pedidos/citas fechados) e EX-31/EX-32 (janelas até 30/06/2026).
- **T4:** Data de **formalização** do asilo decide o regime. Desde 12/06/2026 = PEMA; reposición incompatível e não interrompe prazo judicial.
- **T5:** Não existe alzada universal. Autor do ato + notificação integral governam via e dies a quo. Consulta de estado ≠ resolução. Caixa eletrônica pode produzir efeito sem leitura.
- **T6:** Classificar status/regime antes do checklist: estancia ≠ residência; longa duração nacional ≠ UE ≠ permanente familiar UE; cinco arraigos atuais ≠ catálogo antigo; EX-02 ≠ EX-24 ≠ EX-19.
- **T7:** Dois anos para brasileiro **de origem** é limiar (CC art. 22.1), não cidadania automática. DELE em regra permanece. LMD fechada. EC 131/2023: sem perda automática da nacionalidade BR.
- **T8:** Apostila não traduz nem prova verdade material. Tradução juramentada BR não tem aceitação universal. Taxa/checklist/formulário = fonte viva do dia.
- **T9:** Comparecimento pessoal pode ser eletrônico (art. 197.1), mas entrevista/TIE/biometria/assinatura continuam pessoais. Poder ≠ certificado de acesso ao canal.
- **T10:** Irregularidade é infração grave, não expulsão automática (LO 4/2000 art. 57.1 — proporcionalidade). Preferente ≠ ordinário. Internação depende de juiz.

## Disclaimer (uma linha)
Não substitui profissional habilitado e colegiado na Espanha (abogado/procurador) nem garante concessão de visto, autorização, TIE ou nacionalidade. BOE e páginas oficiais vencem a memória do modelo.


## Rodadas (não pular)

- **R1 Brief:** frente, localização, regime, fase, data crítica e órgão estão no texto?
- **R2 Técnica:** dispositivo + URL + data; cascata UE/lei → RD → hoja; transição auditada?
- **R3 Travas:** T1–T10 aplicadas, não só citadas? Rota fechada permanece fechada? Gap permanece `NAO-PROVADO`?
- **R4 Completude:** gates rodaram; handoff ao correspondente ES se ⚖️ reservado; zero número operacional; sem promessa.

Reprovação em qualquer rodada = retrabalho. Não entregar.


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
