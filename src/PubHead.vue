<template>
    <div>
       <h1>{{ msg }}</h1>
           <Header>
            <Menu mode="horizontal" theme="dark" active-name="1">
                <div class="layout-logo"></div>
                <div class="layout-nav">
                    <MenuItem name="1">
                        <Icon type="ios-navigate"></Icon>
                        首页
                    </MenuItem>
                    <MenuItem name="2">
                        <Icon type="ios-keypad"></Icon>
                        文字识别
                    </MenuItem>
                    <MenuItem name="3">
                        <Icon type="ios-analytics"></Icon>
                        自动阅读
                    </MenuItem>
                    <MenuItem name="4">
                        <Icon type="ios-paper"></Icon>
                        词典
                    </MenuItem>
                </div>
            </Menu>
        </Header>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                msg:'my-head'
            }
        },
        mounted(){

        },
        beforeDestory(){

        },
        methods:{
            
        }
    }
</script>