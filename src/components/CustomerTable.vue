<template>
    <table class="table">
    <thead class="table-secondary">
        <tr>
        <th scope="col">Nama</th>
        <th scope="col">Email</th>
        <th scope="col">Address</th>
        </tr>
    </thead>
    <tbody>
        <tr v-for="customer in customers" :key="customer.id">
        <th>{{ customer.name }}</th>
        <td>{{customer.email}}</td>
        <td>{{customer.address}}</td>
        </tr>
    </tbody>
    </table>
</template>

<script>
export default {
    name: 'customer-table',
    
    props:{
        customers: Array,
    }

}
</script>

style