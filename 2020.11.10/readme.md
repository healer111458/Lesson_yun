# react 学习

## table 表格

### 属性

- column 列
    1. dataIndex  列数据在数据项中对应的路径，支持通过数组查询嵌套路径
    2. key        React 需要的 key，如果已经设置了唯一的 dataIndex，可以忽略这个属性
    3. ellipsis   超过宽度将自动省略
    4. align      对齐方式

- dataSource 数据
    - key        必须指定，并对应column 的 key

- select 选择框
    1. bordered   边框，默认有边框
    2. options    数据化配置选项内容，相比 jsx 定义会获得更好的渲染性能
    3. size       选择框大小默认：middle
    4. value      选中条目的值
    5. allowClear 是否清除，默认：false
    6. disabled   是否禁用 默认：false

## 新知识

- href='javascript:void(0)'  
    不跳转页面，但路由刷新，并加载新组件

- tostring(2)
    for (let i = 1; i < 500; i++) {
            children.push({i.toString(2)});
    }
    * 以二进制循环 push children[i],默认tostring为十进制

- &gt 转义字符 >

- Route 标签
    <Route exact path={`/html/a/view`} component={CompanyList} />
    * exact 路由严格匹配，根据path提供的路径进行严格匹配 html/a/view,如果路由为 a/view 流浪其将会报错
