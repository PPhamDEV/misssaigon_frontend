<script>
import KeyPanel from "./KeyPanel.vue";

export default {
    components: {
        KeyPanel,
    },
    props: {
        input: String,
    },
    data() {
        return {
            post: {
                displayValue: ""
            }

        }
    },
    methods: {
        setDisplayValue(value) {
            this.post.displayValue += value
        }
    }

}
</script>

<template>

    <div>
        <h1 id="titel">Miss Saigon</h1>
        <strong>{{post.displayValue}}</strong>
        <KeyPanel @clickedKey="setDisplayValue"></KeyPanel>
    </div>

</template>