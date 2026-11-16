代发 wailian999

[U77] PHP：模板渲染
来源：http://ruh.xuetiantiany.cn

composer require twig/twig
来源：http://iez.vehdjk.com

[U78] PHP：单元测试
来源：http://vkw.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://vgd.jiagoushi.top

[U79] PHP：静态分析
来源：http://xtd.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://amv.xuanzx.com

[U80] PHP：代码规范修复
来源：http://sih.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fnt.yangfankeji.com

[U81] JS：初始化项目
来源：http://xpa.vehdjk.com

npm init -y;  npm i express
来源：http://stw.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://xaf.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zoh.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://pzj.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fxf.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://jhp.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://mba.hfpthk.cn

[U85] JS：可选链
来源：http://rdg.cucudq.cn

a?.b?.c
来源：http://cru.tianlin.xyz

[U86] JS：空值合并
来源：http://ifx.ivvv.top

a ?? b
来源：http://thf.xuanzx.com

[U87] JS：解构默认值
来源：http://ioc.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://chz.sxryk.cn

[U88] JS：对象展开合并
来源：http://eiq.vehdjk.com

{ ...a, ...b }
来源：http://fgp.chenlongwang.top

[U89] JS：数组去重
来源：http://ule.haohaochexian.top

[...new Set(arr)]
来源：http://xke.zdbjq.cn

[U90] JS：数字数组排序
来源：http://dbd.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://fsf.birdmap.top

[U91] JS：对象键值遍历
来源：http://ezv.52xcode.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uuy.jqgfzy.top

[U92] JS：深拷贝
来源：http://kmj.jinqigfzy.top

structuredClone(obj)
来源：http://szy.redwolf501.top

[U93] JS：模板字符串
来源：http://avs.iojbl.cn

`共 ${n} 条`
来源：http://luw.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://ubr.hammf.cn

const double = x => x * 2;
来源：http://ggv.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://nwa.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://qsy.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://gka.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sbz.shzxlz.cn

[U97] JS：并发请求
来源：http://jrx.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iuc.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://syk.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wai.ehwqpu.com

[U99] JS：事件监听
来源：http://igt.52xcode.cn

el.addEventListener("click", e => {})
来源：http://xfh.tianlin.xyz

[U100] JS：DOM 查询
来源：http://jce.nwbrower.top

document.querySelector(".item")
来源：http://yjx.iojbl.cn

[U101] JS：classList 操作
来源：http://lyz.pycfn.com

el.classList.toggle("active")
来源：http://xoj.redwolf501.top

[U102] JS：本地存储
来源：http://wbc.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hes.zhiwuduotai.top

[U103] JS：定时器
来源：http://sap.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gnt.hnqzz.top

[U104] JS：防抖
来源：http://lsw.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sko.vehdjk.com

[U105] JS：节流
来源：http://ofu.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://syk.yfazqb.com

[U106] JS：日期格式化
来源：http://sdi.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rqh.hnxiangtu.top

[U107] JS：数字千分位
来源：http://rel.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gsy.gotoacloud.top

[U108] JS：随机整数
来源：http://cxy.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gns.birdmap.top

[U109] JS：数组分组
来源：http://bgf.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://cde.316326.xyz

[U110] JS：数组分块
来源：http://uzr.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://npw.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://umn.fengsongda.top

new Map(Object.entries(obj))
来源：http://qvs.iojbl.cn

[U112] JS：字符串补位
来源：http://fau.yj20258.top

"7".padStart(3, "0")
来源：http://trb.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://eot.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://vaw.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://bph.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ldx.yvedp.cn

[U115] JS：生成 UUID
来源：http://wdq.zhijiandao.cn

crypto.randomUUID()
来源：http://vzv.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://xep.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://nut.zhengqikj.top

[U117] JS：单元测试
来源：http://ret.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://iqi.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://ftb.sweek.top

npm i -D vite;  npx vite
来源：http://dbt.daria6918.cn

[U119] JS：生产构建
来源：http://crj.tian-w.cn

npx vite build
来源：http://pwm.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://fdk.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://buo.nanxuanxn.top

================================================================================
来源：http://xdv.fktsv.cn

统计汇总
来源：http://whm.tarul.cn

================================================================================
来源：http://nvu.xuanzx.com

按语言统计（条）：
来源：http://iks.jyoumei.cn

Python ......... 252
来源：http://wbw.svipenyu.cn

PHP ............ 252
来源：http://hmj.uphjek.com

JavaScript ..... 252
来源：http://vba.shzxlz.cn

TypeScript ..... 212
来源：http://xgc.ydjk.org.cn

Java ........... 212
来源：http://bcm.ybcxt.top

Go ............. 212
来源：http://rjs.yuanzhike.top

Ruby ........... 212
来源：http://skg.daxiang520.top

C# ............. 212
来源：http://azu.yanxiufei.cn

C .............. 30
来源：http://nhr.bjfxy.top

C++ ............ 30
来源：http://ocq.wangdashe.top

SQL ............ 90
来源：http://cfk.yuxming.cn

Bash ........... 80
来源：http://bko.ydjk.org.cn

Kotlin ......... 15
来源：http://mpe.fehbvm.com

Swift .......... 15
来源：http://jzb.yfazqb.com

Lua ............ 10
来源：http://xkl.zhijiandao.cn

Perl ........... 10
来源：http://cia.nanxinkj.top

Scala .......... 10
来源：http://mdm.birdmap.top

------------------------------------
来源：http://aql.ppjwa.cn

合计 ........... 2106 条
来源：http://xmh.uphjek.com

按章节统计：
来源：http://hyn.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pxy.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://juj.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://coj.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yzx.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://csa.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sjx.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://luw.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://piu.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cek.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dia.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mfj.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mof.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wxe.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dtz.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tck.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ret.gotoacloud.top

