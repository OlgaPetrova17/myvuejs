<template>

    <h1>Урок № {{ lessonNumber }} : {{  title }}</h1>
    <p>ФИО {{ secondName }} - {{ name }}</p>
    <p>{{ menuItems }}</p>
</template>

<script>
export default {
    data() {
        return {
            lessonNumber: 1,
            title: 'Привязка данных',
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