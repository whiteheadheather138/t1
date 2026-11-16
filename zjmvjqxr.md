代发 wailian999

[U81] JS：初始化项目
来源：http://azx.yj202588.top

npm init -y;  npm i express
来源：http://trt.guannengcc.top

[U82] JS：package.json 脚本
来源：http://qhr.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://awi.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://pix.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://jpd.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://mii.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://spv.yfazqb.com

[U85] JS：可选链
来源：http://atm.hfpthk.cn

a?.b?.c
来源：http://haf.ivvv.top

[U86] JS：空值合并
来源：http://eci.zhoulong.xyz

a ?? b
来源：http://dyz.jiagoushi.top

[U87] JS：解构默认值
来源：http://vsg.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://xtp.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://dxm.sjlbkw.cn

{ ...a, ...b }
来源：http://ekq.hongshengwenyu.top

[U89] JS：数组去重
来源：http://eyl.yj20258888.top

[...new Set(arr)]
来源：http://xvs.smart0.xyz

[U90] JS：数字数组排序
来源：http://jie.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://kbm.fktsv.cn

[U91] JS：对象键值遍历
来源：http://trp.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bif.kuanghao11.cn

[U92] JS：深拷贝
来源：http://iba.fzhhl.top

structuredClone(obj)
来源：http://izc.xziqi.cn

[U93] JS：模板字符串
来源：http://smd.sxryk.cn

`共 ${n} 条`
来源：http://cti.zhengqikj.top

[U94] JS：箭头函数
来源：http://gsa.9152youxi.cn

const double = x => x * 2;
来源：http://ocl.jiagoushi.top

[U95] JS：Promise 包装
来源：http://rmq.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://cel.c1oappe.top

[U96] JS：async/await 与异常
来源：http://pfi.zhijiandao.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zod.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://qas.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pio.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://xom.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vzx.gzhubu.top

[U99] JS：事件监听
来源：http://npt.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://dsf.hesvh.cn

[U100] JS：DOM 查询
来源：http://pqt.yanxiufei.cn

document.querySelector(".item")
来源：http://ypk.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://jev.aizwys.cn

el.classList.toggle("active")
来源：http://ely.guannengcc.top

[U102] JS：本地存储
来源：http://mki.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nfa.hongshengwenyu.top

[U103] JS：定时器
来源：http://fej.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cko.316326.xyz

[U104] JS：防抖
来源：http://xqo.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnz.xinyue.icu

[U105] JS：节流
来源：http://jiw.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wes.uphjek.com

[U106] JS：日期格式化
来源：http://uwk.ydjk.org.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://twr.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://yni.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xwy.aizwys.cn

[U108] JS：随机整数
来源：http://bro.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dzx.daria6918.cn

[U109] JS：数组分组
来源：http://zji.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://mqv.yfazqb.com

[U110] JS：数组分块
来源：http://syy.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tup.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://tpz.hywenlv.cn

new Map(Object.entries(obj))
来源：http://tpd.epnwcf.com

[U112] JS：字符串补位
来源：http://evd.ivvv.top

"7".padStart(3, "0")
来源：http://mlm.9152youxi.cn

[U113] JS：正则替换全部
来源：http://esp.hysaishi.cn

s.replaceAll("a", "b")
来源：http://ezt.daria6918.cn

[U114] JS：JSON 深比较
来源：http://aow.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qcl.xuanzx.com

[U115] JS：生成 UUID
来源：http://cza.fehbvm.com

crypto.randomUUID()
来源：http://abd.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://kdv.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://oxp.sweek.top

[U117] JS：单元测试
来源：http://lbz.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://apl.bbcook.cn

[U118] JS：开发服务器
来源：http://pjp.snrcjt.cn

npm i -D vite;  npx vite
来源：http://lmu.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://qia.jqgfzy.top

npx vite build
来源：http://nwi.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://nae.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://mxq.nanxuanxn.top

================================================================================
来源：http://vxz.gogol.net.cn

统计汇总
来源：http://hjl.hywenlv.cn

================================================================================
来源：http://ixa.chenlongwang.top

按语言统计（条）：
来源：http://ask.yueranfly.top

Python ......... 252
来源：http://ogv.jlsjyb.cn

PHP ............ 252
来源：http://baa.jqgfzy.top

JavaScript ..... 252
来源：http://rdl.zdbjq.cn

TypeScript ..... 212
来源：http://kxp.yonumen.top

Java ........... 212
来源：http://iiy.hnxiangtu.top

Go ............. 212
来源：http://yyn.cashguo.top

Ruby ........... 212
来源：http://jli.daxiang520.top

C# ............. 212
来源：http://qrb.jqgufenzy.top

C .............. 30
来源：http://fdm.yuanzhike.top

C++ ............ 30
来源：http://vqb.hywenlv.cn

SQL ............ 90
来源：http://wtt.yongpay.top

Bash ........... 80
来源：http://hcu.redwolf501.top

Kotlin ......... 15
来源：http://njc.havefunace.top

Swift .......... 15
来源：http://btq.redwolf501.top

Lua ............ 10
来源：http://qzk.52xcode.cn

Perl ........... 10
来源：http://pmw.daxiang520.top

Scala .......... 10
来源：http://fbp.kuanghao11.cn

------------------------------------
来源：http://pfi.kuanghao11.cn

合计 ........... 2106 条
来源：http://dpn.hongshengwenyu.top

按章节统计：
来源：http://coc.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jty.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xgf.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jhk.epnwcf.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://epe.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wff.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://csl.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://evl.zhijiandao.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tcn.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://waw.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://acb.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gji.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jxa.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bpu.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mti.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xjb.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uyt.0kj1m.cn

Q SQL 专题                              90
来源：http://wpy.zycfv.cn

