<template>
    <div>
        <h2>{{ title }}</h2>
        <p><button @click="increment">+1</button> {{ count }} </p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            title: "Counter",
            count: 0
        }
    },
    methods: {
        increment() {
            this.count += 1;
            this.$emit("add", this.count);
        }
    }
}
</script>