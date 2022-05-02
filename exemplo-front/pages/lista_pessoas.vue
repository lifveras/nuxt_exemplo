<template>
  <div class="container">
      <h1>{{titulo}}</h1>
      <ul>
          <li :key="item.id" v-for = "item in pessoas">
              <!-- Saída: Marcio -> 18 anos -->
              {{item.nome}} -> {{item.idade}} anos
          </li>
      </ul>
      <button>Clique aqui</button>
  </div>
</template>

<script>
export default {
    data: function (){
        return {
            titulo: "Lista de pessoas e idades",
            pessoas: [
                {id: 1, nome: "Marcio", idade: 18},
                {id: 2, nome: "Carla", idade: 25},
                {id: 3, nome: "Lais", idade: 30},
                {id: 4, nome: "Carla", idade: 25},
                {id: 5, nome: "Lais", idade: 30},
                {id: 6, nome: "Carla", idade: 25},
                {id: 7, nome: "Lais", idade: 30},
                {id: 8, nome: "Carla", idade: 25},
            ]
        }
    }
}
</script>

<style>

</style>