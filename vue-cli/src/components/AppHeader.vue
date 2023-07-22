<template>
    <header>
        <h1>{{ msg }}</h1>
        <button @click="sendEvent">Send</button>
    </header>
</template>

<script>
export default {
    props: {
        msg: String
    },
    methods: {
        sendEvent: function() {
            this.$emit('renew');
        }
    }
}
</script>