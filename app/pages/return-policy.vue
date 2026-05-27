<template>
  <div class="returns-page">

    <!-- HERO -->
    <section class="hero-section">

      <div class="hero-glow one"></div>
      <div class="hero-glow two"></div>

      <div class="hero-container reveal">

        <p class="eyebrow">
          Customer Support
        </p>

        <h1>
          Return & Replacement Policy
        </h1>

        <p class="hero-text">
          Indi Konnect is committed to providing a smooth and transparent
          replacement experience for all customers and distributors.
        </p>

        <div class="hero-badges">

          <div class="hero-badge">
            <span class="badge-num">7 Days</span>
            <p class="badge-lbl">Replacement Window</p>
          </div>

          <div class="hero-badge">
            <span class="badge-num">15 Days</span>
            <p class="badge-lbl">Delivery Timeline</p>
          </div>

        </div>

      </div>

    </section>

    <!-- CONTENT -->
    <section class="content-section">

      <div class="content-wrapper reveal">

        <h2>
          Return and Replacement of Your Ordered Products
        </h2>

        <div class="legal-point">
          <p>
            <span class="point-number">1.</span>
            In the event the product/s received by you is different from what was
            ordered, you must notify us via email within seven (7) days from the
            date of receipt of the product.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">2.</span>
            In the event of any damage or there is shortage of the product/s
            received; you must notify us via email within seven (7) days of
            receipt of the product/s.
          </p>
        </div>

        <h2 class="section-heading">
          Replacement Process Timeline
        </h2>

        <div class="legal-point">
          <p>
            <span class="point-number">3.</span>
            Customers and distributors must notify Indi Konnect within seven (7)
            days from the date of receipt of the product.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">4.</span>
            Returned products are verified upon receipt at the Indi Konnect
            warehouse and checked against all replacement criteria.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">5.</span>
            Approved exchanged or replacement products will be dispatched and
            delivered within the specified timelines.
          </p>
        </div>

        <h2 class="section-heading">
          Exchange Checklist
        </h2>

        <div class="legal-point">
          <p>
            <span class="point-number">6.</span>
            Physical Product replacement requests are applicable only within
            7 days from the date of receipt of the product.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">7.</span>
            The Distributor should send a mail from his/her registered email ID
            only, within 7 days from the date of receipt, mentioning all
            relevant details to dummy@indikonnect.com
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">8.</span>
            Online form to be downloaded and filled in by the Distributor while
            couriering the product back to the Indi Konnect warehouse for
            product replacement.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">9.</span>
            The Distributor should meet all criteria related to the product
            replacement.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">10.</span>
            Upon receipt of the returned product(s) at the Indi Konnect
            warehouse, and subject to compliance with all the stipulated
            criteria for replacement, the company will initiate dispatch of the
            correct product(s) within seven (7) working days.
          </p>
        </div>

        <div class="legal-point">
          <p>
            <span class="point-number">11.</span>
            In the event of a delay beyond the stipulated timeline due to
            non-availability of stock, the concerned Distributor/Customer will
            be notified via email regarding the revised dispatch schedule.
          </p>
        </div>

        <div class="legal-point last-point">
          <p>
            <span class="point-number">12.</span>
            If approved, the exchanged or replaced product will be delivered
            within 15 days.
          </p>
        </div>

      </div>

    </section>

    <!-- NOTICE -->
    <section class="notice-section">

      <div class="notice-card reveal">

        <div class="note-icon">
          !
        </div>

        <div>

          <p class="notice-title">
            Important Notice
          </p>

          <p class="notice-text">
            Please note: Any updates regarding delays in product deliveries are
            published on the official company website for reference.
          </p>

        </div>

      </div>

    </section>

    <!-- SUPPORT -->
    <section class="support-section">

      <div class="support-card reveal">

        <p class="eyebrow-dark">
          Need Assistance?
        </p>

        <h2>
          Contact Indi Konnect Support
        </h2>

        <div class="support-grid">

          <div class="support-item">

            <span class="support-label">
              Email
            </span>

            <p class="support-value font-medium">
              dummy@indikonnect.com
            </p>

          </div>

          <div class="support-item">

            <span class="support-label">
              Phone
            </span>

            <p class="support-value font-medium">
              +91 12345 67891
            </p>

          </div>

          <div class="support-item">

            <span class="support-label">
              Address
            </span>

            <p class="support-value leading-relaxed">
              Dummy address,<br>
              Chandigarh, India 160022
            </p>

          </div>

        </div>

      </div>

    </section>

  </div>
</template>

<script setup>
import { onMounted } from "vue";

onMounted(() => {

  const revealElements = document.querySelectorAll(".reveal");

  const observer = new IntersectionObserver(
    (entries) => {

      entries.forEach((entry) => {

        if (entry.isIntersecting) {
          entry.target.classList.add("active");
        }

      });

    },
    {
      threshold: 0.08,
    }
  );

  revealElements.forEach((el) => {
    observer.observe(el);
  });

});
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;600;700;800&display=swap');

*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

.returns-page{
  font-family:'Raleway',sans-serif;
  background:#ffffff;
  color:#2D3748;
  overflow-x:hidden;
}

/* HERO */

