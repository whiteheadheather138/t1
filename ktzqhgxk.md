代发 wailian999

[U79] PHP：静态分析
来源：http://hzv.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://arp.daria6918.cn

[U80] PHP：代码规范修复
来源：http://lfu.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tkr.aibaodan.cn

[U81] JS：初始化项目
来源：http://smg.chenjidiqi.icu

npm init -y;  npm i express
来源：http://uqh.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://wyy.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gbw.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://kal.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rcf.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://jrj.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://snt.quarkkingdee.top

[U85] JS：可选链
来源：http://ezt.sjlbkw.cn

a?.b?.c
来源：http://qar.ctjpmb.com

[U86] JS：空值合并
来源：http://voo.haohaochexian.top

a ?? b
来源：http://bxk.svipenyu.cn

[U87] JS：解构默认值
来源：http://vgs.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://szt.gotoacloud.top

[U88] JS：对象展开合并
来源：http://vhh.tarul.cn

{ ...a, ...b }
来源：http://pdv.ppjwa.cn

[U89] JS：数组去重
来源：http://lon.cucudq.cn

[...new Set(arr)]
来源：http://dac.chenzaomai.com

[U90] JS：数字数组排序
来源：http://uvk.chenjidiqi.icu

[...arr].sort((a, b) => a - b)
来源：http://kwz.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://mwn.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cbj.dashuyun.cn

[U92] JS：深拷贝
来源：http://gss.redwolf501.top

structuredClone(obj)
来源：http://euu.cashguo.top

[U93] JS：模板字符串
来源：http://qkx.c1oappe.top

`共 ${n} 条`
来源：http://xyq.zhengqikj.top

[U94] JS：箭头函数
来源：http://yrq.haohaochexian.top

const double = x => x * 2;
来源：http://zps.vehdjk.com

[U95] JS：Promise 包装
来源：http://awr.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://kjh.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://ghz.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fcq.yj20258.top

[U97] JS：并发请求
来源：http://uyk.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://igm.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://ted.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kxa.yueranfly.top

[U99] JS：事件监听
来源：http://yfa.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://qob.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://zdy.shanyushiyangtech.top

document.querySelector(".item")
来源：http://rgo.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://eth.gotoacloud.top

el.classList.toggle("active")
来源：http://hjm.zhoulong.xyz

[U102] JS：本地存储
来源：http://qkz.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://qpu.sjlbkw.cn

[U103] JS：定时器
来源：http://tsc.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ckf.chenjidiqi.icu

[U104] JS：防抖
来源：http://ldo.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://smi.yfazqb.com

[U105] JS：节流
来源：http://csb.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pgz.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://wze.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iqb.hesvh.cn

[U107] JS：数字千分位
来源：http://avs.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nob.xziqi.cn

[U108] JS：随机整数
来源：http://doh.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qkm.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://ffe.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://bls.zhoulong.xyz

[U110] JS：数组分块
来源：http://bym.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gpk.aibaodan.cn

[U111] JS：对象转 Map
来源：http://agn.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://tqs.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://pou.aizwys.cn

"7".padStart(3, "0")
来源：http://ffm.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://bej.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://cxb.yongpay.top

[U114] JS：JSON 深比较
来源：http://cbi.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wkz.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://sxf.gotoacloud.top

crypto.randomUUID()
来源：http://ywb.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://yia.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://zsa.nwbrower.top

[U117] JS：单元测试
来源：http://kdy.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://rgn.epnwcf.com

[U118] JS：开发服务器
来源：http://tvw.yj20258888.top

npm i -D vite;  npx vite
来源：http://qpk.cheryme.top

[U119] JS：生产构建
来源：http://dho.sufxvd.cn

npx vite build
来源：http://cdm.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://okm.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://flf.mhx1999.top

================================================================================
来源：http://kmn.snrcjt.cn

统计汇总
来源：http://ydm.yvedp.cn

================================================================================
来源：http://rib.c1oappe.top

按语言统计（条）：
来源：http://blh.birdmap.top

Python ......... 252
来源：http://ixx.sxryk.cn

PHP ............ 252
来源：http://lpw.hysaishi.cn

JavaScript ..... 252
来源：http://npe.zdqjudy.top

TypeScript ..... 212
来源：http://zmk.vehdjk.com

Java ........... 212
来源：http://vwv.zhixingplan.top

Go ............. 212
来源：http://nfk.havefunace.top

Ruby ........... 212
来源：http://lln.snrcjt.cn

C# ............. 212
来源：http://aal.chenlongwang.top

C .............. 30
来源：http://lbl.316326.xyz

C++ ............ 30
来源：http://vbh.xuanzx.com

SQL ............ 90
来源：http://vza.vehdjk.com

Bash ........... 80
来源：http://kvt.chenlongwang.top

Kotlin ......... 15
来源：http://ahv.sxryk.cn

Swift .......... 15
来源：http://ids.nanxuanxn.top

Lua ............ 10
来源：http://uus.mhx1999.top

Perl ........... 10
来源：http://lpr.nanxinkj.top

Scala .......... 10
来源：http://bqd.gaohongyu789.top

------------------------------------
来源：http://doo.jqgufenzy.top

合计 ........... 2106 条
来源：http://xby.epnwcf.com

按章节统计：
来源：http://day.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wzp.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wan.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wyc.hnxiangtu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uoq.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iqi.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ngf.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tvg.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yfm.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hga.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oki.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gxk.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jut.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wiq.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dwv.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jhk.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ful.xinyue.icu

Q SQL 专题                              90
来源：http://hdo.gotoacloud.top

R Bash 专题                             80
来源：http://pah.zhoulong.xyz

S C / C++ 专题                          60
来源：http://jfi.yuanzhike.top

