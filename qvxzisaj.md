代发 wailian999

[U87] JS：解构默认值
来源：http://zkn.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://mpr.nwbrower.top

[U88] JS：对象展开合并
来源：http://mem.316326.xyz

{ ...a, ...b }
来源：http://qeh.xinyue.icu

[U89] JS：数组去重
来源：http://vnl.xylfe.cn

[...new Set(arr)]
来源：http://dlr.andypj.xyz

[U90] JS：数字数组排序
来源：http://xnp.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://mjt.mhx1999.top

[U91] JS：对象键值遍历
来源：http://bov.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lki.52xcode.cn

[U92] JS：深拷贝
来源：http://ksi.havefunace.top

structuredClone(obj)
来源：http://wcn.vehdjk.com

[U93] JS：模板字符串
来源：http://nuo.yangfankeji.com

`共 ${n} 条`
来源：http://wnu.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://rtq.zhongyouzk.top

const double = x => x * 2;
来源：http://qhg.bjfxy.top

[U95] JS：Promise 包装
来源：http://cir.havefunace.top

new Promise((resolve, reject) => {})
来源：http://bqk.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://bht.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hue.tanke756.top

[U97] JS：并发请求
来源：http://bxf.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eun.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://nmg.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lor.zhijiandao.cn

[U99] JS：事件监听
来源：http://dbx.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://jeo.tian-w.cn

[U100] JS：DOM 查询
来源：http://leh.daxiang520.top

document.querySelector(".item")
来源：http://txa.sjlbkw.cn

[U101] JS：classList 操作
来源：http://tgv.xuetiantiany.cn

el.classList.toggle("active")
来源：http://cov.0kj1m.cn

[U102] JS：本地存储
来源：http://ucc.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://usu.sysykeji.top

[U103] JS：定时器
来源：http://nbt.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hqg.wangshuangyany.cn

[U104] JS：防抖
来源：http://uyz.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ish.sysykeji.top

[U105] JS：节流
来源：http://mtn.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jbc.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://vag.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://upf.jyoumei.cn

[U107] JS：数字千分位
来源：http://iri.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://exo.feifeiyinyue.top

[U108] JS：随机整数
来源：http://adz.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qwi.dashuyun.cn

[U109] JS：数组分组
来源：http://exw.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://oxe.ybcxt.top

[U110] JS：数组分块
来源：http://cmh.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vio.meibo888.top

[U111] JS：对象转 Map
来源：http://eys.ydzc1.top

new Map(Object.entries(obj))
来源：http://shg.nwbrower.top

[U112] JS：字符串补位
来源：http://pxd.birdmap.top

"7".padStart(3, "0")
来源：http://fzd.bbcook.cn

[U113] JS：正则替换全部
来源：http://wdg.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://jqf.smart0.xyz

[U114] JS：JSON 深比较
来源：http://qkh.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jib.hammf.cn

[U115] JS：生成 UUID
来源：http://rlc.52xcode.cn

crypto.randomUUID()
来源：http://gin.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://wwg.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://xfv.haohaochexian.top

[U117] JS：单元测试
来源：http://vis.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://kef.shuidangran.top

[U118] JS：开发服务器
来源：http://piq.iojbl.cn

npm i -D vite;  npx vite
来源：http://ebd.nwbrower.top

[U119] JS：生产构建
来源：http://mqd.sufxvd.cn

npx vite build
来源：http://eao.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://qjj.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://yoo.chenjidiqi.icu

================================================================================
来源：http://tzm.redwolf501.top

统计汇总
来源：http://npz.shanyushiyangkeji.top

================================================================================
来源：http://dim.andypj.xyz

按语言统计（条）：
来源：http://hbr.guowangkeji.top

Python ......... 252
来源：http://bma.pengpengdd.cyou

PHP ............ 252
来源：http://gak.xuanzx.com

JavaScript ..... 252
来源：http://sbj.zdbjq.cn

TypeScript ..... 212
来源：http://yyv.wangshuangyany.cn

