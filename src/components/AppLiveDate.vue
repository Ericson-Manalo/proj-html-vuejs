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


</style>