T 其他语言补充                          60
来源：http://eef.svipenyu.cn

U 高频实用片段                         120
来源：http://vfm.vehdjk.com

------------------------------------
来源：http://dif.feifeiyinyue.top

合计                                  2106 条
来源：http://euh.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://fvy.yj20258.top

使用提醒
来源：http://jkc.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://cgh.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dxr.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tgj.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pxi.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oog.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yfj.chenlongwang.top

—— 文件结束 ——
来源：http://rrz.xuetiantiany.cn

================================================================================
来源：http://dmh.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://que.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://hnf.dianchejie.cn

================================================================================
来源：http://xkk.gotoacloud.top

【收录内容】
来源：http://acl.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://hmz.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qfe.hammf.cn

SQL · Bash · C · C++
来源：http://qxq.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fmj.yangfankeji.com

【使用说明】
来源：http://sqn.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pyc.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xrv.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zhc.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://olk.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qsh.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bpp.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gsk.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yqz.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uoi.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oxf.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hxo.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kii.ehwqpu.com

【文件统计】
来源：http://lbc.hongshengwenyu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vxf.fktsv.cn

--------------------------------------------------------------------------------
来源：http://cwr.jlsjyb.cn

目  录
来源：http://kud.bjfxy.top

--------------------------------------------------------------------------------
来源：http://vcu.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kek.guannengcc.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gty.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tru.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ekt.ppjwa.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yos.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kjv.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lyz.hammf.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sfz.shzxlz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blb.zhixingplan.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fqu.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uus.c1oappe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nck.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mmo.tianlin.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fav.shanyushiyangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mmd.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rfa.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wrb.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://aqm.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jqz.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fzf.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uyp.jlsjyb.cn

================================================================================
来源：http://grs.chenzaomai.com

A. 基础语法与类型
来源：http://fze.zhengqikj.top

================================================================================
来源：http://gsu.yuanzhike.top

[A01] Hello World
来源：http://ijv.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://jzn.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://fvx.hysaishi.cn

JS:   console.log("Hello, World!");
来源：http://uou.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://stc.andypj.xyz

Java: System.out.println("Hello, World!");
来源：http://wbi.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://kta.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://blk.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fpi.gotoacloud.top

[A02] 变量声明与赋值
来源：http://uyw.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aes.c1oappe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zqt.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://viu.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ztn.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://tsl.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://kmc.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://wjl.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://lfi.jinqigufen.top

[A03] 常量定义
来源：http://eyp.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sns.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://wvg.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://ydd.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://tum.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://nhu.zdbjq.cn

Go:   const PI = 3.14159
来源：http://ivu.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://npe.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://gmc.9152youxi.cn

[A04] 判断变量类型
来源：http://czo.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ngv.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pzk.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gzc.sufxvd.cn

TS:   typeof x; x instanceof Date
来源：http://myc.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yvn.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://jkk.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xmj.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://ekl.fanxiaobao.xyz

[A05] 整数除法与取模
来源：http://wyg.yongpay.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nax.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://whd.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hbm.shangyingyoupin.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wcw.feifeiyinyue.top

Java: 7 / 2; 7 % 2
来源：http://mze.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://cct.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://ybu.316326.xyz

C#:   7 / 2; 7 % 2
来源：http://bbp.shzxlz.cn

[A06] 字符串转数字
来源：http://lje.smart0.xyz

Py:   int("42"); float("3.14")
来源：http://czc.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nsg.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fgr.jqgfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://hhx.zhongyouzk.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://utz.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://til.tianlin.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ffl.hammf.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wbk.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://rur.fzhhl.top

Py:   str(42)
来源：http://oki.hywenlv.cn

PHP:  (string) 42; strval(42)
来源：http://nmr.tarul.cn

JS:   String(42); (42).toString()
来源：http://krg.sysykeji.top

TS:   String(42)
来源：http://kll.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://eyl.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://cxh.ctjpmb.com

Ruby: 42.to_s
来源：http://pnt.hnxiangtu.top

C#:   42.ToString()
来源：http://vou.xinyue.icu

[A08] 取整与四舍五入
来源：http://jlv.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sew.jqgufenzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ncg.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rwa.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pru.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hcp.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rtc.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://mte.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kex.hammf.cn

[A09] 绝对值与最大最小值
来源：http://khb.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ecf.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kwu.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fzi.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sxy.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vcw.sxryk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://omo.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eos.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ruc.wangdashe.top

[A10] 生成随机数
来源：http://gdf.zdbjq.cn

Py:   import random; random.randint(1, 100)
来源：http://zxe.jinghuilouyu.cn

PHP:  random_int(1, 100);
来源：http://umm.kuanghao11.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mwr.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://les.kuanghao11.cn

Java: new Random().nextInt(100) + 1
来源：http://kwd.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gsa.zdbjq.cn

Ruby: rand(1..100)
来源：http://ekm.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://jby.uphjek.com

[A11] 条件表达式（三元）
来源：http://pgm.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://hdl.fengsongda.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ikk.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uma.quarkkingdee.top

TS:   x > 0 ? "yes" : "no"
来源：http://xwm.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://rga.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://ffk.sweek.top

Ruby: x > 0 ? "yes" : "no"
来源：http://anj.gotoacloud.top

C#:   x > 0 ? "yes" : "no"
来源：http://bkq.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://vds.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ncz.hongshengwenyu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uwk.yj202588.top

JS:   `Hello, ${name}!`
来源：http://zlq.yanxiufei.cn

TS:   `Hello, ${name}!`
来源：http://nbf.c1oappe.top

Java: "Hello, %s!".formatted(name)
来源：http://mmh.yfazqb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dbx.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://arl.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://gza.sysykeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yqq.chenzaomai.com


<!-- 参考信息 -->