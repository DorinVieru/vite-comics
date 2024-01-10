<!-- SEZIONE JS SCRIPT -->
<script>
export default {
    name: "AppJumbo",

}
</script>

<!-- SEZIONE HTML -->
<template lang="">
<div class="container-fluid jumbo">
    <button type="button" class="btn btn-primary btn-lg button-series">CURRENT SERIES</button>
</div>  
</template>

<!-- SEZIONE STYLE -->
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.jumbo{
    background-image: url('../assets/img/jumbotron.jpg');
    background-size: cover;
    height: 500px;
}

.button-series{
    position: absolute;
    top: 590px;
    left: 175px;
    
}

</style>