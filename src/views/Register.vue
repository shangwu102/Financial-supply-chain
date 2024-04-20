<template>
  <el-row style="height: 100%;">
    <el-col :span="8" :offset="8" style="border-style: solid;border-color: #e6e6e6;margin-top: 5%">
      <el-row>
        <el-col :span="16" :offset="4">
          <el-form label-width="100px">
            <h3>选手填写部分</h3>
            <el-form-item label="组织名称:">
              <el-input type="primary" v-model="选手填写部分"></el-input>
            </el-form-item>
            <el-form-item label="区块链地址:">
              <el-input type="primary" v-model="选手填写部分"></el-input>
            </el-form-item>
            <el-form-item label="组织类型:">
              <el-radio-group v-model="orgType">
                <el-radio :label="1">公司</el-radio>
                <el-radio :label="2">银行</el-radio>
              </el-radio-group>
            </el-form-item>
          </el-form>
        </el-col>
      </el-row>
      <el-row style="padding-bottom:20px">
        <el-button type="primary" 选手填写部分>注册</el-button>
        <el-button type="primary" 选手填写部分>返回</el-button>
      </el-row>
    </el-col>

  </el-row>

</template>

<script>
export default {
  name: "Register",
  data () {
    return {
      orgType: 1,
      username: '',
      address: ''
    }
  },
  methods: {
    register: function() {
      if (this.address == "") {
        alert("选手填写部分")
      } else {
        let postData = {
          orgType: 选手填写部分,
          username: 选手填写部分,
          address: 选手填写部分
        }
        // 选手填写部分
      }
    },
    goback: function() {
      this.orgType = ''
      this.username = ''
      this.address = ''
      // 选手填写部分
    }

  }
}
</script>

<style scoped></style>