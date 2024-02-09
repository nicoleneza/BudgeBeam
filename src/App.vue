<template>
    <Header/>
    <div class="container">
        <Balance/>
        <ExpenseIncome/>
        <AddTransaction/>
        <Balance/>
      </div>
</template>
<script setup>
import Balance from "./components/Balance.vue";
import Header from "./components/Header.vue";
import AddTransaction from "./components/AddTransaction.vue";
import ExpenseIncome from "./components/ExpenseIncome.vue";
import { ref } from 'vue';

const    transactions= ref([
                {id:1, text:'beans',amount:123},
                {id:2, text:'biscuits',amount:-1234}
            ]  ) 

</script>

<!-- <script setup>
import { reactive, computed } from 'vue'

const author = reactive({
  name: 'John Doe',
  books: [
    'Vue 2 - Advanced Guide',
    'Vue 3 
     - Basic Guide',
    'Vue 4 - The Mystery'
  ]
})

// a computed ref
const publishedBooksMessage = computed(() => {
  return author.books.length > 0 ? 'Yes' : 'No'
})
</script>

<template>
  <p>Has published books:</p>
  <span>{{ publishedBooksMessage }}</span>
</template> -->