R Bash 专题                             80
来源：http://vgs.hesvh.cn

S C / C++ 专题                          60
来源：http://swf.fktsv.cn

T 其他语言补充                          60
来源：http://txv.zhongyouzk.top

U 高频实用片段                         120
来源：http://wni.xinyue.icu

------------------------------------
来源：http://vzw.meibo888.top

合计                                  2106 条
来源：http://scc.iojbl.cn

--------------------------------------------------------------------------------
来源：http://tcx.xziqi.cn

使用提醒
来源：http://phm.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://dzj.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vwt.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zvs.xingfuxueyuan.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ybb.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uqt.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uju.hammf.cn

—— 文件结束 ——
来源：http://iks.ivvv.top

================================================================================
来源：http://gug.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://gzc.yj202588.top

Common Programming Examples Cheat Book
来源：http://kat.jlsjyb.cn

================================================================================
来源：http://bck.yanxiufei.cn

【收录内容】
来源：http://tud.zhiwuduotai.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jwp.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cjf.zycfv.cn

SQL · Bash · C · C++
来源：http://vbw.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baj.tanke756.top

【使用说明】
来源：http://umv.hnqzz.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bbq.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://odp.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nfs.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://akt.shzxlz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jtn.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sij.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gzi.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rll.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://udx.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://als.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://frs.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nhi.zhixingplan.top

【文件统计】
来源：http://aqz.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bie.fktsv.cn

--------------------------------------------------------------------------------
来源：http://zxb.vqdsnc.cn

目  录
来源：http://mzs.sxryk.cn

--------------------------------------------------------------------------------
来源：http://ivw.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://frn.kuanghao11.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://row.jinghuilouyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rjb.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vea.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zsm.jinyuanbaomall.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iuh.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hci.yuxming.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nkr.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://arr.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://plq.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aaq.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pwh.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tux.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yvh.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fbs.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ale.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ivj.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://huu.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rsa.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://skg.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cei.ywan-chungtsiang.top

================================================================================
来源：http://rjy.hnxiangtu.top

A. 基础语法与类型
来源：http://ath.yonumen.top

================================================================================
来源：http://flj.jiagoushi.top

[A01] Hello World
来源：http://zrf.hongshengwenyu.top

Py:   print("Hello, World!")
来源：http://iey.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://npl.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://atk.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mgl.uphjek.com

Java: System.out.println("Hello, World!");
来源：http://env.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://ztz.feifeiyinyue.top

Ruby: puts "Hello, World!"
来源：http://zpa.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jhi.jianghu66.top

[A02] 变量声明与赋值
来源：http://doj.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wow.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wwp.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://jmj.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vjj.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://mje.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://nbu.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://usf.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://vld.epnwcf.com

[A03] 常量定义
来源：http://xxl.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jgd.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://mgp.zhixingplan.top

JS:   const PI = 3.14159;
来源：http://hqd.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://vzo.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://rbk.cashguo.top

Go:   const PI = 3.14159
来源：http://mvy.cqqwz.cn

Ruby: PI = 3.14159
来源：http://dto.guowangkeji.top

C#:   const double PI = 3.14159;
来源：http://llq.316326.xyz

[A04] 判断变量类型
来源：http://mtf.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gol.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tqi.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://alh.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://xtp.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mye.zhaomingkeji.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://uol.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ncz.yanxiufei.cn

C#:   x.GetType().Name; x is int
来源：http://gxh.zhengqikj.top

[A05] 整数除法与取模
来源：http://eve.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ajd.dianchejie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lan.vqdsnc.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xvx.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vqs.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://tfv.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://pso.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://ocv.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://mjd.tian-w.cn

[A06] 字符串转数字
来源：http://vog.pycfn.com

Py:   int("42"); float("3.14")
来源：http://qts.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xby.snrcjt.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oyb.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://jsb.xylfe.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xvo.chenlongwang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yof.jinghuilouyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wxa.zhaomingkeji.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ywu.xylfe.cn

[A07] 数字转字符串
来源：http://jse.wangshuangyany.cn

Py:   str(42)
来源：http://ywx.gaohongyu789.top

PHP:  (string) 42; strval(42)
来源：http://dsj.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://dat.zdbjq.cn

TS:   String(42)
来源：http://yms.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ybj.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://erl.sxryk.cn

Ruby: 42.to_s
来源：http://mso.52xcode.cn

C#:   42.ToString()
来源：http://ihk.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://vai.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ggh.0kj1m.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ora.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mkf.xinyue.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gug.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pqg.shuidangran.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://akh.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vjc.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvp.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://rbt.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bjx.fehbvm.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mqw.uphjek.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://skq.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tmn.shuidangran.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aaw.yvedp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wqy.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xte.birdmap.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://imr.9152youxi.cn

[A10] 生成随机数
来源：http://mnf.xziqi.cn

Py:   import random; random.randint(1, 100)
来源：http://cwq.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://eab.xingfuxueyuan.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://koj.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zpb.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://gvp.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vts.zycfv.cn

Ruby: rand(1..100)
来源：http://srd.0kj1m.cn

C#:   new Random().Next(1, 101)
来源：http://gop.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://uvg.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://hlu.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qin.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://pff.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://eew.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://oqu.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://utf.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kme.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://adl.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://oeo.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://omf.svipenyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ttn.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://wno.meibo888.top

TS:   `Hello, ${name}!`
来源：http://yfy.zdqjudy.top

Java: "Hello, %s!".formatted(name)
来源：http://orf.xylfe.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gpz.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://mao.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://lzo.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jbd.cheryme.top

Py:   "第一行\n第二行"
来源：http://zmu.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://rou.andypj.xyz

JS:   "第一行\n第二行"
来源：http://fds.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://ajv.jlsjyb.cn


<!-- 参考信息 -->