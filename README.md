
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Future Pulse</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Poppins',sans-serif;
}

body{
  background:#f5f5f5;
  overflow-x:hidden;
}

/* ================= HEADER ================= */

header{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  padding:10px 7%;
  background:transparent;
  display:flex;
  justify-content:space-between;
  align-items:center;
  z-index:1000;
  transition:0.4s ease;
}

header.scrolled{
  background:white;
  box-shadow:0 5px 20px rgba(0,0,0,0.08);
}

header.scrolled nav a{
  color:#111827;
}

header.scrolled .contact-btn{
  background:#021B2D;
  color:white;
}
.logo img{
  width:150px;
}

nav{
  display:flex;
  gap:35px;
  align-items:center;
}

nav a{
  color:white;
  text-decoration:none;
  font-size:15px;
}

.contact-btn{
  background:white;
  color:#021B2D;
  padding:12px 24px;
  border-radius:40px;
  font-weight:600;
}

/* ================= HERO ================= */

.hero{
  min-height:100vh;
  background:linear-gradient(to right,#001524,#002B47);
  display:flex;
  align-items:center;
  padding:0 7%;
}

.hero-content{
  max-width:700px;
}

.hero-content h1{
  font-size:42px;
  line-height:1.2;
  color:white;
  margin-bottom:25px;
  font-weight:500;
}

.hero-content p{
  color:#D7E7F5;
  line-height:1.9;
  margin-bottom:35px;
}

.hero-btn{
  display:inline-block;
  background:white;
  color:#021B2D;
  padding:16px 30px;
  border-radius:40px;
  text-decoration:none;
  font-weight:600;
}

/* ================= ABOUT ================= */

.about-section{
  padding:100px 7%;
  background:white;
}

.about-container{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:70px;
  align-items:center;
}

.partner-logos{
  display:flex;
  gap:20px;
  margin-bottom:40px;
}

.logo-card{
  width:130px;
  height:90px;
  background:#f5f5f5;
  border-radius:20px;
  display:flex;
  align-items:center;
  justify-content:center;
}

.logo-card img{
  width:80%;
}

.about-left h2{
  font-size:34px;
  line-height:1.5;
  margin-bottom:25px;
  color:#374151;
}

.about-left p{
  line-height:1.9;
  color:#4B5563;
  margin-bottom:20px;
}

.about-btn{
  display:inline-block;
  padding:15px 30px;
  background:#1476C6;
  color:white;
  border-radius:40px;
  text-decoration:none;
}

.about-right img{
  width:100%;
  border-radius:30px;
}

/* ================= EXPERIENCE ================= */

.experience-section{
  background:#021B2D;
  color:white;
  padding:100px 7%;
}

.section-title{
  font-size:50px;
  margin-bottom:20px;
}

.section-subtitle{
  color:#D7E7F5;
  line-height:1.8;
  margin-bottom:60px;
}

.experience-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:80px;
}

.experience-card h3{
  font-size:38px;
  margin-bottom:20px;
}

.experience-card p{
  color:#D7E7F5;
  line-height:1.8;
  margin-bottom:25px;
}

.count{
  font-size:60px;
  font-weight:700;
}

/* ================= PARTNER SLIDER ================= */

.partners{
  background:#f5f5f5;
  padding:100px 0;
  overflow:hidden;
}

.partners h2{
  text-align:center;
  font-size:48px;
  margin-bottom:60px;
  color:#111827;
}

.logo-slider{
  width:100%;
  overflow:hidden;
}

.logo-track{
  display:flex;
  gap:100px;
  align-items:center;
  width:max-content;
  animation:scroll 20s linear infinite;
}

.logo-track img{
  width:180px;
}

@keyframes scroll{

  0%{
    transform:translateX(0);
  }

  100%{
    transform:translateX(-50%);
  }

}

/* ================= SERVICE BOX ================= */

.service-box{
  width:86%;
  margin:80px auto;
  background:white;
  border-radius:30px;
  padding:50px;
  box-shadow:0 10px 30px rgba(0,0,0,0.08);
}

.service-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:60px;
  align-items:center;
}

.service-content h3{
  font-size:36px;
  margin-bottom:30px;
  color:#111827;
}

.service-list{
  display:flex;
  flex-direction:column;
  gap:22px;
  margin-bottom:35px;
}

