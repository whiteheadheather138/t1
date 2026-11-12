代发 wailian999

[U97] JS：并发请求
来源：http://gsp.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kwd.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://rgs.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hom.sxryk.cn

[U99] JS：事件监听
来源：http://xog.iojbl.cn

el.addEventListener("click", e => {})
来源：http://nha.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://ozd.dashuyun.cn

document.querySelector(".item")
来源：http://elh.dianchejie.cn

[U101] JS：classList 操作
来源：http://plw.chenjidiqi.icu

el.classList.toggle("active")
来源：http://use.hysaishi.cn

[U102] JS：本地存储
来源：http://sle.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://azd.xziqi.cn

[U103] JS：定时器
来源：http://gpp.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nwn.xinyue.icu

[U104] JS：防抖
来源：http://ypy.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvm.fktsv.cn

[U105] JS：节流
来源：http://tyd.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://euq.cashguo.top

[U106] JS：日期格式化
来源：http://kwi.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ded.tanke756.top

[U107] JS：数字千分位
来源：http://ekw.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ubu.gotoacloud.top

[U108] JS：随机整数
来源：http://ykh.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pqo.jiagoushi.top

[U109] JS：数组分组
来源：http://pur.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://vpo.nanxinkj.top

[U110] JS：数组分块
来源：http://fox.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rlo.xziqi.cn

[U111] JS：对象转 Map
来源：http://ueb.zdbjq.cn

new Map(Object.entries(obj))
来源：http://avu.sysykeji.top

[U112] JS：字符串补位
来源：http://mty.vehdjk.com

"7".padStart(3, "0")
来源：http://vxk.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://ybl.bjfxy.top

s.replaceAll("a", "b")
来源：http://zbl.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://jcn.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://drs.shuidangran.top

[U115] JS：生成 UUID
来源：http://wzu.yj202588.top

crypto.randomUUID()
来源：http://pyd.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://cle.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://xky.ehwqpu.com

[U117] JS：单元测试
来源：http://jka.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://uhi.aibaodan.cn

[U118] JS：开发服务器
来源：http://smm.gogol.net.cn

npm i -D vite;  npx vite
来源：http://fki.jqgfzy.top

[U119] JS：生产构建
来源：http://bmy.zhaomingkeji.xyz

npx vite build
来源：http://brt.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://rue.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://xcs.xinyue.icu

================================================================================
来源：http://uhd.9152youxi.cn

统计汇总
来源：http://ilp.52xcode.cn

================================================================================
来源：http://hhg.jinghuilouyu.cn

按语言统计（条）：
来源：http://fmj.shuidangran.top

Python ......... 252
来源：http://sjx.jiagoushi.top

PHP ............ 252
来源：http://cpf.jlsjyb.cn

JavaScript ..... 252
来源：http://qoo.hnqzz.top

TypeScript ..... 212
来源：http://amq.nwbrower.top

Java ........... 212
来源：http://idm.guannengcc.top

Go ............. 212
来源：http://ubq.jianghu66.top

Ruby ........... 212
来源：http://jzv.feifeiyinyue.top

C# ............. 212
来源：http://iyk.9152youxi.cn

C .............. 30
来源：http://ssq.vqdsnc.cn

C++ ............ 30
来源：http://pkr.wangshuangyany.cn

SQL ............ 90
来源：http://syj.redwolf501.top

Bash ........... 80
来源：http://ilg.tanke756.top

Kotlin ......... 15
来源：http://dbg.tianlin.xyz

Swift .......... 15
来源：http://hxp.gotoacloud.top

Lua ............ 10
来源：http://sqy.xuetiantiany.cn

Perl ........... 10
来源：http://yif.fengsongda.top

Scala .......... 10
来源：http://azg.epnwcf.com

------------------------------------
来源：http://ehm.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://cwn.xuanzx.com

按章节统计：
来源：http://adn.aibaodan.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ffc.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bra.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xae.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://upw.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xah.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qap.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nmz.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://czk.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oec.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xmy.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iql.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gfv.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ilb.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ymt.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://smn.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eeu.bjfxy.top

Q SQL 专题                              90
来源：http://zij.cashguo.top

R Bash 专题                             80
来源：http://wes.yj202588.top

S C / C++ 专题                          60
来源：http://mfs.vqdsnc.cn

T 其他语言补充                          60
来源：http://mpd.xziqi.cn

U 高频实用片段                         120
来源：http://bkm.zhongyouzk.top

------------------------------------
来源：http://pse.fehbvm.com

合计                                  2106 条
来源：http://tqd.tian-w.cn

--------------------------------------------------------------------------------
来源：http://yme.smart0.xyz

使用提醒
来源：http://apd.sysykeji.top

--------------------------------------------------------------------------------
来源：http://qiu.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gpi.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qta.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ulg.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gfq.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://spn.daxiang520.top

—— 文件结束 ——
来源：http://iye.havefunace.top

================================================================================
来源：http://hoe.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://fxw.fktsv.cn

Common Programming Examples Cheat Book
来源：http://xip.yj202588.top

================================================================================
来源：http://eps.wangdashe.top

【收录内容】
来源：http://pgy.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yks.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vzl.vqdsnc.cn

SQL · Bash · C · C++
来源：http://gca.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://okn.gotoacloud.top

【使用说明】
来源：http://jkv.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://prm.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wdm.yuxming.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mtf.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xry.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pgy.fanxiaobao.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zyy.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rci.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lsb.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cdv.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uro.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ela.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ttl.redwolf501.top

