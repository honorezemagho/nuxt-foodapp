<template>
<section class="masthead center" role="img" aria-label="Image Description">
    <div class="heading">
        <h1>
            Nuxt Food App
        </h1>

        <button>
            <nuxt-link to="/restaurants"> See restaurants</nuxt-link>
        </button>
    </div>

</section>
</template>

<script>
export default {

}
</script>

<style>
.masthead {
    width: 100%;
    height: 100vh;
    padding: 50px;
    overflow: hidden;
    background-size: cover !important;
    background: radial-gradient(ellipse at center, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 47%, rgba(0, 0, 0, 0.65) 100%), url(~assets/headerimg.jpg) no-repeat center center scroll;
}

.center {
    display: flex;
    align-items: center;
    justify-content: center;
}

button {
    width: 100%;
    height: 100%;
    margin-top: 10vh;
}

button>* {
    color: white;
    text-decoration: white;
    font-weight: bold;
}

h1 {
    font-style: normal;
    font-weight: bold;
    color: #eee;
    font-size: 11vmin;
    letter-spacing: 0.03em;
    line-height: 1;
    text-shadow: 1px 2px 4px rgba(0, 0, 0, 0.8);
    margin-bottom: 40px;
}
</style>
