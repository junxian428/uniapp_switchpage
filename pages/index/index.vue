<template>
	   <div class="container">
	     <div class="box">
	       <h1><u>Hello World</u></h1>
		   		<navigator url="/pages/index/list/list" open-type="switchTab" hover-class="other-navigator-hover">
		   						<button type="default" @click="getDemo4">跳转tab页面</button>
		   					</navigator>
	     </div>
	
	   </div>
</template>

<script>
	export default {
		data() { 
			return {
			}
		},
		onLoad() {

		},
		methods: {
			getDemo4(){
				uni.navigateTo({
					url:"/pages/index/list/list"
				})
			}
		}
	}
</script>


<style lang="scss">
.container {
  display: flex;
  justify-content: center;
  align-items: flex-start; /* Aligns content at the top */
  height: 100vh;
}

.box {
  height: 100px;
  background: pink;
  h1 {
    font-size: 40px;
    color: red;
  }
}
</style>