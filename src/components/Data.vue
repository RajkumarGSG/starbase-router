<template>
    <div class="">
        Type: {{ type }}<br>
    </div>
</template>

<script>
export default {
    data() {
        return {
            type: this.$route.params.type
        }
    },
    watch: {
        '$route': 'change'
    },
    methods: {
        change() {
            this.type = this.$route.params.type;
        }
    }
}
</script>