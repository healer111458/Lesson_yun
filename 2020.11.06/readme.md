# 2020.11.06 学习记录

## antd-design

### Row & Button
    1. <Row> 栅格:以24等分来划分‘盒子’,每个栅格至少一个<Col span={24}> 
        eg: 
        <Row>
            <Col span={12}>Col</Col>
            <Col span={12}>Col</Col>
        </Row>

    2. <Button> 按钮属性: 
            type='primary',     //按钮类型：primary、ghost、default、link
            block='true',       //将按钮宽度调整为其父宽度的选项
            ghost='true',       //幽灵按钮(可通过type设置)
            disabled='true'     //按钮失效
            danger='true'       //危险按钮

    3. <Dropdown.Button> 带下拉框的按钮(部分属性与Button一致)
            overlay={menu}             //下拉框中的选项
            icon={<UserOutlined />}    //设置左侧按钮图标样式(menu中也可设置右侧样式)
            placement={topCenter}      //菜单弹出位置
            trigger='hover'            //设置拉下按钮的触发行为，默认:hover

### React 高阶组件

    1. withRouter：作用是将一个组件包裹进Route里面, 然后react-router的三个对象history, location, match就会自动放进这个组件的props属性中. 所以，如果我们某个东西不是一个Router, 但是我们要依靠它去跳转一个页面, 比如点击页面的logo, 返回首页, 这时候就可以使用withRouter来做.
