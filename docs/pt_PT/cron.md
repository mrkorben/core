# Mecanismo de tarefas
**Configurações → Sistema → Mecanismo de Tarefas**

Esta página informa sobre todas as tarefas do aplicativo Jeedom em execução no servidor.
Esta página deve ser usada com conhecimento ou a pedido de suporte técnico.

> **Important**
>
> Em caso de uso indevido nesta página, qualquer solicitação de suporte poderá ser recusada.

## Guia Cron

No canto superior direito, você tem :

- **Desativar o sistema cron** : um botão para desativar ou reativar todas as tarefas (se você desativá-las todas, nada funcionará no seu Jeedom).
- **Legal** : Atualiza a tabela de tarefas.
- **Ajouter** : Adicionar um trabalho cron manualmente.
- **Sauvegarder** : Salve suas alterações.

Abaixo, você tem a tabela de todas as tarefas existentes (atenção, algumas tarefas podem iniciar subtarefas, portanto, é altamente recomendável nunca modificar as informações nesta página).

Nesta tabela, encontramos :

- **\#** : ID da tarefa, útil para vincular um processo em execução ao que ele realmente faz.
- **Actif** : Indica se a tarefa está ativa (pode ser iniciada pelo Jeedom) ou não.
- **PID** : Indica o ID do processo atual.
- **Demônio** : Se esta caixa for "sim", a tarefa deve sempre estar em andamento. Além disso, você encontra a frequência do daemon, é aconselhável nunca modificar esse valor e, especialmente, nunca diminuí-lo.
- **Unique** : Se for "sim", a tarefa será iniciada uma vez e será excluída automaticamente.
- **Classe** : Class PHP chamada para executar a tarefa (pode estar vazia).
- **Fonction** : Função PHP chamada na classe chamada (ou não, se a classe estiver vazia).
- **Programmation** : Programação da tarefa no formato CRON.
- **Timeout** : Tempo máximo de execução da tarefa. Se a tarefa for um daemon, ela será automaticamente interrompida e reiniciada no final do tempo limite.
- **último lançamento** : Data do último lançamento da tarefa.
- **Última duração** : Último tempo de execução da tarefa (um daemon sempre estará em 0s, não se preocupe, outras tarefas podem estar em 0s).
- **Statut** : Status atual da tarefa (como lembrete, uma tarefa daemon é sempre "executada").

- **Action** :
    - **Detalhes** : Veja o cron em detalhes (conforme armazenado na base).
    - **Iniciar / Parar** : Iniciar ou parar a tarefa (dependendo do status).
    - **Suppression** : Excluir tarefa.


## Guia Ouvinte

Os ouvintes são apenas visíveis na leitura e permitem que você veja as funções chamadas em um evento (atualização de um comando ...).

## Guia Demon

Tabela de resumo dos demônios com seu estado, a data do último lançamento, bem como a possibilidade de
- Iniciar / reiniciar um daemon.
- Pare um daemon se o gerenciamento automático estiver desativado.
- Ativar / desativar o gerenciamento automático de um daemon.

> Dica
> Demônios de plugins desativados não aparecem nesta página.