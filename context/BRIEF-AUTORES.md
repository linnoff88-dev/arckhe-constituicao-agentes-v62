# Brief para os autores de aula ê¢â¬â ConstituiêÂ§êÂ£o dos Agentes v6.2

Curso: `~/projetos/constituicao-agentes-v62` (formato-curso-v6, ediêÂ§êÂ£o 6.2, `"glossario": true`, sem perfil têÂ©cnico, sem mêÂ³dulos).

## Leia antes de escrever (nesta ordem)
1. `~/.claude/skills/formato-curso-v6/SKILL.md` e as referêÂªncias: `references/CONTEUDO-INICIANTE.md`, `references/V6-DESIGN.md`, `references/CHECKLIST-V6.md`, `references/TESTE-HUMANO.md` êÂ§1.
2. `context/curriculo.md` ê¢â¬â aluno, profissêÂµes-alvo, vocabulêÂ¡rio fixo e a tabela das 5 aulas.
3. ConteêÂºdo de origem (nenhum fato, nêÂºmero ou regra fora dele e do currêÂ­culo):
   - `~/projetos/constituicao-agentes/docs/LOGICA.md` (a anêÂ¡lise)
   - `~/projetos/constituicao-agentes/modelo/constituicao-modelo.md` (as 9 seêÂ§êÂµes)
   - `~/projetos/constituicao-agentes/modelo/casos-de-teste.md` (os 8 casos)
   - `~/projetos/constituicao-agentes/modelo/prompt-rascunho.md`
   - `~/projetos/constituicao-agentes/exemplos/clinica-atendimento.md` (exemplo da clêÂ­nica)
4. `aulas/aula-1.html` ê¢â¬â **aula-modelo aprovada (10/10)**: copie estrutura, tom, tamanho e padrêÂ£o de visuais.

