<template>
    <div class="container">
        <div class="container-content">
            <h1>Welcome to our website</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.</p>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
.container {
    display: flex;
    padding: 2rem;
    height: 550px;
    /* background-image: url('@/assets/hero.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat; */
    background-color: #000;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    position: relative;
    border: 1px solid green;
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
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;
    color: white;
    border: 1px solid red;
    text-align: center;
    width: 100%;
    padding: 1rem;
}
</style>