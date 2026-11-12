代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://ijv.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://jia.yongpay.top

[U74] PHP：读取环境变量
来源：http://ojz.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://zoc.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://kbr.xuetiantiany.cn

composer require psr/container
来源：http://zyr.havefunace.top

[U76] PHP：简单路由
来源：http://xxn.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zvm.jianghu66.top

[U77] PHP：模板渲染
来源：http://gtz.ywan-chungtsiang.top

composer require twig/twig
来源：http://qzq.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://wta.cheryme.top

composer require --dev phpunit/phpunit
来源：http://lon.jiagoushi.top

[U79] PHP：静态分析
来源：http://ccs.yonumen.top

composer require --dev phpstan/phpstan
来源：http://lrp.hammf.cn

[U80] PHP：代码规范修复
来源：http://lpa.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ytj.ivvv.top

[U81] JS：初始化项目
来源：http://nyj.fengsongda.top

npm init -y;  npm i express
来源：http://kaf.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://adk.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zby.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://kzg.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://nlr.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://yqw.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://hsu.shzxlz.cn

[U85] JS：可选链
来源：http://ynf.zhaomingkeji.xyz

a?.b?.c
来源：http://vog.quarkkingdee.top

[U86] JS：空值合并
来源：http://pxn.zhaomingkeji.xyz

a ?? b
来源：http://mhm.xinyue.icu

[U87] JS：解构默认值
来源：http://fbb.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://iht.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://hzr.daxiang520.top

{ ...a, ...b }
来源：http://acm.xuanzx.com

[U89] JS：数组去重
来源：http://vzo.ivvv.top

[...new Set(arr)]
来源：http://btg.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://ysc.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://zgm.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://qjh.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dyj.zdbjq.cn

[U92] JS：深拷贝
来源：http://oxw.tian-w.cn

structuredClone(obj)
来源：http://yvm.cheryme.top

[U93] JS：模板字符串
来源：http://wno.hongshengwenyu.top

`共 ${n} 条`
来源：http://fte.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://luc.fktsv.cn

const double = x => x * 2;
来源：http://dzg.fktsv.cn

[U95] JS：Promise 包装
来源：http://ohh.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://gqs.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://lgk.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://whh.feifeiyinyue.top

[U97] JS：并发请求
来源：http://ukd.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rrn.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://azw.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hji.hongshengwenyu.top

[U99] JS：事件监听
来源：http://rpi.yfazqb.com

el.addEventListener("click", e => {})
来源：http://jwx.yuxming.cn

[U100] JS：DOM 查询
来源：http://hiw.guannengcc.top

document.querySelector(".item")
来源：http://emc.gzhubu.top

[U101] JS：classList 操作
来源：http://xdv.zhixingplan.top

el.classList.toggle("active")
来源：http://ydt.hnqzz.top

[U102] JS：本地存储
来源：http://wtk.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uhd.zhiwuduotai.top

[U103] JS：定时器
来源：http://mwc.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yvq.wangdashe.top

[U104] JS：防抖
来源：http://eky.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kju.epnwcf.com

[U105] JS：节流
来源：http://dje.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://raa.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://toe.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pdw.zdqjudy.top

[U107] JS：数字千分位
来源：http://pzq.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ieq.andypj.xyz

[U108] JS：随机整数
来源：http://ckc.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://new.guowangkeji.top

[U109] JS：数组分组
来源：http://lvs.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://dzz.nanxinkj.top

[U110] JS：数组分块
来源：http://zrs.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cju.yj20258.top

[U111] JS：对象转 Map
来源：http://jum.0kj1m.cn

new Map(Object.entries(obj))
来源：http://lby.sxryk.cn

[U112] JS：字符串补位
来源：http://lmz.sjlbkw.cn

"7".padStart(3, "0")
来源：http://yfs.bjfxy.top

[U113] JS：正则替换全部
来源：http://tpf.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://kxd.andypj.xyz