Java ........... 212
来源：http://owq.hcnkem.com

Go ............. 212
来源：http://obi.hcnkem.com

Ruby ........... 212
来源：http://utz.svipenyu.cn

C# ............. 212
来源：http://qtt.iojbl.cn

C .............. 30
来源：http://vdq.shangyingyoupin.top

C++ ............ 30
来源：http://ffd.bbcook.cn

SQL ............ 90
来源：http://kfo.fehbvm.com

Bash ........... 80
来源：http://glg.daria6918.cn

Kotlin ......... 15
来源：http://kcs.xylfe.cn

Swift .......... 15
来源：http://kmx.hongshengwenyu.top

Lua ............ 10
来源：http://bmh.316326.xyz

Perl ........... 10
来源：http://lov.ppjwa.cn

Scala .......... 10
来源：http://uht.chenzaomai.com

------------------------------------
来源：http://llg.zhijiandao.cn

合计 ........... 2106 条
来源：http://fpy.tanke756.top

按章节统计：
来源：http://ity.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jgf.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bju.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hii.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dnu.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pto.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lwp.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sel.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ofp.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gof.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ann.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://exb.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nxl.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pps.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oyf.yvedp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xes.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oaf.andypj.xyz

Q SQL 专题                              90
来源：http://nnj.hysaishi.cn

R Bash 专题                             80
来源：http://kti.hcnkem.com

S C / C++ 专题                          60
来源：http://wul.gzhubu.top

T 其他语言补充                          60
来源：http://bnz.chenlongwang.top

U 高频实用片段                         120
来源：http://jrq.pycfn.com

------------------------------------
来源：http://tvb.zhongyouzk.top

合计                                  2106 条
来源：http://szd.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://akq.yj20258.top

使用提醒
来源：http://ebz.fktsv.cn

--------------------------------------------------------------------------------
来源：http://rxo.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ffd.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://arp.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jok.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://qxg.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://idt.c1oappe.top

—— 文件结束 ——
来源：http://lxy.ybcxt.top

================================================================================
来源：http://ctt.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://yxw.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://ybm.yangfankeji.com

================================================================================
来源：http://jmz.yonumen.top

【收录内容】
来源：http://ixc.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://glc.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ezi.jinqigfzy.top

SQL · Bash · C · C++
来源：http://rzy.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ktu.smart0.xyz

【使用说明】
来源：http://yyy.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ahw.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://flx.0kj1m.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ytr.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nfc.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kmk.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nuw.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ibn.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vnw.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gbl.cqqwz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nqu.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lzi.redwolf501.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sro.iojbl.cn

【文件统计】
来源：http://qnb.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rju.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://ixs.sufxvd.cn

目  录
来源：http://ptp.bbcook.cn

--------------------------------------------------------------------------------
来源：http://xig.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sqr.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fhu.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://coe.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tqc.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://stu.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tjn.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ifh.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fdv.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bmw.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ewb.hcnkem.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cvp.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://orq.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://enc.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lyw.uphjek.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rzg.sufxvd.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://krc.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ysa.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cul.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bxi.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fbd.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jjh.dianchejie.cn

================================================================================
来源：http://usl.tarul.cn

A. 基础语法与类型
来源：http://tvo.iojbl.cn

================================================================================
来源：http://uby.svipenyu.cn

[A01] Hello World
来源：http://sxm.sxryk.cn

Py:   print("Hello, World!")
来源：http://ceb.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://nfm.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://tvo.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yjs.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://nar.zhiwuduotai.top

Go:   fmt.Println("Hello, World!")
来源：http://osp.cashguo.top

Ruby: puts "Hello, World!"
来源：http://oob.zhaomingkeji.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://zzw.daria6918.cn

[A02] 变量声明与赋值
来源：http://isx.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fbq.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sal.mhx1999.top

JS:   let name = "Alex"; const age = 20;
来源：http://oor.quarkkingdee.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://emn.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://eva.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://kqp.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://kjf.fzhhl.top

