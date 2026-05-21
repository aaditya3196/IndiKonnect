<template>
  <div class="returns-page">

    <section class="hero-section">
      <div class="hero-glow one"></div>
      <div class="hero-glow two"></div>

      <div class="hero-container reveal">
        <p class="eyebrow">Customer Support</p>
        <h1>Return & Replacement Policy</h1>
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

    <section class="section">
      <div class="policy-card reveal">
        <div class="card-top">
          <div class="card-icon">↺</div>
          <h2>Return and Replacement of Your Ordered Products</h2>
        </div>
        <div class="card-body-text">
          <p>
            In the event the product/s received by you is different from what was
            ordered, you must notify us via email within seven (7) days from the
            date of receipt of the product.
          </p>
          <p>
            In the event of any damage or there is shortage of the product/s
            received; you must notify us via email within seven (7) days of
            receipt of the product/s.
          </p>
        </div>
      </div>
    </section>

    <section class="section light-bg">
      <div class="section-title reveal">
        <p class="sub-title">Important Timelines</p>
        <h2>Replacement Process Timeline</h2>
      </div>

      <div class="timeline-grid">
        <div class="timeline-card reveal">
          <div class="timeline-header">
            <div class="timeline-number">01</div>
            <h3>Report Within 7 Days</h3>
          </div>
          <p>
            Customers and distributors must notify Indi Konnect within seven (7)
            days from the date of receipt of the product.
          </p>
        </div>

        <div class="timeline-card reveal">
          <div class="timeline-header">
            <div class="timeline-number yellow">02</div>
            <h3>Product Verification</h3>
          </div>
          <p>
            Returned products are verified upon receipt at the Indi Konnect
            warehouse and checked against all replacement criteria.
          </p>
        </div>

        <div class="timeline-card reveal">
          <div class="timeline-header">
            <div class="timeline-number">03</div>
            <h3>Dispatch & Delivery</h3>
          </div>
          <p>
            Approved exchanged or replacement products will be dispatched and
            delivered within the specified timelines.
          </p>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-title reveal">
        <p class="sub-title">Product Exchange</p>
        <h2>Exchange Checklist</h2>
      </div>

      <div class="checklist-wrapper">
        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            Physical Product replacement requests are applicable only within
            7 days from the date of receipt of the product.
          </p>
        </div>

        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            The Distributor should send a mail from his/her registered email ID
            only, within 7 days from the date of receipt, mentioning all
            relevant details to <span class="highlight-inline">support@indikonnect.in</span>
          </p>
        </div>

        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            Online form to be downloaded and filled in by the Distributor while
            couriering the product back to the Indi Konnect warehouse for
            product replacement.
          </p>
        </div>

        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            The Distributor should meet all criteria related to the product
            replacement.
          </p>
        </div>

        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            Upon receipt of the returned product(s) at the Indi Konnect
            warehouse, and subject to compliance with all the stipulated
            criteria for replacement, the company will initiate dispatch of the
            correct product(s) within seven (7) working days.
          </p>
        </div>

        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            In the event of a delay beyond the stipulated timeline due to
            non-availability of stock, the concerned Distributor/Customer will
            be notified via email regarding the revised dispatch schedule.
          </p>
        </div>

        <div class="checklist-card reveal">
          <div class="check-icon">✓</div>
          <p>
            If approved, the exchanged or replaced product will be delivered
            within 15 days.
          </p>
        </div>
      </div>
    </section>

    <section class="section dark-bg-section">
      <div class="note-card reveal">
        <div class="note-icon">!</div>
        <div class="note-content">
          <p class="note-title">Important Notice</p>
          <p class="note-text">
            Please note: Any updates regarding delays in product deliveries are
            published on the official company website for reference.
          </p>
        </div>
      </div>
    </section>

    <section class="section support-section">
      <div class="support-card reveal">
        <p class="eyebrow-dark">Need Assistance?</p>
        <h2>Contact Indi Konnect Support</h2>

        <div class="support-grid">
          <div class="support-item">
            <span class="support-label">Email</span>
            <p class="support-value font-medium">support@Indi Konnect.in</p>
          </div>

          <div class="support-item">
            <span class="support-label">Phone</span>
            <p class="support-value font-medium">+91 98765 43210</p>
          </div>

          <div class="support-item">
            <span class="support-label">Address</span>
            <p class="support-value leading-relaxed">
              SCO 112-113, Sector 34A,<br>
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
      threshold: 0.08, // Slightly lowered for better mobile viewport calculation trigger
    }
  );

  revealElements.forEach((el) => {
    observer.observe(el);
  });
});
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;600;700;800&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.returns-page {
  font-family: 'Raleway', sans-serif;
  background: #ffffff;
  color: #2D3748;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* HERO SECTION */
.hero-section {
  position: relative;
  padding: 80px 5% 70px;
  background: #003DA5;
  overflow: hidden;
  display: flex;
  justify-content: center;
}

.hero-container {
  width: 100%;
  max-width: 1140px;
  position: relative;
  z-index: 2;
}

.hero-glow {
  position: absolute;
  border-radius: 50%;
  filter: blur(100px);
  pointer-events: none;
}

.hero-glow.one {
  width: 350px;
  height: 350px;
  background: rgba(255, 199, 44, 0.15);
  top: -100px;
  right: -50px;
}

.hero-glow.two {
  width: 300px;
  height: 300px;
  background: rgba(255, 255, 255, 0.06);
  bottom: -100px;
  left: -50px;
}

.eyebrow {
  color: #FFC72C;
  text-transform: uppercase;
  letter-spacing: 2.5px;
  font-size: 14px;
  margin-bottom: 14px;
  font-weight: 700;
}

.hero-container h1 {
  color: #ffffff;
  font-size: 46px;
  line-height: 1.15;
  margin-bottom: 18px;
  font-weight: 800;
  letter-spacing: -0.5px;
  max-width: 800px;
}

.hero-text {
  color: rgba(255, 255, 255, 0.88);
  font-size: 18px;
  line-height: 1.6;
  max-width: 700px;
  margin-bottom: 32px;
}

.hero-badges {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}

.hero-badge {
  background: rgba(255, 255, 255, 0.07);
  border: 1px solid rgba(255, 255, 255, 0.14);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  padding: 16px 24px;
  border-radius: 16px;
  min-width: 220px;
}

.badge-num {
  display: block;
  color: #FFC72C;
  font-size: 32px;
  font-weight: 800;
  margin-bottom: 4px;
  line-height: 1;
}

.badge-lbl {
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
}

/* UNIVERSAL SECTIONS STRUCTURING */
.section {
  padding: 60px 5%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.section > div {
  width: 100%;
  max-width: 1140px;
}

.light-bg {
  background: #F7FAFC;
}

.dark-bg-section {
  background: #003DA5;
  padding: 50px 5%;
}

/* SECTION TITLES */
.section-title {
  margin-bottom: 40px;
  text-align: left;
}

.sub-title {
  color: #003DA5;
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 13px;
  margin-bottom: 8px;
  font-weight: 700;
}

.section-title h2 {
  font-size: 32px;
  color: #1A202C;
  font-weight: 800;
  letter-spacing: -0.5px;
}

/* POLICY CARD */
.policy-card {
  background: #ffffff;
  border-radius: 24px;
  padding: 40px;
  border: 1px solid rgba(0, 61, 165, 0.08);
  box-shadow: 0 10px 30px rgba(0, 61, 165, 0.03);
}

.card-top {
  display: flex;
  align-items: center;
  gap: 20px;
  margin-bottom: 28px;
}

.card-icon {
  width: 56px;
  height: 56px;
  border-radius: 16px;
  background: #FFC72C;
  color: #003DA5;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 26px;
  font-weight: 700;
  flex-shrink: 0;
}

.policy-card h2 {
  font-size: 28px;
  color: #1A202C;
  font-weight: 800;
  line-height: 1.2;
}

.card-body-text p {
  color: #4A5568;
  line-height: 1.7;
  font-size: 16px;
  margin-bottom: 18px;
}

.card-body-text p:last-child {
  margin-bottom: 0;
}

/* TIMELINE PROCESS CARDS */
.timeline-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

.timeline-card {
  background: #ffffff;
  border-radius: 20px;
  padding: 32px;
  border: 1px solid rgba(0, 61, 165, 0.06);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.02);
  display: flex;
  flex-direction: column;
}

.timeline-header {
  display: flex;
  align-items: center;
  gap: 16px;
  margin-bottom: 20px;
}

.timeline-number {
  width: 48px;
  height: 48px;
  border-radius: 12px;
  background: #003DA5;
  color: #ffffff;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 800;
  font-size: 16px;
  flex-shrink: 0;
}

.timeline-number.yellow {
  background: #FFC72C;
  color: #003DA5;
}

.timeline-card h3 {
  font-size: 20px;
  color: #1A202C;
  font-weight: 700;
}

.timeline-card p {
  color: #4A5568;
  line-height: 1.65;
  font-size: 15px;
}

/* CHECKLIST FIXES */
.checklist-wrapper {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.checklist-card {
  display: flex;
  gap: 18px;
  align-items: flex-start; /* Forces children to align at the top bounds */
  background: #ffffff;
  border-radius: 16px;
  padding: 24px;
  border: 1px solid rgba(0, 61, 165, 0.06);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.01);
}

.check-icon {
  width: 36px;
  height: 36px;
  border-radius: 10px;
  background: rgba(0, 61, 165, 0.08);
  color: #003DA5;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 800;
  font-size: 15px;
  flex-shrink: 0;
  /* Added a tiny top margin so the box is centered with the exact mid-point of the first line text */
  margin-top: 2px; 
}

.checklist-card p {
  color: #4A5568;
  font-size: 15px;
  /* Balanced line height to clean up tracking with multi-line wrap text */
  line-height: 1.65; 
  margin: 0;
  padding: 0;
}

.highlight-inline {
  color: #003DA5;
  font-weight: 600;
}

/* BANNER NOTES */
.note-card {
  display: flex;
  gap: 24px;
  align-items: center;
  background: rgba(255, 255, 255, 0.08);
  border: 1px solid rgba(255, 255, 255, 0.15);
  padding: 32px;
  border-radius: 20px;
}

.note-icon {
  width: 48px;
  height: 48px;
  border-radius: 14px;
  background: #FFC72C;
  color: #003DA5;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 24px;
  font-weight: 800;
  flex-shrink: 0;
}

.note-content {
  flex: 1;
}

.note-title {
  color: #ffffff;
  font-size: 20px;
  margin-bottom: 6px;
  font-weight: 700;
}

.note-text {
  color: rgba(255, 255, 255, 0.88);
  line-height: 1.6;
  font-size: 15px;
}

/* CONTACT SUPPORT CARD */
.support-card {
  background: #F7FAFC;
  border-radius: 28px;
  padding: 48px;
  border: 1px solid rgba(0, 61, 165, 0.08);
  box-shadow: 0 10px 35px rgba(0, 61, 165, 0.02);
}

.eyebrow-dark {
  color: #003DA5;
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 13px;
  margin-bottom: 10px;
  font-weight: 700;
}

.support-card h2 {
  font-size: 36px;
  color: #1A202C;
  font-weight: 800;
  margin-bottom: 36px;
  letter-spacing: -0.5px;
}

.support-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

.support-item {
  background: #ffffff;
  border-radius: 16px;
  padding: 28px;
  border-top: 4px solid #FFC72C;
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.02);
}

