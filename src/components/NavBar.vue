<template>
    <div>
        <b-navbar type="dark">
            <b-navbar-brand href="#" class="float-left">EasyAccomond</b-navbar-brand>

            <b-navbar-nav class="mr-5">
                <b-nav-item href="#">Home</b-nav-item>
                <b-nav-item href="#">About</b-nav-item>
            </b-navbar-nav>

            <b-navbar-nav class="ml-auto">
                <b-nav-item href="#">Sign in</b-nav-item>
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
    
</style>