.service-item{
  display:flex;
  gap:15px;
}

.tick{
  font-size:22px;
}

.service-item p{
  color:#4B5563;
  line-height:1.8;
}

.service-btn{
  display:inline-block;
  padding:14px 28px;
  background:#1476C6;
  color:white;
  text-decoration:none;
  border-radius:40px;
}

.service-image img{
  width:100%;
  border-radius:25px;
}

/* ================= CLIENT SLIDER ================= */

.client-slider-section{
  width:100%;
  padding:90px 0;
  background:white;
  overflow:hidden;
  text-align:center;
}

.client-slider-section h2{
  font-size:48px;
  color:#111827;
  margin-bottom:70px;
  font-weight:500;
}

.client-slider{
  width:100%;
  overflow:hidden;
}

.client-track{
  display:flex;
  align-items:center;
  gap:120px;
  width:max-content;
  animation:clientScroll 20s linear infinite;
}

.client-track img{
  width:220px;
  object-fit:contain;
}

@keyframes clientScroll{

  0%{
    transform:translateX(-50%);
  }

  100%{
    transform:translateX(0%);
  }

}

/* ================= RESPONSIVE ================= */

@media(max-width:1000px){

  .about-container,
  .experience-grid,
  .service-grid{
    grid-template-columns:1fr;
  }

}
*{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins',sans-serif;
    }

    body{
      background:#f5f5f5;
    }

    /* ================= SECTION ================= */

    .industries-section{
      width:100%;
      padding:80px 5%;
      background:#f5f5f5;
      text-align:center;
    }

    .industries-title{
      margin-bottom:60px;
    }

    .industries-title h1{
      font-size:64px;
      font-weight:400;
      color:#111827;
      margin-bottom:12px;
    }

    .industries-title p{
      font-size:22px;
      color:#374151;
    }

    /* ================= IMAGE ================= */

    .industries-image{
      width:100%;
      display:flex;
      justify-content:center;
    }

    .industries-image img{
      width:100%;
      max-width:1150px;
      border-radius:12px;
      display:block;
    }

    /* ================= RESPONSIVE ================= */

    @media(max-width:768px){

      .industries-title h1{
        font-size:42px;
      }

      .industries-title p{
        font-size:17px;
      }

    }
 *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins',sans-serif;
    }

    body{
      background:#f5f5f5;
    }

    /* ================= CERTIFICATIONS SECTION ================= */

    .certifications-section{
      width:100%;
      padding:80px 5%;
      background:#f5f5f5;
      text-align:center;
    }

    .certifications-title{
      margin-bottom:70px;
    }

    .certifications-title h1{
      font-size:82px;
      font-weight:400;
      color:#1f1f1f;
      margin-bottom:15px;
    }

    .certifications-title p{
      font-size:24px;
      color:#2d2d2d;
      font-weight:400;
    }

    /* ================= IMAGE ================= */

    .certifications-image{
      width:100%;
      display:flex;
      justify-content:center;
    }

    .certifications-image img{
      width:100%;
      max-width:1200px;
      display:block;
    }

    /* ================= RESPONSIVE ================= */

    @media(max-width:768px){

      .certifications-title h1{
        font-size:46px;
      }

      .certifications-title p{
        font-size:18px;
      }

    }
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Poppins',sans-serif;
}

body{
  background:#f5f5f5;
}

/* ================= BENEFITS SECTION ================= */

.benefits-section{
  width:100%;
  padding:90px 8%;
  background:#f5f5f5;
  text-align:center;
}

/* ================= TOP TAG ================= */

.feature-tag{
  display:inline-block;
  padding:8px 18px;
  border:1px solid #2196f3;
  border-radius:30px;
  color:#2196f3;
  font-size:15px;
  margin-bottom:30px;
}

/* ================= TITLE ================= */

.benefits-title{
  font-size:72px;
  line-height:1.15;
  color:#1f1f1f;
  font-weight:400;
  max-width:900px;
  margin:0 auto 90px;
}

/* ================= GRID ================= */

.benefits-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:80px 60px;
}

/* ================= CARD ================= */

.benefit-card{
  text-align:center;
}

/* ================= ICON ================= */

