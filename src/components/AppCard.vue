<!-- SEZIONE JS SCRIPT -->
<script>
export default {
    name: "AppCard",
    props: {
        comic: Object,
    }
}
</script>

<!-- SEZIONE HTML -->
<template lang="">
    <div class="col-2">
        <!-- COMIC CARD -->
        <div>
            <div class="comic-img">
                <img :src="comic.thumb" :alt="comic.series">
                <span class="my-price">{{ comic.price }}</span>
            </div>
            <div>
                <h5>{{ comic.series }}</h5>
            </div>
        </div>
    </div>
</template>

<!-- SEZIONE STYLE -->
<style lang="scss" scoped>
@use '../styles/generals.scss' as *;
@use '../styles/partials/variables' as *;

// SECTION CARD

h5 {
    color: $title_main_color;
    text-transform: uppercase;
    font-size: 14px;
}

.my-price {
    color: $title_main_color;
    background-color: $primary_color;
    padding: 2px 7px;
    font-size: 13px;
    border-radius: 10px;
    position: relative;
    bottom: 220px;
    left: 153px;
}

.comic-img {


    img {
        width: 190px;
        height: 230px;
        object-fit: cover;
        object-position: top;
        border-radius: 10px;
    }

}
</style>