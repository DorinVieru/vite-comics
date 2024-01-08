<!-- SEZIONE JS SCRIPT -->
<script>
export default {
    name: "AppMain",
    data() {
        return {
            
        }
    },
}
</script>

<!-- SEZIONE HTML -->
<template lang="">
  <main class="d-flex align-items-center">
      <div>
      <h2 > --> Content goes here <-- </h2>
    </div>
  </main>
</template>

<!-- SEZIONE STYLE -->
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    main{
        background-color: $bg-main-color;
        height: 150px;
    }

    h2{
        color: $title_main_color;
        padding: 20px 30px;
    }
</style>