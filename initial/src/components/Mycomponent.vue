<template>
    <div class="root">
        <label>
            Введите email:
            <input type="email" :value="email" @input="emailInput($event.target.value)" />
        </label>
        <label>
            Введите password:
            <input type="password" :value="password" @input="passwordInput($event.target.value)" />
        </label>
    </div>
    <p>email: {{ email }}</p>
    <p>password: {{ password }}</p>
</template>

<script>
export default {
    name: 'MyComponent',
    data() {
        return {
            email: 'example@mail.ru',
            password: '1231243'
        }
    },
    methods: {
        emailInput(value) {
            this.email = value
        },
        passwordInput(value) {
            this.password = value
        }
    }
}

</script>