## Regras deste curso
- `<section class="view" id="v-aula-N" data-aula="N" data-tempo="NNmin">`; kicker "Aula N de 5"; rodapêÂ© `<p class="aula-pe">Aula N êÂ· ConstituiêÂ§êÂ£o dos Agentes v6.2 êÂ· ARCKHê AI PRO</p>`; nav `ê¢â Â trilha` / `prêÂ³xima aula ê¢â â` (#aula-N+1; na aula 5 o prêÂ³ximo êÂ© `#trilha` com texto "voltar êÂ  trilha ê¢â â").
- Cena: `<figure class="cena"><img src="assets/img/aula-N.webp" width="1280" height="720" alt="ê¢â¬Â¦">` ê¢â¬â as imagens jêÂ¡ existem/estêÂ£o sendo geradas com estas situaêÂ§êÂµes (alt coerente):
  - aula-2: Edson, dono do escritêÂ³rio de contabilidade, escreve êÂ  caneta numa folha dividida em trêÂªs blocos, cafêÂ© ao lado, estantes de pastas.
  - aula-3: Rosana e uma recepcionista jovem diante de um quadro branco com uma tabela de quatro linhas, apontando para uma linha.
  - aula-4: Edson ao telefone com um cliente, anotando num caderno, mesa com pastas e calculadora.
  - aula-5: Rosana no notebook com uma lista impressa ao lado, marcando itens com caneta verde.
- Exemplos: `p[data-ex="coordenadora"]` (Rosana, coordenadora de atendimento de uma clêÂ­nica; o agente atende pacientes no WhatsApp: marca, remarca, responde endereêÂ§o/convêÂªnio; nunca diagnêÂ³stico) e `p[data-ex="contador"]` (Edson, dono de um escritêÂ³rio de contabilidade; o agente lembra prazos e pede documentos aos clientes no WhatsApp; nunca orientaêÂ§êÂ£o fiscal personalizada nem valor de imposto). Alterne os dois; situaêÂ§êÂµes novas em cada aula. **NêÂ£o repita as da aula 1**: paciente com dor no peito, cliente que pergunta valor do imposto, multa da Receita pela metade.
- **Onde fica o documento**: a constituiêÂ§êÂ£o êÂ© escrita no documento **ConstituiêÂ§êÂ£o do agente**, nas Notas do celular ou num documento do computador, criado na aula 2. Nas aulas 3ê¢â¬â5, diga isso e dêÂª a saêÂ­da para quem pulou ("NêÂ£o fez a aula 2? Comece pelo molde abaixo").
- PrêÂ¡tica no chat de IA que o aluno jêÂ¡ usa. Na aula 5 o chat faz o papel do agente: o aluno cola a constituiêÂ§êÂ£o no inêÂ­cio de uma conversa nova e manda os casos de teste. Nada de instalar, nada de terminal, nada de Python (o verificador do kit fica fora das aulas).
- Telas "boas" simuladas nêÂ£o inventam fato que nêÂ£o esteja no pedido. Nada de emoji, hype ou "!!".
- **DefiniêÂ§êÂµes (`.gterm`) ê¢â¬â use EXATAMENTE este `data-def` na 1êÂª vez que o termo aparece em cada aula** (o glossêÂ¡rio junta as aulas):
  - agente: `um assistente de IA que trabalha para a empresa: responde clientes, marca horêÂ¡rios, organiza pedidos. Na clêÂ­nica, atende pacientes no WhatsApp; no escritêÂ³rio, lembra prazos aos clientes.`
  - constituiêÂ§êÂ£o: `o documento que diz para que o agente existe, o que vale mais, o que ele nunca faz e quando chama uma pessoa. A Anthropic escreveu uma para o Claude; na clêÂ­nica e no escritêÂ³rio, ela cabe em uma ou duas pêÂ¡ginas.`
  - prioridades: `a ordem do que vale mais quando duas coisas boas brigam: seguranêÂ§a, honestidade, regras da empresa e ser êÂºtil. Vale a de cima.`
  - limite: `uma coisa que o agente nunca faz, mesmo que o cliente peêÂ§a. Na clêÂ­nica, dar diagnêÂ³stico; no escritêÂ³rio, dizer o valor do imposto.`
  - nêÂ­vel de autonomia: `quanto o agente pode fazer sozinho numa aêÂ§êÂ£o: 0 nêÂ£o toca, 1 propêÂµe e espera, 2 faz e avisa, 3 faz sozinho.`
  - chamar uma pessoa: `o agente para e passa a conversa para alguêÂ©m da equipe, com o histêÂ³rico, em vez de decidir sozinho.`
  - caso difêÂ­cil: `uma situaêÂ§êÂ£o que a regra nêÂ£o resolve sozinha, escrita com o que fazer e o porquêÂª. O porquêÂª êÂ© o que ensina o agente a julgar.`
  - caso de teste: `uma mensagem que vocêÂª manda ao agente, com o comportamento certo jêÂ¡ escrito, para conferir se ele segue a constituiêÂ§êÂ£o.`
  - registro de falhas: `uma lista com uma linha por erro do agente: data, o que quebrou, a menor correêÂ§êÂ£o e se o problema era o texto ou o sistema.`
- Um nome sêÂ³ por conceito (ver vocabulêÂ¡rio do currêÂ­culo).

## VerificaêÂ§êÂ£o (numa cêÂ³pia isolada ê¢â¬â nunca monte no repositêÂ³rio real)
```bash
S=$(mktemp -d); cp -r ~/projetos/constituicao-agentes-v62/{aulas,assets,curso.json,landing.html} $S/
# na cêÂ³pia, apague as aulas que nêÂ£o sêÂ£o suas, exceto a sua (o montador numera pelo que existir)
# se assets/img/aula-N.webp ou trilha.webp ainda nêÂ£o existir na cêÂ³pia, crie um placeholder 1280x720 (PIL) Sêâ na cêÂ³pia
python3 ~/.claude/skills/formato-curso-v6/scripts/montar-curso.py $S
node ~/.claude/skills/formato-curso-v6/scripts/auditar-curso.cjs $S/curso.html
```
Meta: a aula ê¢â°Â¥9/10 (mire 10) e sem falha nos critêÂ©rios 7, 8 e 10. FaêÂ§a o leitor simulado (`TESTE-HUMANO.md` êÂ§1) e corrija.
Copie de volta para `~/projetos/constituicao-agentes-v62/aulas/` **sêÂ³** o seu `aula-N.html`. NêÂ£o toque em `assets/img/`, `curso.json` nem em outras aulas. NêÂ£o faêÂ§a commit.

Relate: nota do auditor, o que corrigiu e qualquer dêÂºvida de conteêÂºdo.
