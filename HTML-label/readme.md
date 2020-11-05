# 2020.11.05

## 表单验证 rules

### 通过 rules 属性添加验证规则

    eg: 
        <form 
            rules={[
                {
                  required: true,
                  message: '请输入你的名字！',
                },
                {
                    ...
                }
            ]}
        >
        </form>