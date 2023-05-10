<template>
	<div id="productCategroys">
		<el-breadcrumb separator="/" style="padding-left:10px;padding-bottom:10px;font-size:12px;">
			<el-breadcrumb-item :to="{ path: '/home' }">首页</el-breadcrumb-item>
			<el-breadcrumb-item>业务管理</el-breadcrumb-item>
			<el-breadcrumb-item>配送方案</el-breadcrumb-item>
		</el-breadcrumb>
		<el-table :data="tableData3" style="width: 100%">
			<el-table-column prop="date" label="日期" width="150"></el-table-column>
			<el-table-column prop="carID" label="车辆编号" width="150">

			</el-table-column>
			<el-table-column prop="dist" label="配送方案" width="500">
				<!--< el-collapse v-model="activeName" accordion>
				  <el-collapse-item title="任务1" name="1">
				    <div> 配送点编号：1   </div>
				    <div> 目的地：长沙经济开发区</div>
					<div> 物资编号：3DFC8EA0-6</div>
				  </el-collapse-item>
				  <el-collapse-item title="任务2" name="2">
				    <div> 配送点编号：2   </div>
				    <div> 目的地：长沙经济开发区</div>
				    <div> 物资编号：3DFC8EA0-6</div>
				  </el-collapse-item>
				  <el-collapse-item title="任务3" name="3">
				    <div> 配送点编号：3   </div>
				    <div> 目的地：长沙经济开发区</div>
					<div> 物资编号：3DFC8EA0-6</div>
				  </el-collapse-item>
				  <el-collapse-item title="任务4" name="4">
				    <div> 配送点编号：4   </div>
				    <div> 目的地：长沙经济开发区</div>
				    <div> 物资编号：3DFC8EA0-6</div>
				  </el-collapse-item>
				  <el-collapse-item title="..." name="5">
				    <div>...</div>
				    <div>...</div>
				  </el-collapse-item>
				</el-collapse> -->
				

			</el-table-column>
			<el-table-column label=" " style="width: 100px;">
		   
				  
			</el-table-column>
			<el-table-column label="方案生成" style="width: 100px;">
				<el-button
				    type="primary"
				    @click="openFullScreen2"
				    v-loading.fullscreen.lock="fullscreenLoading">
				    生成
				  </el-button>
				  
			</el-table-column>
		</el-table>


	</div>
</template>


<script>
	export default {
		data() {
			return {
				tableData3: [{
					date: '2021-05-03',
					carID: '湘AGF388',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区7仓 | 物资总数：20'
				}, {
					date: '2021-05-03',
					carID: '湘AGD728',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区8仓 | 物资总数：20'
				}, {
					date: '2021-05-03',
					carID: '湘AM65D388',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区9仓 | 物资总数：20'
				}, {
					date: '2021-05-03',
					carID: '湘AGF329',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区9仓 | 物资总数：20'
				}, {
					date: '2021-05-03',
					carID: '湘AG6743B',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区2仓 | 物资总数：20'
				}, {
					date: '2021-05-03',
					carID: '湘AG5943B',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区3仓 | 物资总数：20'
				}, {
					date: '2021-05-03',
					carID: '湘A8888',
					dist: '任务编号：1-20 | 取货仓：长沙经济开发区6仓 | 物资总数：20'
				}],
				fullscreenLoading: false
			}
		},
		methods:{
			 openFullScreen2() {
			        const loading = this.$loading({
			          lock: true,
			          text: 'Loading',
			          spinner: 'el-icon-loading',
			          background: 'rgba(0, 0, 0, 0.7)'
			        });
			        setTimeout(() => {
						loading.close();
			         this.$router.push({path:'goto'});
			        }, 1000);
			      }
		}
	}
</script>
<style>
	
</style>
