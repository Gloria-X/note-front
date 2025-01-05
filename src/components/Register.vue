<template>
    <div>
        <el-form ref="form" :model="form" label-width="80px">
            <el-form-item>
                <el-input placeholder="请输入用户名" v-model="form.userName"></el-input>
            </el-form-item>

            <el-form-item>
                <el-input placeholder="请输入密码" v-model="form.password" show-password></el-input>
            </el-form-item>

            <el-form-item>
                <el-button type="primary" @click="onSubmit">立即创建</el-button>
            </el-form-item>
        </el-form>
    </div>
</template>
  
<script>
    export default {
        data() {
            return {
                form: {
                    userName: '',
                    password: ''
                }
            }
        },
        methods: {
            onSubmit() {
                console.log('submit!');
            }
        }
    }
</script>
  
<style scoped>

</style>
  