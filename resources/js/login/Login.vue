<template>
 <v-container>
     <div>
         <v-form  @submit.prevent="login">
             <v-text-field
                     v-model="form.email"
                     label="Email"
                     type="email"
                     required
             ></v-text-field>
             <v-text-field
                     v-model="form.password"
                     type="password"
                     label="E-mail"
                     required
             ></v-text-field>

             <v-btn
                     color="green"
                     type="submit"
             >
                 Login

             </v-btn>
         </v-form>
     </div>
 </v-container>
</template>

<script>
    export default {
       data()
       {
           return {
               form:{
                   email:null,
                   password:null
               }
           }
       },
        methods:{
           login(){
               axios.post('api/auth/login',this.form)
                   .then(res=>console.log(res.data))
                   .catch(error => console.log(error.response.data))
           }
        }
    }
</script>

<style scoped>

</style>