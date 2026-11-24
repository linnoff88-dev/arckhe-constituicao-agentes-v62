# CurrÃ­culo â€” ConstituiÃ§Ã£o dos Agentes v6.2

Base: kit `linnoff88-dev/constituicao-agentes` (docs/LOGICA.md, modelo/, exemplos/clinica-atendimento.md).
NÃ£o repetir o `empresas-2027-v62` (LÃ­via, Wagner; aula 5 "A constituiÃ§Ã£o do seu agente"): aqui cada peÃ§a
da constituiÃ§Ã£o vira uma aula e o aluno sai com o documento inteiro, testado.

## Aluno
Dono, gestor ou lÃ­der de equipe de empresa pequena/mÃ©dia, 30+. JÃ¡ usa ChatGPT ou Claude no navegador e
WhatsApp. Pensa em pÃ´r um agente para atender ou operar e tem medo de que ele "faÃ§a besteira". Sem terminal.

## ProfissÃµes-alvo (data-ex)
- `coordenadora` â€” **Rosana**, coordenadora de atendimento de uma clÃ­nica (agenda, pacientes; nunca diagnÃ³stico).
- `contador` â€” **Edson**, dono de um escritÃ³rio de contabilidade (prazos, documentos de clientes; nunca orientaÃ§Ã£o fiscal personalizada).

## Promessa do curso
Sai com a **constituiÃ§Ã£o de 1 a 2 pÃ¡ginas do agente da sua empresa** â€” missÃ£o, prioridades, limites, nÃ­veis de
autonomia, quando chamar uma pessoa, 3 casos difÃ­ceis com o porquÃª â€” testada com 8 casos e com data de revisÃ£o.

## VocabulÃ¡rio fixo (um nome por conceito)
- **constituiÃ§Ã£o do agente** â€” o documento inteiro.
- **agente** â€” o assistente de IA que trabalha para a empresa (atende, marca, responde).
- **prioridades** â€” a ordem do que vale mais quando duas coisas boas brigam (seguranÃ§a, honestidade, regras da empresa, ser Ãºtil).
- **limites** â€” o que o agente nunca faz.
- **nÃ­vel de autonomia** â€” 0 nÃ£o toca Â· 1 propÃµe Â· 2 faz e avisa Â· 3 faz sozinho.
- **chamar uma pessoa** â€” quando o agente para e passa para alguÃ©m da equipe.
- **caso difÃ­cil** â€” situaÃ§Ã£o + o que fazer + por quÃª.
- **casos de teste** â€” mensagens que vocÃª manda ao agente para ver se ele segue a constituiÃ§Ã£o.
- **registro de falhas** â€” data, o que quebrou, a menor correÃ§Ã£o, se era texto ou sistema.
- Onde fica o documento: "o documento **ConstituiÃ§Ã£o do agente** nas Notas do celular ou num documento do computador" (criado na aula 2). SaÃ­da para quem pulou: o modelo pronto da prÃ³pria aula.

## Aulas
1. **Ordem nÃ£o basta: o agente precisa de critÃ©rio** â€” tipo fundamento, prÃ¡tica `analise`.
   Gancho: o agente que segue a regra ao pÃ© da letra e erra. ConteÃºdo: duas culturas da Anthropic (pessoas: propÃ³sito/autonomia; IA: constituiÃ§Ã£o), o que os nÃºmeros mostram e o que nÃ£o provam (8Ã—, 11:1, 2 pontos), as 4 prioridades do Claude, treino â‰  instruÃ§Ãµes (sua constituiÃ§Ã£o entra nas instruÃ§Ãµes, nÃ£o muda o modelo).
   PrÃ¡tica: dar ao chat um caso sem regra e comparar a resposta com e sem as 4 prioridades.
2. **MissÃ£o, prioridades e limites** â€” prÃ¡tica `prompt`/`tarefa`. Cria o documento. MissÃ£o em 1â€“2 frases; prioridades na ordem; 3 a 5 limites concretos.
3. **Quanto o agente faz sozinho e quando chama uma pessoa** â€” nÃ­veis 0â€“3, tabela de aÃ§Ãµes, regras de chamar uma pessoa (sofrimento/risco, fora da missÃ£o ou limite, falta informaÃ§Ã£o e o erro custa caro, errou 2Ã—), quem e em quanto tempo.
4. **Casos difÃ­ceis com o porquÃª** â€” situaÃ§Ã£o, o que fazer, por quÃª (apontando a prioridade ou o limite). MÃ­nimo 3. Rascunho com o chat a partir do prompt-rascunho do kit, sem inventar regra.
5. **Testar e revisar em ciclo** â€” colar a constituiÃ§Ã£o no inÃ­cio de uma conversa nova (ou nas instruÃ§Ãµes de um Projeto/GPT), mandar os 8 casos de teste, marcar ok/falhou, registro de falhas, regra: mudanÃ§a sÃ³ entra se os casos nÃ£o pioram; data de revisÃ£o.

## Tempo
~15 min por aula, 5 aulas, sem mÃ³dulos. Tema papel. Cenas: pessoas reais, sem robÃ´.
