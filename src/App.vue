<script setup>
import Button from './components/ButtonWithIconAndText.vue'
import { AcademicCapIcon as Icon } from '@heroicons/vue/24/solid'
</script>

<template>
    <!-- <div class="center-by-position"> -->
    <div class="center-by-flex">
        <Button prop_text="Hello, world!" :prop_icon="Icon" />
    </div>
</template>

<style scoped>
.box {
    border: 1px solid black;
    width: 300px;
}

.center-by-flex {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.center-by-position {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>
