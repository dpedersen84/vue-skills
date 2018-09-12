<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key='index'>{{ index + 1 }}. {{ data.skill }}</li>
      </ul>

      <!-- <p v-if="skills.length >=3">You have at least 3 skills</p>
      <p v-else>You have less than 3 skills</p> -->
      <p>These are the skills that you possess.</p>
      <!-- <div v-bind:class="{ alert: showAlert, 'another-class': showClass }"></div> -->
      <!-- <div v-bind:class="alertObject"></div> -->
      <!-- <div v-bind:style="{ backgroundColor: bgColor, width: bgWidth, height: bgHeight }"></div> -->
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      skills: [
        { "skill": "Vue.js" },
        { "skill": "Developer" },
        { "skill": "Rock, paper, scissors" }
      ],
      // showAlert: true,
      // showClass: true,
      // alertObject: {
      //   alert: true,
      // }
      bgColor: 'red',
      bgWidth: '100%',
      bgHeight: '30px'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* .alert {
  background-color: yellow;
  width: 100%;
  height: 30px;
}
.another-class {
  border: 5px solid black;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
} */
.holder {
  background: #fff;
}
ul {
  margin: 0;
  padding: 0;
  list-style-type: none;
}

ul li {
  padding: 20px;
  font-size: 1.3em;
  background-color: #E0EDF4;
  border-left: 5px solid #3EB3F6;
  margin-bottom: 2px;
  color: #3E5252;
}
p {
  text-align:center;
  padding: 30px 0;
  color: gray;
}
</style>