.icon-box{
  width:64px;
  height:64px;
  margin:0 auto 28px;
  border-radius:16px;
  background:linear-gradient(135deg,#2ec7f0,#1675d1);
  display:flex;
  align-items:center;
  justify-content:center;
  color:white;
  font-size:28px;
}

/* ================= HEADING ================= */

.benefit-card h3{
  font-size:22px;
  line-height:1.5;
  color:#222;
  margin-bottom:18px;
  font-weight:500;
}

/* ================= PARAGRAPH ================= */

.benefit-card p{
  font-size:18px;
  line-height:1.7;
  color:#666;
  max-width:320px;
  margin:auto;
}

/* ================= RESPONSIVE ================= */

@media(max-width:1000px){

  .benefits-grid{
    grid-template-columns:repeat(2,1fr);
  }

  .benefits-title{
    font-size:52px;
  }

}

@media(max-width:768px){

  .benefits-grid{
    grid-template-columns:1fr;
  }

  .benefits-title{
    font-size:42px;
  }

  .benefit-card p{
    font-size:16px;
  }

}
/* ================= RESULTS SECTION ================= */

.results-section{
  width:100%;
  padding:100px 5%;
  background:#f5f5f5;
  text-align:center;
}

.results-tag{
  display:inline-block;
  padding:10px 22px;
  border:1px solid #d1d5db;
  border-radius:40px;
  font-size:22px;
  color:#1476C6;
  margin-bottom:35px;
  background:white;
}

.results-section h1{
  font-size:82px;
  font-weight:400;
  color:#111827;
  margin-bottom:90px;
  line-height:1.1;
}

.results-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:0;
}

.result-box{
  padding:10px 35px;
  border-right:1px solid #cbd5e1;
}

.no-border{
  border-right:none;
}

.result-box h2{
  font-size:92px;
  color:#1476C6;
  font-weight:400;
  margin-bottom:18px;
}

.result-box p{
  font-size:20px;
  line-height:1.5;
  color:#2d2d2d;
  font-weight:500;
}

@media(max-width:1000px){

  .results-grid{
    grid-template-columns:repeat(2,1fr);
    gap:50px;
  }

  .result-box{
    border-right:none;
  }

}

@media(max-width:7680px){

  .results-section h1{
    font-size:48px;
  }

  .results-tag{
    font-size:16px;
  }

  .result-box h2{
    font-size:60px;
  }

  .result-box p{
    font-size:17px;
  }

}

@media(max-width:600px){

  .results-grid{
    grid-template-columns:1fr;
  }

}

</style>

</head>

<body>

<!-- ================= HEADER ================= -->

<header>

  <div class="logo">
    <img src="Color.png">
  </div>

  <nav>
    <a href="#">Services</a>
    <a href="#">Careers</a>
    <a href="#">Case Studies</a>
    <a href="#">About Us</a>
    <a href="#">Blog</a>
    <a href="#" class="contact-btn">Contact Us</a>
  </nav>

</header>

<!-- ================= HERO ================= -->

<section class="hero">

  <div class="hero-content">

    <h1>
      Transform Your Business
      with AI-Powered
      CRM Automation
    </h1>

    <p>
      Save thousands of hours with autonomous AI agents built using Salesforce Agentforce and Zoho.
    </p>

    <a href="#" class="hero-btn">
      Book Free ROI Assessment
    </a>

  </div>

</section>

<!-- ================= ABOUT ================= -->

<section class="about-section">

  <div class="about-container">

    <div class="about-left">

      <div class="partner-logos">

        <div class="logo-card">
          <img src="FP01.png">
        </div>

        <div class="logo-card">
          <img src="FP02.png">
        </div>

        <div class="logo-card">
          <img src="FP03.png">
        </div>

      </div>

      <h2>
        We are certified partners for Zoho, Salesforce, and ActiveCampaign.
      </h2>

      <p>
        Our expert team helps simplify workflows and increase growth.
      </p>

      <a href="#" class="about-btn">
        Read More
      </a>

    </div>

    <div class="about-right">
      <img src="FP04.png">
    </div>

  </div>

</section>

<!-- ================= EXPERIENCE ================= -->

<section class="experience-section">

  <h2 class="section-title">
    Our Experience
  </h2>

  <p class="section-subtitle">
    Highlighting our deep proficiency in Salesforce implementation and integration.
  </p>

  <div class="experience-grid">

    <div class="experience-card">

      <h3>Salesforce Specialisation</h3>

      <p>
        Expertise across Salesforce clouds and solutions.
      </p>

    </div>

    <div class="experience-card">

      <h3>Zoho Specialisation</h3>

      <div class="count">20+</div>

      <p>
        Salesforce and Zoho certified specialists
      </p>

    </div>

  </div>