Q SQL 专题                              90
来源：http://hex.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://rcm.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://uae.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://jde.dashuyun.cn

U 高频实用片段                         120
来源：http://cll.hfpthk.cn

------------------------------------
来源：http://pgq.xuanzx.com

合计                                  2106 条
来源：http://gey.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://log.316326.xyz

使用提醒
来源：http://oqp.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://xmk.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vgj.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gme.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nuz.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qcd.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kex.yj202588.top

—— 文件结束 ——
来源：http://kii.ywan-chungtsiang.top

================================================================================
来源：http://awy.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://vlu.hesvh.cn

Common Programming Examples Cheat Book
来源：http://yle.ydjk.org.cn

================================================================================
来源：http://czj.sysykeji.top

【收录内容】
来源：http://hei.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://clz.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lqh.yongpay.top

SQL · Bash · C · C++
来源：http://hge.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cpi.hywenlv.cn

【使用说明】
来源：http://tpc.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ydv.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ixq.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mwi.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zkf.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://plp.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qiu.yj202588.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wre.haohaochexian.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wnq.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vjr.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vso.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://smq.c1oappe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dni.tarul.cn

【文件统计】
来源：http://txb.yvedp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bld.mhx1999.top

--------------------------------------------------------------------------------
来源：http://wmr.redwolf501.top

目  录
来源：http://tdl.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://dod.shuidangran.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mbb.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rgb.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nzt.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cta.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fwx.yj20258.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sjf.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xsb.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nog.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vqh.fanxiaobao.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ths.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ret.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hea.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ktj.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bpw.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rnr.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vzb.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xgm.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://smd.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oxz.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://scn.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oks.wangdashe.top

================================================================================
来源：http://zoy.cucudq.cn

A. 基础语法与类型
来源：http://fzo.bjfxy.top

================================================================================
来源：http://wex.0kj1m.cn

[A01] Hello World
来源：http://mge.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://qjh.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://gvy.ppjwa.cn

JS:   console.log("Hello, World!");
来源：http://edb.chenzaomai.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oro.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://fhk.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://gqa.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://cde.zhongyouzk.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qaj.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://nnd.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pty.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rkh.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://nik.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vsv.yuxming.cn

Java: String name = "Alex"; int age = 20;
来源：http://gzo.xinyue.icu

Go:   name := "Alex"; age := 20
来源：http://qdi.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://uso.chenlongwang.top

C#:   string name = "Alex"; int age = 20;
来源：http://fog.yj20258888.top

[A03] 常量定义
来源：http://imx.zycfv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xnn.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://xlk.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://ufp.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://rfu.yonumen.top

Java: static final double PI = 3.14159;
来源：http://swf.xinyue.icu

Go:   const PI = 3.14159
来源：http://hwq.gotoacloud.top

Ruby: PI = 3.14159
来源：http://ilw.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://qzb.jyoumei.cn

[A04] 判断变量类型
来源：http://mai.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ift.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mgl.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bzb.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://jop.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qcl.cqqwz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qkk.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pne.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://rsh.sxryk.cn

[A05] 整数除法与取模
来源：http://tzm.epnwcf.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sbs.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xmf.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpn.zdbjq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gsy.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://bfu.ivvv.top

Go:   7 / 2; 7 % 2
来源：http://vgu.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://aut.hammf.cn

C#:   7 / 2; 7 % 2
来源：http://usc.hesvh.cn

[A06] 字符串转数字
来源：http://rff.aizwys.cn

Py:   int("42"); float("3.14")
来源：http://thw.bbcook.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pju.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://esq.nanxuanxn.top

TS:   parseInt("42", 10); Number("42")
来源：http://yup.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ucy.pycfn.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://onp.tianlin.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://oww.aizwys.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kfz.fktsv.cn

[A07] 数字转字符串
来源：http://qpe.hammf.cn

Py:   str(42)
来源：http://ari.sweek.top

PHP:  (string) 42; strval(42)
来源：http://zbx.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://kzi.vehdjk.com

TS:   String(42)
来源：http://udn.ydzc1.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uji.yuxming.cn

Go:   strconv.Itoa(42)
来源：http://yho.vehdjk.com

Ruby: 42.to_s
来源：http://wvt.gotoacloud.top

C#:   42.ToString()
来源：http://kog.shuidangran.top

[A08] 取整与四舍五入
来源：http://ngz.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ifd.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wus.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lyd.dianchejie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fkz.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qns.pycfn.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ixb.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ims.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bez.yanxiufei.cn

[A09] 绝对值与最大最小值
来源：http://cvx.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://als.birdmap.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://puw.fzhhl.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hrl.ivvv.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hto.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jan.jinqigfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lrk.gogol.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uyq.hnxiangtu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ofv.kuanghao11.cn

[A10] 生成随机数
来源：http://hlc.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://fmu.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://nkc.gogol.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gcq.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ehw.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://efp.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fcw.hammf.cn

Ruby: rand(1..100)
来源：http://bls.cashguo.top

C#:   new Random().Next(1, 101)
来源：http://gcw.hnqzz.top

[A11] 条件表达式（三元）
来源：http://yic.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://qxa.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ebw.fzhhl.top

JS:   x > 0 ? "yes" : "no"
来源：http://sag.ppjwa.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xfa.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://apj.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qqd.ctjpmb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://sex.cashguo.top

C#:   x > 0 ? "yes" : "no"
来源：http://htv.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://fzy.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ttw.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yol.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://qhw.hywenlv.cn

TS:   `Hello, ${name}!`
来源：http://vig.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://wys.kuanghao11.cn


<!-- 参考信息 -->