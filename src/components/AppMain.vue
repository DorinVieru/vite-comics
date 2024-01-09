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
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1 > --> Content goes here <-- </h1>
            </div>
        </div>
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

    h1{
        color: $title_main_color;
    }
</style>