<template>
    <article class="">
        <slider/>
        <section class="list">
            <div class="item" v-for="item in enters" :key="item.img">
                <router-link :to="{ name: item.href }">
                    <img :src="item.img" :alt="item.title">
                    <h4>{{ item.title }}</h4>
                </router-link>
            </div>
        </section>
    </article>
</template>

<script>
    import Slider from '../../core/slider'

    export default {
        name: 'hslider',
        components: {Slider},
        data(){
            return {
                items: [],
                enters: [{
                    href:'',
                    img: '',
                    title: '',
                }]
            }
        }
    }
</script>

<style scoped>

</style>
