<script>
	export default {
		// globalData:{}      //get().globalData
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style lang="scss">
	/*每个页面公共css */
	/* 样式必须注意，兼容H5/webApp/各类小程序 */
	/* 小程序中不支持*号选择器，以及复杂选择器  */
	/* 相当于*号选择器  对一个不存在的标签进行取反，就是选择所有的标签 */ 
	:not(not){
		// 盒子模型计算方案-内容盒子(默认值)
		// box-sizing: content-box;  //总宽=margin+border+padding+width
		// 盒子模型计算方案-边框盒子
		box-sizing: border-box;   //总宽=margin+width
	}
	/* body(只有H5支持)必须替换为page */
	page{
		background-color: $uni-bg-color;  //f5f5f5
		color: $uni-text-color;  //666
		font-size: $uni-font-size-base;   //14px 
	}
</style>
