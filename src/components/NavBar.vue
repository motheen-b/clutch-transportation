<template>

    <div class="container">
        <div class="nav">
            <div class="nav-items">
                <div class="logo">Clutch Transportation</div>
                <div class="nav-links">
                    <router-link v-for="(route, index) in routes" :key="index" :to="route.path">
                        {{ route.name }}
                    </router-link>
                </div>
                <div class="contact">
                    <div class="phone-number" @click="clickToCall('6479017565')">
                        <svg class="phone-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z" fill="#0056b3"/>
                        </svg>
                        (647) 901-7565
                    </div>
                    <div class="quote-button">GET A QUOTE</div>
                </div>
            </div>
        </div>
    </div>

</template>

<script setup>
import { clickToCall } from '@/composables/clickAction'

const routes = [
    { name: 'TRANSPORTATION', path: '/' },
    { name: 'WAREHOUSING', path: '/' },
    { name: 'ABOUT', path: '/' },
    { name: 'CONTACT', path: '/' }
]
</script>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;700&display=swap');

.container {
    display: flex;
    position: sticky;
    z-index: 10000;
    top: 0;
    width: 100%;
    height: 90px;
    /* border: 1px solid black; */
    background-color: rgb(235, 235, 235);
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
    padding: 0 1rem;
    /* border: 2px solid green; */
    font-family: 'Montserrat', 'sans-serif';
}

.logo {
    display: flex;
    align-items: center;
    /* flex-basis: 100%; */
    /* height: 100%; */
    /* border: 1px solid salmon; */
}

.nav-links {
    display: flex;
    height: 100%;
    align-items: center;
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    font-weight: 700;
    gap: 2rem;
    /* border: 2px solid blue; */
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
    font-weight: 700;
    font-size: 14px;
    padding: 0.5rem;
}

.contact .phone-number:hover {
    cursor: pointer;
}

.phone-icon {
    flex-shrink: 0;
}

.contact .quote-button {
    border-radius: 4px;
    padding: 0.8rem;
    color: white;
    font-size: 14px;
    font-weight: 700;
    background-color: #fa7523;
    transition: transform 0.25s ease-in-out;
    box-shadow: 0 2px 8px rgba(109, 108, 108, 0.3);
}

.contact .quote-button:hover {
    transform: translateY(-3px);
    cursor: pointer;
}

a {
    position: relative;
    color: black;
    font-size: 14px;
    text-decoration: none;
    transition: transform 1s ease-in-out;
    
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
    transition: width 0.5s cubic-bezier(.25, .8, .25, 1);
}

.nav-links a:hover::after,
.nav-links a.nav-link-active::after {
    width: 100%;
}
</style>