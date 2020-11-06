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

### React 
- React 特点
    1.声明式设计 −React采用声明范式，可以轻松描述应用。

    2.高效 −React通过对DOM的模拟，最大限度地减少与DOM的交互。

    3.灵活 −React可以与已知的库或框架很好地配合。

    4.JSX − JSX 是 JavaScript 语法的扩展。React 开发不一定使用 JSX ，但我们建议使用它。

    5.组件 − 通过 React 构建组件，使得代码更加容易得到复用，能够很好的应用在大项目的开发中。

    6.单向响应的数据流 − React 实现了单向响应的数据流，从而减少了重复代码，这也是它为什么比传统数据绑定更简单。

- 高阶组件
    - 高阶组件是参数为组件，返回值为新组件的函数。

    1. withRouter：作用是将一个组件包裹进Route里面, 然后react-router的三个对象history, location, match就会自动放进这个组件的props属性中. 所以，如果我们某个东西不是一个Router, 但是我们要依靠它去跳转一个页面, 比如点击页面的logo, 返回首页, 这时候就可以使用withRouter来做.

    *connect: 是一个返回高阶组件的高阶函数.

- 基础语法
    - history:
        React Router 是建立在 history 之上的。 简而言之，一个 history 知道如何去监听浏览器地址栏的变化， 并解析这个 URL 转化为 location 对象， 然后 router 使用它匹配到路由，最后正确地渲染对应的组件。
    
    - 

- 组件命名
    组件名与文件名需要区分，组件名需要以大写字母开头，即大驼峰命名法 eg：LessonHealer