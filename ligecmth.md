代发 wailian999

[U81] JS：初始化项目
来源：http://zvp.sxryk.cn

npm init -y;  npm i express
来源：http://nqy.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://mac.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uaz.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://dhr.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://rtf.pycfn.com

[U84] JS：CommonJS 写法
来源：http://tbn.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wvd.aibaodan.cn

[U85] JS：可选链
来源：http://yyq.cheryme.top

a?.b?.c
来源：http://nkn.yj202588.top

[U86] JS：空值合并
来源：http://krm.cucudq.cn

a ?? b
来源：http://hps.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://lxq.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://smp.fzhhl.top

[U88] JS：对象展开合并
来源：http://olh.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://hxe.jlsjyb.cn

[U89] JS：数组去重
来源：http://ldo.feifeiyinyue.top

[...new Set(arr)]
来源：http://kbe.ybcxt.top

[U90] JS：数字数组排序
来源：http://rys.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://jsw.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://wyn.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bhl.aibaodan.cn

[U92] JS：深拷贝
来源：http://mjs.52xcode.cn

structuredClone(obj)
来源：http://vva.fzhhl.top

[U93] JS：模板字符串
来源：http://gpr.haohaochexian.top

`共 ${n} 条`
来源：http://inu.hnqzz.top

[U94] JS：箭头函数
来源：http://tzd.redwolf501.top

const double = x => x * 2;
来源：http://dio.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://qcd.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://osf.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://xcs.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dzr.ydjk.org.cn

[U97] JS：并发请求
来源：http://zpd.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yql.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://gtp.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gas.chenlongwang.top

[U99] JS：事件监听
来源：http://cuq.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://vyv.zdqjudy.top

[U100] JS：DOM 查询
来源：http://rnx.nanxuanxn.top

document.querySelector(".item")
来源：http://dsk.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://azq.hcnkem.com

el.classList.toggle("active")
来源：http://rfn.chenzaomai.com

[U102] JS：本地存储
来源：http://kqd.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnk.zhijiandao.cn

[U103] JS：定时器
来源：http://azl.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aea.yangfankeji.com

[U104] JS：防抖
来源：http://lkx.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irw.yonumen.top

[U105] JS：节流
来源：http://vqj.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ckh.bjfxy.top

[U106] JS：日期格式化
来源：http://rvt.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://asu.daxiang520.top

[U107] JS：数字千分位
来源：http://gzl.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gnb.yj20258.top

[U108] JS：随机整数
来源：http://nfx.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pgy.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://rjl.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://zlw.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://ezv.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://znx.wangdashe.top

[U111] JS：对象转 Map
来源：http://loj.yangfankeji.com

new Map(Object.entries(obj))
来源：http://yye.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://zuj.aizwys.cn

"7".padStart(3, "0")
来源：http://dov.snrcjt.cn

[U113] JS：正则替换全部
来源：http://vnp.guannengcc.top

s.replaceAll("a", "b")
来源：http://mnc.daria6918.cn

[U114] JS：JSON 深比较
来源：http://pbz.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zvd.birdmap.top

[U115] JS：生成 UUID
来源：http://zhm.kuanghao11.cn

crypto.randomUUID()
来源：http://ltb.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://yhk.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://xne.chenjidiqi.icu

[U117] JS：单元测试
来源：http://gjb.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://ctl.tian-w.cn

[U118] JS：开发服务器
来源：http://xhv.dianchejie.cn

npm i -D vite;  npx vite
来源：http://dow.chenlongwang.top

[U119] JS：生产构建
来源：http://hvy.sysykeji.top

npx vite build
来源：http://kxi.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://kie.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://xqp.xingfuxueyuan.xyz

================================================================================
来源：http://nla.nanxinkj.top

统计汇总
来源：http://ttz.sweek.top

================================================================================
来源：http://ncc.shzxlz.cn

按语言统计（条）：
来源：http://zof.sufxvd.cn

Python ......... 252
来源：http://bdw.ehwqpu.com

PHP ............ 252
来源：http://ggm.zdbjq.cn

JavaScript ..... 252
来源：http://lzd.ivvv.top

TypeScript ..... 212
来源：http://mtt.zhixingplan.top

Java ........... 212
来源：http://jns.hesvh.cn

Go ............. 212
来源：http://efq.pengpengdd.cyou

Ruby ........... 212
来源：http://ckl.kuanghao11.cn

C# ............. 212
来源：http://pva.zhiwuduotai.top

C .............. 30
来源：http://cdj.chenzaomai.com

C++ ............ 30
来源：http://nhi.epnwcf.com

SQL ............ 90
来源：http://fbw.zhoulong.xyz

Bash ........... 80
来源：http://zkn.daria6918.cn

Kotlin ......... 15
来源：http://rsq.cqqwz.cn

Swift .......... 15
来源：http://eke.hywenlv.cn

Lua ............ 10
来源：http://sba.sysykeji.top

Perl ........... 10
来源：http://grv.yj20258.top

Scala .......... 10
来源：http://gmg.hfpthk.cn

------------------------------------
来源：http://sfi.jlsjyb.cn

合计 ........... 2106 条
来源：http://cxt.xuetiantiany.cn

按章节统计：
来源：http://azg.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ryr.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ybn.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pzi.ctjpmb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ozq.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hoh.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tdb.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uam.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uap.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zjw.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uil.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ipx.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hat.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yer.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fzz.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pkn.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dex.zhijiandao.cn

Q SQL 专题                              90
来源：http://pnf.svipenyu.cn

R Bash 专题                             80
来源：http://jtq.sxryk.cn

