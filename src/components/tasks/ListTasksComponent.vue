<template>
    <div>
        <h1>{{title}}</h1>
            <table class="table table-striped">
                <thead class="thead-dark">
                    <tr>
                        <th>#</th>
                        <th>Nome</th>
                        <th width="180px">Ação</th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="(item, index) in tasks" :key="index">
                        <td>{{item.id}}</td>
                        <td>{{item.name}}</td>
                        <td>
                            <a href="">Editar</a> | 
                            <a href="">Deletar</a>
                        </td>
                    </tr>
                </tbody>
            </table>
    </div>
</template>

<script>
export default {
    data() {
        return {
            title: 'Lista de Tarefas',
            tasks:[]
        }
    }
}
</script>

<style scoped>
   
</style>
