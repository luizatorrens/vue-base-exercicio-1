<script>
import NovoBloco from "@/components/NovoBloco.vue";
export default {
  data() {
    return {
      nomes2: ["rafael", "gabriel"],
    };
  },
  components: { NovoBloco },
};
</script>
<template>
  <main id="content">
    <NovoBloco class="alerta" />
    <NovoBloco :nomes="['Amanda', 'Antonia']" />
    <NovoBloco class="alerta" />
    <NovoBloco class="bloco" />
    <NovoBloco class="bloco" />
    <NovoBloco class="alerta" titulo="Alunos" :nomes="nomes2" />
    <NovoBloco />
    <NovoBloco class="alerta" />
  </main>
</template>
