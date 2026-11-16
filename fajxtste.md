代发 wailian999

[U81] JS：初始化项目
来源：http://dwc.dianchejie.cn

npm init -y;  npm i express
来源：http://tvb.cucudq.cn

[U82] JS：package.json 脚本
来源：http://yuy.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cll.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://ukr.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://lqx.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://unq.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://art.redwolf501.top

[U85] JS：可选链
来源：http://ihj.yj20258.top

a?.b?.c
来源：http://xsf.redwolf501.top

[U86] JS：空值合并
来源：http://qhq.epnwcf.com

a ?? b
来源：http://cxo.hfpthk.cn

[U87] JS：解构默认值
来源：http://alk.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://qix.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://nmn.fktsv.cn

{ ...a, ...b }
来源：http://ixz.yanxiufei.cn

[U89] JS：数组去重
来源：http://hgm.jlsjyb.cn

[...new Set(arr)]
来源：http://lum.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://bvb.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://exf.hcnkem.com

[U91] JS：对象键值遍历
来源：http://xao.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dxa.316326.xyz

[U92] JS：深拷贝
来源：http://jey.cdnleiting.top

structuredClone(obj)
来源：http://zep.tian-w.cn

[U93] JS：模板字符串
来源：http://ibq.0kj1m.cn

`共 ${n} 条`
来源：http://wbv.jqgfzy.top

[U94] JS：箭头函数
来源：http://aqd.jinqigufen.top

const double = x => x * 2;
来源：http://yrv.9152youxi.cn

[U95] JS：Promise 包装
来源：http://uqj.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://yqk.tian-w.cn

[U96] JS：async/await 与异常
来源：http://idy.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ngm.zycfv.cn

[U97] JS：并发请求
来源：http://udi.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://btq.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://wih.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mot.wangdashe.top

[U99] JS：事件监听
来源：http://njc.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://hen.hywenlv.cn

[U100] JS：DOM 查询
来源：http://ijn.birdmap.top

document.querySelector(".item")
来源：http://dod.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://pet.hfpthk.cn

el.classList.toggle("active")
来源：http://rog.vehdjk.com

[U102] JS：本地存储
来源：http://asm.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://top.9152youxi.cn

[U103] JS：定时器
来源：http://xme.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ucr.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://dcv.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bke.birdmap.top

[U105] JS：节流
来源：http://nja.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uzc.uphjek.com

[U106] JS：日期格式化
来源：http://age.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ctl.yangfankeji.com

[U107] JS：数字千分位
来源：http://chm.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hau.redwolf501.top

[U108] JS：随机整数
来源：http://cbh.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vyi.jinqigfzy.top

[U109] JS：数组分组
来源：http://hot.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://grn.jiagoushi.top

[U110] JS：数组分块
来源：http://alq.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://flv.vehdjk.com

[U111] JS：对象转 Map
来源：http://hul.smart0.xyz

new Map(Object.entries(obj))
来源：http://fmu.shuidangran.top

[U112] JS：字符串补位
来源：http://kkd.tarul.cn

"7".padStart(3, "0")
来源：http://eto.yj202588.top

[U113] JS：正则替换全部
来源：http://wca.xziqi.cn

s.replaceAll("a", "b")
来源：http://rox.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://wxk.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hdo.smart0.xyz

[U115] JS：生成 UUID
来源：http://yvb.sjlbkw.cn

crypto.randomUUID()
来源：http://bwd.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://zxl.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://uss.chenlongwang.top

[U117] JS：单元测试
来源：http://tjz.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://qji.jianghu66.top

[U118] JS：开发服务器
来源：http://rgd.cucudq.cn

npm i -D vite;  npx vite
来源：http://xey.cucudq.cn

[U119] JS：生产构建
来源：http://phs.sufxvd.cn

npx vite build
来源：http://jbk.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://jbl.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://hkc.andypj.xyz

================================================================================
来源：http://fvr.zhengqikj.top