.hero-section{
  position:relative;
  padding:80px 5% 65px;
  background:#003DA5;
  overflow:hidden;
  display:flex;
  justify-content:center;
}

.hero-container{
  width:100%;
  max-width:1140px;
  position:relative;
  z-index:2;
}

.hero-glow{
  position:absolute;
  border-radius:50%;
  filter:blur(100px);
}

.hero-glow.one{
  width:350px;
  height:350px;
  background:rgba(255,199,44,0.15);
  top:-100px;
  right:-50px;
}

.hero-glow.two{
  width:300px;
  height:300px;
  background:rgba(255,255,255,0.06);
  bottom:-100px;
  left:-50px;
}

.eyebrow{
  color:#FFC72C;
  text-transform:uppercase;
  letter-spacing:2.5px;
  font-size:14px;
  margin-bottom:14px;
  font-weight:700;
}

.hero-container h1{
  color:white;
  font-size:46px;
  line-height:1.1;
  margin-bottom:16px;
  font-weight:800;
}

.hero-text{
  color:rgba(255,255,255,0.88);
  font-size:17px;
  line-height:1.6;
  max-width:700px;
  margin-bottom:28px;
}

.hero-badges{
  display:flex;
  gap:18px;
  flex-wrap:wrap;
}

.hero-badge{
  background:rgba(255,255,255,0.07);
  border:1px solid rgba(255,255,255,0.14);
  padding:16px 22px;
  border-radius:16px;
  min-width:220px;
}

.badge-num{
  display:block;
  color:#FFC72C;
  font-size:30px;
  font-weight:800;
  margin-bottom:2px;
}

.badge-lbl{
  color:white;
  font-size:14px;
}

/* CONTENT */

.content-section{
  padding:40px 5%;
}

.content-wrapper{
  max-width:1100px;
  margin:auto;
}

.content-wrapper h2{
  font-size:30px;
  color:#003DA5;
  margin-bottom:20px;
  font-weight:800;
}

.section-heading{
  margin-top:34px;
}

.legal-point{
  padding-bottom:18px;
  margin-bottom:18px;
  border-bottom:1px solid rgba(0,61,165,0.08);
}

.last-point{
  margin-bottom:0;
  padding-bottom:0;
  border-bottom:none;
}

.legal-point p{
  color:#4A5568;
  font-size:15px;
  line-height:1.8;
}

.point-number{
  font-weight:700;
  color:#2D3748;
  margin-right:6px;
}

/* NOTICE */

.notice-section{
  background:#003DA5;
  padding:40px 5%;
}

.notice-card{
  max-width:1100px;
  margin:auto;
  display:flex;
  gap:20px;
  align-items:center;
  background:rgba(255,255,255,0.08);
  border:1px solid rgba(255,255,255,0.15);
  padding:28px;
  border-radius:18px;
}

.note-icon{
  width:46px;
  height:46px;
  border-radius:14px;
  background:#FFC72C;
  color:#003DA5;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:22px;
  font-weight:800;
  flex-shrink:0;
}

.notice-title{
  color:white;
  font-size:20px;
  margin-bottom:6px;
  font-weight:700;
}

.notice-text{
  color:rgba(255,255,255,0.88);
  line-height:1.7;
  font-size:15px;
}

/* SUPPORT */

.support-section{
  padding:40px 5%;
}

.support-card{
  max-width:1100px;
  margin:auto;
  background:#F7FAFC;
  border-radius:24px;
  padding:42px;
  border:1px solid rgba(0,61,165,0.08);
}

.eyebrow-dark{
  color:#003DA5;
  text-transform:uppercase;
  letter-spacing:2px;
  font-size:13px;
  margin-bottom:8px;
  font-weight:700;
}

.support-card h2{
  font-size:32px;
  margin-bottom:28px;
  font-weight:800;
}

.support-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.support-item{
  background:white;
  border-radius:16px;
  padding:24px;
  border-top:4px solid #FFC72C;
}

.support-label{
  display:block;
  color:#003DA5;
  font-size:12px;
  font-weight:700;
  text-transform:uppercase;
  margin-bottom:10px;
  letter-spacing:1.5px;
}

.support-value{
  color:#2D3748;
  font-size:15px;
  line-height:1.6;
}

.font-medium{
  font-weight:600;
}

.leading-relaxed{
  line-height:1.7;
}

/* REVEAL */

.reveal{
  opacity:0;
  transform:translateY(20px);
  transition:all 0.8s ease;
}

.reveal.active{
  opacity:1;
  transform:translateY(0);
}

/* RESPONSIVE */

@media (max-width:768px){

  .hero-section{
    padding:60px 6% 50px;
  }

  .hero-container h1{
    font-size:34px;
  }

  .hero-text{
    font-size:16px;
  }

  .content-section,
  .support-section{
    padding:34px 6%;
  }

  .content-wrapper h2,
  .support-card h2{
    font-size:26px;
  }

  .support-grid{
    grid-template-columns:1fr;
  }

  .notice-card{
    flex-direction:column;
    align-items:flex-start;
  }

  .support-card{
    padding:30px 22px;
  }

}

@media (max-width:480px){

  .hero-badges{
    flex-direction:column;
    gap:12px;
  }

  .hero-badge{
    min-width:100%;
  }

}

</style>
