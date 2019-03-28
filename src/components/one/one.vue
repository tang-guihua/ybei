<template>
    <div class="one">
        <div class="one-top">
            <news></news>
        </div>
        <div class="wrapper">
            <div class="wrapper-one">
                <span class="main-word">改善空气质量</span>
                <div class="include-arrow">
                    <span class="main-word">提高呼吸安全的产品</span>
                    <arrow></arrow>
                </div>
            </div>
            <div class="wrapper-two">
                <logo></logo>
                <span class="company-name">上海蕴贝实业有限公司</span>
                <img src="../../../static/one-img/cloud.jpg" class="bgimg"/>
                <div class="include-arrow">
                    <span class="induct">关于我们</span>
                    <arrow></arrow>
                </div>
                <p class="mainword">{{mainWord[0]}}</p>
                <p class="mainword">{{mainWord[1]}}</p>
                <p class="mainword">{{mainWord[2]}}</p>
                <p class="mainword">{{mainWord[3]}}</p>
            </div>
        </div>
    </div>
</template>

<script type="text/ecmascript-6">
import news from 'common/svg/news'
import arrow from 'common/svg/arrow'
import logo from 'common/svg/logo'

export default {
    props: {

    },
    data() {
        return {
            mainWord: ["上海蕴贝实业有限公司成立于2011年，公司致力于改善空气质量、提高呼吸安全的产品生产，产品广泛用于医疗器械、吸尘器、空气清新机、中央空调及吸尘系统、工业生产等领域。","公司从成立开始即将产品定位于中高端市场，与3M、HV、Donaldson 等著名公司战略合作，采用国际先进材料，共同开发、生产高质量的产品，产品出口北美、欧洲等市场 。","公司一贯坚持质量第一的原则，通过莱茵TUV ISO9001：2008质量管理体系认证，并始终严格执行体系要求，不断强化内部管理，确保产品质量稳定、可靠。","对于员工，公司始终提倡和谐、轻松的工作环境，鼓励员工主动、创新，为每个员工提供良好的职业规划和社会保障。"]
        };
    },
    computed: {

    },
    created() {

    },
    mounted() {

    },
    watch: {

    },
    methods: {

    },
    components: {
        arrow,
        news,
        logo
    },
};
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
    @import "~common/styles/variable"
	@import "~common/styles/mixin"
    
    .one
        position: relative
        overflow-y: scroll
        height: 100vh
        .one-top
            position: absolute
            top: 0
            right: 0
        .wrapper
            padding-top: 100px
            .wrapper-one
                margin: 100px 0 0 35px
                .main-word
                    font-size: $f-main-sub
                    color: $c-bg-heavy
                    line-height: 3rem
            .wrapper-two
                margin-left: 35px
                height: auto
                .logo
                    display: block
                    padding-top: 40px
                .company-name
                    font-size: $f-text
                    color: $c-bg-heavy
                    line-height: 2rem
                    margin-bottom: 5px
                .bgimg
                    // height: 600px
                    width: calc(100% - 35px)
                .induct
                    display: block
                    font-size: $f-text
                    color: $c-bg-heavy
                    line-height: 2rem
                    margin-top: 5px
                .mainword
                    font-size: $f-link
                    color: $c-bg-heavy
                    width: calc(100% - 35px)
                    line-height: 1.2rem
                    margin-top: 8px
</style>
