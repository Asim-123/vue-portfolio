<template>
  <div class="about-us">
    <h1 class="about-heading">About us</h1>
    <section>
      <div class="about-section">
        <img
          src="../assets/img2.jpg"
          alt="about us Image"
          width="501"
          height="500"
        />
        <div class="right-section">
          <h1>Muhammad Asim</h1>
          <h4>Web Developer</h4>
          <p>
            Why you can put trust in me: 4 years of experience with website
            application development Complete work on time Worked with clients
            from all over the world Provide Clean and well-commented code to the
            client for future reference My process for developing any projects:
            Discuss requirements with clients Wire framing App flow website
            design Development Test the app before delivery Maintenance and long
            term support.
          </p>
          <button><a href="">Download CV</a></button>
        </div>
      </div>
    </section>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "app-about",
});
</script>

<style scoped>
.about-us {
  margin: 0px;
  height: 100vh;
}

.about-heading {
  color: white;
  font-size: 40px;
}

h1 {
  color: white;
  font-size: 40px;
}
h4 {
  color: #00d4bd;
  font-size: 35px;
}

p {
  color: white;
  line-height: 30px;
  letter-spacing: 1px;
}
.about-heading {
  display: flex;
  justify-content: center;
}
.about-section {
  display: flex;
  justify-content: space-around;
  margin-top: 90px;
}
.right-section {
  width: 40%;
}
button {
  margin-top: 20px;
  width: 200px;
  height: 50px;
  border: 1px solid;
  border-radius: 20px;
  background-color: #057e70;
}
button a {
  text-decoration: none;
  color: white;
  font-size: 20px;
}
button:hover {
  background: #00d4bd;
  transform: translateY(20px);
  transition: 2s;
}

@media only screen and (max-width: 768px) {
  .about-section {
    display: flex;
    flex-direction: column;
  }
  .right-section {
    text-align: center;
    width: 600px;
  }
  p {
  color: white;
  line-height: 20px;
  width: 700px;
}
img {
  display: flex;
  width: 300px;
}

}
</style>