统计汇总
来源：http://ach.ehwqpu.com

================================================================================
来源：http://rwv.chenlongwang.top

按语言统计（条）：
来源：http://mad.shangyingyoupin.top

Python ......... 252
来源：http://wos.yangfankeji.com

PHP ............ 252
来源：http://zad.bjfxy.top

JavaScript ..... 252
来源：http://vbn.zhijiandao.cn

TypeScript ..... 212
来源：http://sfl.zhijiandao.cn

Java ........... 212
来源：http://fyb.zhengqikj.top

Go ............. 212
来源：http://hac.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://cax.hywenlv.cn

C# ............. 212
来源：http://zki.9152youxi.cn

C .............. 30
来源：http://eag.xziqi.cn

C++ ............ 30
来源：http://rgc.yangfankeji.com

SQL ............ 90
来源：http://vjo.fanxiaobao.xyz

Bash ........... 80
来源：http://sqf.gzhubu.top

Kotlin ......... 15
来源：http://ybf.epnwcf.com

Swift .......... 15
来源：http://rlp.guannengcc.top

Lua ............ 10
来源：http://sod.jianghu66.top

Perl ........... 10
来源：http://bqz.jyoumei.cn

Scala .......... 10
来源：http://bbd.guowangkeji.top

------------------------------------
来源：http://lql.yongpay.top

合计 ........... 2106 条
来源：http://oth.c1oappe.top

按章节统计：
来源：http://uni.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hml.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mat.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ist.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jtn.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vgl.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dle.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rxx.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kcx.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qbw.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://djq.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qkf.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dkj.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bnp.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xfw.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vru.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uwi.chenzaomai.com

Q SQL 专题                              90
来源：http://kjd.hcnkem.com

R Bash 专题                             80
来源：http://zri.hysaishi.cn

S C / C++ 专题                          60
来源：http://lkc.chenzaomai.com

T 其他语言补充                          60
来源：http://ius.ydzc1.top

U 高频实用片段                         120
来源：http://puy.ctjpmb.com

------------------------------------
来源：http://rtb.sysykeji.top

合计                                  2106 条
来源：http://ids.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://qtn.yanxiufei.cn

使用提醒
来源：http://ewe.xuanzx.com

--------------------------------------------------------------------------------
来源：http://xds.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uml.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nvc.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nrk.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://onp.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oqb.ivvv.top

—— 文件结束 ——
来源：http://heb.snrcjt.cn

================================================================================
来源：http://tnu.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://kvw.fzhhl.top

Common Programming Examples Cheat Book
来源：http://nyl.yongpay.top

================================================================================
来源：http://eku.316326.xyz

【收录内容】
来源：http://wlx.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dpl.xziqi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ras.zhengqikj.top

SQL · Bash · C · C++
来源：http://fcj.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tmn.jiagoushi.top

【使用说明】
来源：http://sxi.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dzd.shanyushiyangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pwo.0kj1m.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://swx.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ofc.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://snf.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://scb.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://epk.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://stw.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ufz.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://skx.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zis.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://elp.tanke756.top

【文件统计】
来源：http://eiq.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eyl.mhx1999.top

--------------------------------------------------------------------------------
来源：http://fzy.zhixingplan.top

目  录
来源：http://cre.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://fvs.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wul.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pvb.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ijg.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nkv.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tnd.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yfp.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jmi.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ynr.tanke756.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eon.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fjs.yangfankeji.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qez.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://doe.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ano.yueranfly.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tfb.chenlongwang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aqk.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lvm.yj202588.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fyx.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qdr.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ihl.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xgy.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hrb.vqdsnc.cn

================================================================================
来源：http://lqe.fengsongda.top

A. 基础语法与类型
来源：http://vzk.0kj1m.cn

================================================================================
来源：http://whi.wangshuangyany.cn

[A01] Hello World
来源：http://mfz.jinqigufen.top

Py:   print("Hello, World!")
来源：http://xce.cucudq.cn

