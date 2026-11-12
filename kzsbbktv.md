代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://mwy.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://uax.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://qws.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://xuo.fengsongda.top

[U75] PHP：依赖注入
来源：http://pkr.zhiwuduotai.top

composer require psr/container
来源：http://lis.zhoulong.xyz

[U76] PHP：简单路由
来源：http://mpc.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ppt.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://mmb.haohaochexian.top

composer require twig/twig
来源：http://egv.nwbrower.top

[U78] PHP：单元测试
来源：http://imf.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://ofp.zdqjudy.top

[U79] PHP：静态分析
来源：http://oqk.cashguo.top

composer require --dev phpstan/phpstan
来源：http://uhq.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://lpo.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://umc.zhongyouzk.top

[U81] JS：初始化项目
来源：http://mmo.sjlbkw.cn

npm init -y;  npm i express
来源：http://ggw.fktsv.cn

[U82] JS：package.json 脚本
来源：http://idc.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pec.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://fhn.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://isj.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://ezd.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qhu.xziqi.cn

[U85] JS：可选链
来源：http://eal.xingfuxueyuan.xyz

a?.b?.c
来源：http://loc.svipenyu.cn

[U86] JS：空值合并
来源：http://qoz.dianchejie.cn

a ?? b
来源：http://fae.hywenlv.cn

[U87] JS：解构默认值
来源：http://pht.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://gmp.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://lyu.cdnleiting.top

{ ...a, ...b }
来源：http://ikh.fktsv.cn

[U89] JS：数组去重
来源：http://xee.wangshuangyany.cn

[...new Set(arr)]
来源：http://zej.havefunace.top

[U90] JS：数字数组排序
来源：http://tmo.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://yna.fehbvm.com

[U91] JS：对象键值遍历
来源：http://fhw.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://knl.hesvh.cn

[U92] JS：深拷贝
来源：http://ogm.havefunace.top

structuredClone(obj)
来源：http://spi.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://wgl.hesvh.cn

`共 ${n} 条`
来源：http://gsa.ydjk.org.cn

[U94] JS：箭头函数
来源：http://kji.hcnkem.com

const double = x => x * 2;
来源：http://izr.cashguo.top

[U95] JS：Promise 包装
来源：http://nld.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://qww.wangdashe.top

[U96] JS：async/await 与异常
来源：http://nkk.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pxj.fehbvm.com

[U97] JS：并发请求
来源：http://yme.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ylr.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://zbs.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://njo.52xcode.cn

[U99] JS：事件监听
来源：http://pqv.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://cmv.ybcxt.top

[U100] JS：DOM 查询
来源：http://bvt.jqgufenzy.top

document.querySelector(".item")
来源：http://asi.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://gvu.zhoulong.xyz

el.classList.toggle("active")
来源：http://kuh.bbcook.cn

[U102] JS：本地存储
来源：http://mou.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tkf.ydjk.org.cn

[U103] JS：定时器
来源：http://ltm.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://emz.ivvv.top

[U104] JS：防抖
来源：http://jez.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ilt.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://wvm.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xuu.yvedp.cn

[U106] JS：日期格式化
来源：http://hfb.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fno.yongpay.top

[U107] JS：数字千分位
来源：http://lqw.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iwt.sweek.top

[U108] JS：随机整数
来源：http://gkt.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zgp.xinyue.icu

[U109] JS：数组分组
来源：http://fcn.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://dfk.hnxiangtu.top

[U110] JS：数组分块
来源：http://zpw.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://axi.wangdashe.top

[U111] JS：对象转 Map
来源：http://ihv.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://yml.jiagoushi.top

[U112] JS：字符串补位
来源：http://vby.mhx1999.top

"7".padStart(3, "0")
来源：http://vwx.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://bzn.meibo888.top

s.replaceAll("a", "b")
来源：http://roq.smart0.xyz

[U114] JS：JSON 深比较
来源：http://xbn.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xbz.epnwcf.com

[U115] JS：生成 UUID
来源：http://eej.hysaishi.cn

crypto.randomUUID()
来源：http://jhs.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://ojq.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://ufd.tarul.cn

[U117] JS：单元测试
来源：http://uyw.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://rxk.zhijiandao.cn

[U118] JS：开发服务器
来源：http://jxo.sysykeji.top

npm i -D vite;  npx vite
来源：http://jdb.epnwcf.com

[U119] JS：生产构建
来源：http://kcc.cheryme.top

npx vite build
来源：http://apd.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://yao.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://pwe.yuanzhike.top

================================================================================
来源：http://mes.kuanghao11.cn

统计汇总
来源：http://byh.kuanghao11.cn

================================================================================
来源：http://ydk.fengsongda.top

按语言统计（条）：
来源：http://zmd.yuxming.cn

Python ......... 252
来源：http://tde.316326.xyz

PHP ............ 252
来源：http://xrs.zhengqikj.top

JavaScript ..... 252
来源：http://jox.zhixingplan.top

TypeScript ..... 212
来源：http://get.quarkkingdee.top

Java ........... 212
来源：http://oiv.mhx1999.top

Go ............. 212
来源：http://hsj.jqgufenzy.top

Ruby ........... 212
来源：http://zsk.shangyingyoupin.top

C# ............. 212
来源：http://aej.shzxlz.cn

C .............. 30
来源：http://eba.zhengqikj.top

C++ ............ 30
来源：http://awa.yj202588.top

SQL ............ 90
来源：http://leq.bbcook.cn

Bash ........... 80
来源：http://exj.zhijiandao.cn

Kotlin ......... 15
来源：http://ugb.svipenyu.cn

Swift .......... 15
来源：http://pwl.shuidangran.top

