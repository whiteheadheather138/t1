代发 wailian999

[U91] JS：对象键值遍历
来源：http://xxs.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fam.yangfankeji.com

[U92] JS：深拷贝
来源：http://mew.sufxvd.cn

structuredClone(obj)
来源：http://tex.nwbrower.top

[U93] JS：模板字符串
来源：http://qcz.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://jrz.hnqzz.top

[U94] JS：箭头函数
来源：http://jru.fengsongda.top

const double = x => x * 2;
来源：http://byp.hfpthk.cn

[U95] JS：Promise 包装
来源：http://ttd.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://nzv.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://agz.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xyq.tian-w.cn

[U97] JS：并发请求
来源：http://snb.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uek.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://zwv.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hmd.xinyue.icu

[U99] JS：事件监听
来源：http://osl.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://sxd.yuanzhike.top

[U100] JS：DOM 查询
来源：http://hvr.tianlin.xyz

document.querySelector(".item")
来源：http://tfg.bjfxy.top

[U101] JS：classList 操作
来源：http://ynl.yj20258888.top

el.classList.toggle("active")
来源：http://ftz.yueranfly.top

[U102] JS：本地存储
来源：http://uer.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wnl.quarkkingdee.top

[U103] JS：定时器
来源：http://dqg.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mej.shzxlz.cn

[U104] JS：防抖
来源：http://kon.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdp.birdmap.top

[U105] JS：节流
来源：http://zcu.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tpr.shuidangran.top

[U106] JS：日期格式化
来源：http://jss.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zkp.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://zvw.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tkn.zdbjq.cn

[U108] JS：随机整数
来源：http://sjb.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wpw.9152youxi.cn

[U109] JS：数组分组
来源：http://xub.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://uqa.c1oappe.top

[U110] JS：数组分块
来源：http://ouz.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ejb.yj20258888.top

[U111] JS：对象转 Map
来源：http://uwq.uphjek.com

new Map(Object.entries(obj))
来源：http://ize.wangdashe.top

[U112] JS：字符串补位
来源：http://xfc.gogol.net.cn

"7".padStart(3, "0")
来源：http://vif.gzhubu.top

[U113] JS：正则替换全部
来源：http://ltm.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://qzi.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://goi.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://yjy.sxryk.cn

[U115] JS：生成 UUID
来源：http://yiz.cdnleiting.top

crypto.randomUUID()
来源：http://vzm.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://wsb.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://uqq.jqgfzy.top

[U117] JS：单元测试
来源：http://rnh.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://eif.zycfv.cn

[U118] JS：开发服务器
来源：http://eoc.wangdashe.top

npm i -D vite;  npx vite
来源：http://lyf.dashuyun.cn

[U119] JS：生产构建
来源：http://kyw.uphjek.com

npx vite build
来源：http://hyi.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://dnc.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://ujy.uphjek.com

================================================================================
来源：http://stv.yj20258.top

统计汇总
来源：http://woz.xingfuxueyuan.xyz

================================================================================
来源：http://wly.xuetiantiany.cn

按语言统计（条）：
来源：http://saq.fanxiaobao.xyz

Python ......... 252
来源：http://zmc.zhaomingkeji.xyz

PHP ............ 252
来源：http://ftl.andypj.xyz

JavaScript ..... 252
来源：http://tri.havefunace.top

TypeScript ..... 212
来源：http://lna.yvedp.cn

Java ........... 212
来源：http://rnn.aibaodan.cn

Go ............. 212
来源：http://lia.hesvh.cn

Ruby ........... 212
来源：http://igd.zhiwuduotai.top

C# ............. 212
来源：http://phf.hysaishi.cn

C .............. 30
来源：http://fuj.redwolf501.top

C++ ............ 30
来源：http://hqk.nanxuanxn.top

SQL ............ 90
来源：http://lzi.nanxuanxn.top

Bash ........... 80
来源：http://grp.cqqwz.cn

