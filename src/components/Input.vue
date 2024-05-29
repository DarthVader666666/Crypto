<template>
    <ul>
        <li>
            <input min="0" type="number" @input="changeAmount($event.target.value)" placeholder="Enter number">
        </li>
        <li>
            <button @click="convert()">Convert</button>    
        </li>
    </ul>
</template>

<script>
export default {
    props: {
        changeAmount: {
            type: Function,
            required: true
        },
        convert: {
            type: Function,
            required: true
        }
    }
}
</script>

<style scoped>
    input {
        position: relative;
        outline: none;
        width: 500px;
        top: -50px;
        font-size: 1.25em;
        border-radius: 5px;
        border: 4px solid #1a032d;
        padding: 15px 20px;
        background: #fafafa;
        color: #333;
    }

    button {
        position: relative;
        top: -20px;
        padding: 15px 20px;
        color: #fff;
        text-transform: uppercase;
        cursor: pointer;
        background: #1a032d;
        border: 0;
        border-radius: 3px;
    }

    ul {
        list-style: none;
        padding: 0;
    }
</style>