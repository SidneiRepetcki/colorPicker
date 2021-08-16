<template>
  <div id="app">
    <square :initialSelectedColor="initialColor" :colorPickerOptions="selectableColors" />
  </div>
</template>

<script>
import square from './components/Square.vue';

export default {
  name: 'App',
  components: {
    square,
  },
  data() {
    return {
      initialColor: {
        name: 'PRETO',
        color: '#000000',
      },
      selectableColors: [
        {
          name: 'ROXO',
          color: '#6f56f6',
        },
        {
          name: 'VERDE',
          color: '#00e285',
        },
        {
          name: 'AMARELO',
          color: '#ffb858',
        },
        {
          name: 'ROSA ESCURO',
          color: '#ff1261',
        },
        {
          name: 'ROSA CLARO',
          color: '#ffa8c1',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: 'Quicksand', sans-serif;
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
