<template>
    <input type="number" placeholder="Enter number">
</template>

<script>
export default {
    props: {
        changeAmount: {
            type: Function,
            required: true
        }
    }

}
</script>

<style>
    input {
        outline: none;
        width: 500px;
        position: relative;
        top: -50px;
        font-size: 1.25rem;
        border-radius: 5px;
        border: 4px solid #1a032d;
        padding: 15px 20px;
        background: #fafafa;
        color: #333;
    }
</style>