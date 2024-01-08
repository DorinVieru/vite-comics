<!-- SEZIONE JS SCRIPT -->
<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            pages: [
                {
                    label: "CHARACTERS",
                    link: "#",
                    current: false,
                },
                {
                    label: "COMICS",
                    link: "#",
                    current: true,
                },
                {
                    label: "MOVIES",
                    link: "#",
                    current: false,
                },
                {
                    label: "TV",
                    link: "#",
                    current: false,
                },
                {
                    label: "GAMES",
                    link: "#",
                    current: false,
                },
                {
                    label: "COLLECTIBLES",
                    link: "#",
                    current: false,
                },
                {
                    label: "VIDEOS",
                    link: "#",
                    current: false,
                },
                {
                    label: "FANS",
                    link: "#",
                    current: false,
                },
                {
                    label: "NEWS",
                    link: "#",
                    current: false,
                },
                {
                    label: "SHOP",
                    link: "#",
                    current: false,
                },
            ]
        }
    },
}
</script>

<!-- SEZIONE HTML -->
<template lang="">
  <header>
    <div class="container">
        <div class="row my-2">
            <div class="col-2">
                <a href="/" class="brand">
                    <img src="../assets/img/dc-logo.png" alt="Logo DC">
                </a>
            </div>
            <div class="col-10 d-flex align-items-center justify-content-end">
                <nav>
                    <ul class="list-unstyled">
                        <li v-for="(page, index) in pages" :key="index">
                            <a :class="page.current ? 'active': ''" :href="page.link">
                                {{ page.label }}
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </div>
  </header>
</template>

<!-- SEZIONE STYLE -->
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    header{
        height: 100px;
    }

    ul{
        display: flex;
        justify-content: center;

        li a{
            text-decoration: none;
            padding: 0 10px;
            font-weight: 600;
            color: black;

            &.active,
            &.hover{
                color: $primary_color;
                font-weight: 700;
                border-bottom: 3px solid $primary_color;
            }
        }

    }
</style>