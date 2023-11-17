<script>
import AppHeaderInfo from './AppHeaderInfo.vue';
import { store } from '../store';

export default {
    data() {
        return {
            store: store,
        }
    },

    components: {
        AppHeaderInfo,
    }
}
</script>

<template>
    <AppHeaderInfo />

    <div class="hero">
        <div class="nav-header">
            <nav class="nav-container">
                <div class="nav-row">
                    <div class="nav-logo-col">
                        <img class="nav-logo" src="nexgen-logo.svg">
                    </div>

                    <div class="nav-menu-col">
                        <ul class="nav-menu-list">
                            <li class="nav-menu-item">HOME</li>
                            <li class="nav-menu-item">ABOUT</li>
                            <li class="nav-menu-item">SERVICES</li>
                            <li class="nav-menu-item">PROCESS</li>
                            <li class="nav-menu-item">TEAM</li>
                            <li class="nav-menu-item">BLOG</li>

                            <button class="nav-button">GET IN TOUCH</button>
                        </ul>

                    </div>
                </div>
            </nav>
        </div>

        <div class="hero-container">
            <div class="col-6 hero-card">
                <h4 class="hero-min-title">FUSIONS & ACQUISITIONS</h4>
                <h2 class="hero-max-title">INSURANCE<br>CONSULTING</h2>
                <div class="col-row">
                    <col-6>
                        <input class="hero-col-item" type="text" placeholder="Name">
                    </col-6>
                    <col-6>
                        <input class="hero-col-item" type="text" placeholder="Email">
                    </col-6>
                    <col-6>
                        <input class="hero-col-item" type="text" placeholder="Phone">
                    </col-6>
                    <col-6>
                        <input class="hero-col-item" type="text" placeholder="More Info">
                    </col-6>

                </div>
                <div class="col-row">
                    <button class="hero-button-solid">GET IN TOUCH</button>
                    <button class="hero-button">READ MORE</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use 'src/components/style/partials/variables.scss' as *;
@use 'src/components/style/general.scss';

.nav-header {
    background-color: white;
    color: $dark-gray;
    font-size: 14px;
    padding: 10px;
}

.nav-container {
    max-width: 1140px;
    margin: 0 auto;
}

.hero {
    height: 812px;
    background-image: url('header.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    display: flex;
    flex-direction: column;
}

.hero-container {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    margin-top: 150px;
}

.hero-card {
    width: 512px;
}

.col-row {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    margin-bottom: 15px;
}

.nav-row {
    display: flex;
    flex-wrap: wrap;
    height: 50px;
    align-items: center;
    justify-content: space-between;
}

.hero-min-title {
    font-size: 14px;
    font-weight: 500;
    color: $dark-green;
}

.hero-max-title {
    font-size: 65px;
}

.hero-col-item {
    background-color: white;
    border: none;
    color: darkgray;
    height: 50px;
    width: 248px;
    font-size: 16px;
    padding: 0 15px;
    border-radius: 5px;
}

.nav-menu-list {
    display: flex;
    flex-direction: row;
    align-items: center;
}

.nav-menu-item {
    padding: 0 20px;
    font-size: 16px;
}

.nav-button {
    background-color: $dark-green;
    border: none;
    color: white;
    height: 46px;
    width: 171px;
    font-size: 16px;
    text-align: center;
    text-decoration: none;
    border-radius: 5px;
    margin-left: 20px;
}

.hero-button-solid {
    background-color: $dark-green;
    border: none;
    color: white;
    height: 46px;
    width: 171px;
    font-size: 16px;
    text-align: center;
    text-decoration: none;
    border-radius: 5px;
}

.hero-button {
    background-color: white;
    border: 1px solid $dark-green;
    color: $dark-green;
    height: 46px;
    width: 171px;
    font-size: 16px;
    text-align: center;
    text-decoration: none;
    border-radius: 5px;
}

.nav-logo {
    width: 100px;
}

.col-6 {
    flex-basis: calc((100% / 12) * 6);
}
</style>