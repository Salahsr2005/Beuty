<template>
    <!-- nav-bar -->
    <nav class="nav-bar">
        <img src="/assets/logo.svg" alt="Beautieslife.id logo" class="logo">
        <div class="nav-items">
            <a class="nav-link">Fasilitas</a>
            <a class="nav-link">Beautypreneur</a>
            <a class="nav-link">Brand Partner</a>
            <button class="register-button">Registrasi</button>
        </div>
        <button class="burger-menu">
        <span></span>
        <span></span>
        <span></span>
    </button>
    </nav>

     <!-- Home -->
    <div class="landing-container">
      <!-- Left Content -->
      <div class="content-left">
        <h1 class="title">
          Pasti berat<br>
          kalo lari sendirian<span class="title-dot">.</span>
        </h1>
        
        <p class="description">
          Setiap hal pasti butuh hal lain untuk membersamai.<br>
          Begitupun dengan bisnis, Beautieslfie.id hadir untuk membersamai<br>
          kalian untuk menjadi Beautypreneur. Siapapun kamu!!
        </p>
        
        <div class="categories">
          <div class="category">
            <img src="/assets/nestedcircle.svg" alt="" class="circlesvg">
            <span class="category-text">Mahasiswi</span>
          </div>
          <div class="category">
            <img src="/assets/nestedcircle.svg" alt="" class="circlesvg">
            <span class="category-text">Ibu Rumah Tangga</span>
          </div>
          <div class="category">
            <img src="/assets/nestedcircle.svg" alt="" class="circlesvg">
            <span class="category-text">Career Hunter</span>
          </div>
        </div>
        
        <div class="highlight-box">
          <h3 class="bigone">1st Indonesian Beautypreneur Community</h3>
          <p class="smallone">Dengan berbagai fasilitas "advance digital platform"</p>
        </div>
      </div>
      
      <!-- Right Content -->
      <div class="content-right">
        <div class="illustration">
          <!-- Phone Container -->
          <div class="phone">
            <img src="/assets/hsr.svg" alt="Makeup brushes" class="phone-content" />
          </div>
        </div>
    </div>
</div>
  </template>
  
  <script>
  export default {
    name: 'LandingPage'
  }
  </script>
  
  <style scoped>
.landing-container{
    height: 100vh;
    display: flex;
    flex-direction: row;
    margin-top: 120px;
}
.nav-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 36px 0px;
}

.logo {
    height: 40px; 
}

.nav-items {
    display: flex;
    align-items: center;
    gap: 40px;
}

.nav-link {
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 16px;
    letter-spacing: -0.3px;
    color: #555555;
    cursor: pointer;
}

.register-button {
    background: #F39B95;
    border: none;
    padding: 12px 24px;
    border-radius: 8px;
    color: white;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 16px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.register-button:hover {
    background: #EE9591;
}

.content-left{
    display: flex;
    flex-direction: column;
    margin-right: 12px;
}
.title{
    color: #555555;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 900;
    font-size: 70px;
    line-height: 80px;
    letter-spacing: 0.3px;
}
.description{
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 26px;
    letter-spacing: -0.3px;
    color: #888888;
    margin-top: 30px;
}
.categories{
    display: flex;
    flex-direction: row;
    margin-top: 40px;
    align-items: flex-start;
    padding: 0px;
    gap: 30px;



}
.highlight-box{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 15px 22px;
    gap: 6px;
    background: #EE9591;
    box-shadow: 16px 16px 60px rgba(179, 94, 90, 0.4);
    border-radius: 10px;
    margin-top: 40px;

}
.bigone{
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 26px;
    letter-spacing: -0.3px;
    color: #F7F7F7;
}
.smallone{
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 22px;
    letter-spacing: -0.3px;
    color: #F7F7F7;

}
.categories {
    display: flex;
    flex-direction: row;
    margin-top: 40px;
    align-items: flex-start;
    padding: 0px;
    gap: 30px;
}

.category {
    display: flex;
    align-items: center; /* This will vertically center the icon and text */
}

.circlesvg {
    margin-right: 8px; /* Add margin between icon and text */
}

.category-text {
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 700;
    font-size: 16px;
    line-height: 24px;
    letter-spacing: -0.3px;
    color: #888888;
}
/* Keep your existing CSS and add these media queries at the bottom */

@media screen and (max-width: 1024px) {
  .landing-container {
    margin-top: 60px;
    padding: 0 40px;
  }
  
  .nav-bar {
    padding: 20px 40px;
  }
  
  .title {
    font-size: 56px;
    line-height: 64px;
  }
  
  .content-right {
    display: none; /* Hide the right content on tablet */
  }
  
  .description {
    font-size: 14px;
    line-height: 24px;
  }
  
  .categories {
    margin-top: 30px;
    gap: 20px;
  }
  
  .category-text {
    font-size: 14px;
  }
}

@media screen and (max-width: 768px) {
  .landing-container {
    margin-top: 40px;
    padding: 0 20px;
  }
  
  .nav-bar {
    padding: 16px 20px;
  }
  
  .nav-items {
    display: none; /* Hide navigation items */
  }
  
  /* Add hamburger menu visibility */
  .nav-bar::after {
    content: '☰';
    font-size: 24px;
    color: #555555;
    cursor: pointer;
  }
  
  .logo {
    height: 32px;
  }
  
  .title {
    font-size: 40px;
    line-height: 48px;
  }
  
  .description {
    margin-top: 20px;
  }
  
  .categories {
    flex-wrap: wrap;
    gap: 15px;
  }
  
  .category {
    flex: 0 0 auto;
  }
  
  .highlight-box {
    margin-top: 30px;
    padding: 12px 18px;
  }
  
  .bigone {
    font-size: 18px;
    line-height: 24px;
  }
  
  .smallone {
    font-size: 12px;
    line-height: 20px;
  }
  
  /* Show registration button on top */
  .register-button {
    position: fixed;
    top: 16px;
    right: 60px;
    padding: 8px 16px;
    font-size: 12px;
  }
}

/* Add utility class for dots pattern */
.dots-pattern {
  position: absolute;
  top: 20px;
  right: 20px;
  width: 100px;
  height: 100px;
  background-image: radial-gradient(#F39B95 2px, transparent 2px);
  background-size: 10px 10px;
  opacity: 0.3;
}
  </style>