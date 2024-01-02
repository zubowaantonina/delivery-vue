<template>
    <header class="header">
        <div class="container">
            <div class="header-box">
                <router-link to="/" class="header-logo logo">
                    <img src="../assets/img/icon/logo.svg" alt="Logo" />
                </router-link>
                <div class="header-controls">
                    <button class="btn btn-primary">
                        <img src="../assets/img/icon/user.svg" alt="User" />
                        Войти
                    </button>
                    <button class="btn btn-outline" @click="openModal()">
                        <img src="../assets/img/icon/shopping-cart.svg" alt="card" />
                        Корзина
                    </button>
                </div>
            </div>
        </div>
        <!-- /.container  -->
    </header>
</template>
<script setup>
const emit = defineEmits(['toggleModal'])
const openModal = () => emit('toggleModal')
    
    // console.log('open');


</script>
<style scoped>
.header {
    min-height: 124px;
    display: flex;
    align-items: center;

}

.header-box {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header-controls {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 10px;
}
</style>