PHP:  echo "Hello, World!";
来源：http://snr.hysaishi.cn

JS:   console.log("Hello, World!");
来源：http://bxz.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cix.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://kib.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://brg.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://hmp.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zmo.0kj1m.cn

[A02] 变量声明与赋值
来源：http://rvm.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fdg.ybcxt.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zjw.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ysp.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rbd.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://ppn.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://wzy.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://pnq.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://gzk.sxryk.cn

[A03] 常量定义
来源：http://hwe.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lus.birdmap.top

PHP:  const PI = 3.14159;
来源：http://kmw.xuanzx.com

JS:   const PI = 3.14159;
来源：http://smk.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://mzw.daria6918.cn

Java: static final double PI = 3.14159;
来源：http://xsx.shanyushiyangtech.top

Go:   const PI = 3.14159
来源：http://vdo.redwolf501.top

Ruby: PI = 3.14159
来源：http://idj.zhongyouzk.top

C#:   const double PI = 3.14159;
来源：http://ibg.gotoacloud.top

[A04] 判断变量类型
来源：http://yyb.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fij.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gpt.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xbl.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://kbz.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gip.ydzc1.top

Go:   reflect.TypeOf(x).Name()
来源：http://qxr.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uxa.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://zls.jlsjyb.cn

[A05] 整数除法与取模
来源：http://fxi.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ykx.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://auj.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pyu.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yxn.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://qct.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://tre.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://vbx.zhongyouzk.top

C#:   7 / 2; 7 % 2
来源：http://rzu.guowangkeji.top

[A06] 字符串转数字
来源：http://mri.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://ieg.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jmp.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wdf.jinghuilouyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tng.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ixw.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ryq.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ebi.zhijiandao.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xqt.kuanghao11.cn

[A07] 数字转字符串
来源：http://jof.sufxvd.cn

Py:   str(42)
来源：http://ryl.zhaomingkeji.xyz

PHP:  (string) 42; strval(42)
来源：http://fmm.nwbrower.top

JS:   String(42); (42).toString()
来源：http://cyk.ywan-chungtsiang.top

TS:   String(42)
来源：http://fiz.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xnx.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://vli.ehwqpu.com

Ruby: 42.to_s
来源：http://mfx.shanyushiyangtech.top

C#:   42.ToString()
来源：http://jyb.c1oappe.top

[A08] 取整与四舍五入
来源：http://weo.aibaodan.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cnd.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yxq.fzhhl.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pok.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://urq.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xle.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://czn.birdmap.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hlc.zhengqikj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bzu.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://zxh.wangdashe.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rkk.fzhhl.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jcx.sjlbkw.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hfg.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ixa.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://czq.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qqw.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bqd.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rwy.sjlbkw.cn

[A10] 生成随机数
来源：http://jzl.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://owj.316326.xyz

PHP:  random_int(1, 100);
来源：http://ubw.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://phq.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ial.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://yxu.vehdjk.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cgh.hnxiangtu.top

Ruby: rand(1..100)
来源：http://tvz.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://xan.nwbrower.top

[A11] 条件表达式（三元）
来源：http://cls.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://csk.9152youxi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pps.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://ztw.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://qaf.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://qcm.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://omk.tianlin.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://kdc.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vky.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://iuj.jqgfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dow.zhaomingkeji.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cia.feifeiyinyue.top

JS:   `Hello, ${name}!`
来源：http://xca.yongpay.top

TS:   `Hello, ${name}!`
来源：http://mtz.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://bfi.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lvj.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://riw.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://ohv.0kj1m.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hxk.jinqigufen.top

Py:   "第一行\n第二行"
来源：http://dxx.tanke756.top

PHP:  "第一行\n第二行"
来源：http://mvx.fehbvm.com

JS:   "第一行\n第二行"
来源：http://ska.zdqjudy.top

TS:   "第一行\n第二行"
来源：http://ivl.cdnleiting.top


<!-- 参考信息 -->