<script>
export default {
  props: {
    nomes: {
      type: Array,
    },
    titulo: {
      type: String,
      default: "Qualquer valor"
    },
  },
  data() {
    return {};
  },
};
</script>
<template>
  <article id="article" class="block">
    {{ titulo}}
    <hr />
    <ul>
      <li v-for="nome in nomes" :key="nome">{{ nome }}</li>
    </ul>
  </article>
</template>