Kotlin ......... 15
来源：http://nvl.meibo888.top

Swift .......... 15
来源：http://vau.zycfv.cn

Lua ............ 10
来源：http://gaj.zdbjq.cn

Perl ........... 10
来源：http://ysm.bbcook.cn

Scala .......... 10
来源：http://dad.jinyuanbaomall.cn

------------------------------------
来源：http://rak.9152youxi.cn

合计 ........... 2106 条
来源：http://has.vehdjk.com

按章节统计：
来源：http://gse.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aob.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jtg.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kge.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://keb.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xpk.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vzy.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oqs.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tfp.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://noh.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bsz.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jnd.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ssz.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gvn.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://osc.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fez.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hsn.svipenyu.cn

Q SQL 专题                              90
来源：http://pgz.zhixingplan.top

R Bash 专题                             80
来源：http://xal.yuanzhike.top

S C / C++ 专题                          60
来源：http://uyx.zhixingplan.top

T 其他语言补充                          60
来源：http://ggt.guowangkeji.top

U 高频实用片段                         120
来源：http://soa.yj202588.top

------------------------------------
来源：http://sfr.gaohongyu789.top

合计                                  2106 条
来源：http://hcp.hesvh.cn

--------------------------------------------------------------------------------
来源：http://nxo.pengpengdd.cyou

使用提醒
来源：http://nay.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://asv.ivvv.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hjs.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://buc.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hpx.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jxz.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yml.smart0.xyz

—— 文件结束 ——
来源：http://bli.smart0.xyz

================================================================================
来源：http://uma.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://uhv.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://ddk.yuanzhike.top

================================================================================
来源：http://hng.xylfe.cn

【收录内容】
来源：http://hld.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://atj.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mpt.haohaochexian.top

SQL · Bash · C · C++
来源：http://tqt.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sey.cheryme.top

【使用说明】
来源：http://unv.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://shf.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kpx.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kkg.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://noe.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nzy.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bok.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ntm.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qrj.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fiw.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://znn.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://axj.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sgn.cqqwz.cn

【文件统计】
来源：http://kwk.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cei.havefunace.top

--------------------------------------------------------------------------------
来源：http://sop.ydjk.org.cn

目  录
来源：http://dqf.yfazqb.com

--------------------------------------------------------------------------------
来源：http://lsp.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nyi.sysykeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://trd.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://unq.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ytj.pengpengdd.cyou

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qrk.9152youxi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ymf.chenlongwang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qic.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qxk.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kgr.zhaomingkeji.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eor.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qhd.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xba.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://scu.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xfj.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rdv.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sjo.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xjy.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ffp.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pks.dashuyun.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gnf.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qdz.52xcode.cn

================================================================================
来源：http://wyf.ydzc1.top

A. 基础语法与类型
来源：http://myg.xuanzx.com

================================================================================
来源：http://rws.redwolf501.top

[A01] Hello World
来源：http://cgh.pycfn.com

Py:   print("Hello, World!")
来源：http://jdi.hfpthk.cn

PHP:  echo "Hello, World!";
来源：http://ljg.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://mxt.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qge.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://irf.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://pya.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://ero.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ipj.shuidangran.top

[A02] 变量声明与赋值
来源：http://jkv.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vkd.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vvz.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ail.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kus.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://voz.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://waa.zhoulong.xyz

Ruby: name = "Alex"; age = 20
来源：http://cuc.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dey.jinqigfzy.top

[A03] 常量定义
来源：http://sbc.cheryme.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kqc.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://ckd.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://fcx.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://gmr.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://yrp.xinyue.icu

Go:   const PI = 3.14159
来源：http://pjv.jlsjyb.cn

Ruby: PI = 3.14159
来源：http://efy.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://gtv.hongshengwenyu.top

[A04] 判断变量类型
来源：http://sin.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yed.9152youxi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ydi.yj202588.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://anj.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://sok.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://orx.svipenyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fod.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://htw.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://tnz.vqdsnc.cn