C#:   string name = "Alex"; int age = 20;
来源：http://jfz.yangfankeji.com

[A03] 常量定义
来源：http://sef.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://maz.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://bpg.wangdashe.top

JS:   const PI = 3.14159;
来源：http://zuh.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://fvi.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://lbf.fktsv.cn

Go:   const PI = 3.14159
来源：http://kws.fktsv.cn

Ruby: PI = 3.14159
来源：http://wuq.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://ncf.ybcxt.top

[A04] 判断变量类型
来源：http://osy.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gdo.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://chg.yj202588.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iyp.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://jmc.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uxf.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://dpp.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xss.jlsjyb.cn

C#:   x.GetType().Name; x is int
来源：http://rrz.hcnkem.com

[A05] 整数除法与取模
来源：http://ewq.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tyt.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://aql.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wtq.meibo888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nkv.wangdashe.top

Java: 7 / 2; 7 % 2
来源：http://drf.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://uay.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://hum.0kj1m.cn

C#:   7 / 2; 7 % 2
来源：http://dwz.316326.xyz

[A06] 字符串转数字
来源：http://mpv.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://lhy.sysykeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dwp.ydjk.org.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mvv.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vhc.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yei.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yox.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qjg.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jjq.zhengqikj.top

[A07] 数字转字符串
来源：http://twf.chenjidiqi.icu

Py:   str(42)
来源：http://dsg.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://heq.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://hxg.tian-w.cn

TS:   String(42)
来源：http://ddt.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ikn.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://hen.zhixingplan.top

Ruby: 42.to_s
来源：http://eht.wangdashe.top

C#:   42.ToString()
来源：http://uvd.svipenyu.cn

[A08] 取整与四舍五入
来源：http://wdk.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://opn.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bxi.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cbt.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ryu.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sdd.hnxiangtu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jns.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://oge.ctjpmb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gwp.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://fab.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xfe.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://koo.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ehi.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kcn.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vee.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pzd.zhoulong.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gye.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://icx.xziqi.cn

[A10] 生成随机数
来源：http://dwt.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://evo.fengsongda.top

PHP:  random_int(1, 100);
来源：http://czj.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kjf.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://udl.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://zbf.sxryk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dkw.yj20258.top

Ruby: rand(1..100)
来源：http://vcn.c1oappe.top

C#:   new Random().Next(1, 101)
来源：http://qqz.daria6918.cn

[A11] 条件表达式（三元）
来源：http://tuu.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://pty.hnqzz.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ymr.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kno.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://kcy.sysykeji.top

Java: x > 0 ? "yes" : "no"
来源：http://rff.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://pht.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://kzz.zhijiandao.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tad.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://ohk.hnqzz.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ouj.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://skv.snrcjt.cn

JS:   `Hello, ${name}!`
来源：http://mvg.tanke756.top

TS:   `Hello, ${name}!`
来源：http://gut.shanyushiyangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://aat.mhx1999.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xfs.hnqzz.top

Ruby: "Hello, #{name}!"
来源：http://kdi.nanxuanxn.top

C#:   $"Hello, {name}!"
来源：http://eiw.sweek.top

[A13] 多行字符串（练习 \n 转义）
来源：http://bgq.birdmap.top

Py:   "第一行\n第二行"
来源：http://fdp.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://sqz.pycfn.com

JS:   "第一行\n第二行"
来源：http://ohl.yvedp.cn

TS:   "第一行\n第二行"
来源：http://spa.gogol.net.cn

Java: "第一行\n第二行"
来源：http://jao.jyoumei.cn

Go:   "第一行\n第二行"
来源：http://vta.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://swm.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://uco.tanke756.top

[A14] 注释写法
来源：http://ubv.sysykeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://svc.yonumen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tje.yuxming.cn

JS:   // 单行；/* 多行 */
来源：http://xyu.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://dzp.jinqigufen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bhi.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://rxn.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://ovl.bjfxy.top


<!-- 参考信息 -->