<template>

    <!-- Main Navbar -->
    <div class="navbar-container">
        <div class="nav">
            <div class="nav-items">
                <div class="logo">
                    <img src="@/assets/clutch_logo.png" alt="logo">
                </div>
                <div class="nav-links">
                    <a v-for="(route, index) in routes" :key="index" :href="route.path"
                        @click="scrollToSection($event, route.path)">
                        {{ route.name }}
                    </a>
                </div>

                <div class="contact">
                    <div class="phone-number" @click="clickToCall('4167862973')">
                        <svg class="phone-icon" width="20" height="20" viewBox="0 0 24 24" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"
                                fill="#0056b3" />
                        </svg>
                        (416) 786-2973
                    </div>
                    <div class="quote-button">GET A QUOTE</div>
                </div>

                <!-- Hamburger Menu Button -->
                <button class="hamburger" @click="toggleMenu" :class="{ active: isMenuOpen }" aria-label="Toggle menu">
                    <span></span>
                    <span></span>
                    <span></span>
                </button>
            </div>
        </div>
    </div>

    <!-- Mobile Contact Bar - Separate Bar Below -->
    <div class="mobile-contact-bar">
        <div class="mobile-contact-content">
            <div class="mobile-phone" @click="clickToCall('4167862973')">
                <svg class="phone-icon" width="18" height="18" viewBox="0 0 24 24" fill="none"
                    xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"
                        fill="#0056b3" />
                </svg>
                <span>(416) 786-2973</span>
            </div>
            <div class="mobile-quote-button">GET A QUOTE</div>
        </div>
    </div>

    <!-- Mobile Menu Overlay -->
    <div class="mobile-menu" :class="{ open: isMenuOpen }">
        <button class="close-menu" @click="toggleMenu" aria-label="Close menu">
            <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M18 6L6 18M6 6l12 12" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                    stroke-linejoin="round" />
            </svg>
        </button>
        <div class="mobile-menu-logo">
            <img src="@/assets/clutch_logo.png" alt="Clutch Transportation">
        </div>
        <nav class="mobile-nav">
            <a v-for="(route, index) in routes" :key="index" :href="route.path"
                @click="handleMobileClick($event, route.path)">
                {{ route.name }}
            </a>
        </nav>
    </div>

</template>

<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
    isMenuOpen.value = !isMenuOpen.value
}

const handleMobileClick = (event, path) => {
    scrollToSection(event, path)
    isMenuOpen.value = false
}
const routes = [
    { name: 'SERVICES', path: '#services' },
    { name: 'WHY CHOOSE US', path: '#why-choose' },
    { name: 'ABOUT', path: '#about' },
    { name: 'COVERAGE', path: '#coverage' }
]

const clickToCall = (phoneNumber) => {
    const cleanNumber = phoneNumber.replace(/\D/g, '')
    const isMobile = /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)

    if (isMobile) {
        window.location.href = `tel:${cleanNumber}`
    } else {
        navigator.clipboard.writeText(phoneNumber)
            .then(() => {
                console.log('Phone number copied to clipboard!')
            })
            .catch(err => {
                console.error('Failed to copy phone number', err)
            })
    }
}

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
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@500;600;700&display=swap');

.navbar-container {
    display: flex;
    position: fixed;
    z-index: 9999;
    top: 0;
    left: 0;
    width: 100%;
    height: 80px;
    background-color: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease;
}

.nav {
    display: flex;
    position: relative;
    left: 50%;
    transform: translateX(-50%);
    flex-basis: 100%;
    max-width: 1440px;
    min-width: 320px;
    /* border: 1px solid red; */
}

.nav-items {
    display: flex;
    flex-basis: 100%;
    align-items: center;
    padding: 0 2rem;
    font-family: 'Inter', sans-serif;
}

.logo {
    display: flex;
    align-items: center;
}

.logo img {
    width: 175px;
    height: 65px;
    object-fit: contain;
    vertical-align: middle;
}

.nav-links {
    display: flex;
    height: 100%;
    align-items: center;
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    font-weight: 600;
    gap: 2.5rem;
}

