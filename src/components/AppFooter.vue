<template>
    <footer>
        <div class="upper-footer">
            <div class="avada-logo">
                <img src="../assets/images/logo_footer.png" alt="Avada's Logo">
            </div>
            <div class="list-settings">
                <ul>
                    <li v-for="setting in settingList">
                        <a href="#">
                            {{ setting.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'AppFooter',
    data() {
        return {
            settingList:[
                {
                    text: 'Home',
                    active: true
                },
                {
                    text: 'Meet the Band',
                    active: false
                },
                {
                    text: 'Live Dates',
                    active: false
                },
                {
                    text: 'Latest News',
                    active: false
                },
                {
                    text: 'Albums',
                    active: false
                },
                {
                    text: 'Fans',
                    active: false
                }
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../styles/general.scss' as*;
@use '../styles/partials/variables.scss' as*;
@use '../styles/partials/mixins.scss' as*;


div.upper-footer{
    background-color: $gray;
    display: flex;
    align-items: center;
    padding: 3.5rem;
    justify-content: space-between;
}

ul{
    display: flex;   
    margin: 0;

}

ul li{
    list-style: none;
    height: 100%;
    margin-right: 1rem;
    color: white;
}
    
</style>