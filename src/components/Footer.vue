<template>
    <footer class="footer">
        <div class="footer-container">
            <div class="footer-main">
                <div class="footer-left">
                    <h2 class="company-name">Clutch Transportation</h2>
                    <p class="company-tagline">Reliable freight solutions across Ontario</p>
                </div>

                <div class="footer-right">
                    <div class="footer-nav">
                        <a href="#services" @click="scrollToSection($event, '#services')">Services</a>
                        <span class="nav-dot">•</span>
                        <a href="#why-choose" @click="scrollToSection($event, '#why-choose')">Why Choose Us</a>
                        <span class="nav-dot">•</span>
                        <a href="#about" @click="scrollToSection($event, '#about')">About</a>
                        <span class="nav-dot">•</span>
                        <a href="#coverage" @click="scrollToSection($event, '#coverage')">Coverage</a>
                    </div>

                    <div class="footer-contact">
                        <a href="tel:6479017565" class="contact-link">
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"
                                    fill="currentColor" />
                            </svg>
                            (416) 786-2973
                        </a>
                        <a href="mailto:info@clutchtransport.ca" class="contact-link">
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"
                                    stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                    stroke-linejoin="round" fill="none" />
                                <path d="M22 6l-10 7L2 6" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                    stroke-linejoin="round" />
                            </svg>
                            info@clutchtransport.ca
                        </a>
                    </div>
                </div>
            </div>

            <div class="footer-bottom">
                <p class="copyright">&copy; {{ currentYear }} Clutch Transportation. All rights reserved.</p>
            </div>
        </div>
    </footer>
</template>

<script setup>
import { computed } from 'vue'

const currentYear = computed(() => new Date().getFullYear())

const scrollToSection = (event, path) => {
    event.preventDefault()
    if (path.startsWith('#')) {
        const element = document.querySelector(path)
        if (element) {
            element.scrollIntoView({ behavior: 'smooth' })
        }
    }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

.footer {
    background: #111827;
    color: white;
    font-family: 'Inter', sans-serif;
    margin-top: auto;
}

.footer-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 3rem 2rem 1.5rem;
}

.footer-main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    padding-bottom: 2.5rem;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.footer-left {
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
}

.company-name {
    font-size: 1.75rem;
    font-weight: 700;
    color: white;
    margin: 0;
    letter-spacing: -0.02em;
}

.company-tagline {
    font-size: 1rem;
    color: rgba(255, 255, 255, 0.6);
    margin: 0;
    line-height: 1.6;
}

.footer-right {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
    align-items: flex-end;
}

.footer-nav {
    display: flex;
    align-items: center;
    gap: 1rem;
    flex-wrap: wrap;
    justify-content: flex-end;
}

.footer-nav a {
    color: rgba(255, 255, 255, 0.7);
    text-decoration: none;
    font-size: 0.9375rem;
    font-weight: 500;
    transition: color 0.2s ease;
}

.footer-nav a:hover {
    color: #fa7523;
}

.nav-dot {
    color: rgba(255, 255, 255, 0.3);
    font-size: 0.875rem;
}

.footer-contact {
    display: flex;
    gap: 2rem;
    align-items: center;
}

.contact-link {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    color: rgba(255, 255, 255, 0.8);
    text-decoration: none;
    font-size: 0.9375rem;
    font-weight: 500;
    transition: all 0.2s ease;
}

.contact-link svg {
    color: #fa7523;
    flex-shrink: 0;
}

.contact-link:hover {
    color: white;
}

.footer-bottom {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 1.5rem;
}

.copyright {
    font-size: 0.875rem;
    color: rgba(255, 255, 255, 0.5);
    margin: 0;
}

/* Responsive Design */
@media (max-width: 968px) {
    .footer-main {
        grid-template-columns: 1fr;
        gap: 3rem;
    }

    .footer-right {
        align-items: flex-start;
    }

    .footer-nav {
        justify-content: flex-start;
    }

    .footer-contact {
        flex-direction: column;
        align-items: flex-start;
        gap: 1rem;
    }
}

@media (max-width: 768px) {
    .footer-container {
        padding: 2.5rem 1.5rem 1.5rem;
    }

    .footer-main {
        gap: 2.5rem;
        padding-bottom: 2rem;
    }

    .company-name {
        font-size: 1.5rem;
    }

    .company-tagline {
        font-size: 0.9375rem;
    }

    .footer-nav {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.75rem;
    }

    .nav-dot {
        display: none;
    }

    .footer-bottom {
        justify-content: center;
    }
}

@media (max-width: 480px) {
    .footer-container {
        padding: 2rem 1rem 1.5rem;
    }

    .company-name {
        font-size: 1.375rem;
    }

    .company-tagline {
        font-size: 0.875rem;
    }

    .footer-nav a {
        font-size: 0.875rem;
    }

    .contact-link {
        font-size: 0.875rem;
    }

    .copyright {
        font-size: 0.8125rem;
    }
}
</style>
