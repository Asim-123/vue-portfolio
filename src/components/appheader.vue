<template>
  <div class="header">
    <header>
      <div class="head">
        <h1><span>M</span> Asim</h1>
        <img
          src="../assets/icon1.png"
          alt=""
          width="50"
          height="50"
        />
      </div>

      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Portfolio</a></li> 
          <li><a href="#">Contact</a></li>
          <li><a href="#">Download CV</a></li>
        </ul>
      </nav>
      <button><a href="#">Hire Me</a></button>
    </header>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "app-header",
})
</script>

<style scoped>
:root {
  --primarycolor: #00d4bd;
}
header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background: #000000;
}

.head {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.head img {
  display: none;
}

h1 {
  color: white;
}
h1 span {
  color: rgb(77, 19, 238);
}
nav ul {
  display: flex;
}
nav ul li {
  list-style: none;
  margin-left: 20px;
  font-size: 20px;
  font-weight: 10;
}
nav ul li a:hover {
  color: #00d4bd;
  transition: 2s;
}
nav ul li a {
  text-decoration: none;
  color: white;
}
button {
  width: 100px;
  height: 50px;
  border: 1px solid;
  border-radius: 20px;
  background-color: #057e70;
}
button a {
  text-decoration: none;
  color: white;
  font-size: 15px;
}

button:hover {
  background: #00d4bd;
  transform: translateX(20px);
  transition: 2s;
}


@media only screen and (max-width: 768px) {
  header {
    display: flex;
    flex-direction: column;
  }
  header h1 {
    display: flex;
    margin-left: 50px;
    width: 400px;
  }
  nav ul {
    display: none;
    flex-direction: column;
  }
  button {
    display: none;
    margin-left: 30px;
  }
  img {
    flex: none;
  }
  .head img {
    display: flex;
  }
}
</style>
