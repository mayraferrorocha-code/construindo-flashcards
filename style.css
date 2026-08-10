/* Reset e configurações globais */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
}

body {
  background-color: #f0f4f8;
  color: #333;
  padding: 30px 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 100vh;
}

header {
  text-align: center;
  margin-bottom: 40px;
}

header h1 {
  font-size: 2.2rem;
  color: #1e293b;
  margin-bottom: 8px;
}

header p {
  color: #64748b;
  font-size: 1rem;
}

/* Grid do Container */
.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 25px;
  width: 100%;
  max-width: 1000px;
}

/* Estrutura 3D do Flashcard */
.flashcard {
  background-color: transparent;
  width: 100%;
  height: 220px;
  perspective: 1000px; /* Cria o efeito de profundidade 3D */
  cursor: pointer;
  outline: none;
}

.flashcard-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s cubic-bezier(0.4, 0.2, 0.2, 1);
  transform-style: preserve-3d;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.08);
  border-radius: 16px;
}

/* Animação de Giro ao passar o mouse ou focar */
.flashcard:hover .flashcard-inner,
.flashcard:focus .flashcard-inner {
  transform: rotateY(180deg);
}

/* Lados da Carta (Frente e Verso) */
.flashcard-front,
.flashcard-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden; /* Esconde a face traseira durante a rotação */
  border-radius: 16px;
  padding: 25px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

/* Estilo da Frente */
.flashcard-front {
  background: #ffffff;
  color: #1e293b;
  border: 2px solid #e2e8f0;
}

.tag {
  position: absolute;
  top: 16px;
  left: 16px;
  color: #ffffff;
  font-size: 0.75rem;
  font-weight: 700;
  padding: 4px 12px;
  border-radius: 20px;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

/* Cores das tags por matéria */
.tag.biologia { background-color: #10b981; }
.tag.historia { background-color: #f59e0b; }
.tag.quimica  { background-color: #6366f1; }

.flashcard-front h2 {
  font-size: 1.25rem;
  font-weight: 600;
  line-height: 1.4;
}

/* Estilo do Verso */
.flashcard-back {
  background: linear-gradient(135deg, #1e293b, #334155);
  color: #ffffff;
  transform: rotateY(180deg); /* Inicia invertido para aparecer só ao virar */
}

.flashcard-back p {
  font-size: 1.1rem;
  line-height: 1.5;
}

/* Ajustes para telas pequenas */
@media (max-width: 480px) {
  .flashcard {
    height: 200px;
  }
}
