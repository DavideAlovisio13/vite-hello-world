<template>
  <div class="jumbocontainer" >
    <img src="/public/Vitejs-logo.svg" alt="vitelogo" :class="{fadein: !fadeinJumbo}" />
  </div>
</template>

<script>
export default {
    name: 'AppTitle',
    data() {
        return {
            fadeinJumbo: false
        }
    },
        methods: {
        },
        mounted() {
        },
    }
</script>

<style scoped>
.jumbocontainer {
  width: 100%;
  background-blend-mode: difference;
}

img {
  width: 100%;
  object-fit: cover;
}

.fadein {
  animation: fadein 3s;
}

@keyframes fadein {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}
</style>
