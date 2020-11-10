# antd 库

## 常用控件

- Pagination 分页
    1. showTotal：boolean  用于显示数据总量和当前数据顺序
    2. showQuickJumper：boolean  是否可以快速跳转至某页
    3. showSizeChanger: boolean  是否可以改变 pageSize
    4. current:number   当前页数
    5. pageSizeOptions:string[]  指定每页可以显示多少条数据
    6. onChange：func(page,pageSize)  页码改变的回调，参数是改变后的页码及每页条数  