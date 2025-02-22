<template>
        <div class="mentor-container">
    <div class="mentor-header">
      <h2 class="title">
        Meet our <span class="highlight">mentor</span> and <span class="highlight">advisor</span>.
      </h2>
      <p class="subtitle">
        Kita akan berlari ditemani para mentor dan advisor dari Beautieslife.id. Akan banyak ilmu baru dan inspiratif.
      </p>
    </div>

    <div class="mentor-grid">
      <div class="mentor-card">
        <div class="image-wrapper">
          <img src="/assets/mentor1.svg" alt="Chantal Shelburne" class="mentor-image" />
        </div>
        <h3 class="mentor-name">Chantal Shelburne</h3>
        <p class="mentor-role">Founder Beautieslife.id</p>
        <p class="mentor-position">Our Mentor</p>
      </div>

      <div class="mentor-card">
        <div class="image-wrapper">
          <img src="/assets/mentor2.svg" alt="Kylee Danford" class="mentor-image" />
        </div>
        <h3 class="mentor-name">Kylee Danford</h3>
        <p class="mentor-role">Founder & CDO Syabany.com</p>
        <p class="mentor-position">Our Mentor</p>
      </div>

      <div class="mentor-card">
        <div class="image-wrapper">
          <img src="/assets/mentor3.svg" alt="Lauralee Quintero" class="mentor-image" />
        </div>
        <h3 class="mentor-name">Lauralee Quintero</h3>
        <p class="mentor-role">Leader Nasional JAFRA Executive</p>
        <p class="mentor-position">Our Advisor</p>
      </div>

      <div class="mentor-card">
        <div class="image-wrapper">
          <img src="/assets/mentor4.svg" alt="Freida Varnes" class="mentor-image" />
        </div>
        <h3 class="mentor-name">Freida Varnes</h3>
        <p class="mentor-role">Founder Dakwahyu & Wadah Hikmah</p>
        <p class="mentor-position">Our Advisor</p>
      </div>
    </div>

    <!-- Decorative elements -->
    <img src="/assets/pattern2.svg" alt="" class="dot-pattern" />
    <img src="/assets/halfcircle.svg" alt="" class="circle-decoration" />
  </div> 
</template>
<style scoped>
.mentor-container {
  margin: 0 auto;
  padding: 170px 50px;
  position: relative;
  overflow: hidden;
}

.mentor-header {
  text-align: center;
  margin-bottom: 64px;
  position: relative;
  z-index: 2;
}

.title {
font-family: Roboto;
font-style: normal;
font-weight: 700;
font-size: 40px;
line-height: 54px;
text-align: center;
letter-spacing: -0.3px;
color: #555555;
}

.highlight {
  color: #FF9898;
}

.subtitle {
  font-family: Roboto;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 26px;
  text-align: center;
  letter-spacing: -0.3px;
  color: #888888;
  margin-top: 16px;

}

.mentor-grid {
  display: flex;
  gap: 32px;
  justify-content: center;
  flex-wrap: wrap;
  position: relative;
  z-index: 2;
}

.mentor-card {
  width: 270px;
  text-align: left;
}

.image-wrapper {
  width: 100%;
  height: 270px;
  border-radius: 16px;
  overflow: hidden;
  margin-bottom: 20px;
}

.mentor-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  background: #EE9591;
  opacity: 0.8;
  border-radius: 16px;

}

.mentor-name {
  font-size: 24px;
  color: #4A4A4A;
  margin-bottom: 8px;
  font-weight: 500;
}

.mentor-role {
  font-size: 16px;
  color: #FF9898;
  margin-bottom: 4px;
}

.mentor-position {
  font-size: 16px;
  color: #666666;
}

.dot-pattern {
  position: absolute;
  top: 170px;
  right: 76px;
  width: 121px;
  height: 109px;
  pointer-events: none;
}

.circle-decoration {
  position: absolute;
  left: -180px;
  bottom: 0px;
  width: 760px;
  height: 750px;
  pointer-events: none;
}

/* Responsive Design */
@media (max-width: 1200px) {
  .mentor-grid {
    gap: 24px;
    grid-template-columns: repeat(2, 1fr);
    flex-wrap: wrap;
  }

  .mentor-card {
    width: calc(50% - 12px);
    max-width: 270px;
  }
  .dot-pattern{
    visibility: hidden;
  }
  .circle-decoration{
    visibility: hidden;
  }
}

@media (max-width: 768px) {
  .mentor-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 32px;
  }
  .mentor-container {
    padding: 0px 0px;
  }

  .title {
    font-size: 32px;
  }

  .subtitle {
    font-size: 16px;
  }

  .dot-pattern {
    width: 120px;
    height: 120px;
  }

  .circle-decoration{
    visibility: hidden;
  }
  .dot-pattern{
    visibility: hidden;
  }
}

@media (max-width: 640px) {
  .mentor-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
  }
  .title{
    margin-top: 150px;
  }
  .dot-pattern{
    visibility: hidden;
  }
  .mentor-card {
    max-width: 220px;
  }

  .image-wrapper {
    height: 320px;
  }
  .circle-decoration{
    visibility: hidden;
  }
}
</style>
