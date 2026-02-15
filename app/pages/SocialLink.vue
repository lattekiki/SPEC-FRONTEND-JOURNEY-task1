<template>
  <div class="background-page">
    <!-- Back Button -->
    <NuxtLink to="/" class="back-btn">← Back</NuxtLink>

    <div class="container">
      <header class="header">
        <h1>Contact Info</h1>
        <img src="/hawi_colored.jpg">
      </header>

      <section class="section">
        <h2> Linkedin</h2>
        <a href="https://www.linkedin.com/in/hawi-ketema-24b86824b/"> Check out here</a>
      </section>

      <section class="section">
        <h2>Github</h2>
        <a href="https://github.com/lattekiki">Check out here</a>
      </section>
      <section class="section">
        <h2>Email</h2>
        <p>hawiketema1998@gmail.com</p>
      </section>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.background-page {
  min-height: 100vh;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  background-image: url("/main.jpg");
}

/* Container */
.container {
  max-width: 900px;
  margin: auto;
  padding: 50px 20px;
}

/* Back Button */
.back-btn {
  display: inline-block;
  margin: 20px;
  padding: 10px 16px;
  border-radius: 10px;
  font-weight: 600;
  text-decoration: none;
  background: #ffe4f1;
  color: #db2777;
  transition: 0.2s ease;
}

.back-btn:hover {
  background: #fbcfe8;
}

/* Header */
.header {
    display:flex;
    flex-direction: row;
  margin-bottom: 40px;
}
.header img{
    width:20%;
}

.header h1 {
  font-size: 2.3rem;
  font-weight: 800;
  color: #ffffff;
}

/* Section */
.section {
  background: #fafafa;
  border: 1px solid #f3f4f6;
  border-radius: 14px;
  padding: 22px;
  margin-bottom: 18px;
}

.section h2 {
  font-size: 1.2rem;
  font-weight: 800;
  color: #db2777;
  margin-bottom: 10px;
}

.section p {
  font-size: 0.95rem;
  color: #374151;
  line-height: 1.7;
}
</style>
