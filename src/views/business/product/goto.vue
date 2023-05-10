<template>
	<div id="productCategroys">
		
		 <el-carousel :interval="1500" arrow="always">
		    <el-carousel-item v-for="item in 4" :key="item">
		    </el-carousel-item>
		  </el-carousel>
		  
		<el-steps :active="8" align-center>
			<el-step title="任务9"></el-step>
			<el-step title="任务5"></el-step>
			<el-step title="任务1"></el-step>
			<el-step title="任务3"></el-step>
			<el-step title="任务6"></el-step>
			<el-step title="任务10"></el-step>
			<el-step title="任务8"></el-step>
			<el-step title="任务4"></el-step>
			<el-step title="任务2"></el-step>
			<el-step title="任务7"></el-step>
			<el-step title="任务11"></el-step>
			<el-step title="任务14"></el-step>
			<el-step title="任务12"></el-step>
			<el-step title="任务20"></el-step>
			<el-step title="任务13"></el-step>
			<el-step title="任务16"></el-step>
			<el-step title="任务19"></el-step>
			<el-step title="任务18"></el-step>
			<el-step title="任务15"></el-step>
			<el-step title="任务17"></el-step>
		</el-steps>
	<h3 style="text-align: center; ">总里程：<span style="color: #459eff;">871.1174</span>&nbsp;&nbsp;Km</h3>

	</div>
</template>


<script>
	export default {
		

	}
</script>
<style>
	.el-main{
		width: 100%;
	}
.el-steps{
	margin-top: 20px;
	padding: 10px;
	/* border:5px solid #ddd;
	 border-image: linear-gradient(#F80, #2ED) 20 20; */
}
.el-carousel__item h3 {
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    line-height: 300px;
    margin: 0;
  }
  
  .el-carousel__item:nth-of-type(1) {
    background:url(../../../assets/goods1.jpg) no-repeat ;
	background-size:cover;
  }
  .el-carousel__item:nth-of-type(2) {
    background:url(../../../assets/goods2.jpg) no-repeat;
	background-size:cover;
  }
  .el-carousel__item:nth-of-type(3) {
    background:url(../../../assets/goods3.jpg) no-repeat;
	background-size:cover;
  }
  .el-carousel__item:nth-of-type(4) {
    background:url(../../../assets/goods4.jpg) no-repeat;
	background-size:cover;
  }
 

</style>
