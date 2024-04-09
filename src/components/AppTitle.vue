<template>
    <div>
        <h1 :class="{ 'fade-in': !fadeinTitle }">La mia prima app con Vite!</h1>
    </div>
    
</template>

<script>
    export default {
        name: 'AppTitle',
        data() {
            return {
                fadeinTitle: false
            }
        }
    }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    h1 {
        font-size: 3em;
        text-align: center;
        font-family: "Montserrat", sans-serif;
    }

    .fade-in {
        animation: topFadeIn 1s cubic-bezier(0.25, 0.1, 0.25, 1) forwards;
    }

    @keyframes topFadeIn {
        from {
            opacity: 0;
            transform: translateY(-500px);
        }
        to {
            opacity: 1;
            transform: translateY(-300px);
        }
    }
</style>