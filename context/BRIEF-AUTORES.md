# Brief para os autores de aula â€” ConstituiÃ§Ã£o dos Agentes v6.2

Curso: `~/projetos/constituicao-agentes-v62` (formato-curso-v6, ediÃ§Ã£o 6.2, `"glossario": true`, sem perfil tÃ©cnico, sem mÃ³dulos).

## Leia antes de escrever (nesta ordem)
1. `~/.claude/skills/formato-curso-v6/SKILL.md` e as referÃªncias: `references/CONTEUDO-INICIANTE.md`, `references/V6-DESIGN.md`, `references/CHECKLIST-V6.md`, `references/TESTE-HUMANO.md` Â§1.
2. `context/curriculo.md` â€” aluno, profissÃµes-alvo, vocabulÃ¡rio fixo e a tabela das 5 aulas.
3. ConteÃºdo de origem (nenhum fato, nÃºmero ou regra fora dele e do currÃ­culo):
   - `~/projetos/constituicao-agentes/docs/LOGICA.md` (a anÃ¡lise)
   - `~/projetos/constituicao-agentes/modelo/constituicao-modelo.md` (as 9 seÃ§Ãµes)
   - `~/projetos/constituicao-agentes/modelo/casos-de-teste.md` (os 8 casos)
   - `~/projetos/constituicao-agentes/modelo/prompt-rascunho.md`
   - `~/projetos/constituicao-agentes/exemplos/clinica-atendimento.md` (exemplo da clÃ­nica)
4. `aulas/aula-1.html` â€” **aula-modelo aprovada (10/10)**: copie estrutura, tom, tamanho e padrÃ£o de visuais.