.contact {
    display: flex;
    /* height: 100%; */
    gap: 1.8rem;
    align-items: center;
    justify-content: flex-end;
    flex-basis: 100%;
}

.contact .phone-number {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-weight: 600;
    font-size: 14px;
    padding: 0.6rem 1rem;
    color: #374151;
    border-radius: 6px;
    transition: all 0.2s ease;
}

.contact .phone-number:hover {
    cursor: pointer;
    background: #f3f4f6;
    color: #111827;
}

.phone-icon {
    flex-shrink: 0;
}

.contact .quote-button {
    border-radius: 6px;
    padding: 0.6rem 1.25rem;
    color: white;
    font-size: 14px;
    font-weight: 600;
    background-color: #fa7523;
    transition: all 0.2s ease;
    box-shadow: 0 2px 8px rgba(250, 117, 35, 0.25);
}

.contact .quote-button:hover {
    transform: translateY(-2px);
    cursor: pointer;
    background-color: #e06619;
    box-shadow: 0 4px 12px rgba(250, 117, 35, 0.35);
}

a {
    position: relative;
    color: #374151;
    font-size: 14px;
    text-decoration: none;
    transition: color 0.2s ease;
    font-family: 'Inter', sans-serif;
}

a:hover {
    color: #fa7523;
}

a::after {
    content: "";
    position: absolute;
    bottom: -4px;
    left: 50%;
    width: 0;
    height: 2px;
    background-color: #fa7523;
    transform: translateX(-50%);
    transition: width 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.nav-links a:hover::after,
.nav-links a.nav-link-active::after {
    width: 100%;
}

/* Mobile Contact Bar - Separate Fixed Bar */
.mobile-contact-bar {
    display: none;
    position: fixed;
    z-index: 9998;
    top: 90px;
    left: 0;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.mobile-contact-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1.5rem;
    padding: 1rem;
    width: 100%;
    box-sizing: border-box;
}

.mobile-phone {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.75rem;
    font-weight: 600;
    font-size: 16px;
    color: #374151;
    cursor: pointer;
    padding: 1rem 2rem;
    border: 2px solid #fa7523;
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.5);
    transition: all 0.2s ease;
    flex: 1;
    font-family: 'Inter', sans-serif;
}

.mobile-phone:hover {
    color: #fa7523;
    border-color: #fa7523;
    background: rgba(255, 255, 255, 0.9);
}

.mobile-quote-button {
    border-radius: 8px;
    padding: 1rem 2rem;
    color: white;
    font-size: 16px;
    font-weight: 600;
    background-color: #fa7523;
    transition: all 0.2s ease;
    box-shadow: 0 2px 8px rgba(250, 117, 35, 0.25);
    cursor: pointer;
    flex: 1;
    text-align: center;
    font-family: 'Inter', sans-serif;
}

.mobile-quote-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(250, 117, 35, 0.35);
    background-color: #e06619;
}

/* Hamburger Menu */
.hamburger {
    display: none;
    flex-direction: column;
    justify-content: space-around;
    width: 30px;
    height: 25px;
    background: transparent;
    border: none;
    cursor: pointer;
    padding: 0;
    z-index: 10;
    margin-left: auto;
}

.hamburger span {
    width: 30px;
    height: 3px;
    background: #111827;
    border-radius: 3px;
    transition: all 0.3s ease;
    transform-origin: center;
}

.hamburger.active span:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
}

.hamburger.active span:nth-child(2) {
    opacity: 0;
}

.hamburger.active span:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
}

/* Mobile Menu Overlay */
.mobile-menu {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    background: rgba(255, 255, 255, 0.98);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    transform: translateX(-100%);
    transition: transform 0.3s ease;
    z-index: 10000;
    overflow-y: auto;
}

.mobile-menu.open {
    transform: translateX(0);
}

.close-menu {
    position: absolute;
    top: 2rem;
    right: 2rem;
    width: 48px;
    height: 48px;
    background: #ffffff;
    border: 2px solid #e5e7eb;
    border-radius: 10px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #374151;
    transition: all 0.3s ease;
    z-index: 10001;
}

