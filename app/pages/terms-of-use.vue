<template>
  <div class="privacy-page">

    <!-- HERO -->

    <section class="privacy-hero">

      <div class="hero-content">

        <p class="eyebrow">
          Legal Information
        </p>

        <h1>
          Terms of Use
        </h1>

        <p class="hero-description">
          Please read these Terms carefully before using the Indi Konnect website and services.
        </p>

        <div class="updated-tag">
          Updated: January 2026
        </div>

      </div>

    </section>

    <!-- CONTENT -->

    <section class="policy-section">

      <div class="policy-wrapper">

        <!-- INTRO -->

        <div class="policy-card">

          <h2>
            Terms of Use
          </h2>

          <p>
            We provide our services to you through this website based on the Terms of Use (“Terms”).
            Please read the Terms carefully. Your use of this website constitutes your acceptance
            of our Terms.
          </p>

        </div>

        <!-- LICENCE -->

        <div class="policy-card">

          <h3>
            Licence to Use
          </h3>

          <p>
            We grant you a limited licence to access and make personal use of this site.
            Except with our express written consent, you are not allowed to download or
            modify our website, or any portion of it.
          </p>

          <p>
            You are not allowed to reproduce, duplicate, copy or modify our website
            or any portion of it.
          </p>

        </div>

        <!-- DOWNLOADING -->

        <div class="policy-card">

          <h3>
            Downloading
          </h3>

          <p>
            On this website, we may provide materials which you are expressly allowed
            to download. By downloading any such materials, you agree to use the
            materials only for your personal, non-commercial use.
          </p>

          <p>
            You must retain all copyright and other proprietary notices contained
            in the original materials or any copy of those materials.
          </p>

          <p>
            You are not allowed to use these materials for any commercial purposes,
            other than for the purpose of promoting the networking business of the Company,
            or on any other website unless prior approval is obtained from Indi Konnect
            in accordance with Company Policies & Procedures.
          </p>

        </div>

        <!-- ELECTRONIC -->

        <div class="policy-card">

          <h3>
            Electronic Communications
          </h3>

          <p>
            When you make any transaction via our website or send emails to us,
            you agree to receive communications from us electronically.
          </p>

          <p>
            All agreements, notices, disclosures or any other communications that
            we provide to you electronically satisfy any legal requirement that
            such communications be in writing.
          </p>

        </div>

        <!-- COPYRIGHT -->

        <div class="policy-card">

          <h3>
            Copyright
          </h3>

          <p>
            The content of this website, including text, graphics, images,
            logos and the compilation of the content of this website are
            the intellectual property of Indi Konnect.
          </p>

        </div>

        <!-- PERSONAL DATA -->

        <div class="policy-card">

          <h3>
            Personal Data
          </h3>

          <p>
            All personal data you submit to us via this website is governed
            by our Privacy Policy.
          </p>

        </div>

        <!-- LINKS -->

        <div class="policy-card">

          <h3>
            Links to Third Party Websites
          </h3>

          <p>
            Links to third party websites may be provided on our website.
            However, we are not responsible for the content of those
            third-party websites.
          </p>

          <p>
            Please refer to our Disclaimer for further details.
          </p>

        </div>

        <!-- LAW -->

        <div class="policy-card">

          <h3>
            Governing Law and Jurisdiction
          </h3>

          <p>
            These Terms shall be governed by and construed in accordance
            with the laws of India and the parties hereby submit for all
            purposes relating to these Terms to the non-exclusive jurisdiction
            of the courts of India.
          </p>

        </div>

        <!-- CONTACT -->

        <div class="policy-card contact-card">

          <h3>
            Contact Information
          </h3>

          <p>
            If you have any questions regarding these Terms of Use,
            please contact Indi Konnect using the details below.
          </p>

          <div class="contact-grid">

            <div class="contact-item">

              <span>Company</span>

              <strong>
                Indi Konnect Private Limited
              </strong>

            </div>

            <div class="contact-item">

              <span>Address</span>

              <strong>
                SCO 112–113, Sector 34A,<br>
                Chandigarh – 160022,<br>
                Punjab, India
              </strong>

            </div>

            <div class="contact-item">

              <span>Email</span>

              <strong>
                grievance@indikonnect.in<br>
                support@indikonnect.in
              </strong>

            </div>

            <div class="contact-item">

              <span>Phone</span>

              <strong>
                +91 98765 43210<br>
                +91 98111 22334
              </strong>

            </div>

          </div>

        </div>

      </div>

    </section>

  </div>
</template>

<script setup>
useSeoMeta({
  title: 'Terms of Use | Indi Konnect',
  description: 'Read the official Terms of Use of Indi Konnect.',
});
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;600;700;800&display=swap');

* {
  box-sizing: border-box;
}

.privacy-page {
  font-family: 'Raleway', sans-serif;
  background: #f7f9fc;
  color: #333F48;
}

/* HERO */

.privacy-hero {
  background: #003DA5;
  padding: 52px 7% 30px;
}

.hero-content {
  max-width: 820px;
}

.eyebrow {
  color: #FFC72C;
  font-size: 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-weight: 700;
  margin-bottom: 14px;
}

.privacy-hero h1 {
  color: white;
  font-size: 54px;
  line-height: 1;
  margin-bottom: 18px;
  font-weight: 800;
}

.hero-description {
  color: rgba(255,255,255,0.85);
  font-size: 16px;
  line-height: 1.7;
  max-width: 650px;
}

.updated-tag {
  margin-top: 22px;
  display: inline-block;
  padding: 10px 16px;
  border-radius: 10px;
  background: rgba(255,255,255,0.10);
  color: white;
  font-size: 14px;
}

/* CONTENT */

.policy-section {
  padding: 20px 7% 80px;
}

.policy-wrapper {
  max-width: 1100px;
  margin: auto;
}

.policy-card {
  background: white;
  border-radius: 18px;
  padding: 20px;
  margin-bottom: 18px;
  border: 1px solid rgba(0,61,165,0.08);
  box-shadow:
    0 8px 24px rgba(0,0,0,0.04);
}

.policy-card h2 {
  font-size: 34px;
  color: #003DA5;
  margin-bottom: 18px;
}

.policy-card h3 {
  font-size: 24px;
  color: #003DA5;
  margin-bottom: 18px;
}

.policy-card p {
  font-size: 15px;
  line-height: 1.9;
  color: #4c5661;
  margin-bottom: 10px;
  margin-top: 10px;
}

/* CONTACT */

.contact-card {
  background: #003DA5;
}

.contact-card h3,
.contact-card p,
.contact-card strong,
.contact-card span {
  color: white;
}

.contact-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 28px;
}

.contact-item {
  background: rgba(255,255,255,0.08);
  padding: 22px;
  border-radius: 14px;
}

.contact-item span {
  display: block;
  font-size: 12px;
  letter-spacing: 1px;
  text-transform: uppercase;
  margin-bottom: 10px;
  color: rgba(255,255,255,0.70);
}

.contact-item strong {
  line-height: 1.8;
  font-size: 15px;
}

/* RESPONSIVE */

@media (max-width: 768px) {

  .privacy-hero {
    padding: 56px 5% 46px;
  }

  .privacy-hero h1 {
    font-size: 38px;
  }

  .policy-section {
    padding: 34px 5% 60px;
  }

  .policy-card {
    padding: 24px;
    border-radius: 14px;
  }

  .policy-card h2 {
    font-size: 28px;
  }

  .policy-card h3 {
    font-size: 21px;
  }

  .contact-grid {
    grid-template-columns: 1fr;
  }

}

</style>