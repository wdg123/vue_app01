<template>
  <div class="hello">
    <div v-for="i in abc">{{i}}</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      
    }
  },
  computed:{
	  abc:function(){
		var arr=[];
		for(i=1;i<=10000;i++){
			arr.push(i);
		}
		return arr;
	  }
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
