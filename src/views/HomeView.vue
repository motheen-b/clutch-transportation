<template>
    <div class="home-view">
        <Hero />

        <!-- Services Section -->
        <section id="services" class="services-section">
            <div class="container">
                <div class="section-header">
                    <span class="section-badge">What We Do</span>
                    <h2>Transportation Services</h2>
                    <p>Reliable freight solutions designed for the needs of growing businesses</p>
                </div>
                <div class="services-grid">
                    <div class="service-card">
                        <div class="service-number">01</div>
                        <div class="service-icon-wrapper">
                            <svg width="32" height="32" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M20 8h-3V4H3c-1.1 0-2 .9-2 2v11h2c0 1.66 1.34 3 3 3s3-1.34 3-3h6c0 1.66 1.34 3 3 3s3-1.34 3-3h2v-5l-3-4zM6 18.5c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5zm13.5-9l1.96 2.5H17V9.5h2.5zm-1.5 9c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5z"
                                    fill="currentColor" />
                            </svg>
                        </div>
                        <h3>Local Freight Delivery</h3>
                        <p>Comprehensive freight services across Ontario. From parcels to full truckloads, we handle
                            your cargo with care and precision.</p>
                    </div>
                    <div class="service-card">
                        <div class="service-number">02</div>
                        <div class="service-icon-wrapper">
                            <svg width="32" height="32" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path d="M13 3L4 14h7l-1 7 9-11h-7l1-7z" stroke="currentColor" stroke-width="2"
                                    stroke-linecap="round" stroke-linejoin="round" fill="none" />
                            </svg>
                        </div>
                        <h3>Expedited Shipping</h3>
                        <p>Priority handling for time-critical deliveries. Direct routes and dedicated service ensure
                            your shipment arrives when needed.</p>
                    </div>
                    <div class="service-card">
                        <div class="service-number">03</div>
                        <div class="service-icon-wrapper">
                            <svg width="32" height="32" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"
                                    fill="currentColor" />
                            </svg>
                        </div>
                        <h3>Same-Day Service</h3>
                        <p>Express delivery for urgent shipments. Our responsive team and modern fleet guarantee rapid,
                            reliable transportation.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Why Choose Us Section -->
        <section id="why-choose" class="why-choose-section">
            <div class="container">
                <div class="section-header">
                    <span class="section-badge">Why Clutch</span>
                    <h2>Built for Growing Businesses</h2>
                    <p>We understand the challenges small businesses face, and we're here to help you succeed</p>
                </div>
                <div class="features-grid">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <svg width="28" height="28" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path d="M12 2L2 7v10c0 5.55 3.84 9.74 9 11 5.16-1.26 9-5.45 9-11V7l-10-5z"
                                    fill="currentColor" />
                            </svg>
                        </div>
                        <h3>Reliability You Can Trust</h3>
                        <p>Consistent on-time delivery with real-time tracking. Your cargo is in safe hands from pickup
                            to destination.</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">
                            <svg width="28" height="28" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                    fill="currentColor" />
                            </svg>
                        </div>
                        <h3>Ontario Expertise</h3>
                        <p>Deep knowledge of Ontario routes, traffic patterns, and delivery optimization
                            ensures efficiency.</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">
                            <svg width="28" height="28" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M20 8h-3V4H3c-1.1 0-2 .9-2 2v11h2c0 1.66 1.34 3 3 3s3-1.34 3-3h6c0 1.66 1.34 3 3 3s3-1.34 3-3h2v-5l-3-4z"
                                    fill="currentColor" />
                            </svg>
                        </div>
                        <h3>Modern Equipment</h3>
                        <p>Well-maintained fleet equipped with GPS tracking for complete transparency and safe cargo
                            handling.</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">
                            <svg width="28" height="28" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M16 11c1.66 0 2.99-1.34 2.99-3S17.66 5 16 5c-1.66 0-3 1.34-3 3s1.34 3 3 3zm-8 0c1.66 0 2.99-1.34 2.99-3S9.66 5 8 5C6.34 5 5 6.34 5 8s1.34 3 3 3zm0 2c-2.33 0-7 1.17-7 3.5V19h14v-2.5c0-2.33-4.67-3.5-7-3.5zm8 0c-.29 0-.62.02-.97.05 1.16.84 1.97 1.97 1.97 3.45V19h6v-2.5c0-2.33-4.67-3.5-7-3.5z"
                                    fill="currentColor" />
                            </svg>
                        </div>
                        <h3>Personalized Service</h3>
                        <p>Flexible solutions that scale with your business. From one-time shipments to ongoing
                            partnerships.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="about-section">
            <div class="container">
                <div class="about-content">
                    <div class="about-text">
                        <span class="section-badge">Our Story</span>
                        <h2>Small Team, Big Commitment</h2>
                        <p class="about-description">
                            Clutch Transportation is a family-oriented freight company serving businesses across
                            Ontario.
                            As an upcoming business, we bring fresh energy and dedication to every delivery.
                        </p>
                        <p class="about-description">
                            We're building our reputation one shipment at a time, treating each client like a partner in
                            our growth.
                            Our small size means personalized attention, direct communication, and a genuine commitment
                            to your success.
                        </p>
                        <div class="about-stats">
                            <div class="stat">
                                <div class="stat-number">100%</div>
                                <div class="stat-label">Customer Focused</div>
                            </div>
                            <div class="stat">
                                <div class="stat-number">Ontario</div>
                                <div class="stat-label">Wide Coverage</div>
                            </div>
                            <div class="stat">
                                <div class="stat-number">24/7</div>
                                <div class="stat-label">Support Available</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Coverage Area Section -->
        <section id="coverage" class="coverage-section">
            <div class="container">
                <div class="section-header">
                    <span class="section-badge">Service Area</span>
                    <h2>Ontario-Wide Coverage</h2>
                    <p>Comprehensive freight solutions across Ontario's major cities and regions</p>
                </div>
                <div class="coverage-grid">
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Toronto</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Ottawa</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Mississauga</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Hamilton</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>London</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Kitchener</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Windsor</span>
                    </div>
                    <div class="coverage-item">
                        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"
                                fill="currentColor" />
                        </svg>
                        <span>Barrie</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- CTA Section -->
        <section class="cta-section">
            <div class="container">
                <div class="cta-content">
                    <h2>Ready to Partner With Us?</h2>
                    <p>Let's discuss how we can support your transportation needs</p>
                    <div class="cta-buttons">
                        <button class="btn btn-primary">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"
                                    fill="currentColor" />
                            </svg>
                            <span>(416) 786-2973</span>
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Back to Top Button -->
        <button v-show="showBackToTop" @click="scrollToTop" class="back-to-top" aria-label="Back to top">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 19V5M5 12l7-7 7 7" stroke="white" stroke-width="2" stroke-linecap="round"
                    stroke-linejoin="round" />
            </svg>
            <span class="tooltip">Back to Top</span>
        </button>
    </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'
