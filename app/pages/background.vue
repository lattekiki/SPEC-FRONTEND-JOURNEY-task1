<template>
  <div class="background-page">
    <!-- Back Button -->
    <NuxtLink to="/" class="back-btn">← Back</NuxtLink>

    <div class="container">
      <header class="header">
        <h1>Background</h1>
      </header>

      <section class="section">
        <h2>About Me</h2>
        <p>
          I am passionate about technology and problem solving, with an interest in software
          development, data science, and artificial intelligence. I enjoy building real-world
          applications that are both functional and user-friendly.
        </p>
      </section>

      <section class="section">
        <h2>Education</h2>
        <p>
          Currently studying Software Engineering at Jimma University.
        </p>
      </section>
      <section class="section">
        <h2>Certificates</h2>
        <ul>
            <li> CS50P: Introduction to Programming- HarvardX</li>
            <li> Android Application Development Fundamentals- Udacity</li>
            <li> Artificial Intelligence Fundametals- Udacity</li>
        </ul>
      </section>

      <section class="section">
        <h2>Career Interests</h2>
        <p>
          I am interested in building modern applications, AI-powered tools, and data-driven
          solutions that improve everyday processes.
        </p>
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
  padding-bottom: 50px;
  background-image: url("/bg.jpg");
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
  margin-bottom: 40px;
}

.header h1 {
  font-size: 2.3rem;
  font-weight: 800;
  color: #111827;
}

.header p {
  margin-top: 8px;
  font-size: 1rem;
  color: #6b7280;
  line-height: 1.6;
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
