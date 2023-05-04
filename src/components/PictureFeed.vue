<template>
    <div class="wrap_image">
{{info}}
    </div>
</template>
<script>
import axios from 'axios'
export default {
    data(){
        return {
            info: []
        }
    },
    mounted(){
        axios
  .get('https://boiling-refuge-66454.herokuapp.com/images')
  .then(response => {
    this.info = response.data
    console.log(response.data)
    })
  .catch(error => console.log(error));

  console.log('test')
    }
}
</script>
<style lang="scss" scoped>
.wrap_image{
    display: flex;
    flex-wrap: wrap;
    gap: 32px;
}
</style>