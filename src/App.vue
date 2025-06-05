<template>
  <div class="container fade-in">
    <div class="content">
      <div class="text">
        <p class="hello">HELLO</p>
        <h1>I'm <strong>Chindy Aurella Taniya</strong></h1>
        <h2><strong></strong> Basis Data </h2>

        <p class="description">
          Welcome to my portfolio! I'm Chindy Aurella Taniya, born in <strong>Pekanbaru</strong> on <strong>January 8th, 2005</strong>. I am currently a student of Informatics Engineering at Universitas Islam Riau, class of <strong>2023</strong>.
        </p>

        <p class="description">
          I live in <strong>Pekanbaru</strong> with my family. In my spare time, I enjoy playing <strong>badminton</strong> — a sport that keeps me active and energized.
        </p>

        <p class="description">
          As a newcomer to AI, I'm constantly seeking to expand my knowledge and skills in this exciting field. I've explored a variety of AI projects, from natural language processing to computer vision, and I'm always eager to dive deeper into new AI technologies.
        </p>

        <p class="highlight">
          Now, I am studying <strong>data science</strong> and <strong>machine learning</strong> on <span class="brand">Dicoding</span> and hope to create my own portfolio projects in the future.
        </p>

        <!-- Social Media -->
        <div class="socials">
          <a href="https://instagram.com" target="_blank">💗 Instagram</a>
          <a href="https://github.com" target="_blank">💻 GitHub</a>
        </div>
      </div>

      <!-- Foto dan Fun Facts -->
      <div class="photo">
        <div class="photo-frame">
          <img src="/Profile.jpg" alt="Chindy Aurella Taniya" />
          <span class="corner top-left">🌸</span>
          <span class="corner top-right">🌸</span>
          <span class="corner bottom-left">🌸</span>
          <span class="corner bottom-right">🌸</span>
        </div>

        <!-- Fun Facts -->
        <div class="fun-facts">
          <h3>🎀 Fun Facts About Me</h3>
          <ul>
            <li>🍜 Favorite Food: <b>Mie</b></li>
            <li>🎧 Favorite Music: <b>Best Part</b></li>
            <li>🎬 Favorite Movie: <b>Disney</b></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// Tidak ada JavaScript
</script>

<style scoped>
/* RESET */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* BASE */
html, body, #app {
  height: 100%;
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(to right, #e0f7fa, #eceff1);
  color: #333;
}

/* CONTAINER */
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  padding: 20px;
}

/* CONTENT WRAPPER */
.content {
  display: flex;
  flex-direction: row;
  max-width: 1200px;
  width: 100%;
  gap: 50px;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: nowrap;
  background: #ffffffd0;
  padding: 40px;
  border-radius: 20px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
}

/* TEXT */
.text {
  flex: 1;
  min-width: 300px;
}

/* FOTO + FUN FACT */
.photo {
  flex: 1;
  min-width: 250px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.photo-frame {
  position: relative;
  display: inline-block;
}

.photo-frame img {
  width: 280px;
  height: 280px;
  object-fit: cover;
  border-radius: 10px;
  filter: grayscale(20%);
  border: 4px solid #90caf9;
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.15);
  background-color: white;
}

/* Hiasan di sudut */
.corner {
  position: absolute;
  font-size: 1.5rem;
}

.top-left { top: -10px; left: -10px; }
.top-right { top: -10px; right: -10px; }
.bottom-left { bottom: -10px; left: -10px; }
.bottom-right { bottom: -10px; right: -10px; }

/* TYPOGRAPHY */
.hello {
  letter-spacing: 2px;
  font-weight: 600;
  font-size: 0.85rem;
  color: #1565c0;
  text-transform: uppercase;
}

h1 {
  font-size: 2.8rem;
  margin: 10px 0;
  color: #0d47a1;
}

h2 {
  font-size: 1.4rem;
  margin-bottom: 20px;
  color: #1976d2;
}

.description {
  font-size: 1rem;
  line-height: 1.7;
  margin-bottom: 15px;
  color: #444;
}

.highlight {
  font-size: 1rem;
  line-height: 1.7;
  color: #263238;
}

.brand {
  color: #1565c0;
  font-weight: bold;
}

/* FUN FACTS */
.fun-facts {
  background-color: #e3f2fd;
  padding: 15px 20px;
  border-radius: 12px;
  margin-top: 20px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
  width: 100%;
  max-width: 280px;
}

.fun-facts h3 {
  color: #0d47a1;
  margin-bottom: 10px;
  text-align: center;
  font-weight: 700;
}

.fun-facts ul {
  list-style: none;
  padding-left: 0;
}

.fun-facts li {
  margin-bottom: 8px;
  font-size: 1rem;
  color: #1565c0;
}

.fun-facts b {
  color: #0d47a1;
}

/* SOCIAL BUTTONS */
.socials {
  margin-top: 25px;
}

.socials a {
  display: inline-block;
  margin: 8px 10px 0 0;
  padding: 10px 16px;
  background: #90caf9;
  color: #0d47a1;
  border-radius: 20px;
  text-decoration: none;
  font-weight: 500;
  font-size: 0.95rem;
  transition: all 0.3s ease;
}

.socials a:hover {
  background: #64b5f6;
  color: white;
  transform: scale(1.05);
}

/* ANIMASI */
.fade-in {
  animation: fadeIn 1.2s ease-in;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* RESPONSIVE */
@media (max-width: 768px) {
  .content {
    flex-direction: column;
    text-align: center;
    padding: 30px 20px;
  }

  .photo {
    margin-bottom: 20px;
  }

  .fun-facts {
    margin-top: 15px;
  }

  h1 {
    font-size: 2.2rem;
  }

  h2 {
    font-size: 1.2rem;
  }
}
</style>

