<template>
  <div class="background">
      <div class="header-container">
        <header>
            <div id="header-text-container">
                <div id="headerText">
                    Community Collections
                </div>
            </div>
        </header>
      </div>
      <div>
        <allCollections />
      </div>
  </div>
</template>

<script>
import allCollections from '@/components/AllCollections.vue'
export default {
    components: {
        allCollections
    }
}
</script>

<style scoped>
header {
  display: flex;
  font-size: 60px;
}

img {
  border-radius: 40px;
  height: 20%;
  margin-left: 750px;
  position: fixed;
}

.header-container {
  text-align: center;
}
#headerText {
  font-size: 65px;
  font-family: 'PT Serif';
  color: #eee;
  text-shadow: -1px 1px 0 maroon,
                1px 1px 0 #000,
                1px -1px 0 #000,
               -1px -1px 0 #000;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  border-radius: 20px;
  margin-top: 20px;
  position: static;
}

#header-text-container {
  height: 100px;
  width: 1800px;
  position: fixed;
}

.background {
  background-image: url("/images/publiccollectionBG.jpg");
  height: 100vh;
  background-size: cover;
}
</style>