</section>

<!-- ================= PARTNER SLIDER ================= -->

<section class="partners">

  <h2>
    Our Globally Renowned Partners
  </h2>

  <div class="logo-slider">

    <div class="logo-track">

      <img src="FP01.png">
      <img src="FP02.png">
      <img src="FP03.png">
      <img src="FP01.png">
      <img src="FP02.png">

      <img src="FP01.png">
      <img src="FP02.png">
      <img src="FP03.png">
      <img src="FP01.png">
      <img src="FP02.png">

    </div>

  </div>

</section>

<!-- ================= SALESFORCE ================= -->

<div class="service-box">

  <div class="service-grid">

    <div class="service-content">

      <h3>Salesforce Services</h3>

      <div class="service-list">

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Fast deployment for Sales, Service and Experience Cloud</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Custom objects, automations and dashboards</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Secure integrations with core business systems</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Ongoing support and performance optimisation</p>
        </div>

      </div>

      <a href="#" class="service-btn">Read More</a>

    </div>

    <div class="service-image">
      <img src="FP10.png">
    </div>

  </div>

</div>

<!-- ================= ZOHO ================= -->

<div class="service-box">

  <div class="service-grid">

    <div class="service-content">

      <h3>Zoho Solutions</h3>

      <div class="service-list">

        <div class="service-item">
          <span class="tick">✔</span>
          <p>CRM setup and workflow automation</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Custom apps with Zoho Creator</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Accounting and finance migration via Zoho Books</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Project management and analytics rollout</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>HR, support desk, inventory tracking, and reporting</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Full suite orchestration and team training</p>
        </div>

      </div>

      <a href="#" class="service-btn">Read More</a>

    </div>

    <div class="service-image">
      <img src="FP05.png">
    </div>

  </div>

</div>

<!-- ================= WORKDAY ================= -->

<div class="service-box">

  <div class="service-grid">

    <div class="service-content">

      <h3>Workday Services</h3>

      <div class="service-list">

        <div class="service-item">
          <span class="tick">✔</span>
          <p>HR and finance system implementation</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Secure migration and data integrity</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Integration with payroll and third-party tools</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Proactive support and troubleshooting</p>
        </div>

      </div>

      <a href="#" class="service-btn">Read More</a>

    </div>

    <div class="service-image">
      <img src="FP06.png">
    </div>

  </div>

</div>

<!-- ================= MANAGED SERVICES ================= -->

<div class="service-box">

  <div class="service-grid">

    <div class="service-content">

      <h3>Managed Services</h3>

      <div class="service-list">

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Quarterly CRM health checks</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Admin support and user enablement</p>
        </div>

      </div>

      <a href="#" class="service-btn">Read More</a>

    </div>

    <div class="service-image">
      <img src="FP07.png">
    </div>

  </div>

</div>

<!-- ================= CERTIFIED TALENT ================= -->

<div class="service-box">

  <div class="service-grid">

    <div class="service-content">

      <h3>Certified Talent Pool</h3>

      <div class="service-list">

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Rapid access to Salesforce and Workday experts</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Flexible staffing and project delivery</p>
        </div>

      </div>

      <a href="#" class="service-btn">Read More</a>

    </div>

    <div class="service-image">
      <img src="FP08.png">
    </div>

  </div>

</div>

<!-- ================= AI ================= -->

<div class="service-box">

  <div class="service-grid">

    <div class="service-content">

      <h3>AI & Agentforce Automation</h3>

      <div class="service-list">

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Smart agents for support and lead qualification</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Automated reporting and operations</p>
        </div>

        <div class="service-item">
          <span class="tick">✔</span>
          <p>Always-on responses and workflow recommendations</p>
        </div>

      </div>

      <a href="#" class="service-btn">Read More</a>

    </div>

    <div class="service-image">
      <img src="FP09.png">
    </div>

  </div>

</div>

<!-- ================= CLIENT SLIDER ================= -->