import Hero from '@/components/Hero.vue'

const showBackToTop = ref(false)

const handleScroll = () => {
    showBackToTop.value = window.scrollY > 300
}

const scrollToTop = () => {
    window.scrollTo({ top: 0, behavior: 'smooth' })
}

onMounted(() => {
    window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll)
})
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

* {
    font-family: 'Inter', sans-serif;
}

.home-view {
    width: 100%;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
}

.section-badge {
    display: inline-block;
    padding: 0.4rem 1rem;
    background: rgba(250, 117, 35, 0.1);
    border-radius: 50px;
    color: #fa7523;
    font-size: 0.875rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    margin-bottom: 1rem;
}

.section-header {
    text-align: center;
    margin-bottom: 4rem;
}

.section-header h2 {
    font-size: 2.5rem;
    font-weight: 700;
    color: #111827;
    margin-bottom: 1rem;
    letter-spacing: -0.02em;
}

.section-header p {
    font-size: 1.125rem;
    color: #6b7280;
    max-width: 650px;
    margin: 0 auto;
    line-height: 1.7;
}

/* Services Section */
.services-section {
    padding: 5rem 0;
    background: #f9fafb;
}

.services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.service-card {
    position: relative;
    background: #ffffff;
    border: 1px solid #e5e7eb;
    border-radius: 12px;
    padding: 2.5rem 2rem;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.service-card:hover {
    border-color: #fa7523;
    transform: translateY(-4px);
    box-shadow: 0 12px 24px rgba(0, 0, 0, 0.1);
}

.service-number {
    position: absolute;
    top: 1.5rem;
    right: 2rem;
    font-size: 3rem;
    font-weight: 700;
    color: rgba(250, 117, 35, 0.1);
    line-height: 1;
}

.service-icon-wrapper {
    width: 56px;
    height: 56px;
    background: rgba(250, 117, 35, 0.1);
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fa7523;
    margin-bottom: 1.5rem;
    transition: all 0.3s ease;
}

.service-card:hover .service-icon-wrapper {
    background: #fa7523;
    color: white;
}

.service-card h3 {
    font-size: 1.25rem;
    font-weight: 600;
    color: #111827;
    margin-bottom: 0.75rem;
}

.service-card p {
    color: #6b7280;
    line-height: 1.6;
    font-size: 0.9375rem;
}

/* Why Choose Us Section */
.why-choose-section {
    padding: 5rem 0;
    background: #ffffff;
}

.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 2rem;
}