## Regras deste curso
- `<section class="view" id="v-aula-N" data-aula="N" data-tempo="NNmin">`; kicker "Aula N de 5"; rodapÃ© `<p class="aula-pe">Aula N Â· ConstituiÃ§Ã£o dos Agentes v6.2 Â· ARCKHÉ AI PRO</p>`; nav `â† trilha` / `prÃ³xima aula â†’` (#aula-N+1; na aula 5 o prÃ³ximo Ã© `#trilha` com texto "voltar Ã  trilha â†’").
- Cena: `<figure class="cena"><img src="assets/img/aula-N.webp" width="1280" height="720" alt="â€¦">` â€” as imagens jÃ¡ existem/estÃ£o sendo geradas com estas situaÃ§Ãµes (alt coerente):
  - aula-2: Edson, dono do escritÃ³rio de contabilidade, escreve Ã  caneta numa folha dividida em trÃªs blocos, cafÃ© ao lado, estantes de pastas.
  - aula-3: Rosana e uma recepcionista jovem diante de um quadro branco com uma tabela de quatro linhas, apontando para uma linha.
  - aula-4: Edson ao telefone com um cliente, anotando num caderno, mesa com pastas e calculadora.
  - aula-5: Rosana no notebook com uma lista impressa ao lado, marcando itens com caneta verde.
- Exemplos: `p[data-ex="coordenadora"]` (Rosana, coordenadora de atendimento de uma clÃ­nica; o agente atende pacientes no WhatsApp: marca, remarca, responde endereÃ§o/convÃªnio; nunca diagnÃ³stico) e `p[data-ex="contador"]` (Edson, dono de um escritÃ³rio de contabilidade; o agente lembra prazos e pede documentos aos clientes no WhatsApp; nunca orientaÃ§Ã£o fiscal personalizada nem valor de imposto). Alterne os dois; situaÃ§Ãµes novas em cada aula. **NÃ£o repita as da aula 1**: paciente com dor no peito, cliente que pergunta valor do imposto, multa da Receita pela metade.
- **Onde fica o documento**: a constituiÃ§Ã£o Ã© escrita no documento **ConstituiÃ§Ã£o do agente**, nas Notas do celular ou num documento do computador, criado na aula 2. Nas aulas 3â€“5, diga isso e dÃª a saÃ­da para quem pulou ("NÃ£o fez a aula 2? Comece pelo molde abaixo").
- PrÃ¡tica no chat de IA que o aluno jÃ¡ usa. Na aula 5 o chat faz o papel do agente: o aluno cola a constituiÃ§Ã£o no inÃ­cio de uma conversa nova e manda os casos de teste. Nada de instalar, nada de terminal, nada de Python (o verificador do kit fica fora das aulas).
- Telas "boas" simuladas nÃ£o inventam fato que nÃ£o esteja no pedido. Nada de emoji, hype ou "!!".
- **DefiniÃ§Ãµes (`.gterm`) â€” use EXATAMENTE este `data-def` na 1Âª vez que o termo aparece em cada aula** (o glossÃ¡rio junta as aulas):
  - agente: `um assistente de IA que trabalha para a empresa: responde clientes, marca horÃ¡rios, organiza pedidos. Na clÃ­nica, atende pacientes no WhatsApp; no escritÃ³rio, lembra prazos aos clientes.`
  - constituiÃ§Ã£o: `o documento que diz para que o agente existe, o que vale mais, o que ele nunca faz e quando chama uma pessoa. A Anthropic escreveu uma para o Claude; na clÃ­nica e no escritÃ³rio, ela cabe em uma ou duas pÃ¡ginas.`
  - prioridades: `a ordem do que vale mais quando duas coisas boas brigam: seguranÃ§a, honestidade, regras da empresa e ser Ãºtil. Vale a de cima.`
  - limite: `uma coisa que o agente nunca faz, mesmo que o cliente peÃ§a. Na clÃ­nica, dar diagnÃ³stico; no escritÃ³rio, dizer o valor do imposto.`
  - nÃ­vel de autonomia: `quanto o agente pode fazer sozinho numa aÃ§Ã£o: 0 nÃ£o toca, 1 propÃµe e espera, 2 faz e avisa, 3 faz sozinho.`
  - chamar uma pessoa: `o agente para e passa a conversa para alguÃ©m da equipe, com o histÃ³rico, em vez de decidir sozinho.`
  - caso difÃ­cil: `uma situaÃ§Ã£o que a regra nÃ£o resolve sozinha, escrita com o que fazer e o porquÃª. O porquÃª Ã© o que ensina o agente a julgar.`
  - caso de teste: `uma mensagem que vocÃª manda ao agente, com o comportamento certo jÃ¡ escrito, para conferir se ele segue a constituiÃ§Ã£o.`
  - registro de falhas: `uma lista com uma linha por erro do agente: data, o que quebrou, a menor correÃ§Ã£o e se o problema era o texto ou o sistema.`
- Um nome sÃ³ por conceito (ver vocabulÃ¡rio do currÃ­culo).

## VerificaÃ§Ã£o (numa cÃ³pia isolada â€” nunca monte no repositÃ³rio real)
```bash
S=$(mktemp -d); cp -r ~/projetos/constituicao-agentes-v62/{aulas,assets,curso.json,landing.html} $S/
# na cÃ³pia, apague as aulas que nÃ£o sÃ£o suas, exceto a sua (o montador numera pelo que existir)
# se assets/img/aula-N.webp ou trilha.webp ainda nÃ£o existir na cÃ³pia, crie um placeholder 1280x720 (PIL) SÃ“ na cÃ³pia
python3 ~/.claude/skills/formato-curso-v6/scripts/montar-curso.py $S
node ~/.claude/skills/formato-curso-v6/scripts/auditar-curso.cjs $S/curso.html
```
Meta: a aula â‰¥9/10 (mire 10) e sem falha nos critÃ©rios 7, 8 e 10. FaÃ§a o leitor simulado (`TESTE-HUMANO.md` Â§1) e corrija.
Copie de volta para `~/projetos/constituicao-agentes-v62/aulas/` **sÃ³** o seu `aula-N.html`. NÃ£o toque em `assets/img/`, `curso.json` nem em outras aulas. NÃ£o faÃ§a commit.

Relate: nota do auditor, o que corrigiu e qualquer dÃºvida de conteÃºdo.