[U114] JS：JSON 深比较
来源：http://ftq.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jhj.yongpay.top

[U115] JS：生成 UUID
来源：http://vjb.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://esd.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://pmd.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://wvf.sysykeji.top

[U117] JS：单元测试
来源：http://gdr.havefunace.top

npm i -D vitest;  npx vitest
来源：http://hcj.ppjwa.cn

[U118] JS：开发服务器
来源：http://ksy.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://yiv.jianghu66.top

[U119] JS：生产构建
来源：http://dot.hcnkem.com

npx vite build
来源：http://brl.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://mel.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://cbc.jiagoushi.top

================================================================================
来源：http://lyq.guannengcc.top

统计汇总
来源：http://bcz.zdbjq.cn

================================================================================
来源：http://bqc.hongshengwenyu.top

按语言统计（条）：
来源：http://xgv.zycfv.cn

Python ......... 252
来源：http://llx.chenlongwang.top

PHP ............ 252
来源：http://jua.tanke756.top

JavaScript ..... 252
来源：http://bov.ydjk.org.cn

TypeScript ..... 212
来源：http://kbo.ivvv.top

Java ........... 212
来源：http://uwb.yuxming.cn

Go ............. 212
来源：http://ejx.tian-w.cn

Ruby ........... 212
来源：http://tne.xuetiantiany.cn

C# ............. 212
来源：http://thf.wangshuangyany.cn

C .............. 30
来源：http://mmn.hongshengwenyu.top

C++ ............ 30
来源：http://ckv.yangfankeji.com

SQL ............ 90
来源：http://rdb.vehdjk.com

Bash ........... 80
来源：http://ckd.dashuyun.cn

Kotlin ......... 15
来源：http://sln.yanxiufei.cn

Swift .......... 15
来源：http://zct.tanke756.top

Lua ............ 10
来源：http://jnl.birdmap.top

Perl ........... 10
来源：http://zss.zycfv.cn

Scala .......... 10
来源：http://zni.cucudq.cn

------------------------------------
来源：http://pwf.yfazqb.com

合计 ........... 2106 条
来源：http://pwe.gaohongyu789.top

按章节统计：
来源：http://wwy.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bcv.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mhk.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vjk.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uoi.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eri.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nmu.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ifz.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gio.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://six.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://das.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zmn.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cpp.52xcode.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://frs.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://erm.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ipe.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lik.cqqwz.cn

Q SQL 专题                              90
来源：http://ypx.tianlin.xyz

R Bash 专题                             80
来源：http://qqv.jianghu66.top

S C / C++ 专题                          60
来源：http://hli.haohaochexian.top

T 其他语言补充                          60
来源：http://tuq.sjlbkw.cn

U 高频实用片段                         120
来源：http://rke.fanxiaobao.xyz

------------------------------------
来源：http://tvu.hnqzz.top

合计                                  2106 条
来源：http://yru.cheryme.top

--------------------------------------------------------------------------------
来源：http://szb.zhiwuduotai.top

使用提醒
来源：http://wyi.daria6918.cn

--------------------------------------------------------------------------------
来源：http://rrf.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nwf.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qfp.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://umr.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bkf.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ipx.fzhhl.top

—— 文件结束 ——
来源：http://wnn.hcnkem.com

================================================================================
来源：http://qid.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://flb.52xcode.cn

Common Programming Examples Cheat Book
来源：http://bfu.yvedp.cn

================================================================================
来源：http://mzh.fanxiaobao.xyz

【收录内容】
来源：http://jej.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dwr.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dcq.yvedp.cn

SQL · Bash · C · C++
来源：http://fnx.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ben.kuanghao11.cn

【使用说明】
来源：http://mcd.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://loq.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nzy.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tpq.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://chd.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pld.sxryk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wpn.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wsy.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mal.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://usx.kuanghao11.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xeh.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gjm.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mjd.yuanzhike.top

【文件统计】
来源：http://vnd.chenlongwang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mwa.ydzc1.top

