<template>
    <div>
        <b-navbar type="dark" class="fixed-top">
            <b-navbar-brand href="#" class="float-left">EasyAccomond</b-navbar-brand>

            <b-navbar-nav class="mr-5">
                <b-nav-item href="#">Home</b-nav-item>
                <b-nav-item href="#">About</b-nav-item>
            </b-navbar-nav>

            <b-navbar-nav class="ml-auto">
                <b-nav-item ><router-link to="login" class="text-nav"> Login </router-link></b-nav-item>
                <b-nav-item href="#">Sign up</b-nav-item>
                <b-nav-item href="#">Get started</b-nav-item>
            </b-navbar-nav>
        </b-navbar>
    </div>
</template>

<script>
export default {
    name : 'NavBar',
    props : {},
    components : {
    },
    methods : {

    }
}
</script>

<style scoped>
    .nav-masterhead .nav-link {
        padding: .25rem 0;
    }
    .text-nav {
        color: rgba(255,255,255,.5) !important;
    }
    
</style>