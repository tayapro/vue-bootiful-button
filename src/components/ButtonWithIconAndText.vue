<script setup>
defineProps(['prop_text', 'prop_icon'])
</script>

<template>
    <button>
        <div class="button-with-icon">
            <component :is="prop_icon" class="icon" />
            <p>{{ prop_text }}</p>
        </div>
    </button>
</template>

<style scoped>
.button-with-icon {
    display: flex;
    padding: 0.3rem;
    align-items: center;
    cursor: pointer;
    gap: 0.5rem;
    color: #f5f5f5;
}

button {
    border: none;
    background-color: #009999;
    border-radius: 5px;
}

button:hover {
    background-color: #0099cc;
    border-color: #0099cc;
}

.icon {
    width: 1.5rem;
    height: 1.5rem;
    color: #f5f5f5;
}
</style>
