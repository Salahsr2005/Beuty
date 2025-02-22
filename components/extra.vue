<template>
    <div class="stats-container">
      <!-- Background Circle -->
      <div class="background-circle"></div>
      <div class="background-circle2"></div>
      
      <div class="content-wrapper">
        <!-- Left Content -->
        <div class="left-content">
          <h1 class="title">Beautypreneur<span class="dot">.</span></h1>
          <p class="subtitle">'byoodē prəˈnər (noun)'</p>
          <p class="description">
            Bukan sekedar bisnis yang hits dengan segudang untung.
            Tren <span class="highlight">beautypreneur</span> di Indonesia sudah mulai terlihat
            sejak beberapa tahun terakhir, industri kecantikan dalam negeri
            mulai berkembang pesat.
          </p>
          <div class="pink-shape"></div>
        </div>
  
        <!-- Right Content -->
        <div class="right-content">
          <div class="stat-card">
            <div class="stat-inner">
              <div class="dots-pattern"></div>
              <h2 class="stat-number">50<span class="percent">%</span></h2>
              <p class="stat-text">
                Bingung bagaimana caranya memulai bisnis
                <span class="italic">healthy beauty</span>. Sedangkan
                demand di sektor ini begitu melimpah.
              </p>
            </div>
          </div>
  
          <div class="stat-card">
            <div class="stat-inner">
              <div class="dots-pattern"></div>
              <h2 class="stat-number">23,7<span class="percent">%</span></h2>
              <p class="stat-text">
                Khawatir butuh modal usaha yang sangat besar. Padahal banyak
                cara agar dapat berbinis di sektor ini (Healthy Beauty)
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'BeautypreneurStats'
  }
  </script>
  
  <style scoped>
  .stats-container {
    position: relative;
    min-height: 70vh;
    display: flex;
    align-items: center;
    background-color: #FFFFFF;
    overflow: hidden;
    padding: 2rem;
  }
  .pink-shape{
  width: 100px;
  height: 12px;
  background: #EE9591;
  border-radius: 100px;
  flex: none;
  order: 3;
  flex-grow: 0;
  margin-top: 23px;
  }
  .background-circle {
    position: absolute;
    right: 10%;
    top: 50%;
    transform: translateY(-50%);
    width: 400px;
    height: 400px;
    background: rgba(243, 155, 149, 0.1);
    border-radius: 50%;
    z-index: 0;
  }
  .background-circle2 {
    position: absolute;
    right: 15%;
    top: 50%;
    transform: translateY(-50%);
    width: 400px;
    height: 400px;
    border: 2px solid rgba(243, 155, 149, 0.1);
    border-radius: 50%;
    z-index: 0;
  }
  
  .content-wrapper {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 4rem;
    position: relative;
    z-index: 1;
  }
  
  .left-content {
    flex: 0 1 40%;
  }
  
  .right-content {
    flex: 0 1 60%;
    display: flex;
    gap: 2rem;
    justify-content: flex-end;
  }
  
  .title {
    font-size: 3.5rem;
    font-weight: 700;
    color: #555555;
    margin-bottom: 0.5rem;
  }
  
  .dot {
    color: #F39B95;
  }
  
  .subtitle {
    color: #888888;
    font-size: 1rem;
    margin-bottom: 1.5rem;
    font-style: italic;
  }
  
  .description {
    color: #555555;
    font-size: 1.1rem;
    line-height: 1.6;
    max-width: 90%;
  }
  
  .highlight {
    color: #888888;
    font-weight: 800;
    text-decoration: underline;
  }
  
  .stat-card {
    width: 350px;
    height: 270px;
    position: relative;
    perspective: 1000px;
  }
  
  .stat-inner {
    padding: 2rem;
    height: 100%;
    background: linear-gradient(117.78deg, #F9A8A5 34.55%, #E28A86 79.96%);
    border: 8px solid #F7F7F7;
    border-radius: 20px;
    box-shadow: -40px 40px 50px rgba(85, 85, 85, 0.14);
    position: relative;
  }
  
  .stat-number {
    font-size: 5rem;
    font-weight: 700;
    color: #FFFFFF;
    margin-bottom: 1rem;
    line-height: 1;
  }
  
  .percent {
    font-size: 3.5rem;
  }
  
  .stat-text {
    color: #FFFFFF;
    font-size: 0.875rem;
    line-height: 1.5;
  }
  
  .italic {
    font-style: italic;
  }
  
  .dots-pattern {
    position: absolute;
    top: 1rem;
    right: 1rem;
    width: 80px;
    height: 80px;
    background-image: radial-gradient(circle, rgba(255,255,255,0.2) 1px, transparent 1px);
    background-size: 8px 8px;
  }
  
  @media (max-width: 1200px) {
    .content-wrapper {
      flex-direction: column;
      gap: 3rem;
    }
  
    .left-content, .right-content {
      flex: 0 1 100%;
    }
  
    .right-content {
      justify-content: center;
      flex-wrap: wrap;
    }
  
    .background-circle {
      opacity: 0.4;
      width: 400px;
      height: 400px;
    }
  }
  
  @media (max-width: 768px) {
    .stats-container {
      padding: 1rem;
    }
  
    .title {
      font-size: 2.5rem;
    }
  
    .description {
      font-size: 1rem;
    }
  
    .stat-card {
      width: 100%;
      max-width: 320px;
    }
  
    .stat-number {
      font-size: 4rem;
    }
  
    .percent {
      font-size: 2.5rem;
    }
  
    .right-content {
      gap: 1.5rem;
      width: 100%;
    }
  }
  </style>