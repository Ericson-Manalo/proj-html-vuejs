<template>
    <header>
        <div class="logo">
            <img src="../assets/images/avada-music-logo.png" alt="Avada Music Logo">
        </div>
    </header>
</template>
<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            
        }
    },
}
</script>
<style lang="scss">
@use '../styles/general.scss' as*;
    header{
        background-image: url('../assets/images/home_slider.jpg');
        height: 100vh;
        background-size: cover;
    }
    
</style>