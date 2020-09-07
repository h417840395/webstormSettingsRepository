<template>
<div style="height: 100vh" class="vertical">
#[[$END$]]#
</div>
</template>

<script>
export default {
name: "${COMPONENT_NAME}",
data() {
            return {};
        },
                // 使用 DOM 中的模板时，camelCase的 prop 名需要使用其等价的 kebab-case命名
        props: {
            // val: {
            //     type: Number,
            //     default: 0,
            //     required: true,
            //     validator: function (val) {
            //         return val >= 0
            //     }
            // }
        },
        methods: {
        },
        computed:{},
        watch:{},
        beforeCreate() {
            // beforecreate : 可以在这加个loading事件，在加载实例时触发
        },
        created() {
            // created : 初始化完成时的事件写在这里，如在这结束loading事件，异步请求也适宜在这里调用
        },
        mounted() {
            // mounted : 挂载元素，获取到DOM节点
        },
        updated() {
            // updated : 如果对数据统一处理，在这里写上相应函数
        },
        beforeDestroy() {
            // beforeDestroy : 可以做一个确认停止事件的确认框
        }
}
</script>

<style lang="stylus" scoped>
    @import '~assets/main.styl'
    .vertical {
        flex-y()
    }

    .horizontal {
        flex-x()
    }
    
        .divider {
        background-color transparent
        width 100%
        height 1px
    }
    .space {
        background-color transparent
        width 100%
        height vw(10)
    }
</style>