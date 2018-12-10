<template>
    <v-toolbar>
        <!--<v-toolbar-side-icon></v-toolbar-side-icon>-->
        <v-toolbar-title>Programmer spiritual</v-toolbar-title>
        <v-spacer></v-spacer>
        <div class="hidden-sm-and-down">
            <router-link to="/forum">
                <v-btn flat>Forum</v-btn>
            </router-link>
            <router-link><v-btn flat>Pose tes questions</v-btn></router-link>
            <router-link> <v-btn flat>Category des questions</v-btn></router-link>
            <router-link to="/login"><v-btn flat>Login</v-btn></router-link>




        </div>
    </v-toolbar>
</template>

<script>

</script>

<style scoped>

</style>