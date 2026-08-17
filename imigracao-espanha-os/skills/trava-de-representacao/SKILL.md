---
name: trava-de-representacao
description: "GATE 2 — poder administrativo, atos pessoais, OAB, Colegio e correspondente espanhol. Frentes 💼⚖️. Travas T1,T9. Espanha — LO 4/2000 + RD 1155/2024/RD 316/2026. Zero número operacional hardcoded; URL oficial + data. Use em: representar, OAB, abogado, Colegio, consultor, Mercurio, poder."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# TRAVA DE REPRESENTACAO

> **Camada C1** · Frentes: 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-espanha-os` · Régua: `context/anexo-travas-espanha.md` (10 travas)

## Papel
GATE 2 — poder administrativo, atos pessoais, OAB, Colegio e correspondente espanhol

## Anexos
`context/anexo-representacao-abogacia.md`, `context/anexo-travas-espanha.md`

## Travas aplicáveis
- **T1:** Representação administrativa (Ley 39/2015 art. 5 + RD 1155/2024 art. 197.4) ≠ abogacía (Ley 34/2006 + RD 135/2021). OAB sozinha não é título espanhol nem Colegio.
- **T9:** Comparecimento pessoal pode ser eletrônico (art. 197.1), mas entrevista/TIE/biometria/assinatura continuam pessoais. Poder ≠ certificado de acesso ao canal.

## Disclaimer (uma linha)
Não substitui profissional habilitado e colegiado na Espanha (abogado/procurador) nem garante concessão de visto, autorização, TIE ou nacionalidade. BOE e páginas oficiais vencem a memória do modelo.


## A interseção espanhola (não é a lista fechada dos EUA nem a OA portuguesa)

| Quem | Pode | Não pode |
|---|---|---|
| **Cliente** | Atos pessoais; entrevista, TIE, biometria, assinatura quando exigidas | Transferir ato personalíssimo por mandato |
| **Representante administrativo** | Atuar com poder notarial/apud acta ou habilitação do art. 197.4 | Transformar-se em abogado; escolher tese jurídica ES |
| **Abogado colegiado ejerciente** | Consulta, estratégia, audiência, contencioso (com procurador quando a LJCA exigir) | Atuar sem título + Colegio |
| **Só OAB (sem título ES)** | Direito BR, documentos BR, preparação, logística, coordenação | “Advogado na Espanha”, parecer de Direito ES, assinatura reservada, G-28-style |
| **“Consultor de imigração”** | Logística/educação geral **sem** conselho jurídico individualizado | Título de abogado; licença estatal autônoma **não** foi provada |

### Frases bloqueadas
- “Com OAB você já é abogado na Espanha.”
- “Só advogado pode protocolar extranjería.” (falso — Ley 39/2015 art. 5)
- “Sou representante credenciado da Oficina/UGE.” (sem fonte)
- “O RD 936/2001 cobre título brasileiro.” (é UE/EEE)

### Modelo legítimo
Cliente (atos pessoais) + camada BR (OAB/docs) + abogado espanhol identificado (consulta/contencioso), com escopos e honorários separados — ver `arquitetura-do-servico-espanha`.


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
