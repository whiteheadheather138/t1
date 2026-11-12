代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://dfw.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://njr.zdbjq.cn

[U84] JS：CommonJS 写法
来源：http://vrm.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://rks.vqdsnc.cn

[U85] JS：可选链
来源：http://fma.yfazqb.com

a?.b?.c
来源：http://wut.ybcxt.top

[U86] JS：空值合并
来源：http://uwq.mhx1999.top

a ?? b
来源：http://ppd.jlsjyb.cn

[U87] JS：解构默认值
来源：http://uhu.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://axd.yuxming.cn

[U88] JS：对象展开合并
来源：http://uxr.zhongyouzk.top

{ ...a, ...b }
来源：http://agg.bjfxy.top

[U89] JS：数组去重
来源：http://nav.9152youxi.cn

[...new Set(arr)]
来源：http://ezz.redwolf501.top

[U90] JS：数字数组排序
来源：http://ysu.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://sjp.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://elx.redwolf501.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ket.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://qvf.gzhubu.top

structuredClone(obj)
来源：http://wok.zdbjq.cn

[U93] JS：模板字符串
来源：http://vcy.iojbl.cn

`共 ${n} 条`
来源：http://fzq.ybcxt.top

[U94] JS：箭头函数
来源：http://rjh.cucudq.cn

const double = x => x * 2;
来源：http://oii.tarul.cn

[U95] JS：Promise 包装
来源：http://ytj.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://set.epnwcf.com

[U96] JS：async/await 与异常
来源：http://adh.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hxv.yj20258888.top

[U97] JS：并发请求
来源：http://jvd.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ujy.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://ozk.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cls.hywenlv.cn

[U99] JS：事件监听
来源：http://zvt.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://orl.aibaodan.cn

[U100] JS：DOM 查询
来源：http://ria.yonumen.top

document.querySelector(".item")
来源：http://olf.tarul.cn

[U101] JS：classList 操作
来源：http://dvu.zhijiandao.cn

el.classList.toggle("active")
来源：http://hrq.ybcxt.top

[U102] JS：本地存储
来源：http://jix.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zds.ydzc1.top

[U103] JS：定时器
来源：http://zes.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hrj.ybcxt.top

[U104] JS：防抖
来源：http://kqx.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hjb.yj20258888.top

[U105] JS：节流
来源：http://vov.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iij.hammf.cn

[U106] JS：日期格式化
来源：http://rqj.zhixingplan.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yky.ydjk.org.cn

[U107] JS：数字千分位
来源：http://gqf.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xty.wangdashe.top

[U108] JS：随机整数
来源：http://nlt.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pju.tian-w.cn

[U109] JS：数组分组
来源：http://mel.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://bzm.yueranfly.top

[U110] JS：数组分块
来源：http://drs.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nmx.andypj.xyz

[U111] JS：对象转 Map
来源：http://hei.c1oappe.top

new Map(Object.entries(obj))
来源：http://rrx.zhongyouzk.top

[U112] JS：字符串补位
来源：http://rkh.jianghu66.top

"7".padStart(3, "0")
来源：http://kmz.316326.xyz

[U113] JS：正则替换全部
来源：http://evp.mhx1999.top

s.replaceAll("a", "b")
来源：http://ile.tian-w.cn

[U114] JS：JSON 深比较
来源：http://mvu.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://joi.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://wfm.zhengqikj.top

crypto.randomUUID()
来源：http://zuw.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://zke.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://qrg.wangdashe.top

[U117] JS：单元测试
来源：http://khl.cheryme.top

npm i -D vitest;  npx vitest
来源：http://xsl.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://vot.tarul.cn

npm i -D vite;  npx vite
来源：http://qfk.aizwys.cn

[U119] JS：生产构建
来源：http://ywt.chenlongwang.top

npx vite build
来源：http://zdf.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://hqg.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://gzd.xziqi.cn

================================================================================
来源：http://tgy.yangfankeji.com

统计汇总
来源：http://hil.ehwqpu.com

================================================================================
来源：http://wsr.wangdashe.top

