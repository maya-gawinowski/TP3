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
        color: {
            type: String,
            default: () => "primary"
        }
    },
    methods: {
        handleClick() {
            console.log("Hello World");
        },
    },
};
</script>

<style scoped>
    .buttonprimary {
        background-color: #42b983
    }

    .buttonprimary:hover{
        background-color: #4cce93;
    }

    .buttonwarn {
        background-color: #ff5722;
    }

    .buttonwarn:hover {
        background-color: #ff7043;
    }

    .buttondanger {
        background-color: #e53935;
    }

    .buttondanger:hover {
        background-color: #ef5350;
    }
</style>