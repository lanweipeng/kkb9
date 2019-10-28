<template>
  <div id="app">
    <l-form>
      <l-formItems label="用户">
      <l-input v-model="username" type="username"></l-input>
    </l-formItems>
    <l-formItems label="密码">
      <l-input v-model="password" type="password"></l-input>
    </l-formItems>
      </l-form> 
    
  </div>
</template>

<script>
import LInput from '@/components/LInput.vue'
import LFormItems from '@/components/LFormItems.vue'
import LForm from '@/components/LForm'
export default {
  name: 'App',
  provide(){
    return{
            someval:'hh'
    }
  },
  components:{
    LInput,LFormItems,LForm
  },data(){
        return {
            username:'',password:'',value:''
        }
    }
}
</script>

<style>
</style>
