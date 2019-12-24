<template>
    <div style="width: 940px;margin: auto">
        <el-row>
            <el-row>
                <h1 style="text-align: left">豆瓣电影排行榜</h1>
                <div style="float: left;margin-top:-30px;color:#072;">
                    <h3>豆瓣新片榜· · · · · ·</h3>
                </div>
            </el-row>
            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[0].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[0].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[0].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                            disabled v-model="movie[0].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">9.1</a> &nbsp; <a style=" color: #666;">(61135人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[1].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[1].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[1].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[1].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">8.8</a>  &nbsp;<a style=" color: #666;">(392521人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[2].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[2].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[2].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[2].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">8.7</a> &nbsp; <a style=" color: #666;">(64380人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[3].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[3].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[3].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[3].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">7.3</a>  &nbsp;<a style=" color: #666;">(81284人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[4].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[4].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[4].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[4].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">8.8</a>  &nbsp;<a style=" color: #666;">(41001人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[5].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[5].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[5].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[5].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">6.7</a>  &nbsp;<a style=" color: #666;">(29531人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[6].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[6].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[6].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[6].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">8.6</a>  &nbsp;<a style=" color: #666;">(8862人评价)</a></div>
                </el-col>
            </el-row>

            <hr style="border: 1px dashed;color: lightgray "/>
            <el-row v-for="movie in movieList" type="flex" justify="left"
                    style="margin-top: 10px;">
                <el-col :span="4">
                    <img v-bind:src="movie[7].imgUrl"style="width: 105px;height: 145px;margin-right: 30px">
                </el-col>
                <el-col :span="10" style="width:760px;text-align: left;margin-top: 13px;">
                    <a href="#" style="text-decoration: none">{{movie[7].name}}</a>
                    <p style="width:760px;font-size:14px;margin-top: 17px;color:#666">
                        {{movie[7].actor}}
                    </p>
                    <el-rate style="margin-top:18px"
                             disabled v-model="movie[7].score">
                    </el-rate>
                    <div style="margin-top: -20px;margin-left: 120px;font-size: 14px;"><a style="color: #ffad2f">7.5</a>  &nbsp;<a style=" color: #666;">(18354人评价)</a></div>
                </el-col>
            </el-row>
        </el-row>
    </div>
</template>

<script>
    export default{
        data:function(){
            return{
                movieList:[
                    [
                        {
                            name:'爱尔兰人 / 爱尔兰杀手(港) / 听说你刷房子了',
                            score:4.5,
                            imgUrl:require('../assets/6.jpg'),
                            actor:"2019-09-27(纽约电影节) / 2019-11-01(美国点映) / 2019-11-27(美国网络) / 罗伯特·德尼罗 / 阿尔·帕西诺 / 乔·佩西 / 安娜·帕奎因 / " +
                                "杰西·普莱蒙 / 哈威·凯特尔 / 斯蒂芬·格拉汉姆 / 鲍比·坎纳瓦尔 / 杰克·休斯顿 / 阿莱卡萨·帕拉迪诺 / 凯瑟琳·纳杜奇..."
                        },
                        {
                            name:'小丑 / 小丑起源电影：罗密欧 / Romeo',
                            score:4.5,
                            imgUrl:require('../assets/1.jpg'),
                            actor:"2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 " +
                                "/ 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普..."
                        },
                        {
                            name:'82年生的金智英 / 82年生金智英 / Kim Ji-young,Born 1982',
                            score:4.5,
                            imgUrl:require('../assets/12.jpg'),
                            actor:"2019-10-23(韩国) / 2019-11-07(中国香港) / 郑有美 / 孔侑 / 金美京 / 孔敏晶 / 朴成妍 / 李凤莲 / 金圣喆 / 李乌 / 李海云 / 孙成灿 / 金正英 / 李娜云 " +
                                "/ 禹志贤 / 韩国 / 金度英 / 118分钟 / 82年生的金智英 / 剧情 / 刘英雅 Yeong-ah Yoo / 赵南珠 Nam-joo..."
                        },
                        {
                            name:'好莱坞往事 / 从前，有个荷里活(港) / 从前，有个好莱坞...(台)',
                            score:3.5,
                            imgUrl:require('../assets/2.jpg'),
                            actor:"2019-05-21(戛纳电影节) / 2019-07-26(美国) / 2019(中国大陆) / 莱昂纳多·迪卡普里奥 / 布拉德·皮特 / 玛格特·罗比 / 埃米尔·赫斯基 / 玛格丽特·库里 " +
                                "/ 蒂莫西·奥利芬特 / 茱莉亚·巴特斯 / 奥斯汀·巴特勒 / 达科塔·范宁 / 布鲁斯·邓恩 /..."
                        },
                        {
                            name:'婚姻故事',
                            score:4.5,
                            imgUrl:require('../assets/13.jpg'),
                            actor:"2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 " +
                                "/ 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普..."
                        },
                        {
                            name:'准备好了没/弑婚游戏(台)/爆血新婚夜(港)',
                            score:3.5,
                            imgUrl:require('../assets/8.jpg'),
                            actor:"2019-08-21(美国) / 萨玛拉·维文 / 安迪·麦克道威尔 / 马克·奥布莱恩 / 亚当·布罗迪 / 亨利·科泽尼 / 妮基·瓜达尼 / 梅兰妮·斯科洛凡诺 / " +
                                "克里斯蒂安·布鲁恩 / 伊利斯 莱韦斯克 / 约翰·拉尔斯顿 / 达妮埃拉·巴博萨 / 伊拉娜·盖尔 /..."
                        },
                        {
                            name:'克劳斯：圣诞节的秘密 / 圣诞老人',
                            score:4.5,
                            imgUrl:require('../assets/11.jpg'),
                            actor:"2019-11-08(西班牙) / 2019-11-08(英国) / J·K·西蒙斯 / 詹森·舒瓦兹曼 / 拉什达·琼斯 / 琼·库萨克 / 诺曼·麦克唐纳徳 / 威尔·萨索 / " +
                                "塞尔希奥·巴勃罗斯 / 米拉·布雷纳 / 内达·玛格丽特·拉巴 / 悉尼·布朗 / 泰迪·布鲁姆 / 艾玛·香农 / 肯德尔·卓依..."
                        },
                        {
                            name:'第一滴血5：最后的血 / 第一滴血：终极血战(港) / 蓝波：最后一滴血(台)',
                            score:4,
                            imgUrl:require('../assets/14.jpg'),
                            actor:"2019-09-18(印度尼西亚) / 2019-09-20(美国) / 2019-09-27(西班牙) / 西尔维斯特·史泰龙 / 帕斯·贝加 / 塞尔吉奥·佩里斯-门切塔 /" +
                                " 艾德里安娜·巴拉扎 / 维特·蒙雷尔 / 吉妮·金 / 华金·科西奥 / 帕斯卡西奥·洛佩斯 / 奥斯卡·贾恩那达 / 亚历山大·迪米特罗夫..."
                        },
                    ]
                ]
            }
        }

    }
</script>