.feature-card {
    background: #f9fafb;
    border-radius: 12px;
    padding: 2rem 1.75rem;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.feature-card:hover {
    background: #ffffff;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
    transform: translateY(-2px);
}

.feature-icon {
    width: 48px;
    height: 48px;
    background: #fa7523;
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    margin-bottom: 1.25rem;
}

.feature-card h3 {
    font-size: 1.125rem;
    font-weight: 600;
    color: #111827;
    margin-bottom: 0.75rem;
}

.feature-card p {
    color: #6b7280;
    line-height: 1.6;
    font-size: 0.9375rem;
}

/* About Section */
.about-section {
    padding: 5rem 0;
    background: linear-gradient(135deg, #16213e 0%, #1a1a2e 100%);
}

.about-content {
    max-width: 900px;
    margin: 0 auto;
}

.about-text {
    text-align: center;
    color: white;
}

.about-text h2 {
    font-size: 2.5rem;
    font-weight: 700;
    color: white;
    margin-bottom: 1.5rem;
    letter-spacing: -0.02em;
}

.about-description {
    font-size: 1.0625rem;
    color: rgba(255, 255, 255, 0.85);
    line-height: 1.7;
    margin-bottom: 1.5rem;
    max-width: 750px;
    margin-left: auto;
    margin-right: auto;
}

.about-stats {
    display: flex;
    justify-content: center;
    gap: 4rem;
    margin-top: 3rem;
}

.stat {
    text-align: center;
}

.stat-number {
    font-size: 2.5rem;
    font-weight: 700;
    color: #fa7523;
    margin-bottom: 0.5rem;
    line-height: 1;
}

.stat-label {
    font-size: 0.9375rem;
    color: rgba(255, 255, 255, 0.7);
    font-weight: 500;
}

/* Coverage Section */
.coverage-section {
    padding: 5rem 0;
    background: #f9fafb;
}

.coverage-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 1.25rem;
}

.coverage-item {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.625rem;
    background: #ffffff;
    border: 1.5px solid #e5e7eb;
    border-radius: 10px;
    padding: 1.25rem 1rem;
    font-weight: 600;
    font-size: 0.9375rem;
    color: #374151;
    transition: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
}

.coverage-item svg {
    color: #9ca3af;
    flex-shrink: 0;
    transition: color 0.2s ease;
}

.coverage-item:hover {
    border-color: #fa7523;
    background: rgba(250, 117, 35, 0.05);
    transform: translateY(-2px);
}

.coverage-item:hover svg {
    color: #fa7523;
}

/* CTA Section */
.cta-section {
    padding: 5rem 0;
    background: #ffffff;
}

.cta-content {
    text-align: center;
    max-width: 700px;
    margin: 0 auto;
}

.cta-content h2 {
    font-size: 2.5rem;
    font-weight: 700;
    color: #111827;
    margin-bottom: 1rem;
    letter-spacing: -0.02em;
}

.cta-content p {
    font-size: 1.125rem;
    color: #6b7280;
    margin-bottom: 2.5rem;
    line-height: 1.7;
}

.cta-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
}

.btn {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 1rem 2rem;
    font-size: 1rem;
    font-weight: 600;
    border-radius: 8px;
    border: none;
    cursor: pointer;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    font-family: 'Inter', sans-serif;
}

.btn-primary {
    background: #fa7523;
    color: #ffffff;
    box-shadow: 0 4px 12px rgba(250, 117, 35, 0.25);
}

.btn-primary:hover {
    background: #e06619;
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(250, 117, 35, 0.35);
}

.btn-primary svg {
    transition: transform 0.3s ease;
    animation: arrowPulse 2s ease-in-out infinite;
}

.btn-primary:hover svg {
    transform: translateX(4px);
    animation: arrowSlide 0.6s ease-in-out infinite;
}

@keyframes arrowPulse {

    0%,
    100% {
        transform: translateX(0);
    }

    50% {
        transform: translateX(3px);
    }
}

@keyframes arrowSlide {

    0%,
    100% {
        transform: translateX(4px);
    }

    50% {
        transform: translateX(8px);
    }
}

.btn-secondary {
    background: #ffffff;
    color: #fa7523;
    border: 2px solid #fa7523;
    font-weight: 700;
    box-shadow: 0 2px 8px rgba(250, 117, 35, 0.15);
}

