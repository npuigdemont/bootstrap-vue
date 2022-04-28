<template>
   <div class="mt-4">
    <ul>
        <li v-for="user in users" :key="user.id">
            <h3>{{user.name}}</h3>
        </li>
    </ul>
    </div>
</template>

<script>
import axios from 'axios';
export default {
    async created() {
        const response = await axios.get('https://jsonplaceholder.typicode.com/users');
        this.users = response.data;
    },
    data() {
        return {
            
            users: []
        }
    },
    name: 'Axios'
}
</script>