<template>
    <div class="h-100 w-100 mx-auto d-flex flex-column">
        <header class="mb-auto py-3">
        </header>

        <main class="px-auto">
            <b-tabs class="bg-white shadow w-25 mx-auto text-dark" justified >
                <b-tab title="Login" class="p-5">
                    <div class="w-100 h-100">
                        <router-link to="/" class="text-dark"><h1 class="mb-4">EzAccmd</h1></router-link>
                        <b-input-group class="mx-auto w-75 my-3 shadow" >
                           <b-form-input  class="login-input" :state="usernameState" placeholder="Username" v-model="username" aria-describedby="username-input"></b-form-input>
                        </b-input-group>
                        <b-form-invalid-feedback id="username-input">Enter at least 4 character </b-form-invalid-feedback>

                        <b-input-group class="mx-auto w-75 my-3 shadow">
                            <b-form-input type="password" class="login-input" placeholder="Password"></b-form-input>
                        </b-input-group>

                        <b-button squared class="shadow " variant="success" size="lg">Login</b-button>
                        <br>
                    </div>
                </b-tab>

                <b-tab title="Sign up" class="p-5">
                    <div class="w-100 h-100 d-flex flex-column">
                        <header class="mb-auto w-100">
                            <h1 class="mb-4">Sign up</h1>
                        </header>

                        <main class="d-flex flex-column mb-5 justify-content-center">
                            <b-form-input class="mx-auto w-75 my-2 shadow login-input" placeholder="Firstname"></b-form-input>
                            <b-form-input class="mx-auto w-75 my-2 shadow login-input" placeholder="Lastname"></b-form-input>
                            <b-form-input class="mx-auto w-75 my-2 shadow login-input" placeholder="Username"></b-form-input>
                            <b-form-input class="mx-auto w-75 my-2 shadow login-input" type="password" placeholder="Password"></b-form-input>
                            <b-form-input class="mx-auto w-75 my-2 shadow login-input" placeholder="Email"></b-form-input>
                            <b-button squared class="shadow w-50 mx-auto mt-4" variant="success">Sign up</b-button>
                        </main>

                        <footer class="mt-auto w-100 d-flex justify-content-left">
                            <router-link to="/"><b-icon-arrow-left></b-icon-arrow-left><small class="text-dark"> Back to home </small></router-link>
                        </footer>
                        
                    </div>
                </b-tab>
            </b-tabs>
        </main>

        <footer class="mt-auto">
        </footer>
    </div>
</template>

<style scoped>
    .login-input {
        border-radius: 0;
        text-align: center;
        font-size: 1em;
        padding: 1em 1em 1em 1em;
    }

    .title-pane {
        margin-bottom: 3rem ;
    }
    

</style>

<script>
export default {
    name : 'Login',
    computed: {
        usernameState() {
            return this.username.length > 5 ? true : false
        }
    },
    data() {
        return {
            username : ""
        } 
    }
}
</script>