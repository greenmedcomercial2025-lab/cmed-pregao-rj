# CMED — Pregões RJ

Projeto separado para consulta e conferência de preços máximos de medicamentos em compras públicas no Estado do Rio de Janeiro.

## Estrutura
- `dados/modelo_cmed_rj.csv`: modelo de base para cadastro/consulta.
- `docs/regras_cmed.md`: regras de aplicação CAP, PF, PMVG e ICMS.
- `config/cmed_config.csv`: parâmetros vigentes usados pelo projeto.

## Regra principal para compras públicas
- CAP SIM → teto = PMVG.
- CAP NÃO + sem decisão judicial → teto = PF.
- Decisão judicial → teto = PMVG.
- A alíquota de ICMS deve ser conferida na coluna correspondente da lista CMED e conforme a operação aplicável.

## Vigência do CAP
A Resolução CTE-CMED nº 1, de 25/05/2026, atualizou o rol de produtos sujeitos ao CAP e fixou o CAP em 19,79%, com vigência a partir de 24/09/2026.

## Fonte oficial
ANVISA/CMED — Compras públicas e listas de preços.
