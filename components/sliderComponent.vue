<template>
    <div>
    {{value}}
    <input
        type='range'
        :min='1'
        :max='100'
        :value='input'
        @change='emitInput'
        class='slider--component'
    />
    {{input}}
    </div>
</template>

<script>
export default {
    props: {
        value: {
            type: Number,
            required: true
        },
        min: {
            type: Number,
            default: 1
        },
        max: {
            type: Number,
            default: 100
        }
    },
    data () {
        return {
            input: this.value
        }
    },
    methods: {
        emitInput (event) {
            this.input = event.target.value
            this.$emit('input', this.input)
        }
    }
}
</script>

<style lang='scss' scoped>
.slider--component {
    width: 100%;
}
</style>
