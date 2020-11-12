<template>
<nav>
    <ul>
        <li>
            <nuxt-link exact to="/">
                <AppLogo />
            </nuxt-link>
        </li>
        <li>
            <nuxt-link to="/restaurants">Restaurant</nuxt-link>
        </li>
    </ul>
    <div class="smallnum" v-if="cart.length">{{CartItems}}</div>
    <nuxt-link to="/cart">Cart</nuxt-link>
</nav>
</template>

<script>
import AppLogo from "@/components/AppLogo.vue";
import {
    mapState
} from "vuex";

export default {
    components: {
        AppLogo
    },
    computed: {
        ...mapState([
            'cart'
        ]),
    }
}
</script>

<style scoped>

</style>
