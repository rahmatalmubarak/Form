<template>
  <div class="container">
    <h1 class="mb-4">Daftar Pelanggan</h1>
    <p>
      <button class="btn btn-primary" type="button" data-toggle="collapse" data-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
        Tambah Pelanggan
        </button>
    </p>

      <customer-table :customers='customers'/>

        <div class="collapse" id="collapseExample">
        <div class="card card-body">
          <h2>Tambah Data Pelanggan</h2>
          <customer-form/>
        </div>
      </div>
  </div>
</template>

<script>
import CustomerTable from '@/components/CustomerTable'
import CustomerForm from '@/components/CustomerForm'

export default {
  name: 'App',
  components: {
    CustomerTable,
    CustomerForm
  },

  data(){
    return{
      customers:[
        {
          id: 1,
          name: 'rahmat',
          email: 'rahmat@gmail.com',
          address: 'padang'
        },
        {
          id: 1,
          name: 'rahmat',
          email: 'rahmat@gmail.com',
          address: 'padang'
        },
        {
          id: 1,
          name: 'rahmat',
          email: 'rahmat@gmail.com',
          address: 'padang'
        }
      ],
      
    }
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
