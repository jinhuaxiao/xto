XTO
===

Just an API for Node.js to query each express.

Because many Chinese express companies are called [*]to (eg: sto, zto, gto, etc.), I call this project XTO.

ESSENCE
-------

It just simply call the 'SEEM-PRIVATE' API of [kuaidi100](http://www.kuaidi100.com/).

INSTALLATION
------------

    $ npm install xto

USAGE
-----

The code below is base usage:

    var xto = require("xto");
    xto.query(NUMBER, COMPANY_NAME, function(status, msg, json) {
        //... Do something
    });

You can even get a company's information:

    var info = xto.getCompanyInfo(COMPANY_NAME);

And you have to know the `state` field in the json by using:

    var text = xto.stateToText(json["state"]);

CONTACT ME
----------

If you want contribute to this project, you can fork it!

And if you have some question, you can post it to ISSUES or contact me:

  + Email: admin#xcoder.in
  + Website: http://xcoder.in

COMPANIES SUPPORTED
-------------------

You can use one company's name, shortname and english code to query. Here's a list for the companies:

  + 申通快递(申通, shentong)
  + EMS(EMS, ems)
  + 顺丰速运(顺丰, shunfeng)
  + 韵达快递(韵达, yunda)
  + 圆通速递(圆通, yuantong)
  + 中通速递(中通, zhongtong)
  + 汇通快运(汇通, huitongkuaidi)
  + 天天快递(天天, tiantian)
  + 宅急送(宅急送, zhaijisong)
  + 鑫飞鸿(鑫飞鸿, xinhongyukuaidi)
  + CCES/国通快递(CCES, cces)
  + 全一快递(全一, quanyikuaidi)
  + 彪记快递(彪记, biaojikuaidi)
  + 星晨急便(星晨急便, xingchengjibian)
  + 亚风速递(亚风, yafengsudi)
  + 源伟丰(源伟丰, yuanweifeng)
  + 全日通(全日通, quanritongkuaidi)
  + 安信达(安信达, anxindakuaixi)
  + 民航快递(民航, minghangkuaidi)
  + 凤凰快递(凤凰, fenghuangkuaidi)
  + 京广速递(京广, jinguangsudikuaijian)
  + 配思货运(配思, peisihuoyunkuaidi)
  + 中铁物流(中铁, ztky)
  + UPS(UPS, ups)
  + FedEx-国际件(FedEx, fedex)
  + TNT(TNT, tnt)
  + DHL-中国件(DHL, dhl)
  + AAE-中国件(AAE, aae)
  + 大田物流(大田, datianwuliu)
  + 德邦物流(德邦, debangwuliu)
  + 新邦物流(新邦, xinbangwuliu)
  + 龙邦速递(龙邦, longbanwuliu)
  + 一邦速递(一邦, yibangwuliu)
  + 速尔快递(速尔, suer)
  + 联昊通(联昊通, lianhaowuliu)
  + 广东邮政(广东邮政, guangdongyouzhengwuliu)
  + 中邮物流(中邮, zhongyouwuliu)
  + 天地华宇(华宇, tiandihuayu)
  + 盛辉物流(盛辉, shenghuiwuliu)
  + 长宇物流(长宇, changyuwuliu)
  + 飞康达(飞康达, feikangda)
  + 元智捷诚(元智捷诚, yuanzhijiecheng)
  + 包裹/平邮(邮政国内, youzhengguonei)
  + 国际包裹(邮政国际, youzhengguoji)
  + 万家物流(万家, wanjiawuliu)
  + 远成物流(远成, yuanchengwuliu)
  + 信丰物流(信丰, xinfengwuliu)
  + 文捷航空(文捷, wenjiesudi)
  + 全晨快递(全晨, quanchenkuaidi)
  + 佳怡物流(佳怡, jiayiwuliu)
  + 优速物流(优速, youshuwuliu)
  + 快捷速递(快捷, kuaijiesudi)
  + D速快递(D速, dsukuaidi)
  + 全际通(全际通, quanjitong)
  + 能达速递(能达, ganzhongnengda)
  + 青岛安捷快递(安捷, anjiekuaidi)
  + 越丰物流(越丰, yuefengwuliu)
  + DPEX(DPEX, dpex)
  + 急先达(急先达, jixianda)
  + 百福东方(百福东方, baifudongfang)
  + BHT(BHT, bht)
  + 伍圆速递(伍圆, wuyuansudi)
  + 蓝镖快递(蓝镖, lanbiaokuaidi)
  + COE(COE, coe)
  + 南京100(南京100, nanjing)
  + 恒路物流(恒路, hengluwuliu)
  + 金大物流(金大, jindawuliu)
  + 华夏龙(华夏龙, huaxialongwuliu)
  + 运通中港(运通, yuntongkuaidi)
  + 佳吉快运(佳吉, jiajiwuliu)
  + 盛丰物流(盛丰, shengfengwuliu)
  + 源安达(源安达, yuananda)
  + 加运美(加运美, jiayunmeiwuliu)
  + 万象物流(万象, wanxiangwuliu)
  + 宏品物流(宏品, hongpinwuliu)
  + GLS(GLS, gls)
  + 上大物流(上大, shangda)
  + 中铁快运(中铁, zhongtiewuliu)
  + 原飞航(原飞航, yuanfeihangwuliu)
  + 海外环球(海外环球, haiwaihuanqiu)
  + 三态速递(三态, santaisudi)
  + 晋越快递(晋越, jinyuekuaidi)
  + 联邦快递(联邦, lianbangkuaidi)
  + 飞快达(飞快达, feikuaida)
  + 全峰快递(全峰, quanfengkuaidi)
  + 如风达(如风达, rufengda)
  + 乐捷递(乐捷递, lejiedi)
  + 忠信达(忠信达, zhongxinda)
  + 芝麻开门(芝麻开门, zhimakaimen)
  + 赛澳递(赛澳递, saiaodi)
  + 海红网送(海红网送, haihongwangsong)
  + 共速达(共速达, gongsuda)
  + 嘉里大通(嘉里大通, jialidatong)
  + OCS(OCS, ocs)
  + USPS(USPS, usps)
  + 美国快递(美国, meiguokuaidi)
  + 立即送(立即送, lijisong)
  + 银捷速递(银捷, yinjiesudi)
  + 门对门(门对门, menduimen)
  + 递四方(递四方, disifang)
  + 郑州建华(郑州建华, zhengzhoujianhua)
  + 河北建华(河北建华, hebeijianhua)
  + 微特派(微特派, weitepai)
  + DHL-德国件(DHL, dhlde)
  + 通和天下(通和天下, tonghetianxia)
  + EMS-国际件(EMS-国际件, emsguoji)
  + FedEx-美国件(FedEx, fedexus)
  + 风行天下(风行天下, fengxingtianxia)
  + 康力物流(康力, kangliwuliu)
  + 跨越速递(跨越, kuayue)
  + 海盟速递(海盟, haimengsudi)
  + 圣安物流(圣安, shenganwuliu)
  + 一统飞鸿(一统飞鸿, yitongfeihong)
  + 中速快递(中速, zhongsukuaidi)
  + 新蛋奥硕(新蛋奥硕, neweggozzo)
  + OnTrac(OnTrac, ontrac)
  + 七天连锁(七天连锁, sevendays)
  + 明亮物流(明亮, mingliangwuliu)
  + 凡客配送(凡客, vancl)
  + 华企快运(华企, huaqikuaiyun)
  + 城市100(城市100, city100)
  + 红马甲物流(红马甲, sxhongmajia)
  + 穗佳物流(穗佳, suijiawuliu)
  + 飞豹快递(飞豹, feibaokuaidi)
  + 传喜物流(传喜, chuanxiwuliu)
  + 捷特快递(捷特, jietekuaidi)
  + 隆浪快递(隆浪, longlangkuaidi)
  + EMS-英文(EMS-英文, emsen)
  + 中天万运(中天万运, zhongtianwanyun)
  + 香港邮政(香港邮政, hkpost)
  + 邦送物流(邦送, bangsongwuliu)
  + 国通快递(国通, guotongkuaidi)
  + 澳大利亚邮政(auspost, auspost)
  + 加拿大邮.政.(加拿大邮.政., canpost)
  + 加拿大邮.政.(加拿大邮.政., canpostfr)
  + UPS-全球件(UPS-全球件, upsen)
  + TNT-全球件(TNT-全球件, tnten)
  + DHL-全球件(DHL, dhlen)
  + 顺丰-美国件(顺丰-美国件, shunfengen)
  + 汇强快递(汇强, huiqiangkuaidi)
  + 希优特(希优特, xiyoutekuaidi)
  + 昊盛物流(昊盛, haoshengwuliu)
  + 尚橙物流(尚橙, shangcheng)
  + 亿领速运(亿领, yilingsuyun)
  + 大洋物流(大洋, dayangwuliu)
  + 递达速运(递达, didasuyun)
  + 易通达(易通达, yitongda)
  + 邮必佳(邮必佳, youbijia)
  + 亿顺航(亿顺航, yishunhang)
  + 飞狐快递(飞狐, feihukuaidi)
  + 潇湘晨报(潇湘晨报, xiaoxiangchenbao)
  + 巴伦支(巴伦支, balunzhi)
  + Aramex(Aramex, aramex)
  + 闽盛快递(闽盛, minshengkuaidi)
  + 佳惠尔(佳惠尔, syjiahuier)
  + 民邦速递(民邦, minbangsudi)
  + 上海快通(上海快通, shanghaikuaitong)
  + 北青小红帽(北青小红帽, xiaohongmao)
  + GSM(GSM, gsm)
  + 安能物流(安能, annengwuliu)
  + KCS(KCS, kcs)
  + City-Link(City-Link, citylink)
  + 店通快递(店通, diantongkuaidi)
  + 凡宇快递(凡宇, fanyukuaidi)
  + 平安达腾飞(平安达腾飞, pingandatengfei)
  + 广东通路(广东通路, guangdongtonglu)
  + 中睿速递(中睿, zhongruisudi)
  + 快达物流(快达, kuaidawuliu)
  + 佳吉快递(佳吉, jiajikuaidi)
  + ADP国际快递(ADP, adp)
  + 颿达国际快递(颿达, fardarww)
  + 颿达国际快递(英文)(颿达国际, fandaguoji)
  + 林道国际快递(林道, shlindao)
  + 中外运速递(中文)(中外运, sinoex)
  + 中外运速递(中外运速递, zhongwaiyun)
  + 深圳德创物流(深圳德创, dechuangwuliu)
  + 林道国际快递(英文)(林道国际快递(英文), ldxpres)
  + 瑞典邮.政.(瑞典邮.政., ruidianyouzheng)
  + Posten AB(Posten AB, postenab)
  + 偌亚奥国际快递(偌亚奥, nuoyaao)
  + 城际速递(城际, chengjisudi)
  + 祥龙运通物流(祥龙运通, xianglongyuntong)
  + 品速心达快递(品速心达, pinsuxinda)
  + 宇鑫物流(宇鑫, yuxinwuliu)
  + 陪行物流(陪行物流, peixingwuliu)
  + 户通物流(户通物流, hutongwuliu)
  + 西安城联速递(西安城联速递, xianchengliansudi)
  + 煜嘉物流(煜嘉物流, yujiawuliu)
  + 一柒国际物流(一柒国际物流, yiqiguojiwuliu)
  + Fedex中文(FedEx, fedexcn)
  + 联邦(联邦, lianbangkuaidien)
  + 中通（带电话）(中通（带电话）, zhongtongphone)
  + 赛澳递for买卖宝(赛澳递for买卖宝, saiaodimmb)
  + 上海无疆for买卖宝(上海无疆for买卖宝, shanghaiwujiangmmb)
  + 新加坡邮政(新加坡邮政, singpost)
  + 比利时邮政(比利时邮政, bpost)
  + 音素快运(音素快运, yinsu)
  + 南方传媒物流(南方传媒物流, ndwl)
  + 速呈宅配(速呈宅配, sucheng)
  + 创一快递(创一快递, chuangyi)
  + 云南滇驿物流(云南滇驿物流, dianyi)
  + 重庆星程快递(重庆星程快递, cqxingcheng)
  + 四川星程快递(四川星程快递, scxingcheng)
  + 贵州星程快递(贵州星程快递, gzxingcheng)
  + 运通中港快递(运通中港快递, ytkd)
  + gati官网英文通道(gati官网英文通道, gatien)
  + gati官网中文通道(gati官网中文通道, gaticn)
  + jcex官网通道(jcex官网通道, jcex)
  + 派尔快递官网通道(派尔快递官网通道, peex)
  + 凯信达官网通道(凯信达官网通道, kxda)
  + 安达信官网通道(安达信官网通道, advancing)
  + 汇文官网通道(汇文官网通道, huiwen)
  + 亿翔官网通道(亿翔官网通道, yxexpress)
  + 东红合作通道(东红合作通道, donghong)
  + 飞远配送(飞远配送, feiyuanvipshop)
  + 深圳EMS(深圳EMS, szems)
  + 好运来(好运来, hlyex)
  + dpex国际(dpex国际, dpexen)