.btn-secondary:hover {
    background: #fa7523;
    color: #ffffff;
    border-color: #fa7523;
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(250, 117, 35, 0.3);
}

.btn-secondary svg {
    transition: transform 0.3s ease;
}

.btn-secondary:hover svg {
    transform: scale(1.1);
}

/* Back to Top Button */
.back-to-top {
    position: fixed;
    bottom: 2rem;
    right: 2rem;
    width: 48px;
    height: 48px;
    background: #fa7523;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 4px 16px rgba(250, 117, 35, 0.3);
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    z-index: 999;
}

.back-to-top:hover {
    background: #e06619;
    box-shadow: 0 6px 20px rgba(250, 117, 35, 0.4);
    transform: translateY(-2px);
}

.back-to-top:hover .tooltip {
    opacity: 1;
    visibility: visible;
    transform: translateX(-50%) translateY(-5px);
}

.tooltip {
    position: absolute;
    bottom: 100%;
    left: 50%;
    transform: translateX(-50%) translateY(0);
    background: #111827;
    color: #ffffff;
    padding: 0.5rem 1rem;
    border-radius: 6px;
    font-size: 0.875rem;
    font-weight: 500;
    white-space: nowrap;
    opacity: 0;
    visibility: hidden;
    transition: all 0.3s ease;
    margin-bottom: 0.5rem;
    pointer-events: none;
    font-family: 'Inter', sans-serif;
}

.tooltip::after {
    content: "";
    position: absolute;
    top: 100%;
    left: 50%;
    transform: translateX(-50%);
    border: 6px solid transparent;
    border-top-color: #111827;
}

/* Responsive Design */
@media (max-width: 1024px) {
    .container {
        padding: 0 1.5rem;
    }

    .section-header h2 {
        font-size: 2.25rem;
    }

    .services-section,
    .why-choose-section,
    .about-section,
    .coverage-section,
    .cta-section {
        padding: 4rem 0;
    }

    .about-stats {
        gap: 3rem;
    }
}

@media (max-width: 768px) {
    .container {
        padding: 0 1rem;
    }

    .section-header {
        margin-bottom: 3rem;
    }

    .section-header h2 {
        font-size: 2rem;
    }

    .section-header p,
    .cta-content p {
        font-size: 1rem;
    }

    .services-section,
    .why-choose-section,
    .about-section,
    .coverage-section,
    .cta-section {
        padding: 3.5rem 0;
    }

    .services-grid {
        grid-template-columns: 1fr;
    }

    .features-grid {
        grid-template-columns: 1fr;
    }

    .about-stats {
        flex-direction: column;
        gap: 2rem;
    }

    .coverage-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .cta-content h2 {
        font-size: 2rem;
    }

    .cta-buttons {
        flex-direction: column;
    }

    .btn {
        width: 100%;
        max-width: 320px;
        margin: 0 auto;
        justify-content: center;
    }

    .back-to-top {
        bottom: 1.5rem;
        right: 1.5rem;
        width: 44px;
        height: 44px;
    }
}

@media (max-width: 480px) {
    .container {
        padding: 0 1rem;
    }

    .section-header {
        margin-bottom: 2.5rem;
    }

    .section-header h2 {
        font-size: 1.75rem;
    }

    .section-header p {
        font-size: 0.9375rem;
    }

    .services-section,
    .why-choose-section,
    .about-section,
    .coverage-section,
    .cta-section {
        padding: 3rem 0;
    }

    .service-card h3,
    .feature-card h3 {
        font-size: 1.0625rem;
    }

    .service-card p,
    .feature-card p {
        font-size: 0.875rem;
    }

    .about-text h2 {
        font-size: 2rem;
    }

    .about-description {
        font-size: 0.9375rem;
    }

    .about-stats {
        gap: 1.5rem;
    }

    .stat-number {
        font-size: 2rem;
    }

    .stat-label {
        font-size: 0.875rem;
    }

    .coverage-grid {
        grid-template-columns: 1fr;
    }

    .cta-content h2 {
        font-size: 1.75rem;
    }

    .cta-content p {
        font-size: 0.9375rem;
    }

    .btn {
        max-width: 280px;
    }

    .back-to-top {
        bottom: 1rem;
        right: 1rem;
        width: 42px;
        height: 42px;
    }

    .back-to-top svg {
        width: 18px;
        height: 18px;
    }

    .tooltip {
        font-size: 0.8125rem;
        padding: 0.4rem 0.8rem;
    }
}
</style>