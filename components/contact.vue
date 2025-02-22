<template>
  <div class="digital-pattern">
    <div class="content-wrapper">
      <!-- Header Section -->
      <div class="header-section">
        <h1 class="main-title">
          Beauty Selling <span class="highlight">with</span> Digital Pattern<span class="highlight">.</span>
        </h1>
        <p class="subtitle">
          Pasar yang besar ditunjang dengan wadah yang tepat, insyaAllah akan bebuah keberhasilan
        </p>
      </div>

      <!-- Main Content -->
      <div class="main-content">
        <!-- Cards Section -->
        <div class="cards-section">
          <div class="cards-grid">
            <!-- Left Column -->
            <div class="cards-column">
              <div class="feature-card platform-card">
                <div class="icon-group">
                  <img src="/assets/Image.svg" alt="" class="main-icon" style="width: 75px;margin-right: -45px;">
                  <div class="icon-shadows">
                    <div class="shadow-icon pink"></div>
                    <div class="shadow-icon gray"></div>
                    <div class="border-circle"></div>
                  </div>
                </div>
                <p class="feature-title">Beautieslife.id Platform</p>
              </div>

              <div class="feature-card social-card">
                <div class="icon-group social">
                  <img src="/assets/LinkedIN.svg" alt="" style="transform: translateY(-5px);">
                  <img src="/assets/Facebook.svg" alt="">
                  <img src="/assets/Instagram.svg" alt="">
                  <img src="/assets/Twitter.svg" alt="">
                </div>
                <p class="feature-title">Social Media Platform</p>
              </div>
            </div>

            <!-- Right Column -->
            <div class="cards-column right">
              <div class="feature-card tools-card">
                <div class="icon-group tools">
                  <img src="/assets/Trello.svg" alt="">
                  <img src="/assets/Gmail.svg" alt="">
                  <img src="/assets/Zoom.svg" alt="">
                  <img src="/assets/Google.svg" alt="">
                </div>
                <p class="feature-title">Management Tools</p>
              </div>

              <div class="feature-card chat-card">
                <div class="icon-group chat">
                  <img src="/assets/Telegram.svg" alt="">
                  <img src="/assets/Slack.svg" alt="">
                  <img src="/assets/Messenger.svg" alt="">
                  <img src="/assets/WhatsApp.svg" alt="">
                </div>
                <p class="feature-title">Enhance Chat Tools</p>
              </div>
            </div>
          </div>
        </div>

        <!-- Right Content -->
        <div class="content-right">
          <div class="pink-shape"></div>
          <h2 class="secondary-title">
            Bukan saatnya menunda 
            <span class="highlight">digitalisasi</span><span class="highlight">.</span>
          </h2>
          
          <p class="description">
            Ayo kita hadapi bersama era peralihan ini. <span class="highlight">Beautieslife.id</span> akan
            bantu kamu belajar berbisnis dengan berbagai tools digital
            yang diharapkan akan mendorong kemudahan dan kelancaran
            bisnis <em>beauty</em> kamu.
          </p>

          <ul class="benefits-list">
            <li v-for="(benefit, index) in benefits" :key="index">
              <img src="/assets/nestedcircle.svg" alt="" class="bullet-icon">
              <span>{{ benefit }}</span>
            </li>
          </ul>
        </div>
      </div>

      <!-- Background Elements -->
      <img src="/assets/pattern.svg" alt="" class="dots-pattern">
      <img src="/assets/bg-circle.svg" alt="" class="bg-circle">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      benefits: [
        'Udah bukan jamannya gaptek',
        'Udah gak ada lagi bingung pake tools apaan',
        'Gak ada lagi istilah siapa yang bakan ngajarin aku',
        'Udah bukan musimnya jalan sendirian!!'
      ]
    }
  }
}
</script>

<style scoped>
.digital-pattern {
  min-height: 100vh;
  padding: 80px 120px;
  background-color: #FFF5F5;
  position: relative;
  overflow: hidden;
}

.content-wrapper {
  max-width: 1400px;
  margin: 0 auto;
  position: relative;
}

