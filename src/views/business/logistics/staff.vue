<template>
    <div class="staff">
        <el-breadcrumb separator="/" style="padding-left:10px;padding-bottom:10px;font-size:12px;">
            <el-breadcrumb-item :to="{ path: '/home' }">首页</el-breadcrumb-item>
            <el-breadcrumb-item>物流管理</el-breadcrumb-item>
            <el-breadcrumb-item>配送人员</el-breadcrumb-item>
        </el-breadcrumb>
        <span>配送人员</span>

    </div>
</template>

<script>
    export default {
        name: "staff"
    }
</script>

<style scoped>

</style>
