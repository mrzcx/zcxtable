# zcxtable
<template #topData>顶部插槽</template>
<template #Search>搜索条件插槽</template> 如果使用此插槽，需要传:searchFrom给子组件zTable
<template #upBtn>表格上方按钮插槽</template>
<template #downBtn>表格下方按钮插槽</template>
<template #editView>新增编辑插槽</template>如果使用此插槽，需要传:form="form" :rules="rules"给子组件zTable

// 表格字段配置说明
zTableOption: {
    height: 427, // 表格高度
    rowKey: "", // 表格主键ID，必填
    selectShow: true, // 是否显示选择列
    searchBtn: true, // 是否显示查询功能
    exportBtn: true, // 是否显示导出按钮
    exportFileName: "", // 导出文件名称
    addButton: true, // 是否显示新增按钮
    tableColumn: [
        label: "", // 表头名
        prop: "", // 表头值
        hidden: false, // 是否隐藏列
        custom: false, // 是否自定义
        fixed: "", // 固定列
        width: 250, // 列宽
        operate: true, // 是否成为操作列
        search: true, // 是否成为搜索条件
        searchType: 0, // 0单选选择框，1选择日期范围框,2输入框
        searchSpan: 6, // 搜索条件宽度
        disabled: false, // 是否禁用搜索条件
        format: true, // 是否开启格式化
        formatType: 0, // 格式化类型：0labelValue转化，1时间转化，2千分位转化
        timeType: "", // 时间格式yyyy-MM-dd，yyyy-MM-dd HH:mm:ss
        moneyIcon: "", // 钱币符号
        dicUrl: "", // 获取labelValue的Url
        labelValue: [], // 下拉选值
        colclass: "", // 整列样式名
        edit: false, // 是否新增编辑字段
        editType: 0, // 0单选选择框，1输入框，2富文本
        inputType:"textarea", // editType为1的时候，用此属性变成textarea文本域
        required: true, // 是否必填字段
        editSpan: 24 // 新增编辑字段宽度
    ]
}
