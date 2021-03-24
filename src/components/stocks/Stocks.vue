<template>
    <div>
        <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
    </div>
</template>

<script>
    import Stock from './Stock.vue'
    export default {
        data() {
            return {
                stocks: [
                    { id: 1, name:'Google', price:250 },
                    { id: 2, name:'Apple', price:300 },
                    { id: 3, name:'Samsong', price:150 },
                    { id: 4, name:'Twitter', price:100 },
                ]
            }
        },

        components: {
            appStock: Stock
        }
    }
</script>