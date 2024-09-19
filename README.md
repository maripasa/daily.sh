# daily.sh

Um pequeno script de terminal feito para automatizar a tediosa tarefa de criar dailys!

## Como Usar

Para executar o script, use o seguinte comando:

```
daily [opções] [tarefas...]
```

## Opções

- `-h, --help`                   Mostra esta mensagem de ajuda.
- `-o, -y, --ontem, --yesterday` Usa a data de ontem e altera 'hoje' para 'ontem'.
- `-n, --nome, --name <NAME>`      Altera o nome permanentemente (padrão: 'Your Name').
- `-p, --problema, --problem <TEXT>` Altera a descrição do problema (padrão: 'Não').
- `-t, --tag <SPACES>`             Define o número de espaços em branco antes da bolinha (padrão: 4).

As tarefas são as atividades que você deseja listar para o dia.

## Funcionalidades

- **Data**: O script usa a data atual por padrão, mas pode ser ajustado para "ontem".
- **Nome e Problemas**: Permite personalizar seu nome e descrever problemas.
- **Formatação**: Controla a quantidade de espaços antes dos itens da lista.
- **Copia para a área de transferência**: O resultado final é copiado automaticamente para a área de transferência para fácil acesso.

## Exemplo de Uso

Para criar uma daily com um nome e problema específicos, e listar tarefas:

```
daily -n "Seu Nome" -p "Nada" "Reunião" "Revisar código"
```

## Observações

- O script utiliza `xclip` para copiar a saída para a área de transferência. Certifique-se de que ele esteja instalado.