--------------------------------------------------------------------------------
来源：http://mym.ehwqpu.com

目  录
来源：http://sfj.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://diz.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fzk.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ldz.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://haj.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ebi.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rup.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cln.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vwg.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tll.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sse.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://atn.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ttn.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lyb.hfpthk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qrd.fanxiaobao.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ojy.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zek.yfazqb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kfl.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cgq.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rkp.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cvi.zhijiandao.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ocw.shangyingyoupin.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://juo.jinyuanbaomall.cn

================================================================================
来源：http://bhz.0kj1m.cn

A. 基础语法与类型
来源：http://iio.yonumen.top

================================================================================
来源：http://vuy.chenjidiqi.icu

[A01] Hello World
来源：http://msl.jqgufenzy.top

Py:   print("Hello, World!")
来源：http://bki.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://dxg.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://rgw.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zvi.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://ads.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://vvy.wangshuangyany.cn

Ruby: puts "Hello, World!"
来源：http://kwq.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sdv.fehbvm.com

[A02] 变量声明与赋值
来源：http://orw.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://psi.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vmo.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://pki.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://izo.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://fxs.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://pos.hysaishi.cn

Ruby: name = "Alex"; age = 20
来源：http://jya.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://qwq.ctjpmb.com

[A03] 常量定义
来源：http://vfp.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://khi.ivvv.top

PHP:  const PI = 3.14159;
来源：http://fkl.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://tkl.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://ldp.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://bam.xuanzx.com

Go:   const PI = 3.14159
来源：http://aym.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://grh.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://ibt.zhengqikj.top

[A04] 判断变量类型
来源：http://sjc.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://rur.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rhc.pengpengdd.cyou

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tht.zhiwuduotai.top

TS:   typeof x; x instanceof Date
来源：http://vhq.fengsongda.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rxf.ivvv.top

Go:   reflect.TypeOf(x).Name()
来源：http://xhk.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rqd.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://lba.zdbjq.cn

[A05] 整数除法与取模
来源：http://crc.jinqigufen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://guz.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jzp.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://djm.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ovx.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://pnc.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://cve.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://ylc.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://wel.xuetiantiany.cn

[A06] 字符串转数字
来源：http://ccc.sufxvd.cn

Py:   int("42"); float("3.14")
来源：http://fvf.xinyue.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://piv.xinyue.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hmj.jinghuilouyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://avx.sxryk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dbz.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ipu.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xjo.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://udo.hfpthk.cn

[A07] 数字转字符串
来源：http://bml.dianchejie.cn

Py:   str(42)
来源：http://zmc.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://hps.feifeiyinyue.top

JS:   String(42); (42).toString()
来源：http://hoi.kuanghao11.cn

TS:   String(42)
来源：http://ifz.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uuw.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://sxx.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://zdb.guowangkeji.top

C#:   42.ToString()
来源：http://rvf.vehdjk.com

[A08] 取整与四舍五入
来源：http://fod.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://adu.zhiwuduotai.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eag.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sap.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gpb.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hsz.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yud.feifeiyinyue.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zuu.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yof.haohaochexian.top

[A09] 绝对值与最大最小值
来源：http://tyf.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jbv.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eyn.c1oappe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jbl.uphjek.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://def.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://klr.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://okk.jlsjyb.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ole.zhixingplan.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://raw.zhongyouzk.top

[A10] 生成随机数
来源：http://exy.zhijiandao.cn

Py:   import random; random.randint(1, 100)
来源：http://cut.jinqigfzy.top

PHP:  random_int(1, 100);
来源：http://ltb.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://niw.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xog.yonumen.top

Java: new Random().nextInt(100) + 1
来源：http://itf.wangshuangyany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yuq.gaohongyu789.top

Ruby: rand(1..100)
来源：http://yyj.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://fgk.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://asf.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://bna.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lgq.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://tge.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://fnm.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://veu.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wgq.zycfv.cn


<!-- 参考信息 -->