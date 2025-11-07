<template>
<section class="cta-section">
  <div class="cta-overlay">
    <div class="cta-content">
      <!-- Left: Bag Image -->
      <div class="cta-image">
        <img
          src="https://images.pexels.com/photos/2081199/pexels-photo-2081199.jpeg"
          alt="BagPoint Backpack"
        />
      </div>

      <!-- Right: CTA Text + Form -->
      <div class="cta-text">
        <h2>Stay Connected with BagPoint</h2>
        <p>
          Have a question or want to know more about our new collection?
          Reach out and we’ll get back to you within 24 hours.
        </p>

        <form class="cta-form">
          <input type="text" placeholder="Your Name" required />
          <input type="email" placeholder="Your Email" required />
          <textarea placeholder="Message" rows="3"></textarea>
          <button type="submit">Send Message</button>
        </form>
      </div>
    </div>
  </div>
</section>

</template>
<style scoped>
.cta-section {
  position: relative;
  background: url('https://images.unsplash.com/photo-1581291519195-ef11498d1cf5?auto=format&fit=crop&w=1600&q=80')
    center/cover no-repeat;
  padding: 100px 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.cta-overlay {
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(12px);
  border-radius: 20px;
  padding: 50px;
  width: 100%;
  max-width: 1100px;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
}

.cta-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  align-items: center;
  gap: 50px;
  color: #fff;
}

.cta-image img {
  width: 100%;
  border-radius: 16px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
  transition: transform 0.4s ease;
}

.cta-image img:hover {
  transform: scale(1.05);
}

.cta-text h2 {
  font-size: 2.4rem;
  margin-bottom: 15px;
  color: #fff;
}

.cta-text p {
  color: #e2e8f0;
  margin-bottom: 25px;
  line-height: 1.7;
}

.cta-form {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.cta-form input,
.cta-form textarea {
  background: rgba(255, 255, 255, 0.2);
  border: 1px solid rgba(255, 255, 255, 0.3);
  color: #fff;
  padding: 12px;
  border-radius: 10px;
  font-size: 1rem;
  outline: none;
  transition: 0.3s;
}

.cta-form input::placeholder,
.cta-form textarea::placeholder {
  color: #cbd5e1;
}

.cta-form input:focus,
.cta-form textarea:focus {
  background: rgba(255, 255, 255, 0.3);
  border-color: #60a5fa;
}

.cta-form button {
  background: linear-gradient(135deg, #2563eb, #3b82f6);
  color: #fff;
  border: none;
  padding: 12px 20px;
  border-radius: 10px;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
}

.cta-form button:hover {
  background: linear-gradient(135deg, #1e40af, #2563eb);
  transform: translateY(-2px);
}

</style>
