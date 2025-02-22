<template>
    <div class="testimonial-page">
      <!-- Testimonial Section -->
      <div class="testimonial-section">
        <span class="section-label">Testimonial</span>
        <h2 class="section-title">Apa kata <span class="highlight">mereka</span>?</h2>
        
        <!-- Testimonial Slider -->
        <div class="testimonial-container">
          <div class="testimonial-card">
            <div class="testimonial-image-wrapper">
              <img src="/assets/annabel.svg" alt="Annabel Rohan" class="testimonial-image" />
            </div>
            <div class="testimonial-content">
              <h3 class="testimonial-name">Annabel Rohan</h3>
              <p class="testimonial-role">Leader Nasional JAFRA Executive</p>
              <p class="testimonial-text">
                Arcu sed etiam proin natoque at lectus aliquam. Faucibus ipsum porta eleifend facilisis cras in.Sed etiam proin natoque 
              </p>
              <a href="#" class="next-link">
                next <span class="arrow">→</span>
              </a>
            </div>
          </div>
        </div>
      </div>
  
      <!-- Footer Section -->
      <div class="footer-wrapper">
        <footer class="footer">
          <!-- Left Column with Background -->
          <div class="footer-left">
            <div class="footer-left-content">
              <img src="/assets/logo2.svg" alt="Beautieslife.id" class="footer-logo" />
              <h3 class="footer-title">Indonesian Beautypreneur Community.</h3>
              <p class="footer-description">
                Wadah positif bagi para Beautypreneur. Berpenghasilan dari rumah dengan memanfaatkan teknologi. 
                Bergabung bersama beautypreneur lainnya.
              </p>
              <div class="supported-by">
                <img src="/assets/support.svg" alt="Supported by Syabany.com" class="support-logo" />
                <span>syabany.com</span>
              </div>
              <p class="copyright">© 2022 Beautieslife.id. Made with love</p>
            </div>
          </div>
  
          <!-- Middle Column - Links -->
          <div class="footer-links">
            <div class="links-group">
              <h4>About</h4>
              <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Beautypreneur</a></li>
                <li><a href="#">Brand Partner</a></li>
                <li><a href="#">Official Partner</a></li>
              </ul>
            </div>
            <div class="links-group">
              <h4>Support</h4>
              <ul>
                <li><a href="#">Kelas Geratis *</a></li>
                <li><a href="#">Fasilitas</a></li>
                <li><a href="#">FAQs</a></li>
                <li><a href="#">Contact</a></li>
              </ul>
            </div>
          </div>
  
          <!-- Right Column -->
          <div class="footer-right">
            <img src="/assets/syabany.svg" alt="Syabany" class="syabany-image"/>
          </div>
        </footer>
      </div>
    </div>
  </template>
  
  <style scoped>
  .testimonial-page {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    background-color: #fff;
  }
  
  .testimonial-section {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0px;
    position: absolute;
    top: 4300px;
    right: 500px;
    width: 50%;
    max-width: 600px;
  }
  
  .section-label {
    color: #FF9898;
    font-size: 18px;
    font-weight: 500;
    margin-bottom: 16px;
    display: block;
  }
  
  .section-title {
    font-size: 48px;
    color: #4A4A4A;
    margin-bottom: 40px;
    font-weight: 600;
  }
  
  .highlight {
    color: #FF9898;
  }
  
  .testimonial-container {
    width: 100%;
  }
  
  .testimonial-card {
    display: flex;
    gap: 64px;
    align-items: center;
  }
  
  .testimonial-image-wrapper {
    width: 180px;
    height: 180px;
    overflow: hidden;
    flex-shrink: 0;
    border-radius: 10px 173px 170px 169px;
  }
  
  .testimonial-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  
  .testimonial-content {
    flex-grow: 1;
  }
  
  .testimonial-name {
    font-size: 32px;
    color: #4A4A4A;
    margin-bottom: 12px;
    font-weight: 600;
  }
  
  .testimonial-role {
    color: #FF9898;
    font-size: 18px;
    margin-bottom: 24px;
  }
  
  .testimonial-text {
    color: #666666;
    line-height: 1.8;
    font-size: 16px;
    margin-bottom: 32px;
    max-width: 400px;
  }
  
  .next-link {
    color: #666666;
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    gap: 8px;
    font-size: 16px;
    transition: all 0.3s ease;
  }
  
  .next-link:hover {
    color: #FF9898;
  }
  
  .arrow {
    color: #FF9898;
    font-size: 20px;
  }
  
  /* Footer Styles */
  .footer-wrapper {
    margin-top: auto;
    position: relative;
    width: 100%;
  }
  
  .footer {
    display: flex;
    position: relative;
    min-height: 450px;
    width: 100%;
  }
  
  .footer-left {
    background: #EE9591;
    border-radius: 0 96px 0 0;
    width: 540px;
    height: 450px;
    padding: 80px 100px;
    position: relative;
  }
  
  .footer-left-content {
    max-width: 280px;
  }
  
  .footer-logo {
    margin-bottom: 30px;
    height: 48px;
  }
  
  .footer-title {
    font-size: 14px;
    margin-bottom: 16px;
    font-weight: 700;
    color: white;
  }
  
  .footer-description {
    line-height: 1.6;
    margin-bottom: 32px;
    font-size: 14px;
    font-weight: 400;
    color: white;
    opacity: 0.9;
    max-width: 260px;
  }
  
  .supported-by {
    display: flex;
    align-items: center;
    gap: 16px;
    margin-bottom: 32px;
    color: white;
  }
  
  .support-logo {
    height: 32px;
  }
  
  .copyright {
    font-size: 14px;
    color: white;
    opacity: 0.8;
  }
  
  /* Links Section */
  .footer-links {
    display: flex;
    gap: 60px;
    padding: 80px 60px;
    margin: 0 auto;
  }
  
  .links-group h4 {
    font-size: 18px;
    margin-bottom: 24px;
    font-weight: 600;
    color: #EE9591;
  }
  
  .links-group ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  
  .links-group li {
    margin-bottom: 16px;
  }
  
  .links-group a {
    color: #666666;
    text-decoration: none;
    font-size: 14px;
    transition: opacity 0.3s ease;
  }
  
  .links-group a:hover {
    opacity: 0.8;
  }
  
  /* Right Section */
  .footer-right {
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
    padding: 0 60px 0 60px;
    height: 450px;
  }
  
  .syabany-image {
    width: 500px;
    height: auto;
    object-fit: contain;
    display: block;
  }
  
  /* Responsive Styles */
  @media (max-width: 1440px) {
    .testimonial-page {
padding: 20px 20px;
  }
    .testimonial-section {
      right: 40px;
      width: 45%;
    }
  
    .footer {
      display: flex;
      align-items: flex-start;
    }
  
    .footer-left {
      width: 540px;
      flex-shrink: 0;
    }
  
    .footer-links {
      padding: 80px 40px;
      flex-shrink: 0;
    }
  
    .footer-right {
      padding: 0 20px 0 20px;
    }
  
    .syabany-image {
      width: 400px;
    }
  }
  
  @media (max-width: 1280px) {
    .testimonial-section {
      right: 20px;
      width: 40%;
    }
  
    .footer-left {
      width: 480px;
    }
  
    .syabany-image {
      width: 350px;
    }
  }
  
  @media (max-width: 1024px) {
    .testimonial-section {
      position: static;
      width: 100%;
      max-width: 100%;
      padding: 40px;
      margin: 0 auto;
    }
  
    .testimonial-card {
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
  
    .testimonial-text {
      max-width: 100%;
    }
  
    .footer {
      flex-direction: column;
    }
  
    .footer-left {
      width: 100%;
      height: auto;
      padding: 60px 40px;
      border-radius: 0 48px 0 0;
    }
  
    .footer-left-content {
      max-width: 100%;
    }
  
    .footer-description {
      max-width: 100%;
    }
  
    .footer-links {
      padding: 40px;
      justify-content: center;
    }
  
    .footer-right {
      padding: 0 40px 40px;
      height: auto;
      justify-content: center;
    }
  
    .syabany-image {
      width: 300px;
      margin: 0 auto;
    }
  }
  
  @media (max-width: 768px) {
    .testimonial-section {
      padding: 30px;
    }
  
    .section-title {
      font-size: 36px;
    }
  
    .testimonial-image-wrapper {
      width: 160px;
      height: 160px;
      margin: 0 auto;
    }
  
    .footer-links {
      flex-direction: column;
      gap: 40px;
      align-items: center;
      text-align: center;
    }
  }
  
  @media (max-width: 480px) {
    .testimonial-section {
      padding: 20px;
    }
  
    .section-title {
      font-size: 32px;
    }
  
    .testimonial-image-wrapper {
      width: 140px;
      height: 140px;
    }
  
    .footer-left {
      padding: 40px 20px;
      border-radius: 0 32px 0 0;
    }
  
    .footer-links,
    .footer-right {
      padding: 20px;
    }
  
    .syabany-image {
      width: 200px;
    }
  }
  </style>