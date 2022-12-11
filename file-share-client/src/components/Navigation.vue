<template>
    <header class="flex flex-wrap md:flex-no-wrap items-center justify-between mb-6 -mt-3">
        
        <ul class="flex items-center">
        <li>
            <router-link :to="{ name: 'home'}">Home</router-link>
        </li>

        <li>
            <a href="" class="text-sm inline-block p-3 text-gray-800">Your files</a>
        </li>        
        </ul>
        {{ authenticated }}
        <ul class="flex items-center">
        <li>
            <router-link :to="{ name: 'login'}">Sign in</router-link>
        </li>
        <li>
            <a href="#" class="text-sm inline-block p-3 text-gray-800">Create Account</a>
        </li>        
        </ul>
    
    </header>
</template>

<script>
    import { mapGetters } from 'vuex'

    export default {
        computed: {
            ...mapGetters({
                authenticated: 'auth/authenticated'
            })
        }
    }
</script>