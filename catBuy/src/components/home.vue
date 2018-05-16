<template>
    <div class="adm-home fillcontain">
        <div class="el-row fillcontain">
            <div class="el-col el-col-4 fillcontain">
                <div class="grid-content bg-purple-dark fillcontain">
                    <adm-manage-menu></adm-manage-menu>
                </div>
                
            </div>
            <div class="el-col el-col-20 fillcontain">
                <div class="grid-content bg-purple-light fillcontain">
                    <adm-manage-content></adm-manage-content>
                </div>
                
            </div>
        </div>
    </div>
</template>
<script>
    import admManageMenu from './admManageMenu.vue'
    import admManageContent from './admManageContent.vue'
    export default {
        data:function(){
            return {

            }
        },
        components:{
            'adm-manage-menu':admManageMenu,
            'adm-manage-content':admManageContent
        }
    }
</script>
<style lang='less'>
.el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
  .fillcontain{
      height: 100%;
  }
</style>