按语言统计（条）：
来源：http://izg.shzxlz.cn

Python ......... 252
来源：http://pmm.hnqzz.top

PHP ............ 252
来源：http://qkb.zhengqikj.top

JavaScript ..... 252
来源：http://qde.pycfn.com

TypeScript ..... 212
来源：http://yim.yfazqb.com

Java ........... 212
来源：http://vso.zdbjq.cn

Go ............. 212
来源：http://nnh.ywan-chungtsiang.top

Ruby ........... 212
来源：http://fiy.yonumen.top

C# ............. 212
来源：http://gqy.hnxiangtu.top

C .............. 30
来源：http://leb.wangdashe.top

C++ ............ 30
来源：http://ynk.tanke756.top

SQL ............ 90
来源：http://vel.smart0.xyz

Bash ........... 80
来源：http://pvv.ydjk.org.cn

Kotlin ......... 15
来源：http://dgl.ppjwa.cn

Swift .......... 15
来源：http://vtb.zhaomingkeji.xyz

Lua ............ 10
来源：http://wpx.jqgfzy.top

Perl ........... 10
来源：http://ibg.zhaomingkeji.xyz

Scala .......... 10
来源：http://syi.vqdsnc.cn

------------------------------------
来源：http://xwm.gzhubu.top

合计 ........... 2106 条
来源：http://ugu.yongpay.top

按章节统计：
来源：http://exb.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gti.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hjb.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vnq.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jhp.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zcj.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ldr.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hxf.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://syp.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yes.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ucu.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kiz.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ret.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dqa.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qlu.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jhr.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jpf.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://tys.zdbjq.cn

R Bash 专题                             80
来源：http://dej.daria6918.cn

S C / C++ 专题                          60
来源：http://due.yj202588.top

T 其他语言补充                          60
来源：http://hje.yongpay.top

U 高频实用片段                         120
来源：http://lwc.dianchejie.cn

------------------------------------
来源：http://rrt.bjfxy.top

合计                                  2106 条
来源：http://hpj.xinyue.icu

--------------------------------------------------------------------------------
来源：http://ibg.zhaomingkeji.xyz

使用提醒
来源：http://zah.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://csx.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fgb.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://trj.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uuk.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://aie.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pol.cheryme.top

—— 文件结束 ——
来源：http://fvq.52xcode.cn

================================================================================
来源：http://fnu.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://vpn.pycfn.com

Common Programming Examples Cheat Book
来源：http://noh.wangshuangyany.cn

================================================================================
来源：http://suj.jinqigfzy.top

【收录内容】
来源：http://dqv.guannengcc.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://egn.pycfn.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://noi.kuanghao11.cn

SQL · Bash · C · C++
来源：http://mdw.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zmh.zhijiandao.cn

【使用说明】
来源：http://gae.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qrr.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ieu.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jla.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vhr.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gil.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ysw.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xal.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://skw.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bdb.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wxn.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tix.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://huc.ctjpmb.com

【文件统计】
来源：http://crn.ybcxt.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hyn.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://gch.bjfxy.top

目  录
来源：http://twn.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://phe.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qzs.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vln.gzhubu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tko.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sxg.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hwx.jlsjyb.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wnw.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jcl.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://odm.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gwx.xziqi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aco.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lwq.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uuj.mhx1999.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cxw.zhiwuduotai.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jjn.zhengqikj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://and.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yuv.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wtu.shanyushiyangtech.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ejd.zhongyouzk.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lej.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nbf.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ebw.wangshuangyany.cn

================================================================================
来源：http://tzn.nanxinkj.top

A. 基础语法与类型
来源：http://jkh.c1oappe.top

================================================================================
来源：http://lrz.shuidangran.top

[A01] Hello World
来源：http://ghq.smart0.xyz

Py:   print("Hello, World!")
来源：http://omx.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://eyr.hongshengwenyu.top

JS:   console.log("Hello, World!");
来源：http://okv.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qlo.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://udj.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://dgc.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://qvl.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fgk.xingfuxueyuan.xyz