【文件统计】
来源：http://odu.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aqt.gzhubu.top

--------------------------------------------------------------------------------
来源：http://atv.svipenyu.cn

目  录
来源：http://fap.cucudq.cn

--------------------------------------------------------------------------------
来源：http://cwe.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://arp.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sny.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pna.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sib.chenlongwang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rrs.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ohn.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mwk.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://djf.daria6918.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://olp.gotoacloud.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fee.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://phc.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mhp.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cyd.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rxt.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qfv.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zal.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cbg.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vbf.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ixp.yj202588.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yyr.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://onz.zhongyouzk.top

================================================================================
来源：http://qoj.jinghuilouyu.cn

A. 基础语法与类型
来源：http://amt.guowangkeji.top

================================================================================
来源：http://yzm.cheryme.top

[A01] Hello World
来源：http://uhq.cucudq.cn

Py:   print("Hello, World!")
来源：http://vzc.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://mba.tanke756.top

JS:   console.log("Hello, World!");
来源：http://ics.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lyi.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://eqx.sxryk.cn

Go:   fmt.Println("Hello, World!")
来源：http://mar.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://hyh.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hbm.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://crm.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nup.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ezd.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jyv.yj20258888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hsx.jinqigufen.top

Java: String name = "Alex"; int age = 20;
来源：http://khq.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://lwa.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://qfl.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pbx.chenjidiqi.icu

[A03] 常量定义
来源：http://ezw.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jyl.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://qiu.sysykeji.top

JS:   const PI = 3.14159;
来源：http://rga.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://hnc.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://ohd.pycfn.com

Go:   const PI = 3.14159
来源：http://vur.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://shq.ywan-chungtsiang.top

C#:   const double PI = 3.14159;
来源：http://pwj.dashuyun.cn

[A04] 判断变量类型
来源：http://guv.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://iha.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ysu.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dwa.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://jsj.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zur.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pbi.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://chl.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://bqh.cdnleiting.top

[A05] 整数除法与取模
来源：http://kpb.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://esl.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://bcz.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hbo.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rsg.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://ovu.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://gts.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://ces.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://uwz.shzxlz.cn

[A06] 字符串转数字
来源：http://znk.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://qpp.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ids.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ahu.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://okx.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gbr.52xcode.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xaw.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://uov.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tcc.kuanghao11.cn

[A07] 数字转字符串
来源：http://slb.hysaishi.cn

Py:   str(42)
来源：http://zlg.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://lxt.gotoacloud.top

JS:   String(42); (42).toString()
来源：http://jlz.dianchejie.cn

TS:   String(42)
来源：http://cpy.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qzk.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://zxi.tian-w.cn

Ruby: 42.to_s
来源：http://mkr.xuanzx.com

C#:   42.ToString()
来源：http://vom.xylfe.cn

[A08] 取整与四舍五入
来源：http://uxl.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ncf.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kzx.aizwys.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jji.0kj1m.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rxv.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eqk.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gsk.cheryme.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hdo.iojbl.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rse.jqgfzy.top

[A09] 绝对值与最大最小值
来源：http://wpv.9152youxi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gxj.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mqm.snrcjt.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bea.jyoumei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ozt.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wot.yj202588.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://npl.iojbl.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uve.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xyx.nanxuanxn.top

[A10] 生成随机数
来源：http://svr.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://xhp.yueranfly.top

PHP:  random_int(1, 100);
来源：http://jab.c1oappe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pvk.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wsi.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://ehd.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fsz.yj20258.top

Ruby: rand(1..100)
来源：http://xlv.daxiang520.top

C#:   new Random().Next(1, 101)
来源：http://gfq.sysykeji.top

[A11] 条件表达式（三元）
来源：http://enc.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://tkb.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vam.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://whg.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://wru.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://ikg.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fiq.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gsb.jinyuanbaomall.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wig.mhx1999.top

[A12] 字符串插值 / 格式化
来源：http://xkt.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ukq.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hea.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://zqm.yueranfly.top

TS:   `Hello, ${name}!`
来源：http://eis.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://cma.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zkz.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://fsq.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://cvd.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mjz.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://kkb.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://ifj.jqgufenzy.top

JS:   "第一行\n第二行"
来源：http://fpu.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://jtx.jqgfzy.top

Java: "第一行\n第二行"
来源：http://sra.epnwcf.com

Go:   "第一行\n第二行"
来源：http://rln.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://omn.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://wik.jlsjyb.cn

[A14] 注释写法
来源：http://ezb.aizwys.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wsg.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gab.tian-w.cn

JS:   // 单行；/* 多行 */
来源：http://vgv.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://twu.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lsh.jyoumei.cn

Go:   // 单行；/* 多行 */
来源：http://bhm.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jcc.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://heh.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://hjb.ybcxt.top

Py:   value = data or "默认值"
来源：http://ymn.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://tnm.sweek.top

JS:   const value = data ?? "默认值";
来源：http://zhu.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://nfn.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://slo.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://llh.yongpay.top

Ruby: value = data || "默认值"
来源：http://tqo.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://amw.cashguo.top

[A16] 真假值判断规则
来源：http://waa.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qun.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://smz.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yng.chenjidiqi.icu

TS:   if (!x) {}
来源：http://zgf.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mzh.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fja.hcnkem.com

Ruby: unless x            # nil 与 false 为假
来源：http://mte.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nmx.epnwcf.com

[A17] 位运算
来源：http://mru.gogol.net.cn


<!-- 参考信息 -->