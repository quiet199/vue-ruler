<template>
    <div>
                <Cruler @post-NumValue="rulerNum" 
                    @scroll-start='startEvent' 
                    @scroll-end="endEvent" 
                    :NowNum='100' 
                    :maxNum='200' 
                    :minNum='-30' 
                    :ruleWidth='40' 
                    :numSize='50'></Cruler>
    </div>
</template>

<script>
    import Cruler from '@/components/Cruler.vue'
    export default{
        name:'CsRuler',
        components: {
            Cruler
        },
        data() {
            return {
                NumValue: '',
                color: 'red'
            }
        },
        methods: {
            //子组件传递刻度表
            rulerNum(vul){
                this.NumValue = vul
                // console.log(vul)
            },
            endEvent(val){
                // console.log(val)
            },
            startEvent(val){
                // console.log(val)
            }
        },
    }
</script>