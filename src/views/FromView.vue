<template>
    
    <div class="text-purple-800">
        <div>this is onlick dropdown</div>
        <button class="bg-blue-200" @click="dropdown=!dropdown">menu</button>
        <div class="rounded-lg bg-red-500 animate-fadeIn" v-if="dropdown">this is dropdown</div>
        <div> this is onchange</div>
        <input type="text bg-gradient-to-r" @change="count++">
        <div>
            count is {{count}}
        </div>
        <div>this is v-mode</div>
        <input type="text bg-gradient-to-r" v-model="name">
        <div>{{name}}</div> 
    </div>
  
</template>

<script>
export default {
    data()
    {
        return{
            count: 0,
            dropdown: false,
            name: ' '
        }
    }
}
</script>

<style>

</style>