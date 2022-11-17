<template>
  <div class="home">
    <!-- <HelloWorld msg="Welcomee to Your Vue.js App"/> -->
    <div class="hero__wrapp">
      <span class="logo">
        <div class="cat_icon"/>
        <p class="logotext">CatGramClone</p>
      </span>
      <SearchBar/>
        <div class="user_hero"></div>
      
    </div>
    <div class="content__wrapp">
      <Left/>
      <!-- <div class="leftcontainer">Left</div> -->
      <div class="corecontainer">Core</div>
      <div class="rightcontainer">Right</div>
    </div>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'
import SearchBar from '@/components/SearchBar.vue'
import Left from '@/components/Left.vue'
export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    SearchBar,
    Left,
  }
}
</script>
<style scooped>
body{
  background-color: rgb(239, 239, 239);
  max-width: 100vw;
  margin: 0;
  padding: 0;
}
.hero__wrapp{
  background-color: #000;
  height: 20vh;
  color: white;
  display: grid;
  grid-template-columns: repeat(3,1fr);
  justify-items: center;
  align-items: center;
}
.content__wrapp{
  width: 100vw;
  display: grid;
  grid-template-columns: 25% 50% 25%;
}

.cat_icon{
  max-width: 50px;
  min-height: 50px;
  background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTMMGLxQEfdpy6t8CusncYij1V3vxA2PsHVd1TI3N74Lg&s');
  background-position: center;
  background-size: cover;
  filter: invert(100%);
  margin: 0;
  text-align: center;
  margin-left: 50px;
}
.logo {
  display: grid;
  grid-template-columns: repeat(2,1fr);
  align-items: center;
  /* justify-items: center; */
}
.logotext{
  font-style: italic;
}

.user_hero{
  width: 90px;
  height: 100px;
  background-color: rgb(240, 240, 240);
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url('https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/883af5d2-b2c0-412a-a8a3-8a3324c30914/d5ohyoq-6107c225-a442-40bc-b907-5ec4c788effb.png/v1/fill/w_539,h_724,strp/business_cat_vector_by_baronius_d5ohyoq-fullview.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9NzI0IiwicGF0aCI6IlwvZlwvODgzYWY1ZDItYjJjMC00MTJhLWE4YTMtOGEzMzI0YzMwOTE0XC9kNW9oeW9xLTYxMDdjMjI1LWE0NDItNDBiYy1iOTA3LTVlYzRjNzg4ZWZmYi5wbmciLCJ3aWR0aCI6Ijw9NTM5In1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmltYWdlLm9wZXJhdGlvbnMiXX0.SC85pFDKFuNDhy1TULcqFBAd8NxiLSINCKq8kK4jwzE');
  background-size: cover;
  background-position: center;
}
</style>
