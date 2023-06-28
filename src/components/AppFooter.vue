<template>
    <footer>
        <div class="upper-footer">
            <div class="avada-logo">
                <img src="../assets/images/logo_footer.png" alt="Avada's Logo">
            </div>
            <div class="list-settings">
                <ul>
                    <li v-for="setting in optionList" :class="setting.link ? 'active' : ''">
                        <a href="#">
                            {{ setting.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <div class="lower-footer">
            <p class="footer-settings">
                © Copyright 2012 - 2023 | <span>Avada Website Builder</span>  by <span>ThemeFusion</span>  | All Rights Reserved | Powered by <span>WordPress</span> 
            </p>

            <div class="footer-icons">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-youtube"></i>
            </div>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'AppFooter',
    data() {
        return {
            optionList:[
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
    color: #7d7b8d;
    font-size: 13px;

    li.active{
    color: white;
    }
}

div.lower-footer{
    background-color: $darkgray;
    padding: 3rem 2rem;
    display: flex;
    justify-content: space-between;

    p{
        color:#7d7b8d;
        font-size: 14px;
        margin: 0;
        display: flex;
        align-items: center;

        span{
            color: $red;
        }
    }
}

div.footer-icons i{
    background-color: $gray;
    color: $lightgray;
    padding: 1rem;
    margin-left: .5rem;
    border-radius: 4px;
}


    
</style>