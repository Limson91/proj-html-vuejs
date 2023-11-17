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

.nav-row {
    display: flex;
    flex-wrap: wrap;
    height: 50px;
    align-items: center;
    justify-content: space-between;
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

.nav-logo {
    width: 100px;
}
</style>