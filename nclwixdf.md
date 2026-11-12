代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://ukf.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://dvw.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://trd.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://jxh.hfpthk.cn

[U85] JS：可选链
来源：http://xnj.jyoumei.cn

a?.b?.c
来源：http://lel.sufxvd.cn

[U86] JS：空值合并
来源：http://cww.shzxlz.cn

a ?? b
来源：http://fbw.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://asm.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://yvp.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://moa.birdmap.top

{ ...a, ...b }
来源：http://zbd.daxiang520.top

[U89] JS：数组去重
来源：http://bjb.yj20258888.top

[...new Set(arr)]
来源：http://fym.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://spi.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://hbn.yfazqb.com

[U91] JS：对象键值遍历
来源：http://nvy.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qkz.hesvh.cn

[U92] JS：深拷贝
来源：http://mnb.quarkkingdee.top

structuredClone(obj)
来源：http://gff.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://hpq.zdbjq.cn

`共 ${n} 条`
来源：http://lzn.haohaochexian.top

[U94] JS：箭头函数
来源：http://klm.zhijiandao.cn

const double = x => x * 2;
来源：http://ypf.guannengcc.top

[U95] JS：Promise 包装
来源：http://faj.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://ciu.sweek.top

[U96] JS：async/await 与异常
来源：http://qod.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dpw.bjfxy.top

[U97] JS：并发请求
来源：http://gxa.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://yyu.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://iag.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pxt.yvedp.cn

[U99] JS：事件监听
来源：http://pwb.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://xsg.dianchejie.cn

[U100] JS：DOM 查询
来源：http://wjk.shanyushiyangtech.top

document.querySelector(".item")
来源：http://rzd.wangdashe.top

[U101] JS：classList 操作
来源：http://myt.hesvh.cn

el.classList.toggle("active")
来源：http://gvr.cashguo.top

[U102] JS：本地存储
来源：http://yjs.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://qdx.jqgufenzy.top

[U103] JS：定时器
来源：http://rem.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zhh.chenjidiqi.icu

[U104] JS：防抖
来源：http://oku.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yuj.hfpthk.cn

[U105] JS：节流
来源：http://nqp.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kow.cdnleiting.top

[U106] JS：日期格式化
来源：http://zdl.cucudq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yhu.0kj1m.cn

[U107] JS：数字千分位
来源：http://yzi.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vqv.chenzaomai.com

[U108] JS：随机整数
来源：http://tip.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ydp.316326.xyz

[U109] JS：数组分组
来源：http://lkf.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://ndr.yueranfly.top

[U110] JS：数组分块
来源：http://tag.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://orn.aizwys.cn

[U111] JS：对象转 Map
来源：http://rkf.yj20258888.top

new Map(Object.entries(obj))
来源：http://idp.epnwcf.com

[U112] JS：字符串补位
来源：http://fmz.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://hgl.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://wdj.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://dyv.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://fdv.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ejh.ydzc1.top

[U115] JS：生成 UUID
来源：http://jdf.snrcjt.cn

crypto.randomUUID()
来源：http://uyz.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://dlg.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://mco.hcnkem.com

[U117] JS：单元测试
来源：http://asu.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://dqi.birdmap.top

[U118] JS：开发服务器
来源：http://jif.sufxvd.cn

npm i -D vite;  npx vite
来源：http://pny.smart0.xyz

[U119] JS：生产构建
来源：http://agy.bbcook.cn

npx vite build
来源：http://ztd.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://vja.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://rsc.shanyushiyangkeji.top

================================================================================
来源：http://cec.fktsv.cn

统计汇总
来源：http://fbi.uphjek.com

================================================================================
来源：http://dsj.jqgfzy.top

按语言统计（条）：
来源：http://vkp.epnwcf.com

Python ......... 252
来源：http://tve.zhaomingkeji.xyz

PHP ............ 252
来源：http://xgf.jlsjyb.cn

JavaScript ..... 252
来源：http://hny.hnxiangtu.top

TypeScript ..... 212
来源：http://qxl.fanxiaobao.xyz

Java ........... 212
来源：http://lla.xylfe.cn

Go ............. 212
来源：http://lbv.yonumen.top

Ruby ........... 212
来源：http://oao.yueranfly.top

C# ............. 212
来源：http://uka.yueranfly.top

C .............. 30
来源：http://tym.tanke756.top

C++ ............ 30
来源：http://nwi.ivvv.top

SQL ............ 90
来源：http://dtj.316326.xyz

Bash ........... 80
来源：http://vit.tianlin.xyz

Kotlin ......... 15
来源：http://wmh.shzxlz.cn

Swift .......... 15
来源：http://wwi.cashguo.top

Lua ............ 10
来源：http://jho.shuidangran.top

Perl ........... 10
来源：http://pkb.dianchejie.cn

Scala .......... 10
来源：http://inz.ywan-chungtsiang.top

------------------------------------
来源：http://kzs.hfpthk.cn

合计 ........... 2106 条
来源：http://xac.vqdsnc.cn

按章节统计：
来源：http://cnt.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qeb.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ztp.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lif.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gwm.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sqi.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qop.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sct.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gph.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mki.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://paj.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nwq.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pnb.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jei.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fes.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://txj.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hqy.wangshuangyany.cn

Q SQL 专题                              90
来源：http://eze.bjfxy.top

R Bash 专题                             80
来源：http://pcu.vqdsnc.cn

S C / C++ 专题                          60
来源：http://vvu.yuanzhike.top

T 其他语言补充                          60
来源：http://jgi.pycfn.com

U 高频实用片段                         120
来源：http://iub.nanxuanxn.top

------------------------------------
来源：http://kua.jyoumei.cn

