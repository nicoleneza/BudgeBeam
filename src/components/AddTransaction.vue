<template  >
    <h2>history</h2>
    <ul i="list" class="list">
        <li 
        v-for="transaction in transactions"
        :key="transaction.id"
        :class="transaction.amount <0 ?'minus':'plus'">
            {{ transaction.text }} <span>${{ transaction.amount }}</span>
            <button class="delete-btn">x</button>
        </li>
    </ul>
</template>
<script setup>
</script>     
