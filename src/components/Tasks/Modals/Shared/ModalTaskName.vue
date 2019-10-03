<template>
	<div class="row q-mb-sm">
    <q-input
    	outlined
    	:value="name"
    	@input="$emit('update:name', $event)"
    	:rules="[val => !!val || 'o campo deve ser preenchido']"
    	autofocus
    	ref="name"
    	label="Nome da Tarefa"
    	class="col">
			<template v-slot:append>
        <q-icon
        	v-if="name"
        	@click="$emit('update:name', '')"
        	name="close"
        	class="cursor-pointer" />
      </template>
    </q-input>
	</div>
</template>

<script>
	export default {
		props: ['name']
	}
</script>