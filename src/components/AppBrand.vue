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
                                        3
                                    </div>
                                    <div class="col-12 col-lg-6 mb-3 sounds-card">
                                        2
                                    </div>
                                    <div class="col-12 flavor-rock-card ">
                                    1
                                </div>
                            </div>
                        </div>

                        <div class="col-12 col-lg-4">
                            <div class="col-12 old-school-card">
                                        1
                            </div>
                            <div class="col-12 stage-card">
                                        1
                            </div>
                        </div>
                        

                    </div>
                </div>
            </div>
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
}

div.band-section{
    color: #7d7b8d;
}

section.band{
    background-color: $darkgray;
    padding-bottom: 6rem;
}

div.container-fluid{
    max-width: 65%;
}

div.technology-card{
    height: 300px;
    background-image: url('../assets/images/blog_music_techo-800x400.jpg');
    background-repeat: no-repeat;
}

div.guitar-card{
    background-image: url('../assets/images/blog-post3-400x600.jpg');
    height: 600px;
    border-right: 4px solid $darkgray;

}

div.sounds-card{
    background-image: url('../assets/images/blog-post4-400x600.jpg');
    height: 600px;
    border-left: 4px solid $darkgray;

}

div.flavor-rock-card{
    height: 300px;
    background-image: url('../assets/images/blog_flavor_rock-800x400.jpg');

}

div.old-school-card{
    background-image: url('../assets/images/blog-post1-400x600.jpg');
    height: 600px;
    margin-bottom: 30px;
    background-repeat: no-repeat;
}

div.stage-card{
    background-image: url('../assets/images/blog-post2-400x600.jpg');
    height: 600px;
    background-repeat: no-repeat;

}

.row{
    padding-right: 1rem;
}
    
</style>