<template>
    <div>
        Работает! Отобразилось содиржимое template App.vue
    </div>
    <div>
        Колличество likes: <strong>{{ likes }}</strong>
        Колличество dislikes: <strong>{{ dislikes }}</strong>
    </div>
    <button v-on:click="addLikes"> likes</button>
    <button v-on:click="addDisLikes"> dislikes</button>  
</template>

<script>
    export default {
        data() {
            return {
                likes: 0,
                dislikes: 0,
            }
        },
        methods: {
            addLikes() {
                this.likes += 1;
            },

            addDisLikes() {
                this.dislikes += 1;
            },


        }
    }
</script>

<style>
</style>