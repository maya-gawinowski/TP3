<template>
    <Button @click="handleClick">{{buttonText}}</Button>
</template>

<script>
export default {
    props: {
        buttonText: {
            type: String,
            default: () => "Label"
        },
    },
    methods: {
        handleClick() {
            console.log("Hello World");
        },
    },
};
</script>