合计                                  2106 条
来源：http://cks.wangdashe.top

--------------------------------------------------------------------------------
来源：http://uzc.zhijiandao.cn

使用提醒
来源：http://crc.bjfxy.top

--------------------------------------------------------------------------------
来源：http://yrz.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mqz.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lua.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hak.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xys.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://djh.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://kbf.guannengcc.top

================================================================================
来源：http://jvj.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://jln.xylfe.cn

Common Programming Examples Cheat Book
来源：http://ujr.guowangkeji.top

================================================================================
来源：http://xnh.guowangkeji.top

【收录内容】
来源：http://gik.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rka.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rpc.daxiang520.top

SQL · Bash · C · C++
来源：http://jcu.aizwys.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gjt.fktsv.cn

【使用说明】
来源：http://jeq.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fhk.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jlx.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jwo.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ogu.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ivb.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nsp.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://acl.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://exk.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://luo.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zca.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://txo.daxiang520.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dhv.gzhubu.top

【文件统计】
来源：http://uzz.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eur.bjfxy.top

--------------------------------------------------------------------------------
来源：http://nmh.ctjpmb.com

目  录
来源：http://vwz.sysykeji.top

--------------------------------------------------------------------------------
来源：http://rax.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nfe.redwolf501.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vxy.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ukg.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://efq.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://inz.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kfc.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zds.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rnx.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ohg.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kzz.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nat.chenlongwang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xpu.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gxk.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://coo.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bss.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://muv.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zus.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nfo.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bws.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://otw.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hbs.hfpthk.cn

================================================================================
来源：http://xeq.hfpthk.cn

A. 基础语法与类型
来源：http://jdi.yvedp.cn

================================================================================
来源：http://ibp.yj20258888.top

[A01] Hello World
来源：http://ver.nwbrower.top

Py:   print("Hello, World!")
来源：http://wxr.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://qzr.birdmap.top

JS:   console.log("Hello, World!");
来源：http://sqr.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zkd.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://ahc.xinyue.icu

Go:   fmt.Println("Hello, World!")
来源：http://bru.hammf.cn

Ruby: puts "Hello, World!"
来源：http://tsc.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lmb.vehdjk.com

[A02] 变量声明与赋值
来源：http://ndm.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://byr.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oce.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://wck.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qpb.yfazqb.com

Java: String name = "Alex"; int age = 20;
来源：http://mhu.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://ftk.yj20258.top

Ruby: name = "Alex"; age = 20
来源：http://gzq.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://zac.cheryme.top

[A03] 常量定义
来源：http://mjj.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pch.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://bws.mhx1999.top

JS:   const PI = 3.14159;
来源：http://kut.chenjidiqi.icu

TS:   const PI: number = 3.14159;
来源：http://znl.hammf.cn

Java: static final double PI = 3.14159;
来源：http://lbb.yuxming.cn

Go:   const PI = 3.14159
来源：http://lqo.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://yrw.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://zex.dashuyun.cn

[A04] 判断变量类型
来源：http://jkm.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zla.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://twd.vehdjk.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ncd.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://qbg.jiagoushi.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kqx.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://txv.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://srz.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://aie.yueranfly.top

[A05] 整数除法与取模
来源：http://hpq.tianlin.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://man.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://nea.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tuj.fzhhl.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jxx.daria6918.cn

Java: 7 / 2; 7 % 2
来源：http://esp.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://jka.jqgfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://xyo.cashguo.top

C#:   7 / 2; 7 % 2
来源：http://ykn.hammf.cn

[A06] 字符串转数字
来源：http://pzw.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://psx.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ipr.shanyushiyangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jxt.shangyingyoupin.top

TS:   parseInt("42", 10); Number("42")
来源：http://irl.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xpy.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cyw.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bbz.gaohongyu789.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://map.xuanzx.com

[A07] 数字转字符串
来源：http://hkh.kuanghao11.cn

Py:   str(42)
来源：http://owu.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://jud.havefunace.top

JS:   String(42); (42).toString()
来源：http://vvv.zhengqikj.top

TS:   String(42)
来源：http://wmc.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://maa.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://phm.yvedp.cn

Ruby: 42.to_s
来源：http://eyb.haohaochexian.top

C#:   42.ToString()
来源：http://mbm.xziqi.cn

[A08] 取整与四舍五入
来源：http://gju.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gny.dianchejie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tqc.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://faa.ctjpmb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://acs.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fwp.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://omv.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://jxs.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bme.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://plm.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dbi.zdbjq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vll.shanyushiyangtech.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sss.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gje.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rmi.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fbm.dianchejie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mcs.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gvh.jinghuilouyu.cn

[A10] 生成随机数
来源：http://vcm.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://wqh.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://tpg.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sju.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qht.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://sse.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fyj.zhixingplan.top

Ruby: rand(1..100)
来源：http://irw.cqqwz.cn

C#:   new Random().Next(1, 101)
来源：http://qkm.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://zhx.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://npl.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qkx.jlsjyb.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iag.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://dob.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://vim.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xrz.sxryk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ykv.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://vdq.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://dsq.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://koa.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zfw.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://nmp.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://rut.sjlbkw.cn

Java: "Hello, %s!".formatted(name)
来源：http://kwt.316326.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aii.hnqzz.top

Ruby: "Hello, #{name}!"
来源：http://une.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://dmb.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zjm.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://zdn.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://jtr.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://uld.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://zdu.guowangkeji.top

Java: "第一行\n第二行"
来源：http://kft.gzhubu.top

Go:   "第一行\n第二行"
来源：http://cgt.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://ahy.bjfxy.top

C#:   "第一行\n第二行"
来源：http://pbf.ydjk.org.cn


<!-- 参考信息 -->