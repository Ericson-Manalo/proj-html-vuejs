<template>
    <main>
        <!--MUSIC SECTION-->
        <section class="music">
            <div class="music-section">
                <div></div>
                <h2 class="h2-fs">
                    Music Is Life
                </h2>
                <hr>
                <p class="line-height">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum finibus cursus egestas. Cras quis vehicula quam, a tempus velit. Ut feugiat augue in sodales luctus
                </p>
            </div>
        </section>

        <AppBand/>

        
    </main>
</template>
<script>
import AppBand from './AppBrand.vue'
export default {
    name: 'AppMain',
    data() {
        return {
            
        }
    },
    components:{
        AppBand
    }
}
</script>
<style lang="scss" scoped>
@use '../styles/general.scss' as*;
@use '../styles/partials/variables.scss' as*;
@use '../styles/partials/mixins.scss' as*;

section.music{
    background-color: $gray;
    position: relative;
}

div.music-section div{
    width: 23%;
    height: 16px;
    background-color: $red;
    position: absolute;
    top: 0;
}

div.music-section{
    width: 40%;
    display: flex;
    @include centering(center, center, column);
    text-align: center;
    padding: 5rem 0 4rem;
}

div.music-section p{
    color: #7d7b8d;
}





</style>