.close-menu:hover {
    background: #fa7523;
    border-color: #fa7523;
    color: #ffffff;
    transform: rotate(90deg);
}

.mobile-menu-logo {
    position: absolute;
    top: 2rem;
    left: 2rem;
    z-index: 10001;
}

.mobile-menu-logo img {
    width: 150px;
    height: auto;
}

.mobile-nav {
    display: flex;
    flex-direction: column;
    padding-top: calc(90px + 2rem);
    padding-left: 2rem;
    padding-right: 2rem;
    padding-bottom: 2rem;
    gap: 0;
}

.mobile-nav a {
    padding: 1.25rem 1rem;
    font-size: 1.125rem;
    font-weight: 600;
    color: #374151;
    text-decoration: none;
    border-bottom: 1px solid #e5e7eb;
    transition: all 0.2s ease;
    font-family: 'Inter', sans-serif;
}

.mobile-nav a:hover {
    background: rgba(250, 117, 35, 0.05);
    padding-left: 1.5rem;
    color: #fa7523;
}

/* Mobile Responsive */
@media (max-width: 1200px) {
    .navbar-container {
        height: 70px;
    }

    .nav {
        height: 70px;
    }

    .logo img {
        width: 140px;
        height: 52px;
    }

    .nav-links {
        display: none;
    }

    .contact {
        display: none;
    }

    .hamburger {
        display: flex;
        margin-right: 1rem;
    }

    .mobile-contact-bar {
        display: block;
        top: 70px;
    }

    .mobile-menu {
        top: 0;
        height: 100vh;
    }

    .mobile-nav {
        padding-top: calc(70px + 55px + 2rem);
    }
}

@media (max-width: 900px) {
    .mobile-phone {
        font-size: 14px;
        padding: 0.9rem 1.5rem;
    }

    .mobile-quote-button {
        font-size: 14px;
        padding: 0.9rem 1.5rem;
    }
}

@media (max-width: 700px) {
    .mobile-phone {
        font-size: 13px;
        padding: 0.8rem 1.25rem;
        gap: 0.5rem;
    }

    .mobile-phone .phone-icon {
        width: 16px;
        height: 16px;
    }

    .mobile-quote-button {
        font-size: 13px;
        padding: 0.8rem 1.25rem;
    }

    .mobile-contact-content {
        gap: 1rem;
    }
}

@media (max-width: 480px) {
    .navbar-container {
        height: 60px;
    }

    .nav {
        height: 60px;
    }

    .logo img {
        width: 120px;
        height: 45px;
    }

    .hamburger {
        width: 26px;
        height: 22px;
        margin-right: 0.75rem;
    }

    .hamburger span {
        width: 26px;
        height: 2.5px;
    }

    .mobile-contact-bar {
        top: 60px;
    }

    .mobile-contact-content {
        padding: 0.75rem 0.5rem;
        gap: 0.75rem;
    }

    .mobile-phone {
        font-size: 11px;
        padding: 0.75rem 1rem;
    }

    .mobile-phone .phone-icon {
        width: 14px;
        height: 14px;
    }

    .mobile-quote-button {
        font-size: 11px;
        padding: 0.75rem 1rem;
    }

    .mobile-menu {
        top: 0;
        height: 100vh;
    }

    .mobile-nav {
        padding-top: calc(60px + 50px + 1.5rem);
        padding-left: 1.5rem;
        padding-right: 1.5rem;
        padding-bottom: 1.5rem;
    }

    .mobile-nav a {
        padding: 1rem 0.75rem;
        font-size: 1rem;
    }

    .close-menu {
        top: 1.5rem;
        right: 1.5rem;
        width: 44px;
        height: 44px;
    }

    .close-menu svg {
        width: 28px;
        height: 28px;
    }

    .mobile-menu-logo {
        top: 1.5rem;
        left: 1.5rem;
    }

    .mobile-menu-logo img {
        width: 130px;
    }
}
</style>