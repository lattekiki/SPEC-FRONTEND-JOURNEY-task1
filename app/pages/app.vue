<script setup>
import BaseCard from '@/components/BaseCard.vue'
const route= useRoute()
</script>
<template>
  <div v-if="route.path === '/'" class="portfolio-wrapper">
    <section class="hero">
      <div class="logo-container">
        <span class="letter p-special">P</span>
        <span class="letter o-tilt">O</span>
        <span class="letter r-tilt">R</span>
        <span class="letter t-tilt">T</span>
        <img src="/hawi.png2.png" class="hero-image" />
        <span class="letter f-special">f</span>
        <span class="letter o2-tilt">O</span>
        <span class="letter l-tilt">L</span>
        <span class="letter i-tilt">I</span>
        <div class="o-badge-wrapper">
          <span class="letter">O</span> 
        </div>
      </div>

    </section>
    <p class="name">HAWI K. BACHA</p>
  <div class = "content">
    <img src = "/hawi_id.png" class="id">
    <div class="content-text">
      <h3 class="name_bold">Hi, I am Hawi</h3>
       <p>
       I am a Software Engineering student at Jimma University.
        My passion is solving problems using AI and I am working to dive deeper into the area. 
     </p>
     </div>
   </div>
   <div class="ProjectCard">
   <BaseCard
         title="Projects" 
         image="/Projects.jpg"
         to="/projects"/>
   <BaseCard
       title="Background"
       image="/Education.jpg"
       to="/background"/>
   <BaseCard
       title="Contacts"
       image="/Contacts.jpg"
       to="/SocialLink"/>
    
  </div>
  </div>  
  <NuxtPage/>
</template>
<style>
.ProjectCard{
  display: flex;
  flex-direction: row;
}
.project-container{
     background-color: rgb(255, 255, 255);
  border: 2px solid #ce50a8;
  border-radius: 10px;
  margin-top: 10px;
  margin-left: 500px;
  font-size: larger;
  color:rgb(0, 0, 0);
  font-weight: 1000;
  width:200px;

}
.name_bold{
  font-weight: 800;
  color: #ce50a8;
}
.portfolio-wrapper {
  background: #fff;
  }

.content{ 
    display: flex;             
    align-items: center;       
    gap: 15px;
}
.content img {
    width: 300px;           
    height: auto;              
    border-radius: 8px;     
}
.content-text{
  max-width: 650px;
  margin: 60px auto; 
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  text-align: left;
  font-size: 20px;
}
.id{
  margin-left:50px;
}
.name{
   background-color: rgb(255, 255, 255);
  border: 2px solid #ce50a8;
  border-radius: 10px;
  margin-top: 10px;
  margin-left: 500px;
  font-size: larger;
  color:rgb(0, 0, 0);
  font-weight: 1000;
  width:200px;
  text-align: center;
}
.hero {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 50vh; 
}

.logo-container {
  display: flex;
  align-items: center;
  justify-content: center;
  letter-spacing: 10px; 
    z-index: 1;
}

.logo-container .hero-image {
  width: 250px;
  height: auto;
  z-index: 2;
  margin: 0 -20px; 
  display: inline-block;
  transform: translateY(15px);
}

.letter {
  font-size: clamp(3rem, 10vw, 7rem); 
  font-weight: 900;
  display: inline-block;
  z-index: 2;
}

.f-special {
  font-size: clamp(4rem, 12vw, 8.5rem);
  transform: rotate(10deg) translateY(-15px);
  margin: 0 -10px;
}
.p-special {
  font-size: clamp(4rem, 12vw, 8.5rem);
  transform: rotate(-10deg) translateY(15px);
  margin: 0 -15px;
}

.o-badge-wrapper {
  position: relative;
  display: flex;
}

</style>