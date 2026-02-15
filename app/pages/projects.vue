<template>
  

  <div class="projects-page">
    <div class="container">
<!-- Back Button -->2
  <NuxtLink to="/" class="back-btn">← Back to Dashboard</NuxtLink>
      <!-- Page Title -->
      <header class="page-header">
        <h1>My Projects</h1>
              </header>

      <div class="grid lg:grid-cols-3 gap-8">

        <!-- Left Column -->
        <aside class="space-y-6">

          <!-- Technical Skills -->
          <div class="card">
            <h3 class="card-title">Technical Skills</h3>
            <div class="tags">
              <span class="tag">Python</span>
              <span class="tag">SQL</span>
              <span class="tag">C++</span>
              <span class="tag">Data Analysis</span>
              <span class="tag">Kotlin</span>
            </div>
          </div>

          <!-- Tools & Platforms -->
          <div class="card">
            <h3 class="card-title">Tools & Platforms</h3>
            <div class="tags">
              <span class="tag">Streamlit</span>
              <span class="tag">Nuxt 3</span>
              <span class="tag">LLMs (RAG)</span>
              <span class="tag">HTML / CSS / JS</span>
            </div>
          </div>
          <div class="card">
            <h3 class="card-title">Career Focus</h3>
            <p class="text-gray-600 text-sm leading-relaxed">
              Passionate about building intelligent systems, modern web apps,
              and AI-driven tools that solve real-world problems.
            </p>
          </div>
        </aside>
        <main class="lg:col-span-2 space-y-6">
          <h2 class="section-heading">Portfolio Projects</h2>

          <!-- Project 1 -->
          <div class="project-card">
            <h4 class="project-title">Intelligent Chat Agent</h4>
            <p class="project-subtitle">RAG + Streamlit + LLM</p>

            <ul class="project-list">
              <li>
                Developed a Retrieval-Augmented Generation (RAG) agent using an LLM to analyze
                text and interact with users via a Streamlit chat interface.
              </li>
            </ul>
          </div>

          <!-- Project 2 -->
          <div class="project-card">
            <h4 class="project-title">Dynamic Data Explorer</h4>
            <p class="project-subtitle">Streamlit + Data Visualization</p>

            <ul class="project-list">
              <li>
                Created a Streamlit application that takes CSV files and generates interactive
                data visualizations, allowing users to ask natural language questions about the insights.
              </li>
            </ul>
          </div>

          <!-- Project 3 -->
          <div class="project-card">
            <h4 class="project-title">Professional Web Presence</h4>
            <p class="project-subtitle">Streamlit + GitHub + HTML/CSS/JS</p>

            <ul class="project-list">
              <li>
                Built and deployed both a static resume web app (using Streamlit) and a simple,
                engaging birthday card website (using HTML, CSS, and JavaScript on GitHub).
              </li>
            </ul>
          </div>

        </main>

      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.projects-page {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  background-image: url("/bg_project.jpg");
}

/* Container */
.container {
  max-width: 1100px;
  margin: auto;
  padding: 40px 20px;
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
  transition: 0.2s;
}

.back-btn:hover {
  background: #fbcfe8;
}

/* Header */
.page-header {
  margin-bottom: 35px;
}

.page-header h1 {
  font-size: 2.2rem;
  font-weight: 800;
  color: #ffffff;
}

.page-header p {
  margin-top: 6px;
  color: #6b7280;
  font-size: 0.95rem;
}

/* Section heading */
.section-heading {
  font-size: 1.5rem;
  font-weight: 800;
  color: #ffffff;
  border-left: 5px solid #ec4899;
  padding-left: 12px;
  margin-bottom: 10px;
}

/* Cards */
.card {
  background: #fafafa;
  border: 1px solid #f3f4f6;
  border-radius: 14px;
  padding: 18px;
  margin-bottom: 10px;
}

.card-title {
  font-size: 1.1rem;
  font-weight: 700;
  color: #111827;
  margin-bottom: 12px;
}

/* Tags */
.tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.tag {
  font-size: 0.75rem;
  font-weight: 600;
  padding: 6px 12px;
  border-radius: 999px;
  background: #ffe4f1;
  color: #db2777;
}

/* Project Cards */
.project-card {
  background: white;
  border: 1px solid #f3f4f6;
  border-radius: 16px;
  padding: 22px;
  transition: 0.2s;
  margin-bottom: 10px;
}

.project-card:hover {
  background-color: #f7d9ea;
  box-shadow: 0px 6px 18px rgba(0, 0, 0, 0.06);
}

/* Project Title */
.project-title {
  font-size: 1.2rem;
  font-weight: 800;
  color: #111827;
}

.project-subtitle {
  font-size: 0.85rem;
  margin-top: 4px;
  color: #ec4899;
  font-weight: 600;
}

/* Project list */
.project-list {
  margin-top: 14px;
  padding-left: 18px;
  color: #374151;
  font-size: 0.9rem;
  line-height: 1.6;
}
</style>
