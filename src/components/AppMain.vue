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

        <!--LATEST BRAND SECTION-->
        <section class="band">
            <div class="d-flex justify-content-center">
                <div class="band-section">
                <h2 class="h2-fs">
                    Latest Band News
                </h2>
                <hr>
                <p class="line-height">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum finibus cursus egestas. Cras quis vehicula quam, a tempus velit. Ut feugiat augue in sodales luctus
                </p>
                </div>
            </div>
            
            <div class="wrapper d-flex justify-content-center">
                <div class="image-container">
                    <div class="left-side h-100">
                        <div class="first">
                            1
                        </div>

                        <div class="second">
                            2
                        </div>
                        <div class="third">
                            3
                        </div>
                    </div>


                </div>
            </div>
        </section>
    </main>
</template>
<script>
export default {
    name: 'AppMain',
    data() {
        return {
            
        }
    },
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

div.music-section,
div.band-section{
    width: 40%;
    display: flex;
    @include centering(center, center, column);
    text-align: center;
    padding: 5rem 0 4rem;
}

div.music-section p,
div.band-section{
    color: #7d7b8d;
}

section.band{
    background-color: $darkgray;
}

div.image-container{
    background-color: red;
    width: 75%;
    height: 1600px;
}

div.first{
    width: 62%;
    height: 20%;
    background-color: blue;
}

div.second{
    width: 62%;
    background-color: green;
    height: 60%;
}

div.third{
    width: 62%;
    height: 20%;
    background-color: blue;
}

div.fourth{
    width: 35%;
    background-color: yellow;
    height: 60%;
}

</style>