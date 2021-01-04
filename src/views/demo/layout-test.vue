<!-- 布局测试组件 -->
<template>
  <div class="layout-test">
    <span class="fixed-center">企业信息详情页</span>
    <br/>
    <br/>
    <br/>
    <span class="fixed-top" >企业评分：99 &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
    &nbsp&nbsp&nbsp&nbsp&nbsp企业等级：AA</span>
    <br/>
    <br/>
    <table>
      <tbody>
        <tr>
          <td class="bt">客商名称</td>
          <td class="nr">xxx公司</td>
          <td class="bt">法人</td>
          <td class="nr">张三</td>
        </tr>
        <tr>
            <td class="bt">类别</td>
            <td class="nr">经销商</td>
            <td class="bt">电话</td>
            <td class="nr">13342452335</td>
          </tr>
        <tr>
            <td class="bt">营业执照</td>
            <td class="nr">营业执照编号</td>
            <td class="bt">身份证</td>
            <td class="nr">42046433561945213</td>
          </tr>
        <tr>
            <td class="bt">地区</td>
            <td class="nr">湖南省 长沙市</td>
            <td class="bt">银行卡开户行</td>
            <td class="nr">湖南省长沙县星沙建行分行</td>
          </tr>
        <tr>
            <td class="bt">地址</td>
            <td class="nr">xxxx</td>
            <td class="bt">卡号</td>
            <td class="nr">324500757599699</td>
          </tr>
          <tr>
              <td colspan="2" rowspan="3">
                显示营业执照照片，没有不显示
              </td>
          </tr>
          <tr>
           <td colspan="2" rowspan="3">
                </td>
            </tr>
      </tbody>

    </table>

    <textarea class="bz" name="reworkmes"   cols="50"  rows="4" ></textarea>


  </div>
</template>

<script>
export default {
  name: "test",
  components: {},
  data() {
    return {};
  },
  props: {},
  computed: {},
  methods: {},
  watch: {},
  created() {}
};
</script>

<style lang="less" scoped>
.layout-test {
  text-align: center;
  padding: 16px;
  span {
    font-size: 18px;
  }
  ul {
    padding-top: 20px;
  }
  li {
    text-align: left;
  }
   .fixed-center {
      position: fixed;
      float: center;
    }
  .fixed-top {
    //position: fixed; /*固定作用*/
    margin: 0 auto;
    font-size:12px;
    float:left;
  }
  .bt {
    width:100px;
  }
  .nr {
      font-size:14px;
      border:0.1px solid gray;
      width:410px;
      height:35px;
      text-align:left;
  }
  td{
     font-size:14px;
     border:0.1px solid gray;
     width:410px;
     height:35px;
  }
  table {
  border-collapse:collapse;
    //border:1px solid gray;
  }
  .bz {
    border-collapse:collapse;
    OVERFLOW:hidden;
    width:1000px;
  }

}
</style>
