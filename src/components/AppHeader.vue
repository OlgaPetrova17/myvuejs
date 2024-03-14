<template>
    <v-app>
        <p>Данные {{title}} - {{age}}</p>
        <p>ФИО {{secondName}} - {{name}}</p>
    </v-app>
</template>

<script>
export default {
    data() {
        return {
            age: 4,
            title: 'Какой-то текст',
            secondName: 'Петрова',
            name: 'Ольга'
        }
    },

    computed: {
        menuItems() {
            return [
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

<style lang="scss" scoped></style>