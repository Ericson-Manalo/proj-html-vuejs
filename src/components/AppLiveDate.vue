<template>
    <section class="live-dates">
        <div class="d-flex justify-content-center">
            <div class="live-section">
                <h2 class="h2-fs">
                    Live Dates
                </h2>
                <hr>
                <p class="line-height">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum finibus cursus egestas. Cras quis vehicula quam, a tempus velit. Ut feugiat augue in sodales luctus
                </p>
            </div>
        </div>

        <div class="accordion" id="accordion">
            <div class="accordion-item">
                <h2 class="accordion-header" id="headingOne">
                <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                    <strong>17/08/2020 GEM FESTIVAL 2020 ANAKALIA, GEORGIA</strong>
                </button>
                </h2>
                <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordion">
                    <div class="accordion-body">
                        <div class="map">
                            <img src="../assets/images/staticmap.png" alt="Map">
                        </div>
                        <div class="untold-stories">
                            <h5>
                                Untold Stories
                            </h5>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                            </p>
                            <button>
                                BOOK NOW
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
        </div>
    </section>
</template>
<script>
export default {
    name: 'AppLiveDate',
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

section.live-dates{
    background-color: $darkgray;
}

div.live-section{
    width: 40%;
    display: flex;
    @include centering(center, center, column);
    text-align: center;
    padding: 5rem 0 4rem;
    color: #7d7b8d;
}

div.accordion{
    display: flex;
    justify-content: center;

    div.accordion-item{
        width: 60%;
        border: none;
        border-radius: 0;
    }
}

button.accordion-button{
    background-color: $gray;
}

strong{
    color: $red;
}

div.accordion-body{
    display: flex;
    background-color:$gray;
    div.map img{
        width: 300px;


    }
}

div.untold-stories{
    margin-left: 2rem;
    margin-top: 1rem;
}

</style>