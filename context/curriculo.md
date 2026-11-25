ï»¿# CurrêÂ­culo ê¢â¬â ConstituiêÂ§êÂ£o dos Agentes v6.2

Base: kit `linnoff88-dev/constituicao-agentes` (docs/LOGICA.md, modelo/, exemplos/clinica-atendimento.md).
NêÂ£o repetir o `empresas-2027-v62` (LêÂ­via, Wagner; aula 5 "A constituiêÂ§êÂ£o do seu agente"): aqui cada peêÂ§a
da constituiêÂ§êÂ£o vira uma aula e o aluno sai com o documento inteiro, testado.

## Aluno
Dono, gestor ou lêÂ­der de equipe de empresa pequena/mêÂ©dia, 30+. JêÂ¡ usa ChatGPT ou Claude no navegador e
WhatsApp. Pensa em pêÂ´r um agente para atender ou operar e tem medo de que ele "faêÂ§a besteira". Sem terminal.

## ProfissêÂµes-alvo (data-ex)
- `coordenadora` ê¢â¬â **Rosana**, coordenadora de atendimento de uma clêÂ­nica (agenda, pacientes; nunca diagnêÂ³stico).
- `contador` ê¢â¬â **Edson**, dono de um escritêÂ³rio de contabilidade (prazos, documentos de clientes; nunca orientaêÂ§êÂ£o fiscal personalizada).

## Promessa do curso
Sai com a **constituiêÂ§êÂ£o de 1 a 2 pêÂ¡ginas do agente da sua empresa** ê¢â¬â missêÂ£o, prioridades, limites, nêÂ­veis de
autonomia, quando chamar uma pessoa, 3 casos difêÂ­ceis com o porquêÂª ê¢â¬â testada com 8 casos e com data de revisêÂ£o.

## VocabulêÂ¡rio fixo (um nome por conceito)
- **constituiêÂ§êÂ£o do agente** ê¢â¬â o documento inteiro.
- **agente** ê¢â¬â o assistente de IA que trabalha para a empresa (atende, marca, responde).
- **prioridades** ê¢â¬â a ordem do que vale mais quando duas coisas boas brigam (seguranêÂ§a, honestidade, regras da empresa, ser êÂºtil).
- **limites** ê¢â¬â o que o agente nunca faz.
- **nêÂ­vel de autonomia** ê¢â¬â 0 nêÂ£o toca êÂ· 1 propêÂµe êÂ· 2 faz e avisa êÂ· 3 faz sozinho.
- **chamar uma pessoa** ê¢â¬â quando o agente para e passa para alguêÂ©m da equipe.
- **caso difêÂ­cil** ê¢â¬â situaêÂ§êÂ£o + o que fazer + por quêÂª.
- **casos de teste** ê¢â¬â mensagens que vocêÂª manda ao agente para ver se ele segue a constituiêÂ§êÂ£o.
- **registro de falhas** ê¢â¬â data, o que quebrou, a menor correêÂ§êÂ£o, se era texto ou sistema.
- Onde fica o documento: "o documento **ConstituiêÂ§êÂ£o do agente** nas Notas do celular ou num documento do computador" (criado na aula 2). SaêÂ­da para quem pulou: o modelo pronto da prêÂ³pria aula.

## Aulas
1. **Ordem nêÂ£o basta: o agente precisa de critêÂ©rio** ê¢â¬â tipo fundamento, prêÂ¡tica `analise`.
   Gancho: o agente que segue a regra ao pêÂ© da letra e erra. ConteêÂºdo: duas culturas da Anthropic (pessoas: propêÂ³sito/autonomia; IA: constituiêÂ§êÂ£o), o que os nêÂºmeros mostram e o que nêÂ£o provam (8êâ, 11:1, 2 pontos), as 4 prioridades do Claude, treino ê¢â°Â  instruêÂ§êÂµes (sua constituiêÂ§êÂ£o entra nas instruêÂ§êÂµes, nêÂ£o muda o modelo).
   PrêÂ¡tica: dar ao chat um caso sem regra e comparar a resposta com e sem as 4 prioridades.
2. **MissêÂ£o, prioridades e limites** ê¢â¬â prêÂ¡tica `prompt`/`tarefa`. Cria o documento. MissêÂ£o em 1ê¢â¬â2 frases; prioridades na ordem; 3 a 5 limites concretos.
3. **Quanto o agente faz sozinho e quando chama uma pessoa** ê¢â¬â nêÂ­veis 0ê¢â¬â3, tabela de aêÂ§êÂµes, regras de chamar uma pessoa (sofrimento/risco, fora da missêÂ£o ou limite, falta informaêÂ§êÂ£o e o erro custa caro, errou 2êâ), quem e em quanto tempo.
4. **Casos difêÂ­ceis com o porquêÂª** ê¢â¬â situaêÂ§êÂ£o, o que fazer, por quêÂª (apontando a prioridade ou o limite). MêÂ­nimo 3. Rascunho com o chat a partir do prompt-rascunho do kit, sem inventar regra.
5. **Testar e revisar em ciclo** ê¢â¬â colar a constituiêÂ§êÂ£o no inêÂ­cio de uma conversa nova (ou nas instruêÂ§êÂµes de um Projeto/GPT), mandar os 8 casos de teste, marcar ok/falhou, registro de falhas, regra: mudanêÂ§a sêÂ³ entra se os casos nêÂ£o pioram; data de revisêÂ£o.

## Tempo
~15 min por aula, 5 aulas, sem mêÂ³dulos. Tema papel. Cenas: pessoas reais, sem robêÂ´.
