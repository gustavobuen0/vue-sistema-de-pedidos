<template>
  <div>
    <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
    <p>Utilizo essas tecnologias: {{ tecnologias }}</p>
    <Info />
    <Form />
  </div>
</template>

<script>
import Info from "./Info";
import Form from "./Form";

export default {
  name: 'Pessoa',
  data() {
    return {
      nome: "Gustavo",
      tecnologias: "PHP, Laravel, Vue.js, Tailwind, Bootstrap",
    };
  },
  components: {
    Info,
    Form
  },
};
</script>