.support-label {
  display: block;
  color: #003DA5;
  font-size: 12px;
  font-weight: 700;
  text-transform: uppercase;
  margin-bottom: 12px;
  letter-spacing: 1.5px;
}

.support-value {
  color: #2D3748;
  font-size: 16px;
  line-height: 1.5;
}

.font-medium {
  font-weight: 600;
}

/* SCROLL INTERSECTION REVEAL */
.reveal {
  opacity: 0;
  transform: translateY(30px);
  filter: blur(4px);
  transition:
    opacity 0.8s cubic-bezier(0.215, 0.61, 0.355, 1),
    transform 0.8s cubic-bezier(0.215, 0.61, 0.355, 1),
    filter 0.8s cubic-bezier(0.215, 0.61, 0.355, 1);
}

.reveal.active {
  opacity: 1;
  transform: translateY(0);
  filter: blur(0);
}

/* RESPONSIVE MEDIA BREAKPOINTS */
@media (max-width: 1024px) {
  .timeline-grid {
    grid-template-columns: repeat(2, 1fr);
  }
  .support-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
  .hero-section {
    padding: 60px 6% 50px;
  }

  .hero-container h1 {
    font-size: 34px;
  }

  .hero-text {
    font-size: 16px;
  }

  .section {
    padding: 40px 6%;
  }

  .section-title h2,
  .support-card h2 {
    font-size: 26px;
  }

  .policy-card {
    padding: 28px;
  }

  .policy-card h2 {
    font-size: 22px;
  }

  .timeline-grid,
  .support-grid {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .note-card {
    flex-direction: column;
    align-items: flex-start;
    gap: 16px;
    padding: 24px;
  }

  .support-card {
    padding: 32px 24px;
  }
}

@media (max-width: 480px) {
  .hero-badges {
    flex-direction: column;
    gap: 12px;
  }
  
  .hero-badge {
    min-width: 100%;
  }

  .card-top {
    flex-direction: column;
    align-items: flex-start;
    gap: 14px;
  }
}
</style>