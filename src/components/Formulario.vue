<!-- <template>
    
    <form @submit.prevent="cadastraTarefa">
        <div class="row">
            <div class="col">
                <input :value="estado.tarefaTemp" @change="evento => estado.tarefaTemp = evento.target.value" required
                    type="text" name="" id="" placeholder="Digite aqui a descrição da tarefa" class="form-control">
            </div>
            <div class="col-md-2">
                <button type="submit" class="btn btn-primary">Cadastrar</button>
            </div>
            <div class="col-md-2">
                <select @change="evento => estado.filtro = evento.target.value" class="form-control">
                    <option value="todas">Todas as tarefas</option>
                    <option value="pendentes">Pendentes</option>
                    <option value="finalizadas">Finalizadas</option>
                </select>
            </div>
        </div>
    </form>
</template> -->


<script setup>
    const props = defineProps(['tarefaTemp', 'cadastraTarefa', 'trocarFiltro', 'editaTarefaTemp']);
</script>

<template>
    <form @submit.prevent="props.cadastraTarefa">
        <div class="row">
            <div class="col">
                <input :value="props.tarefaTemp" @change="props.editaTarefaTemp" required
                    type="text" class="form-control" placeholder="Digite sua tarefa">
            </div>
            <div class="col-md-2">
                <button type="submit" class="btn btn-primary">Adicionar</button>
            </div>
            <div class="col-md-2">
                <select @change="props.trocarFiltro" class="form-control">
                    <option value="todas">Todas as tarefas</option>
                    <option value="pendentes">Pendentes</option>
                    <option value="finalizadas">Finalizadas</option>
                </select>
            </div>
        </div>
    </form>
</template>

