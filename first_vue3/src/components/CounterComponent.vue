<script>
export default {
    props: {
        initial: Number,
        increment: Number
    },
    data() {
        return {
            count: 0
        }
    },
    created: function() {
        this.count = this.initial;
    },
    methods: {
        incrementHandler() {
            this.count += this.increment;
        }
    }
}
</script>

<template>
  <button @click="incrementHandler">You clicked me {{ count }} times.</button>
</template>