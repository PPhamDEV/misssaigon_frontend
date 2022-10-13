
<script>
export default {
    components: {
    
    },
    data() {
        return {
            menu: {
                m1: {
                    number: 1,
                    desc: "Krabben Chips",
                    price: 3.60
                },
                m2: {
                    number: 2,
                    desc: "Vegetarische Minifrühlingsrollen",
                    price: 3.60
                },
                m3: {
                    number: 3,
                    desc: "Gebackenes Hühnerfleisch",
                    price: 3.60
                }
            }

        }
    },
    methods: {
        onClickChild(value) {
            this.$emit('clickedKey', value);
        }
    }


}
</script>


<template>
    <div>
        <button @click="onClickChild(menu.m1.number)">{{menu.m1.number}}. {{menu.m1.desc}}</button>
    </div>
    
</template>