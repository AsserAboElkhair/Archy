<template>
  <div class="hello container">
     <mu-text-field hintText="Search" type="text" fullWidth icon="search"/><br/>
    <div class="row">
      <div v-for="(img) in imgs" :key="img" class="col-4">
        <mu-card>
          <mu-card-media title="Suspense Mosque" subTitle="Marceline">
            <img :src="img" />
          </mu-card-media>
          <mu-card-text>
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
          </mu-card-text>
          <mu-card-actions>
            <mu-flat-button label="Show on map" />
            <mu-flat-button label="More info" />
          </mu-card-actions>
        </mu-card>
      </div>
    </div>
    <br>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      imgs: [
        "https://i.imgur.com/AGpP2lS.jpg",
        "https://i.imgur.com/GJyGwcq.jpg",
        "https://i.imgur.com/YidfAq2.jpg"
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.mu-card-media{
position: relative;
height: 300px;
}
button {
  font-weight: bold;
}
a {
  color: #42b983;
}
img {
  width: 100%;
  height: 300px;
  object-fit: cover;
}
</style>
