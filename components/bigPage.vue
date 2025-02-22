<template>
  <div class="features-container">
    <div class="features-header">
      <div class="pink-shape"></div>
      <h2 class="title">
        Pokonya udah pasti kita bimbing,
        <br />
        dengan <span class="highlight">berbagai fasilitas.</span>
      </h2>
    </div>

    <div class="features-wrapper">
      <img src="/assets/pattern2.svg" alt="" class="dot-pattern">
      <img src="/assets/circle2.svg" alt="" class="nested-circle" />
      
      <div class="features-grid">
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/smile.svg" alt="Intens Mentoring" class="icon" />
          </div>
          <h3 class="feature-title">Intens Mentoring</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/heart.svg" alt="Kajian Rutin" class="icon" />
          </div>
          <h3 class="feature-title">Kajian Rutin</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/prize.svg" alt="Rewards" class="icon" />
          </div>
          <h3 class="feature-title">Rewards</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/earth.svg" alt="Free Web Profile" class="icon" />
          </div>
          <h3 class="feature-title">Free Web Profile</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/money.svg" alt="Kelas Bisnis" class="icon" />
          </div>
          <h3 class="feature-title">Kelas Bisnis</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/computer.svg" alt="Kelas Digital" class="icon" />
          </div>
          <h3 class="feature-title">Kelas Digital</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/fire.svg" alt="Kelas Skin Care" class="icon" />
          </div>
          <h3 class="feature-title">Kelas Skin Care</h3>
        </div>
        <div class="feature-card">
          <div class="icon-wrapper">
            <img src="/assets/inbox.svg" alt="Product Knowledge" class="icon" />
          </div>
          <h3 class="feature-title">Product Knowledge</h3>
        </div>
      </div>
    </div>
    <women style="z-index: 1;"/>
    
  </div>
</template>

<style scoped>
.features-container {
  padding: 60px 24px;
  min-height: 100vh;
  background: linear-gradient(to bottom, transparent 40%, #FFFFFF 40%);
  position: relative;
  overflow: hidden;
}

.features-header {
  margin-bottom: 48px;
  max-width: 1200px;
  margin: 0 auto 48px;
}

.pink-shape {
  width: 100px;
  height: 12px;
  background: #EE9591;
  border-radius: 100px;
  margin-bottom: 35px;
}

.title {
  font-weight: 700;
  font-size: 40px;
  line-height: 1.35;
  letter-spacing: -0.3px;
  color: #555555;
}

.highlight {
  color: #FF9898;
}

.features-wrapper {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 24px;
  position: relative;
  z-index: 2;
}

.feature-card {
  background: #FFFBFB;
  box-shadow: 0 8px 24px rgba(85, 85, 85, 0.08);
  border-radius: 16px;
  padding: 24px;
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 200px;
  transition: transform 0.3s ease;
}

.feature-card:hover {
  transform: translateY(-5px);
}

.icon-wrapper {
  width: 76px;
  height: 76px;
  background: #F7C7C4;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 24px;
}

.icon {
  width: 42px;
  height: 42px;
}

.feature-title {
  font-weight: 500;
  font-size: 22px;
  text-align: center;
  color: #888888;
  margin: 0;
}

.nested-circle {
  position: absolute;
  top: -100px;
  right: -150px;
  width: 300px;
  height: 300px;
  pointer-events: none;
  opacity: 0.1;
}

.dot-pattern {
  position: absolute;
  top: 150px;
  left: -60px;
  width: 120px;
  height: 120px;
  pointer-events: none;
}

@media (max-width: 1200px) {
  .features-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
  }
  
  .features-container {
    padding: 40px 20px;
  }
  
  .title {
    font-size: 32px;
  }
}

@media (max-width: 900px) {
  .features-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 16px;
  }
  
  .nested-circle {
    visibility: hidden;
    width: 200px;
    height: 200px;
    right: -100px;
  }
  
  .dot-pattern {
    width: 80px;
    height: 80px;
  }
}

@media (max-width: 600px) {
  .features-container {
    padding: 30px 16px;
    background: linear-gradient(to bottom, transparent 30%, #FFFFFF 30%);
  }

  .features-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
  }

  .feature-card {
    min-height: 160px;
    padding: 16px;
  }

  .icon-wrapper {
    width: 60px;
    height: 60px;
    margin-bottom: 16px;
  }

  .icon {
    width: 32px;
    height: 32px;
  }

  .feature-title {
    font-size: 16px;
  }

  .title {
    font-size: 24px;
  }

  .pink-shape {
    width: 80px;
    height: 8px;
    margin-bottom: 24px;
  }

  .nested-circle,
  .dot-pattern {
    display: none;
  }
}
</style>