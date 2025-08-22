<template>
    <div class="container">
        <div class="container-content">
            <h1>Cross Docking Services</h1>
            <p>Maximize efficiency with ET Transport's Cross Docking Services. Our advanced crossdock facilities and warehouse systems seamlessly integrate cross docking and inventory management, enhancing your supply chain by reducing storage costs. Explore our cross dock solutions where warehousing meets rapid shipping efficiency.</p>
            
            <div class="button-group">
                <button class="btn btn-primary">Get A Quote</button>
                <button class="btn btn-secondary">Learn More</button>
            </div>
            
            <div class="social-media">
                <a href="#" class="social-link facebook">
                    <svg width="28" height="28" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M22.46 6c-.77.35-1.6.58-2.46.69.88-.53 1.56-1.37 1.88-2.38-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29 0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15 0 1.49.75 2.81 1.91 3.56-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.22 4.22 0 0 1-1.93.07 4.28 4.28 0 0 0 4 2.98 8.521 8.521 0 0 1-5.33 1.84c-.34 0-.68-.02-1.02-.06C3.44 20.29 5.7 21 8.12 21 16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56.84-.6 1.56-1.36 2.14-2.23z" fill="#1877F2"/>
                    </svg>
                </a>
                <a href="#" class="social-link instagram">
                    <svg width="28" height="28" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.354 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" fill="url(#instagram-gradient)"/>
                        <defs>
                            <linearGradient id="instagram-gradient" x1="0%" y1="0%" x2="100%" y2="100%">
                                <stop offset="0%" style="stop-color:#405DE6"/>
                                <stop offset="10%" style="stop-color:#5851DB"/>
                                <stop offset="20%" style="stop-color:#833AB4"/>
                                <stop offset="30%" style="stop-color:#C13584"/>
                                <stop offset="40%" style="stop-color:#E1306C"/>
                                <stop offset="50%" style="stop-color:#FD1D1D"/>
                                <stop offset="60%" style="stop-color:#F56040"/>
                                <stop offset="70%" style="stop-color:#FCAF45"/>
                                <stop offset="80%" style="stop-color:#FFDC80"/>
                                <stop offset="90%" style="stop-color:#FFDC80"/>
                                <stop offset="100%" style="stop-color:#405DE6"/>
                            </linearGradient>
                        </defs>
                    </svg>
                </a>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;700&display=swap');

.container {
    display: flex;
    height: 550px;
    background-image: url('@/assets/hero-logo.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    position: relative;
    /* border: 1px solid green; */
}

.container::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.4);
    z-index: 1;
}

.container-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: absolute;
    gap: 0.7rem;
    line-height: 1.5;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;
    color: white;
    /* border: 1px solid red; */
    backdrop-filter: blur(8px);
    border-radius: 12px;
    text-align: center;
    padding: 1rem;
    font-family: 'Montserrat', 'sans-serif';
    font-size: 18px;
}

.button-group {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
}

.btn {
    padding: 0.8rem 1.5rem;
    border: none;
    border-radius: 4px;
    font-weight: 600;
    font-size: 14px;
    cursor: pointer;
    transition: all 0.3s ease;
    font-family: 'Montserrat', sans-serif;
}

.btn-primary {
    background-color: #fa7523;
    color: white;
}

.btn-primary:hover {
    background-color: #e6681a;
    transform: translateY(-2px);
}

.btn-secondary {
    background-color: transparent;
    color: white;
    border: 2px solid white;
}

.btn-secondary:hover {
    background-color: white;
    color: black;
    transform: translateY(-2px);
}

.social-media {
    display: flex;
    gap: 1rem;
    margin-top: 0.5rem;
}

.social-link {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: rgba(255, 255, 255, 0.1);
    transition: all 0.3s ease;
    backdrop-filter: blur(5px);
}

.social-link:hover {
    transform: translateY(-2px);
}

.social-link.facebook:hover {
    background-color: rgba(24, 119, 242, 0.3);
    animation: facebookShift 2s ease-in-out infinite;
    box-shadow: 0 0 20px rgba(24, 119, 242, 0.4);
}

.social-link.instagram:hover {
    background-color: rgba(225, 48, 108, 0.3);
    animation: instagramShift 3s ease-in-out infinite;
    box-shadow: 0 0 20px rgba(225, 48, 108, 0.4);
}

@keyframes facebookShift {
    0%, 100% {
        filter: hue-rotate(0deg) saturate(1);
    }
    50% {
        filter: hue-rotate(5deg) saturate(1.1);
    }
}

@keyframes instagramShift {
    0%, 100% {
        filter: hue-rotate(0deg) saturate(1) brightness(1);
    }
    25% {
        filter: hue-rotate(10deg) saturate(1.2) brightness(1.05);
    }
    50% {
        filter: hue-rotate(20deg) saturate(1.1) brightness(1.1);
    }
    75% {
        filter: hue-rotate(15deg) saturate(1.15) brightness(1.05);
    }
}
</style>