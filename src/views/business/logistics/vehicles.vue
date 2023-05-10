<template>
    <div class="vehicles">
        <el-breadcrumb separator="/" style="padding-left:10px;padding-bottom:10px;font-size:12px;">
            <el-breadcrumb-item :to="{ path: '/home' }">首页</el-breadcrumb-item>
            <el-breadcrumb-item>物流管理</el-breadcrumb-item>
            <el-breadcrumb-item>配送车辆</el-breadcrumb-item>
        </el-breadcrumb>

        <span>配送中心</span>


    </div>
</template>

<script>
    export default {
        name: "vehicles"
    }
</script>

<style scoped>

</style>
