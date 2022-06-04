<template>
    <b-row no-gutters class="elevate w-100 bg-white">
        <b-col cols="12">
            <b-navbar toggleable="lg" type="light">
                <b-row no-gutters class="flex-fill w-100">
                    <b-col cols="12" lg="2" class="d-flex align-items-center justify-content-between justify-content-lg-start">
                        <b-navbar-brand href="#">
                            <img class="eestec-logo" src="../assets/eestec-logo.png" alt="eestec-logo">
                        </b-navbar-brand>
                    </b-col>
                    <b-col lg="8" xl="8" class="d-none d-lg-flex justify-content-center align-items-right">
                        <b-collapse id="nav-collapse" is-nav @hidden="$store.commit('toggleNav', false)" class="bg-white position-absolute menu">
                            <b-navbar-nav>
                                <b-nav-item class="text-uppercase" :to="{ name: 'about' }">o nas</b-nav-item>
                                <b-nav-item class="text-uppercase" :to="{ name: 'timetable' }">artykuły</b-nav-item>
                                <b-nav-item class="text-uppercase" :to="{ name: 'speakers' }">projekty</b-nav-item>
                                <b-nav-item class="text-uppercase" :to="{ name: 'partners' }">partnerzy</b-nav-item>
                                <b-nav-item class="text-uppercase" :to="{ name: 'previousEditions' }">aktualności</b-nav-item>
                                <b-nav-item class="text-uppercase mb-2" href="http://bit.ly/aplikujnaSSA10" target="_blank">
                                </b-nav-item>
                            </b-navbar-nav>
                        </b-collapse>
                    </b-col>
                    <!--
                    <b-col lg="2" class="d-none d-lg-flex justify-content-end align-items-center">
                    <b-button size="lg" href="https://forms.gle/mRgEjxCq6FqFncFN7" target="_blank">ZAPISY</b-button>
                    </b-col>
                    -->
                </b-row>


            </b-navbar>
        </b-col>
    </b-row>
</template>

<script>

export default {
    name: 'MyHeader',
    components: {

    }
}
</script>

<style scoped lang="scss">
    .eestec-logo {
        width: 40%;
    }
    .elevate {
        z-index: 90;
    }

</style>