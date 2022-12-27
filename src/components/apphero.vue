<template>
    <div class="hero">
        <section>
            <h1><span>Muhammad</span> Asim</h1>
            <h4>Web Developer</h4>
            <button><a href="">Get In Touch</a>
            </button>
        </section>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'app-hero'
})
</script>

<style scoped>
section {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
h1 {
    height: 0px;
    color: #00d4bd;
    font-size: 50px;
}
span {
    color: white;
}
h4 {
    color: #00d4bd;
    font-size: 30px;
}

button {
    width: 200px;
    height: 50px;
    border: 1px solid;
    border-radius: 20px;
    background-color: #057e70;
   }
   button a {
    text-decoration: none;
    color: white;
    font-size: 20px ;
   }
   button:hover{
    background: #00d4bd;
    transform: translateX(20px);
    transition: 2s;
   }
</style>
