<!-- <script setup>
    const props = defineProps(['tarefasPendentes']);
</script>

<template>
    <header class="p-5 mb-4 mt-4 bg-light rounded-3">
        <h1>Minhas tarefas</h1>
        <p>
            Você possui {{ props.tarefasPendentes }} tarefas pendentes.  (antes, em vez de props.tarefasPendentes, era 'getTarefasPendentes().length' )
        </p>
    </header>
</template> 
-->

<script setup>
    const props = defineProps(['tarefasPendentes']);
</script>

<template>
    <header class="p-5 mb-4 mt-4 bg-light rounded-3">
        <h1>Minhas tarefas</h1>
        <p>
            Você possui {{ props.tarefasPendentes }} tarefas pendentes. <!-- antes, em vez de props.tarefasPendentes, era 'getTarefasPendentes().length' -->
        </p>
    </header>
</template>