<style scoped>
.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
}
.layout-logo{
    width: 100px;
    height: 30px;
    background: #5b6270;
    border-radius: 3px;
    float: left;
    position: relative;
    top: 15px;
    left: 20px;
}
.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}
.layout-footer-center{
    text-align: center;
}
</style>
<template>
    <div class="layout">
        <Layout>
        	<pub-head></pub-head>
            <Content :style="{padding: '0 50px'}">
                <Breadcrumb :style="{margin: '20px 0'}">
                    <BreadcrumbItem>Home</BreadcrumbItem>
                    <BreadcrumbItem>Components</BreadcrumbItem>
                    <BreadcrumbItem>Layout</BreadcrumbItem>
                </Breadcrumb>
                <Card>
                    <div style="min-height: 200px;">
                        <Upload action="//127.0.0.1/edu/upload_file.php">
                            <Button type="ghost" icon="ios-cloud-upload-outline">上传图片</Button>
                        </Upload>
                        <div>
                        	<ul>
                        		<li v-for="item in items">
                        			<p v-text="item.label"></p>
                        		</li>
                        	</ul>
                        </div>
                    </div>
                </Card>
            </Content>
            <Footer class="layout-footer-center">2011-2018 &copy; 学习小助手</Footer>
        </Layout>
    </div>
</template>
<script>
import PubHead from "./PubHead.vue";
    export default {
        data () {
            return {
            	items:[
            		{
            			label:'history-001'
            		},
            		{
            			label:'history-002'
            		}
            	]
            }
        },
        mounted () {

        },
        beforeDestroy () {

        },
        methods: {

        },
        components:{
        	PubHead
        }
    }
</script>
