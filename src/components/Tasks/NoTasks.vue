<template>
	<q-banner class="bg-grey-3">
    <template v-slot:avatar>
      <q-icon name="check" color="primary" />
    </template>
    Nenhuma Tarefa Agendada para Hoje
    <template v-slot:action>
      <q-btn
        @click="$root.$emit('showAddTask')"
      	flat
      	color="primary"
      	label="Adicionar Tarefa" />
    </template>
  </q-banner>
</template>

<script>
	export default {
	
	}
</script>