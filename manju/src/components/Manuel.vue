<template>
  <div class="greetings">
    <div class="heart-bg">
      <span v-for="n in 12" :key="n" class="heart">❤</span>
    </div>

    <div class="content">
      <h3 class="sub-text">
       You will always be my breath and my safe place, <br>
       The place i belong to is you and i will forever figt for us <br>
       Even whenever you dont see the light i will be there <br>
       Either to fix the light or sit in the dark by your side
      </h3>
      <h1 class="love-text">I Love You</h1>
    </div>
  </div>
</template>

<style scoped>
.greetings {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  width: 100%;
  overflow: hidden;
  background: linear-gradient(135deg, #fff5f5 0%, #fed7d7 100%);
  font-family: 'Inter', sans-serif;
  text-align: center;
}

.content {
  z-index: 2;
  padding: 20px;
}

.love-text {
  font-size: 4rem;
  font-weight: 800;
  color: #e53e3e;
  margin-bottom: 0.5rem;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
  letter-spacing: -1px;
}

.sub-text {
  font-size: 1.1rem;
  color: #718096;
  font-weight: 400;
}

.sub-text span {
  color: #e53e3e;
  font-weight: 600;
}

.heart-bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
}

.heart {
  position: absolute;
  color: rgba(229, 62, 62, 0.15);
  font-size: 2rem;
  animation: float 15s infinite linear;
}

.heart:nth-child(1) { left: 10%; animation-duration: 12s; font-size: 1.5rem; }
.heart:nth-child(2) { left: 25%; animation-duration: 18s; animation-delay: 2s; }
.heart:nth-child(3) { left: 40%; animation-duration: 14s; }
.heart:nth-child(4) { left: 55%; animation-duration: 20s; animation-delay: 5s; }
.heart:nth-child(5) { left: 70%; animation-duration: 16s; }
.heart:nth-child(6) { left: 85%; animation-duration: 12s; animation-delay: 3s; }

@keyframes float {
  0% {
    transform: translateY(110vh) rotate(0deg);
    opacity: 0;
  }
  10% { opacity: 1; }
  90% { opacity: 1; }
  100% {
    transform: translateY(-10vh) rotate(360deg);
    opacity: 0;
  }
}
</style>