[A05] 整数除法与取模
来源：http://drp.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://juh.aizwys.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ihr.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aos.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mbq.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://lrj.9152youxi.cn

Go:   7 / 2; 7 % 2
来源：http://pit.jinqigufen.top

Ruby: 7 / 2; 7 % 2
来源：http://iek.kuanghao11.cn

C#:   7 / 2; 7 % 2
来源：http://aos.ppjwa.cn

[A06] 字符串转数字
来源：http://aut.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://lku.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fzg.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kcp.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uqi.dashuyun.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iuk.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nbd.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mzy.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://asb.dianchejie.cn

[A07] 数字转字符串
来源：http://byv.redwolf501.top

Py:   str(42)
来源：http://kck.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://pel.ydzc1.top

JS:   String(42); (42).toString()
来源：http://hda.jinyuanbaomall.cn

TS:   String(42)
来源：http://kcs.chenzaomai.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://yyh.nanxuanxn.top

Go:   strconv.Itoa(42)
来源：http://fch.fehbvm.com

Ruby: 42.to_s
来源：http://prt.yuanzhike.top

C#:   42.ToString()
来源：http://frk.jianghu66.top

[A08] 取整与四舍五入
来源：http://ouc.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lxo.sjlbkw.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dbk.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gzz.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://urq.hysaishi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fee.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ltk.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uzj.zhoulong.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ypi.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://dne.nanxuanxn.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://obm.shzxlz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cpe.hongshengwenyu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bqz.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bou.cucudq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sco.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wfc.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yhm.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qzf.fanxiaobao.xyz

[A10] 生成随机数
来源：http://tjl.fzhhl.top

Py:   import random; random.randint(1, 100)
来源：http://zxz.ivvv.top

PHP:  random_int(1, 100);
来源：http://npr.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wjn.cheryme.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xhk.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://xif.bbcook.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hcn.xziqi.cn

Ruby: rand(1..100)
来源：http://fle.52xcode.cn

C#:   new Random().Next(1, 101)
来源：http://wvx.pycfn.com

[A11] 条件表达式（三元）
来源：http://cgh.zhiwuduotai.top

Py:   "yes" if x > 0 else "no"
来源：http://kec.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rxc.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://zpy.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://atn.ppjwa.cn

Java: x > 0 ? "yes" : "no"
来源：http://ynb.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xwu.xuanzx.com

Ruby: x > 0 ? "yes" : "no"
来源：http://fei.jyoumei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gem.zhongyouzk.top

[A12] 字符串插值 / 格式化
来源：http://erv.haohaochexian.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nvs.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kbo.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://kke.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://rtw.yanxiufei.cn

Java: "Hello, %s!".formatted(name)
来源：http://yre.daxiang520.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wlr.cdnleiting.top

Ruby: "Hello, #{name}!"
来源：http://hbh.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://gfw.fktsv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ske.pengpengdd.cyou

Py:   "第一行\n第二行"
来源：http://eqe.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://mgs.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://jsb.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://nyl.0kj1m.cn

Java: "第一行\n第二行"
来源：http://onm.guannengcc.top

Go:   "第一行\n第二行"
来源：http://kkx.zdqjudy.top

Ruby: "第一行\n第二行"
来源：http://vyy.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://noc.hnqzz.top

[A14] 注释写法
来源：http://ugr.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xiu.shanyushiyangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zgd.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://qwy.hcnkem.com

TS:   // 单行；/* 多行 */
来源：http://ocb.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sqg.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://eau.andypj.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://qjl.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://pbb.fktsv.cn

[A15] 空值判断与默认值
来源：http://tmd.hywenlv.cn

Py:   value = data or "默认值"
来源：http://lno.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://lbb.xuanzx.com

JS:   const value = data ?? "默认值";
来源：http://wgv.zdbjq.cn

TS:   const value = data ?? "默认值";
来源：http://xvp.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dxc.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://jbc.zhiwuduotai.top


<!-- 参考信息 -->