<section class="client-slider-section">

  <h2>
    Our Globally Renowned Clients
  </h2>

  <div class="client-slider">

    <div class="client-track">

      <img src="slide06.png">
      <img src="slide02.png">
      <img src="slide03.png">
      <img src="slide04.png">
      <img src="slide05.png">

      <img src="slide06.png">
      <img src="slide02.png">
      <img src="slide03.png">
      <img src="slide04.png">
      <img src="slide05.png">

    </div>

  </div>

</section>
<!-- ================= INDUSTRIES SECTION ================= -->

  <section class="industries-section">

    <div class="industries-title">

      <h1>
        Industries We Serve
      </h1>

      <p>
        One Platform. Many Industries. Specialist Experience.
      </p>

    </div>

    <div class="industries-image">

      <!-- USE YOUR SINGLE IMAGE HERE -->

      <img src="Industries.png" alt="Industries We Serve">

    </div>
  </section>
 <!-- ================= CERTIFICATIONS SECTION ================= -->

  <section class="certifications-section">

    <div class="certifications-title">

      <h1>
        Our Certifications
      </h1>

      <p>
        One Platform. Many Industries. Specialist Experience.
      </p>

    </div>

    <div class="certifications-image">

      <!-- USE YOUR SINGLE IMAGE -->

      <img src="FP11.png" alt="Our Certifications">

    </div>
<script>

window.addEventListener("scroll",function(){

  const header=document.querySelector("header");

  header.classList.toggle("scrolled",window.scrollY > 50);

});

</script>
<!-- ================= BENEFITS SECTION ================= -->

<section class="benefits-section">

  <div class="feature-tag">
    ⚙ Features
  </div>

  <h1 class="benefits-title">
    Key benefits that set us apart from other firms
  </h1>

  <div class="benefits-grid">

    <!-- CARD 1 -->

    <div class="benefit-card">

      <div class="icon-box">⚙</div>

      <h3>
        Autonomous AI Automation
      </h3>

      <p>
        Agentforce AI eliminates repetitive tasks, saving 20+ hours weekly.
      </p>

    </div>

    <!-- CARD 2 -->

    <div class="benefit-card">

      <div class="icon-box">✎</div>

      <h3>
        Elite Certified Expertise
      </h3>

      <p>
        100+ Years Combined CRM Experience led by multiple Salesforce Architects.
      </p>

    </div>

    <!-- CARD 3 -->

    <div class="benefit-card">

      <div class="icon-box">▣</div>

      <h3>
        Measurable, Guaranteed ROI
      </h3>

      <p>
        Guaranteed results: 40% sales increase and 27% reduction in service costs.
      </p>

    </div>

    <!-- CARD 4 -->

    <div class="benefit-card">

      <div class="icon-box">◔</div>

      <h3>
        End-to-End CRM Transformation
      </h3>

      <p>
        Full lifecycle support: Strategy, Implementation, and Ongoing Managed Services.
      </p>

    </div>

    <!-- CARD 5 -->

    <div class="benefit-card">

      <div class="icon-box">▤</div>

      <h3>
        Multi-Platform Ecosystem Mastery
      </h3>

      <p>
        Official partners for Salesforce, Zoho, and Workday for unified systems.
      </p>

    </div>

    <!-- CARD 6 -->

    <div class="benefit-card">

      <div class="icon-box">◍</div>

      <h3>
        Global Reach
      </h3>

      <p>
        Melbourne HQ with global development resources.
      </p>

    </div>

  </div>

</section>
<!-- ================= RESULTS SECTION ================= -->

<section class="results-section">

  <div class="results-tag">
    ✓ Success Stories
  </div>

  <h1>
    Measurable Results for Businesses
  </h1>

  <div class="results-grid">

    <!-- BOX 1 -->

    <div class="result-box">
      <h2>40%</h2>
      <p>
        Average increase in sales effectiveness
      </p>
    </div>

    <!-- BOX 2 -->

    <div class="result-box">
      <h2>27%</h2>
      <p>
        Reduction in customer service costs
      </p>
    </div>

    <!-- BOX 3 -->

    <div class="result-box">
      <h2>20+</h2>
      <p>
        Hours saved per week through automation
      </p>
    </div>

    <!-- BOX 4 -->

    <div class="result-box no-border">
      <h2>95%</h2>
      <p>
        Client satisfaction rating
      </p>
    </div>

  </div>

</section>
</body>
</html>
