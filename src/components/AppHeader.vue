<template>
   <v-app>
        <v-toolbar app dark class="primary" image="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg">
            <v-toolbar-title v-text="'My VueJs'"></v-toolbar-title>
            <v-spacer></v-spacer>
            <v-toolbar-items>
                <!-- <v-btn v-for="(item, i) in menuItems" flat: key="'menuItem${i}'" :to="item.route">
                    <v-icon left v-html="item.icon"></v-icon>
                    {{ item.title }}
                    </v-btn> -->

                    <v-btn> <svg-icon type="mdi" :path="path"></svg-icon> Моя кнопка</v-btn>



                    <!-- <p style="color: bisque;">Текст 1 </p>
                    <p>Текст 2 </p>                    
                    <p>Текст 3 </p>                    
                    <p v-for="(b) in menuItems" :key="b.icon" style="color: bisque;" >{{ b.title }}</p> -->                    
            </v-toolbar-items>
        </v-toolbar>
   </v-app>
</template>

<script>
    export default {
        computed: {
            menuItems(){
                return[
                    {
                        icon: 'visibility',
                        title: 'Читать',
                        route: '/books',
                    },
                    {
                        icon: 'extention',
                        title: 'Учить слова',
                        route: '/words',
                    },
                    {
                        icon: 'account_circle',
                        title: 'Мой кабинет',
                        route: '/profile',
                    },
                    {
                        icon: 'exit_to_app',
                        title: 'Выход',
                        route: '/logout',
                    },
                    {
                        icon: 'input',
                        title: 'Войти',
                        route: '/signin',
                    },
                    {
                        icon: 'lock_open',
                        title: 'Зарегистрироваться',
                        route: '/signup',
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>