<template>
  <div>
    <el-table
      :data="tableData6"
      :span-method="objectSpanMethod"
      border
      style="width: 75.4%; margin-top: 20px; border:1px solid green; border-color: green"
      
    >
      <el-table-column prop="name" width="60" style="border:1px solid green; border-color: green"></el-table-column>
      <el-table-column label="类别" prop="type" width="50" style="border:1px solid green; border-color: green"></el-table-column>
      <el-table-column label="序号" prop="numberID" width="50"></el-table-column>
      <el-table-column prop="content" label="目标内容" width="200"></el-table-column>
      <el-table-column prop="step" label="方法和措施" width="200"></el-table-column>
      <el-table-column prop="time" label="起止时间" width="105"></el-table-column>
      <el-table-column prop="right" label="完成打“√”" width="90"></el-table-column>
    </el-table>
  </div>
</template>

<script>
export default {
  data () {
    return {
      tableData6: [{
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '事业(工作)目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '财富目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '财富目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '财富目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '财富目标',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '家庭生活',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '家庭生活',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '家庭生活',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }, {
        name: '家庭生活',
        type: '',
        numberID: '1',
        content: '12987122',
        step: '',
        time: '',
        right: ''
      }]
    };
  },
  methods: {

    objectSpanMethod ({ row, column, rowIndex, columnIndex }) {
      if (columnIndex === 0) {
        if (rowIndex === 0) {
          return {
            rowspan: 8,
            colspan: 1
          };
        } else if (rowIndex === 8) {
          return {
            rowspan: 4,
            colspan: 1
          }
        } else if (rowIndex === 12) {
          return {
            rowspan: 4,
            colspan: 1
          }
        } else {
          return {
            rowspan: 0,
            colspan: 0
          };
        }
      }
    }
  }
};
</script>
<style scoped>

</style>