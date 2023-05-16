<template>
    <div class="saluteUser">
        <nav class="navbar">
            <div class="container-fluid">
                <span class="navbar welcomeTag">Merhaba {{name}} 👋, Hoşgeldin... </span>
                <span class="navbar calendarTag">🗓 Bugün {{ date }}</span>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    data(){
        return{
            name: this.$route.params.email,
            date: new Date().toLocaleDateString(),
        }
    }

}
</script>

<style lang="scss">





</style>