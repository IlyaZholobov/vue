<template>
    <div class="root">
        <p>
            Введите кол-во продуктов:
        </p>
        <button @click="minusClick()">-</button>
        <input type="number" :value="count" @change="changeInput($event.target.value)" max="10" min="1">
        <button @click="plusClick()">+</button>
    </div>
</template>

<script>
export default {
    name: 'HomeTask',
    data() {
        return {
            count: 1
        }
    },
    methods: {
        changeInput(value) {
            this.count = parseInt(value)
        },
        minusClick() {
            if (this.count != 1) {
                this.count -= 1
            }
        },
        plusClick() {
            if (this.count != 10) {
                this.count += 1
            }
        }
    }

}
</script>