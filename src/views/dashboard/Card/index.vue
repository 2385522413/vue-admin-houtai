<template>
  <div>
    <el-row :gutter="10">
      <el-col :span="6">
        <el-card>
          <Detail title="总销售额" count="¥ 126560">
            <template slot="charts">
              <span>周同比&nbsp;&nbsp;56.67%
                <i class="el-icon-caret-bottom"></i>
              </span>
              &nbsp;&nbsp;
              <span>日同比&nbsp;19.96%
                <i class="el-icon-caret-top"></i>
              </span>
            </template>
            <template slot="footer">
              <span>日销售额￥ 12423</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="总销售额" count="¥ 126560">
            <template slot="charts">
              <lineCharts></lineCharts>
            </template>
            <template slot="footer">
              <span>日访问量 1234</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="总销售额" count="¥ 126560">
            <template slot="charts">
              <barCharts></barCharts>
            </template>
            <template slot="footer">
              <span>转换率64%</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="总销售额" count="¥ 126560">
            <template slot="charts">
              <progressCharts></progressCharts>
            </template>
            <template slot="footer">
               <span>周同比&nbsp;&nbsp;12%
                <i class="el-icon-caret-bottom"></i>
              </span>
              &nbsp;&nbsp;
              <span>日同比&nbsp;11%
                <i class="el-icon-caret-top"></i>
              </span>
            </template>
          </Detail>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  import Detail from "./Detail/index";
  import lineCharts from './lineChart'
  import barCharts from './barCharts'
  import progressCharts from './progressCharts'
  export default {
    name: "Card",
    components: {
      Detail,
      lineCharts,
      barCharts,
      progressCharts
    }
  };
</script>

<style scoped>

</style>
