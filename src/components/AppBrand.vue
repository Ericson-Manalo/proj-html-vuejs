<template>
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
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-12 col-lg-8">
                            <div class="row">
                                <div class="col-12 mb-3 technology-card">
                                    <div class="details-card">
                                        <h4>
                                        Technology and music
                                        </h4>
                                        <p>
                                            Sed sit amet sem turpis. Curabitur cursus lacinia est interdum risus id condimentum.
                                        </p>
                                    </div>
 
                                </div>
                                <div class="col-12 col-lg-6 guitar-card">
                                    <div class="details-card">
                                        <h4>
                                        While my guitar gently weeps
                                        </h4>
                                        <p>
                                            Sed sit amet sem turpis. Curabitur cursus lacinia est interdum risus id condimentum.
                                        </p>
                                    </div>
                                </div>
                                <div class="col-12 col-lg-6 mb-3 sounds-card">
                                    <div class="details-card">
                                        <h4>
                                        It just sounds better
                                        </h4>
                                        <p>
                                            Sed sit amet sem turpis. Curabitur cursus lacinia est interdum risus id condimentum.
                                        </p>
                                    </div>
                                </div>
                                <div class="col-12 flavor-rock-card ">
                                    <div class="details-card">
                                        <h4>
                                        The flavor of rock
                                        </h4>
                                        <p>
                                            Sed sit amet sem turpis. Curabitur cursus lacinia est interdum risus id condimentum.
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <div class="col-12 col-lg-4">
                            <div class="col-12 old-school-card">
                                <div class="details-card">
                                    <h4>
                                    Taking it back to the old school
                                    </h4>
                                    <p>
                                        Sed sit amet sem turpis. Curabitur cursus lacinia est interdum risus id condimentum.
                                    </p>
                                </div>
                            </div>
                            <div class="col-12 stage-card">
                                <div class="details-card">
                                    <h4>
                                    Sharing the stage with a legened
                                    </h4>
                                    <p>
                                        Sed sit amet sem turpis. Curabitur cursus lacinia est interdum risus id condimentum.
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="d-flex justify-content-center banner align-items-center h-100">
                <p class="m-0">
                    VIEW ALL LATEST NEWS
                </p>
            </div>

            <section class="citation">
                <div class="citation">
                    <p>
                        “I just listened to it and said to myself, “Man, I really love this album.” Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They’re good. And they’re inventive. I haven’t heard anything this year that’s as inventive. I don’t really expect to.”
                    </p>
                    <a href="#">
                        <img src="../assets//images/band_interview_play_icon.png" alt="Band interview play icon">
                    </a>
                    
                </div>
            </section>

        </section>
</template>
<script>
export default {
    name: 'AppBand',
    data() {
        return {
            
        }
    },
}
</script>
<style lang="scss">
@use '../styles/general.scss' as*;
@use '../styles/partials/variables.scss' as*;
@use '../styles/partials/mixins.scss' as*;

div.band-section{
    width: 40%;
    display: flex;
    @include centering(center, center, column);
    text-align: center;
    padding: 5rem 0 4rem;
    color: #7d7b8d;
}


div.wrapper{
    padding-bottom: 8rem;
}

section.band{
    background-color: $darkgray;
}

div.container-fluid{
    max-width: 65%;
}

div.technology-card{
    height: 300px;
    background-image: url('../assets/images/blog_music_techo-800x400.jpg');
    background-repeat: no-repeat;
    position: relative;
}

div.details-card{
    position: absolute;
    bottom: 0;
    left: 0;
    padding: 1.3rem;
    background-color: $gray;
    width: 100%;
}

div.details-card h4{
    margin-bottom: .8rem;
    color: $red;
}

div.details-card p{
    color: $lightgray;
}

div.guitar-card{
    background-image: url('../assets/images/blog-post3-400x600.jpg');
    height: 600px;
    border-right: 4px solid $darkgray;
    position: relative;
}

div.sounds-card{
    background-image: url('../assets/images/blog-post4-400x600.jpg');
    height: 600px;
    border-left: 4px solid $darkgray;
    position: relative;
}

div.flavor-rock-card{
    height: 300px;
    background-image: url('../assets/images/blog_flavor_rock-800x400.jpg');
    position: relative;
}

div.old-school-card{
    background-image: url('../assets/images/blog-post1-400x600.jpg');
    height: 600px;
    margin-bottom: 30px;
    background-repeat: no-repeat;
    position: relative;
    background-position: center;
}

div.stage-card{
    background-image: url('../assets/images/blog-post2-400x600.jpg');
    height: 600px;
    background-repeat: no-repeat;
    position: relative;
    background-position: center;
}

.row{
    padding-right: 1rem;
}

div.banner{
    padding: 3rem;
    background-color: $red;
    color: white;
    font-size: 18px;
    font-weight: 700;
}

div.banner:hover{
    background-color: white;
    color: black;
    cursor: pointer;
}

section.citation{
    background-image: url('../assets/images/home-testimonial-parallax.jpg');
    height: 90vh;
    display: flex;
    justify-content: center;
}

div.citation{
    width: 40%;
    display: flex;
    @include centering (center, center, column);
    text-align: center;
    height: 100%;
}

div.citation p{
    color: white;
    font-style: italic;
    font-size: 22px;
    line-height: 44px;
    font-weight: 400;
    font-family: 'Merriweather', serif;
    padding-bottom: 3rem;
}   

</style>