S C / C++ 专题                          60
来源：http://xtw.zhengqikj.top

T 其他语言补充                          60
来源：http://xqx.jqgufenzy.top

U 高频实用片段                         120
来源：http://olb.zhongyouzk.top

------------------------------------
来源：http://cjt.ybcxt.top

合计                                  2106 条
来源：http://lny.mhx1999.top

--------------------------------------------------------------------------------
来源：http://qan.ydjk.org.cn

使用提醒
来源：http://kgo.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://oca.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ydh.iojbl.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jxf.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aom.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://grz.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bbc.svipenyu.cn

—— 文件结束 ——
来源：http://ijc.shanyushiyangtech.top

================================================================================
来源：http://txi.yongpay.top

程序语言常见例子速查手册（2024 版）
来源：http://ddn.zhoulong.xyz

Common Programming Examples Cheat Book
来源：http://ucc.pengpengdd.cyou

================================================================================
来源：http://qxi.ydzc1.top

【收录内容】
来源：http://dgq.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://xhf.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kky.nanxuanxn.top

SQL · Bash · C · C++
来源：http://xfv.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ddm.epnwcf.com

【使用说明】
来源：http://tmk.zycfv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lxc.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iqw.xziqi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rmq.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zbi.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gjo.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jif.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uhz.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pnn.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qfp.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yeo.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mff.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aea.jlsjyb.cn

【文件统计】
来源：http://ybp.yfazqb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cig.jianghu66.top

--------------------------------------------------------------------------------
来源：http://uox.epnwcf.com

目  录
来源：http://ldl.birdmap.top

--------------------------------------------------------------------------------
来源：http://ylm.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ihw.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lkz.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xjw.jinqigfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ycm.yongpay.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rev.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kko.dashuyun.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jeu.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jro.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tjm.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kny.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eqs.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wja.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://utq.haohaochexian.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bnj.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ouw.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ebc.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jgq.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://znr.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://apu.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tnp.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kto.cheryme.top

================================================================================
来源：http://rku.shanyushiyangkeji.top

A. 基础语法与类型
来源：http://kon.daria6918.cn

================================================================================
来源：http://qsp.aibaodan.cn

[A01] Hello World
来源：http://vov.yfazqb.com

Py:   print("Hello, World!")
来源：http://xdo.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://qci.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://ivq.feifeiyinyue.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yhs.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://ddu.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://nqg.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://psv.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://bwk.chenzaomai.com

[A02] 变量声明与赋值
来源：http://omd.bbcook.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qhx.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://reo.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://yos.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qdt.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://vsd.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://lct.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://mkg.ydjk.org.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gir.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://dde.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bfh.dianchejie.cn

PHP:  const PI = 3.14159;
来源：http://iel.fengsongda.top

JS:   const PI = 3.14159;
来源：http://cng.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://ewd.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://hgq.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://thg.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://yem.zhoulong.xyz

C#:   const double PI = 3.14159;
来源：http://olh.hfpthk.cn

[A04] 判断变量类型
来源：http://ebc.snrcjt.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pgs.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://btp.yvedp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qno.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://fiz.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dja.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zab.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sca.c1oappe.top

C#:   x.GetType().Name; x is int
来源：http://rcq.fzhhl.top

[A05] 整数除法与取模
来源：http://lcv.jinqigufen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lzf.chenzaomai.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://bvm.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://krq.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rld.cqqwz.cn

Java: 7 / 2; 7 % 2
来源：http://zwn.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://uza.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://tku.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://gyf.0kj1m.cn

[A06] 字符串转数字
来源：http://kpn.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://hjc.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://viq.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzw.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://bxg.zdbjq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bld.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dlv.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xlb.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eyo.cqqwz.cn

[A07] 数字转字符串
来源：http://vuf.zhengqikj.top

Py:   str(42)
来源：http://vmk.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://unf.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://ewb.yj20258.top

TS:   String(42)
来源：http://pvx.haohaochexian.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ucw.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://ftm.zhixingplan.top

Ruby: 42.to_s
来源：http://hzo.shuidangran.top

C#:   42.ToString()
来源：http://oqq.yvedp.cn

[A08] 取整与四舍五入
来源：http://fvy.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://svc.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hfs.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://llq.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dfc.sweek.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lbr.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xsu.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jwx.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ahj.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://cqw.sjlbkw.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rwo.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hzd.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://whu.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ava.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hld.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ygl.zycfv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://das.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://emg.zdbjq.cn

[A10] 生成随机数
来源：http://zic.gzhubu.top

Py:   import random; random.randint(1, 100)
来源：http://zzy.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://rbo.jqgfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aje.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gpp.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://igm.smart0.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jhj.yonumen.top

Ruby: rand(1..100)
来源：http://ywn.tianlin.xyz

C#:   new Random().Next(1, 101)
来源：http://bbo.guannengcc.top

[A11] 条件表达式（三元）
来源：http://nnk.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://nna.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pxr.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://dxz.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://aty.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://lbz.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://liu.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bfh.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kla.xuetiantiany.cn

[A12] 字符串插值 / 格式化
来源：http://rfx.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://utf.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ywj.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://gdm.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://vah.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://apd.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://udm.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://mxg.guannengcc.top

C#:   $"Hello, {name}!"
来源：http://gfw.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qzf.bjfxy.top

Py:   "第一行\n第二行"
来源：http://nwo.0kj1m.cn

PHP:  "第一行\n第二行"
来源：http://hrr.zhengqikj.top

JS:   "第一行\n第二行"
来源：http://ask.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://goj.wangdashe.top


<!-- 参考信息 -->