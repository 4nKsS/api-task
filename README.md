# API de Tarefas

A API permite gerenciar tarefas com operações de criação, listagem, atualização e exclusão.

---

## Exemplo de corpo (JSON)
- **id**: (Integer) Identificador único da tarefa (gerado automaticamente).  

 - **nome**: (String) O nome da tarefa.

 - **dataEntrega**: (LocalDate) Data de entrega da tarefa.

 - **responsavel**: (String) Pessoa responsável pela tarefa.

```json
{
    "nome": "Estudar",
    "dataEntrega": "dd/mm/aaaa",
    "responsavel": "Pedro"
}
```

## Adicionar Tarefa

- **Método:** `POST` 
- **URL:** `http://localhost:8080/tarefas`
- **Resultado esperado:** `Criar uma nova tarefa e retornar os detalhes salvos.`

## Listar Tarefas

- **Método:** `GET` 
- **URL:** `http://localhost:8080/tarefas`
- **Resultado esperado:** `Listar todas as Tarefas salvas.`

## Atualizar Tarefa

- **Método:** `PUT` 
- **URL:** `http://localhost:8080/tarefas/{id}`
- **Resultado esperado:** `Atualizar a tarefa correspondente ao id informado.`

## Excluir Tarefa
- **Método:** `DELETE`
- **URL:** `http://localhost:8080/tarefas/{id}`
- **Resultado esperado:** `Remove a tarefa com o id informado.`