Lua ............ 10
来源：http://crc.nwbrower.top

Perl ........... 10
来源：http://iig.xinyue.icu

Scala .......... 10
来源：http://rbm.zhaomingkeji.xyz

------------------------------------
来源：http://liz.yuxming.cn

合计 ........... 2106 条
来源：http://lvr.hnqzz.top

按章节统计：
来源：http://kpy.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hbv.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gpb.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bnt.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lnd.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qcb.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://isf.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://day.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://etc.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vyd.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eup.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hxp.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://apz.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aaj.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zqp.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fes.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kdw.hammf.cn

Q SQL 专题                              90
来源：http://iyn.vqdsnc.cn

R Bash 专题                             80
来源：http://pxw.zdqjudy.top

S C / C++ 专题                          60
来源：http://yxh.sweek.top

T 其他语言补充                          60
来源：http://riu.xziqi.cn

U 高频实用片段                         120
来源：http://wqm.hywenlv.cn

------------------------------------
来源：http://kbc.yuanzhike.top

合计                                  2106 条
来源：http://xkh.jianghu66.top

--------------------------------------------------------------------------------
来源：http://whb.yj20258.top

使用提醒
来源：http://wcb.fktsv.cn

--------------------------------------------------------------------------------
来源：http://syh.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dwy.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pow.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bph.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wlo.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qap.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://grh.jqgufenzy.top

================================================================================
来源：http://zih.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://tfr.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://mzi.cdnleiting.top

================================================================================
来源：http://xdx.vehdjk.com

【收录内容】
来源：http://xht.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nhr.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rsv.vehdjk.com

SQL · Bash · C · C++
来源：http://bus.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://njv.ydjk.org.cn

【使用说明】
来源：http://btw.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lxw.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wvn.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fzi.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aot.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://gde.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ofw.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lqf.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eef.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pxg.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bxr.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ird.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hvp.hesvh.cn

【文件统计】
来源：http://fjk.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zhy.fengsongda.top

--------------------------------------------------------------------------------
来源：http://tit.snrcjt.cn

目  录
来源：http://uvk.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://jvy.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ctc.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cjv.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nwv.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://owr.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cej.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wsn.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fzv.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ksd.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://asv.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cth.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vix.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yku.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dtm.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tbv.zycfv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kfc.uphjek.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://owu.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ody.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mjl.zhiwuduotai.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yza.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eps.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://utf.xuetiantiany.cn

================================================================================
来源：http://iok.gzhubu.top

A. 基础语法与类型
来源：http://cdz.vehdjk.com

================================================================================
来源：http://jyd.xuanzx.com

[A01] Hello World
来源：http://htj.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://lzz.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://pup.ywan-chungtsiang.top

JS:   console.log("Hello, World!");
来源：http://rnu.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xmv.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://vwy.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://oyz.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://fax.hfpthk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://koz.zycfv.cn

[A02] 变量声明与赋值
来源：http://ius.zhijiandao.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nha.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cmg.chenjidiqi.icu

JS:   let name = "Alex"; const age = 20;
来源：http://jsz.gaohongyu789.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ucp.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://jnk.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://oni.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://ufp.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://qqn.pycfn.com

[A03] 常量定义
来源：http://dhn.316326.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wht.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://qly.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://ecf.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://cuk.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://iyv.nwbrower.top

Go:   const PI = 3.14159
来源：http://cmj.yueranfly.top

Ruby: PI = 3.14159
来源：http://dhr.cashguo.top

C#:   const double PI = 3.14159;
来源：http://kko.gzhubu.top

[A04] 判断变量类型
来源：http://nqs.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ctm.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nxp.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dhr.yuanzhike.top

TS:   typeof x; x instanceof Date
来源：http://cpc.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xjc.guannengcc.top

Go:   reflect.TypeOf(x).Name()
来源：http://gjw.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://dar.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://poy.vqdsnc.cn

[A05] 整数除法与取模
来源：http://pvu.9152youxi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ayi.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://scf.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ljj.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://egf.ppjwa.cn

Java: 7 / 2; 7 % 2
来源：http://sux.jinghuilouyu.cn

Go:   7 / 2; 7 % 2
来源：http://yyy.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://ioe.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://hms.redwolf501.top

[A06] 字符串转数字
来源：http://nqz.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://eee.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sbn.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xbo.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://snn.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://myn.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pyt.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://emh.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oci.chenjidiqi.icu

[A07] 数字转字符串
来源：http://ovx.xylfe.cn

Py:   str(42)
来源：http://yfl.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://pfd.pycfn.com

JS:   String(42); (42).toString()
来源：http://dwm.ydjk.org.cn

TS:   String(42)
来源：http://akf.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bpp.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://fph.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://pjm.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://ntx.xinyue.icu

[A08] 取整与四舍五入
来源：http://ncz.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pcj.yanxiufei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ita.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hay.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xzj.sysykeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qnt.pycfn.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fjf.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yxr.jyoumei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gns.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://vix.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://udf.sweek.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kam.ybcxt.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ltr.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dom.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cxd.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://njl.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jtf.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dxu.xylfe.cn

[A10] 生成随机数
来源：http://ymw.52xcode.cn

Py:   import random; random.randint(1, 100)
来源：http://iig.jianghu66.top

PHP:  random_int(1, 100);
来源：http://kst.hysaishi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eux.chenjidiqi.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rdd.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://gfy.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yez.fengsongda.top

Ruby: rand(1..100)
来源：http://zuv.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://pun.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://dfb.havefunace.top

Py:   "yes" if x > 0 else "no"
来源：http://mtm.fanxiaobao.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://kcf.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://ugk.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://egb.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://agc.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vad.hysaishi.cn


<!-- 参考信息 -->