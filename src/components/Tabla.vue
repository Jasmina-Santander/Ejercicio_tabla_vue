<template>
  <div class="container mt-4 ">
    <table class="table table-dark table-bordered table-striped">
      <thead>
        <tr>
          <th>Nombre</th>
          <th>Apellido</th>
          <th>Fecha de Nacimiento</th>
          <th>Edad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item,index) in items" :key="index">
          <td>{{ item.nombre }}</td>
          <td>{{ item.apellido }}</td>
          <td>{{ item.nacimiento }}</td>
          <td>{{ item.edad }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
name : 'tabla',
  data : () => ({
      items: [
        {
          nombre: "Juan",
          apellido: "Donoso",
          nacimiento: "12/09/1976",
          edad: 58,
        },
        {
          nombre: "Pedro",
          apellido: "Soto",
          nacimiento: "12/09/1970",
          edad: 52,
        },
        {
          nombre: "Raul",
          apellido: "Santos",
          nacimiento: "12/09/2000",
          edad: 22,
        },
      ],
    })
  };
</script>

<style>

</style>