.header-section {
  text-align: center;
  max-width: 800px;
  margin: 0 auto 100px;
}

.main-title {
  font-size: 70px;
  line-height: 80px;
  color: #555;
  margin-bottom: 40px;
  letter-spacing: -1.5px;
}

.highlight {
  color: #EE9591;
}

.subtitle {
  font-size: 16px;
  color: #888;
  line-height: 1.6;
  margin-bottom: 120px;
}

.main-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 100px;
  position: relative;
}

.cards-section {
  position: relative;
  padding-top: 40px;
}

.cards-grid {
  display: flex;
  gap: 40px;
}

.cards-column {
  display: flex;
  flex-direction: column;
  gap: 40px;
  flex: 1;
}

.cards-column.right {
  margin-top: -50px;
}

.feature-card {
  background: #FFFBFB;
  border-radius: 16px;
  padding: 30px;
  box-shadow: 30px 30px 60px rgba(85, 85, 85, 0.1);
  min-height: 200px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  z-index: 10;
}

.icon-group {
  display: flex;
  margin-bottom: 25px;
}

.icon-group img {
  width: 80px;
  height: 80px;
  margin-right: -35px;
  transition: transform 0.3s ease;
}

.icon-group img:hover {
  transform: translateY(-5px);
}

.icon-shadows {
  display: flex;
  margin-left: 25px;
}

.shadow-icon {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  margin-right: -45px;
}

.pink { background: #EE9591; }
.gray { background: #888; }

.border-circle {
  width: 70px;
  height: 70px;
  border: 2px solid #EE9591;
  border-radius: 50%;
}

.content-right {
  padding-top: 80px;
}

.pink-shape {
  width: 100px;
  height: 12px;
  background: #EE9591;
  border-radius: 100px;
  margin-bottom: 35px;
}

.secondary-title {
  font-size: 32px;
  line-height: 1.4;
  color: #555;
  margin-bottom: 30px;
  letter-spacing: -0.5px;
}

.description {
  font-size: 16px;
  line-height: 1.7;
  color: #666;
  margin-bottom: 40px;
}

.benefits-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.benefits-list li {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-bottom: 25px;
  font-size: 16px;
  color: #666;
}

.dots-pattern {
  position: absolute;
  right: -80px;
  bottom: 0px;
  width: 100px;
  z-index: 1;
}

.bg-circle {
  position: absolute;
  bottom: -20px;
  left: 0px;
  z-index: 0;
  width: 500px;
}

/* Tablet Styles */
@media (max-width: 1024px) {
  .digital-pattern {
    padding: 60px 40px;
  }

  .main-title {
    font-size: 48px;
    line-height: 56px;
  }

  .main-content {
    grid-template-columns: 1fr;
    gap: 60px;
  }

  .cards-grid {
    flex-direction: row;
  }

  .cards-column.right {
    margin-top: 0;
  }

  .feature-card {
    min-height: 180px;
    padding: 25px;
  }

  .content-right {
    padding-top: 0;
  }
}

/* Mobile Styles */
@media (max-width: 768px) {
  .digital-pattern {
    padding: 40px 10px;
  }

  .header-section {
    margin-bottom: 60px;
  }

  .main-title {
    font-size: 32px;
    line-height: 40px;
  }

  .subtitle {
    margin-bottom: 80px;
  }

  .cards-grid {
    gap: 20px;
  }

  .cards-column {
    gap: 20px;
  }

  .feature-card {
    min-height: 160px;
    padding: 20px;
  }

  .icon-group img {
    width: 60px;
    height: 60px;
    margin-right: -25px;
  }

  .shadow-icon {
    width: 60px;
    height: 60px;
  }

  .dots-pattern {
    display: none;
  }

  .secondary-title {
    font-size: 24px;
    margin-bottom: 20px;
  }

  .description {
    font-size: 14px;
    margin-bottom: 30px;
  }

  .benefits-list li {
    font-size: 14px;
    margin-bottom: 20px;
  }

  .pink-shape {
    margin-top: 40px;
  }

  .bg-circle {
    width: 300px;
    opacity: 0.5;
  }
}
</style>
