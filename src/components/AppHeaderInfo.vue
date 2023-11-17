<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
export default {
    props: {
        companyNumber: String
    }
}
</script>

<template>
    <div class="info-header">
        <nav class="info-container">
            <div class="info-row">
                <div class="info-col">Orari</div>
                <div class="info-col">Contatti</div>
            </div>
        </nav>
    </div>
</template>

<style lang="scss">
@use 'src/components/style/partials/variables.scss' as *;
@use 'src/components/style/general.scss';

.info-header {
    background-color: $dark-gray;
    color: white;
    font-size: 14px;
    padding: 10px;
}

.info-container {
    max-width: 1140px;
    margin: 0 auto;
}

.info-row {
    display: flex;
    flex-wrap: wrap;
    height: 50px;
    align-items: center;
    justify-content: space-between;
}
</style>