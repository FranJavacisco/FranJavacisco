<!-- Estilos CSS optimizados para todos los dispositivos -->
<style>
/* Variables CSS para mantener consistencia */
:root {
  --terminal-green: #00ff00;
  --terminal-dark: #001100;
  --terminal-black: #000000;
  --glow-effect: 0 0 5px rgba(0, 255, 0, 0.5);
  --border-color: #00ff00;
  --bg-gradient: linear-gradient(180deg, #001100 0%, #000000 100%);
}

/* Estilos base responsivos */
.terminal-container {
  max-width: 100%;
  margin: 0 auto;
  padding: clamp(0.5rem, 2vw, 2rem);
  background: var(--terminal-black);
  font-family: 'Share Tech Mono', 'Courier New', monospace;
  color: var(--terminal-green);
  text-shadow: var(--glow-effect);
  line-height: 1.6;
  overflow-x: hidden;
}

/* Headers Responsivos */
.terminal-header {
  font-size: clamp(1rem, 3vw, 1.5rem);
  text-align: center;
  margin-bottom: 2rem;
  padding: 1rem;
  border: 2px solid var(--border-color);
  border-radius: 5px;
  background: var(--terminal-dark);
  box-shadow: var(--glow-effect);
}

/* Secciones con mejor espaciado */
.terminal-section {
  margin: 2rem 0;
  padding: clamp(1rem, 3vw, 2rem);
  border: 1px solid var(--border-color);
  border-radius: 5px;
  background: var(--terminal-dark);
  transition: transform 0.3s ease;
}

.terminal-section:hover {
  transform: translateY(-2px);
  box-shadow: 0 0 15px rgba(0, 255, 0, 0.2);
}

/* Grid System Mejorado */
.terminal-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(100%, 300px), 1fr));
  gap: clamp(1rem, 3vw, 2rem);
  align-items: start;
}

/* Cards de Proyecto Optimizadas */
.project-card {
  background: var(--terminal-dark);
  border: 1px solid var(--border-color);
  border-radius: 5px;
  padding: 1rem;
  transition: all 0.3s ease;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 20px rgba(0, 255, 0, 0.3);
}

/* Imágenes Responsivas */
.project-image {
  width: 100%;
  height: auto;
  border-radius: 3px;
  margin: 1rem 0;
  filter: sepia(50%) hue-rotate(70deg) brightness(90%) contrast(130%);
  transition: filter 0.3s ease;
}

.project-image:hover {
  filter: sepia(30%) hue-rotate(70deg) brightness(100%) contrast(120%);
}

/* Progress Bars Estilizados */
.progress-bar {
  height: 20px;
  background: var(--terminal-dark);
  border: 1px solid var(--border-color);
  border-radius: 3px;
  overflow: hidden;
  margin: 0.5rem 0;
}

.progress-fill {
  height: 100%;
  background: var(--terminal-green);
  opacity: 0.7;
  transition: width 1s ease-in-out;
}

/* Botones Retro */
.terminal-button {
  display: inline-block;
  padding: 0.5rem 1rem;
  margin: 0.5rem;
  background: var(--terminal-dark);
  border: 1px solid var(--border-color);
  border-radius: 3px;
  color: var(--terminal-green);
  text-decoration: none;
  text-align: center;
  transition: all 0.3s ease;
}

.terminal-button:hover {
  background: var(--terminal-green);
  color: var(--terminal-black);
  box-shadow: 0 0 10px var(--terminal-green);
}

/* Efectos de Terminal */
.scanline {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: repeating-linear-gradient(
    0deg,
    rgba(0, 255, 0, 0.03) 0%,
    rgba(0, 255, 0, 0.03) 1px,
    transparent 1px,
    transparent 2px
  );
  pointer-events: none;
  z-index: 2;
}

/* Optimizaciones para móvil */
@media (max-width: 768px) {
  .terminal-container {
    padding: 0.5rem;
  }
  
  .terminal-section {
    padding: 1rem;
    margin: 1rem 0;
  }
  
  .terminal-grid {
    gap: 1rem;
  }
  
  .project-card {
    margin: 0.5rem 0;
  }
  
  .terminal-button {
    width: calc(50% - 1rem);
    padding: 0.75rem;
  }
}

/* Animaciones */
@keyframes pulse {
  0% { opacity: 0.8; }
  50% { opacity: 1; }
  100% { opacity: 0.8; }
}

.terminal-text {
  animation: pulse 2s infinite;
}

/* Loading Bar Animation */
@keyframes loading {
  0% { width: 0; }
  100% { width: 100%; }
}

.loading-bar {
  height: 2px;
  background: var(--terminal-green);
  animation: loading 2s linear;
}
</style>

<!-- Contenido del README con las nuevas optimizaciones -->
<div class="terminal-container">
  <div class="loading-bar"></div>
  
  <header class="terminal-header">
    <div class="terminal-text">SYSTEM v2.0.24 - Developer Profile</div>
    <small>Last updated: 23/11/2024</small>
  </header>

  <!-- Sección de identificación -->
  <section class="terminal-section">
    <img src="https://readme-typing-svg.herokuapp.com?font=Share+Tech+Mono&size=24&duration=3000&pause=1000&color=00FF00&center=true&vCenter=true&repeat=false&width=435&lines=>>+Initializing+Profile...;>>+Loading+Complete" alt="Loading Animation"/>
    
    <div class="terminal-grid">
      <div>
        <h2>>> Developer Info</h2>
        <p>Name: Francisco López</p>
        <p>Role: Front-End & Security</p>
        <p>Status: Active</p>
      </div>
      <div>
        <h2>>> Current Focus</h2>
        <p>🔒 Security-First Development</p>
        <p>🎨 UI/UX Excellence</p>
        <p>📱 Responsive Design</p>
      </div>
    </div>
  </section>

  <!-- Tech Stack con barras de progreso animadas -->
  <section class="terminal-section">
    <h2>>> Tech Stack Analysis</h2>
    <div class="terminal-grid">
      <!-- Frontend -->
      <div>
        <h3>Frontend</h3>
        <div class="progress-bar">
          <div class="progress-fill" style="width: 90%"></div>
          <span>HTML5 90%</span>
        </div>
        <!-- Más barras de progreso... -->
      </div>
      
      <!-- Backend -->
      <div>
        <h3>Backend</h3>
        <!-- Barras de progreso backend... -->
      </div>
      
      <!-- Security -->
      <div>
        <h3>Security</h3>
        <!-- Barras de progreso security... -->
      </div>
    </div>
  </section>

  <!-- Proyectos con mejor presentación -->
  <section class="terminal-section">
    <h2>>> Active Projects</h2>
    <div class="terminal-grid">
      <!-- Proyecto 1 -->
      <article class="project-card">
        <h3>Agent_Smith</h3>
        <img class="project-image" src="./assets/Agent_Smith.png" alt="Agent Smith Project">
        <p class="terminal-text">Matrix-inspired login system with advanced security features</p>
        <div>
          <a href="#" class="terminal-button">View Code</a>
          <a href="#" class="terminal-button">Live Demo</a>
        </div>
      </article>
      <!-- Más proyectos... -->
    </div>
  </section>

  <!-- Secciones adicionales con el mismo estilo... -->

  <div class="scanline"></div>
</div>