<template>
  <div class="row">
    <ul>
      <li v-for="(profesor, index) in profesores" :class="{'text-warning': isPar(index)}"> {{profesor.name}} </li>
    </ul>
  </div>
</template>

<script>
  import Profesor from '../models/Profesor';
  const profesoresList = [
    new Profesor(0, 'Alfonso'),
    new Profesor(1, 'Fran'),
    new Profesor(2, 'Jorge'),
    new Profesor(3, 'Cesar'),
    new Profesor(4, 'Juan'),
    new Profesor(5, 'Marta'),
    new Profesor(100, 'Los de empresa'),
    new Profesor(200, 'Los de FOL')
  ];
  export default {
    name: 'Profesores',
    data() {
      return {
        profesores: profesoresList
      }
    },
    methods: {
      isPar(index) {
        return index % 2 == 0;
      }
    }
  }
</script>
