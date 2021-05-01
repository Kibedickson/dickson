<template>
  <p class="text-sm">
    <span class="font-bold">Solution driven</span> Web Developer adept at contributing to a
    <span class="font-bold">highly collaborative </span> work environment, finding
    <span class="font-bold">solutions</span> and determining
    <span class="font-bold">customer satisfaction.</span> Working in
    <span class="font-bold">web domain</span> for
    <span class="font-bold">more than {{ yearsOfExperience }} years</span> and
    have expert level expertise in
    <span class="font-bold">Laravel, Vue</span> stack.
  </p>
</template>

<script>
export default {
  name: 'ProfessionalSummary',
  computed: {
    yearsOfExperience () {
      return new Date().getFullYear() - 2020;
    },
  },
};
</script>
