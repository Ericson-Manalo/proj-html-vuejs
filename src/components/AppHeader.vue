<template>
    <header>
        <div class="upper-header">
            <div class="logo">
                <img src="../assets/images/avada-music-logo.png" alt="Avada Music Logo">
            </div>
            <div class="hamburger">
                <i class="fa-solid fa-bars"></i>
            </div>
        </div>
        <div class="header-content">
            <h1>
                Untold Stories
            </h1>
            <p class="mb-4">
                There is an untold story behind every favorite song.
            </p>
            <div class="buttons">
                <button class="btn-latest-album">
                    LATEST ALBUM
                </button>
                <button class="btn-live-dates">
                    LIVE DATES
                </button>
            </div>
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
<style lang="scss" scoped>
@use '../styles/general.scss' as*;
@use '../styles/partials/variables' as*;
    header{
        background-image: url('../assets/images/home_slider.jpg');
        height: 100vh;
        background-size: cover;
        position: relative;
        background-position: center;
    }

    div.upper-header{
        display: flex;
        justify-content: space-between;
        height: 90px;
        padding: 0 2rem;
        background-color: $colorheader;
        align-items: center;
        width: 100%;
        z-index: 1;
        position: fixed;

        div.hamburger i{
            font-size: 2rem;
            color: white;
        }
    }
    div.header-content{
        position: absolute;
        top: 50%;
        left: 50%;
        transform:translate(-50%, -50%);
        text-align: center;
        color: white;
        width: 100%;
    }

    h1{
        font-size: 150px;
        font-weight: 700;
        margin: 0 auto;
    }

    p{
        font-size: 24px;
        font-weight: 400;
    }

    button{
        padding: 1rem 2rem;
        font-size: 18px;
        font-weight: 700;
        color: white;
        margin: .7rem;
    }

    .btn-latest-album{
        background-color: $red;
        border: 1px solid $red;
    }

    .btn-latest-album:hover,
    .btn-live-dates:hover
    {
            background-color: white;
            color: black;
            border: 1px solid white;
        }

    .btn-live-dates{
        background-color: transparent;
    }

    
</style>