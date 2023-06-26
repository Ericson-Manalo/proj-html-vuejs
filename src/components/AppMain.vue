<template>
    <main>
        <section class="music">
            <div class="music-section">
                <h2 class="h2-fs">
                Music Is Life
                </h2>
                <hr>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum finibus cursus egestas. Cras quis vehicula quam, a tempus velit. Ut feugiat augue in sodales luctus
                </p>
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
@use '../styles/partials/variables' as*;
@use '../styles/partials/mixins.scss' as*;

section.music{
    background-color: $gray;
    display: flex;
    justify-content: center;
}

div.music-section{
    width: 60%;
    display: flex;
    @include centering(center, center, column);
    text-align: center;
}

</style>