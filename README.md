# stickymessage

Mensagem que gruda no fim de um canal. Criado pra **testar a capacidade do framework** sora (componentsv2, eventos, persistência), não pra um cliente específico.

Módulo do bot de Discord construído sobre o framework **sora**. Foi criado pra ser usado em cima dele: a pasta do módulo vai em `src/usermodules/` e o loader a carrega sozinho, sem registro manual.

## O que faz

Reposta a mensagem configurada sempre que alguém escreve no canal, mantendo-a como a última. Suporta blocos separados por `---`, cor de destaque e cooldown. Desativa a sticky de um canal após falhas de envio seguidas.

Comando: `stickymessage` com os subcomandos `add`, `edit`, `remove`, `list` e `cooldown`.

## Instalação

Clone este repositório dentro de `src/usermodules/` do seu projeto sora e reinicie o bot (ou use `!bot reload`). O nome da pasta não importa: o módulo é identificado pelo `name` do cog (`stickymessage`).

## Banco

As migrations rodam sozinhas no carregamento do módulo (Postgres do framework).
