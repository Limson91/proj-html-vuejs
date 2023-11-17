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
</template>

<style scoped lang="scss">
@use 'src/components/style/partials/variables.scss' as *;
@use 'src/components/style/general.scss';
</style>