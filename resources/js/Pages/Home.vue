<template>
    <h1>Home</h1>
    <Nav></Nav>
    <p>
    <ul>
        <li v-for="framework of frameworks" v-text="framework"></li>
    </ul>
    </p>
</template>

<script>
import Nav from "../Shared/Nav"
export default {
    components: { Nav },
    props: {
        name: String,
        frameworks: Array
    }
}
</script>