[A02] 变量声明与赋值
来源：http://xxt.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://upz.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xld.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://quz.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xeg.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://peo.sweek.top

Go:   name := "Alex"; age := 20
来源：http://nuv.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://tyy.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://lnw.guannengcc.top

[A03] 常量定义
来源：http://eie.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fsb.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://xvm.fzhhl.top

JS:   const PI = 3.14159;
来源：http://wtk.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://brt.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://psu.yangfankeji.com

Go:   const PI = 3.14159
来源：http://rqm.9152youxi.cn

Ruby: PI = 3.14159
来源：http://cqr.gaohongyu789.top

C#:   const double PI = 3.14159;
来源：http://kki.yangfankeji.com

[A04] 判断变量类型
来源：http://tir.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lra.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nqb.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://awx.shanyushiyangtech.top

TS:   typeof x; x instanceof Date
来源：http://nlu.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://spc.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://drc.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://noq.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://htt.tarul.cn

[A05] 整数除法与取模
来源：http://pio.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xbt.dianchejie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rxi.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jsi.iojbl.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ouo.jiagoushi.top

Java: 7 / 2; 7 % 2
来源：http://jjt.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://wme.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://ine.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://tij.zhengqikj.top

[A06] 字符串转数字
来源：http://gbc.havefunace.top

Py:   int("42"); float("3.14")
来源：http://xhc.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rgl.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://usd.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://koe.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jpp.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jgh.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kpg.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://owr.zhoulong.xyz

[A07] 数字转字符串
来源：http://jvx.gogol.net.cn

Py:   str(42)
来源：http://quy.sufxvd.cn

PHP:  (string) 42; strval(42)
来源：http://xks.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://imd.c1oappe.top

TS:   String(42)
来源：http://axv.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ecu.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://oct.cheryme.top

Ruby: 42.to_s
来源：http://bfu.havefunace.top

C#:   42.ToString()
来源：http://nyk.yongpay.top

[A08] 取整与四舍五入
来源：http://fli.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bki.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tvo.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://orw.yfazqb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ktg.zdbjq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://irv.feifeiyinyue.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://drw.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yrz.uphjek.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fpu.sweek.top

[A09] 绝对值与最大最小值
来源：http://uat.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xcv.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ehz.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://axj.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gdp.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rmb.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oqr.hnxiangtu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ttr.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ayr.dashuyun.cn

[A10] 生成随机数
来源：http://rsv.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://exd.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://lzg.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mbx.havefunace.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xem.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://unc.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ixv.dashuyun.cn

Ruby: rand(1..100)
来源：http://jiz.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://yig.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://qib.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://ied.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qzo.hnqzz.top

JS:   x > 0 ? "yes" : "no"
来源：http://qfv.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sfd.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://usi.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://nkj.fktsv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://krx.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ggz.hcnkem.com

[A12] 字符串插值 / 格式化
来源：http://gin.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blw.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cvj.yj202588.top

JS:   `Hello, ${name}!`
来源：http://tgu.birdmap.top

TS:   `Hello, ${name}!`
来源：http://aic.daria6918.cn

Java: "Hello, %s!".formatted(name)
来源：http://rcr.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://smb.snrcjt.cn

Ruby: "Hello, #{name}!"
来源：http://ttp.ydzc1.top

C#:   $"Hello, {name}!"
来源：http://ctd.xylfe.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zew.xylfe.cn

Py:   "第一行\n第二行"
来源：http://rau.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://ypu.yj20258888.top

JS:   "第一行\n第二行"
来源：http://kbl.vqdsnc.cn

TS:   "第一行\n第二行"
来源：http://kri.zdbjq.cn

Java: "第一行\n第二行"
来源：http://iug.sxryk.cn

Go:   "第一行\n第二行"
来源：http://eub.316326.xyz

Ruby: "第一行\n第二行"
来源：http://aox.sweek.top

C#:   "第一行\n第二行"
来源：http://iea.xuetiantiany.cn


<!-- 参考信息 -->