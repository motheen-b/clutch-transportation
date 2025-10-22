<template>
    <div class="hero-container">
        <div class="hero-overlay"></div>
        <div class="hero-content">
            <div class="content-wrapper">
                <span class="hero-badge">Professional Transportation Services</span>
                <h1 class="hero-title">Moving Your Business Forward</h1>
                <p class="hero-description">
                    Clutch Transportation delivers reliable freight solutions across Ontario.
                    We're a dedicated team committed to providing big results for your business.
                </p>
                <div class="hero-actions">
                    <button class="btn btn-primary">
                        <span>Request a Quote</span>
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M5 12h14M12 5l7 7-7 7" stroke="currentColor" stroke-width="2"
                                stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <div class="hero-scroll-indicator">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 5v14M5 12l7 7 7-7" stroke="white" stroke-width="2" stroke-linecap="round"
                    stroke-linejoin="round" />
            </svg>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

.hero-container {
    position: relative;
    width: 100%;
    height: 70vh;
    min-height: 500px;
    max-height: 700px;
    background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
}

.hero-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background:
        radial-gradient(circle at 20% 50%, rgba(250, 117, 35, 0.08) 0%, transparent 50%),
        radial-gradient(circle at 80% 80%, rgba(250, 117, 35, 0.05) 0%, transparent 50%);
    z-index: 1;
}

.hero-content {
    position: relative;
    z-index: 2;
    width: 100%;
    max-width: 1200px;
    padding: 0 2rem;
    display: flex;
    align-items: center;
    justify-content: center;
}

.content-wrapper {
    width: 100%;
    max-width: 800px;
    text-align: center;
    color: white;
}

.hero-badge {
    display: inline-block;
    padding: 0.5rem 1.25rem;
    background: rgba(250, 117, 35, 0.1);
    border: 1px solid rgba(250, 117, 35, 0.3);
    border-radius: 50px;
    color: #fa7523;
    font-family: 'Inter', sans-serif;
    font-size: 0.875rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    margin-bottom: 1.5rem;
}

.hero-title {
    font-family: 'Inter', sans-serif;
    font-size: 3.5rem;
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 1.5rem;
    color: white;
    letter-spacing: -0.02em;
}

.hero-description {
    font-family: 'Inter', sans-serif;
    font-size: 1.125rem;
    font-weight: 400;
    line-height: 1.7;
    color: rgba(255, 255, 255, 0.85);
    margin-bottom: 2.5rem;
    max-width: 650px;
    margin-left: auto;
    margin-right: auto;
}

.hero-actions {
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
    font-family: 'Inter', sans-serif;
    font-size: 1rem;
    font-weight: 600;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    white-space: nowrap;
}

.btn-primary {
    background: #fa7523;
    color: white;
    box-shadow: 0 4px 20px rgba(250, 117, 35, 0.3);
}

.btn-primary:hover {
    background: #e06619;
    transform: translateY(-2px);
    box-shadow: 0 8px 30px rgba(250, 117, 35, 0.4);
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

.hero-scroll-indicator {
    position: absolute;
    bottom: 2rem;
    left: 50%;
    transform: translateX(-50%);
    z-index: 3;
    animation: bounce 2s ease-in-out infinite;
    opacity: 0.7;
    cursor: pointer;
    transition: opacity 0.3s ease;
}

.hero-scroll-indicator:hover {
    opacity: 1;
}

@keyframes bounce {

    0%,
    100% {
        transform: translateX(-50%) translateY(0);
    }

    50% {
        transform: translateX(-50%) translateY(10px);
    }
}

/* Responsive Design */
@media (max-width: 1200px) {
    .hero-title {
        font-size: 3rem;
    }

    .hero-description {
        font-size: 1.0625rem;
    }
}

@media (max-width: 992px) {
    .hero-container {
        height: 65vh;
        min-height: 480px;
    }

    .hero-title {
        font-size: 2.5rem;
    }

    .hero-description {
        font-size: 1rem;
        margin-bottom: 2rem;
    }

    .btn {
        padding: 0.875rem 1.75rem;
        font-size: 0.9375rem;
    }
}

@media (max-width: 768px) {
    .hero-container {
        height: 60vh;
        min-height: 450px;
    }

    .hero-content {
        padding: 0 1.5rem;
    }

    .hero-badge {
        font-size: 0.8125rem;
        padding: 0.4rem 1rem;
        margin-bottom: 1.25rem;
    }

    .hero-title {
        font-size: 2rem;
        margin-bottom: 1.25rem;
    }

    .hero-description {
        font-size: 0.9375rem;
        margin-bottom: 1.75rem;
    }

    .hero-actions {
        flex-direction: column;
        align-items: center;
    }

    .btn {
        width: 100%;
        max-width: 280px;
        justify-content: center;
        padding: 0.875rem 1.5rem;
    }

    .hero-scroll-indicator {
        bottom: 1.5rem;
    }
}

@media (max-width: 480px) {
    .hero-container {
        height: 55vh;
        min-height: 420px;
    }

    .hero-content {
        padding: 0 1rem;
    }

    .hero-badge {
        font-size: 0.75rem;
        padding: 0.35rem 0.875rem;
    }

    .hero-title {
        font-size: 1.75rem;
        margin-bottom: 1rem;
    }

    .hero-description {
        font-size: 0.875rem;
        line-height: 1.6;
        margin-bottom: 1.5rem;
    }

    .btn {
        padding: 0.8rem 1.25rem;
        font-size: 0.875rem;
        max-width: 260px;
    }

    .btn svg {
        width: 14px;
        height: 14px;
    }

    .hero-scroll-indicator {
        bottom: 1rem;
    }

    .hero-scroll-indicator svg {
        width: 20px;
        height: 20px;
    }
}
</style>
