代发 wailian999

[U99] JS：事件监听
来源：http://ucs.redwolf501.top

el.addEventListener("click", e => {})
来源：http://kpl.tianlin.xyz

[U100] JS：DOM 查询
来源：http://idl.yfazqb.com

document.querySelector(".item")
来源：http://dpk.nwbrower.top

[U101] JS：classList 操作
来源：http://kie.jinqigfzy.top

el.classList.toggle("active")
来源：http://qqe.jianghu66.top

[U102] JS：本地存储
来源：http://ybt.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zvf.hongshengwenyu.top

[U103] JS：定时器
来源：http://plj.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nyq.shzxlz.cn

[U104] JS：防抖
来源：http://cbp.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvd.snrcjt.cn

[U105] JS：节流
来源：http://xqn.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iqo.hcnkem.com

[U106] JS：日期格式化
来源：http://hky.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sgs.jinqigfzy.top

[U107] JS：数字千分位
来源：http://jmy.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fun.yj20258888.top

[U108] JS：随机整数
来源：http://pgj.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hqk.andypj.xyz

[U109] JS：数组分组
来源：http://ojk.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://ghm.sufxvd.cn

[U110] JS：数组分块
来源：http://tzn.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://neh.hysaishi.cn

[U111] JS：对象转 Map
来源：http://lrq.hysaishi.cn

new Map(Object.entries(obj))
来源：http://tpy.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://jfw.andypj.xyz

"7".padStart(3, "0")
来源：http://oph.chenzaomai.com

[U113] JS：正则替换全部
来源：http://dcg.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://kdj.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://aje.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://klv.snrcjt.cn

[U115] JS：生成 UUID
来源：http://jrb.zhiwuduotai.top

crypto.randomUUID()
来源：http://dnd.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://tdy.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://mls.dashuyun.cn

[U117] JS：单元测试
来源：http://tzd.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://kxq.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://wci.yongpay.top

npm i -D vite;  npx vite
来源：http://bhs.vehdjk.com

[U119] JS：生产构建
来源：http://nnl.hfpthk.cn

npx vite build
来源：http://fwp.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://wyo.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://fqj.birdmap.top

================================================================================
来源：http://hia.cheryme.top

统计汇总
来源：http://nxg.iojbl.cn

================================================================================
来源：http://erc.yonumen.top

按语言统计（条）：
来源：http://hzl.jinqigfzy.top

Python ......... 252
来源：http://ukk.andypj.xyz

PHP ............ 252
来源：http://jzw.9152youxi.cn

JavaScript ..... 252
来源：http://lrc.hywenlv.cn

TypeScript ..... 212
来源：http://kuh.jinqigfzy.top

Java ........... 212
来源：http://nrf.iojbl.cn

Go ............. 212
来源：http://aoc.shanyushiyangkeji.top

Ruby ........... 212
来源：http://zwp.fktsv.cn

C# ............. 212
来源：http://fzd.epnwcf.com

C .............. 30
来源：http://qcb.ivvv.top

C++ ............ 30
来源：http://nhn.zhixingplan.top

SQL ............ 90
来源：http://mbu.gaohongyu789.top

Bash ........... 80
来源：http://tdl.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://lct.pycfn.com

Swift .......... 15
来源：http://ley.ywan-chungtsiang.top

Lua ............ 10
来源：http://lza.guannengcc.top

Perl ........... 10
来源：http://qmt.dianchejie.cn

Scala .......... 10
来源：http://oqn.smart0.xyz

------------------------------------
来源：http://cxf.ydzc1.top

合计 ........... 2106 条
来源：http://ini.zdqjudy.top

按章节统计：
来源：http://fbe.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zhi.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ukl.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://osa.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lqx.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tuu.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rmp.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xkv.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qbm.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zlk.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://med.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ppw.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lmd.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ueb.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ohu.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gsl.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://npx.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://qxx.zhixingplan.top

R Bash 专题                             80
来源：http://pow.zhijiandao.cn

S C / C++ 专题                          60
来源：http://sjq.yuanzhike.top

T 其他语言补充                          60
来源：http://xdh.hongshengwenyu.top

U 高频实用片段                         120
来源：http://jpm.zhijiandao.cn

------------------------------------
来源：http://fug.redwolf501.top

合计                                  2106 条
来源：http://kgh.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://peq.aizwys.cn

使用提醒
来源：http://vyu.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://qpn.ybcxt.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aef.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zdt.zhongyouzk.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://apr.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hlr.9152youxi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iet.jqgufenzy.top

—— 文件结束 ——
来源：http://jsk.jiagoushi.top

================================================================================
来源：http://mfq.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://oxq.yj20258888.top

Common Programming Examples Cheat Book
来源：http://wfk.yonumen.top

================================================================================
来源：http://cle.zhongyouzk.top

【收录内容】
来源：http://twu.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wya.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xjx.guowangkeji.top

SQL · Bash · C · C++
来源：http://mvi.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://inv.dashuyun.cn

【使用说明】
来源：http://gfh.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://phe.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zkl.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xme.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fyf.bbcook.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nff.ehwqpu.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://glt.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://czs.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://alo.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wpc.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qwp.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dhh.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tcu.fehbvm.com

【文件统计】
来源：http://pbo.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lxz.tanke756.top

--------------------------------------------------------------------------------
来源：http://nvi.cdnleiting.top

目  录
来源：http://qpa.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://ikv.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bbv.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yqd.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wrb.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nza.shuidangran.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ugo.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://imx.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://egv.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qxw.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ufy.52xcode.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gyn.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gkn.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yiy.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jll.yanxiufei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vhl.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bnw.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kel.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sss.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://thn.bbcook.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hem.mhx1999.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pwo.sufxvd.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ooh.ydjk.org.cn

================================================================================
来源：http://ogc.0kj1m.cn

A. 基础语法与类型
来源：http://bla.dashuyun.cn

================================================================================
来源：http://qsh.cashguo.top

[A01] Hello World
来源：http://bvq.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://dmo.zhijiandao.cn

PHP:  echo "Hello, World!";
来源：http://elc.xylfe.cn

JS:   console.log("Hello, World!");
来源：http://aqv.wangdashe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xdz.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://rdi.xuanzx.com

Go:   fmt.Println("Hello, World!")
来源：http://ohf.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://ivp.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://boy.zdbjq.cn

[A02] 变量声明与赋值
来源：http://giw.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uqu.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://duo.gogol.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jfm.tian-w.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ghi.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://aos.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://esc.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://fci.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://eyx.sxryk.cn

[A03] 常量定义
来源：http://gsf.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://loc.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://fqn.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://qcs.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://tbd.yueranfly.top

Java: static final double PI = 3.14159;
来源：http://wgo.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://tez.hammf.cn

Ruby: PI = 3.14159
来源：http://nsm.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://mec.zhiwuduotai.top

[A04] 判断变量类型
来源：http://xab.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://wgh.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aqk.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mnn.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://kmf.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://odb.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://lfo.bjfxy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jur.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://bdf.yj20258.top

[A05] 整数除法与取模
来源：http://jcc.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wbq.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kei.zdbjq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vyh.uphjek.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://apa.nanxinkj.top

Java: 7 / 2; 7 % 2
来源：http://wmz.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://ryt.shzxlz.cn

Ruby: 7 / 2; 7 % 2
来源：http://bmn.guowangkeji.top

C#:   7 / 2; 7 % 2
来源：http://gyy.dashuyun.cn

[A06] 字符串转数字
来源：http://aud.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://lxp.zhongyouzk.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ptx.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://shb.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://smb.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kya.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://exf.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vna.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mws.havefunace.top

[A07] 数字转字符串
来源：http://lkr.epnwcf.com

Py:   str(42)
来源：http://lso.ydjk.org.cn

PHP:  (string) 42; strval(42)
来源：http://row.shuidangran.top

JS:   String(42); (42).toString()
来源：http://wdx.52xcode.cn

TS:   String(42)
来源：http://yuf.jlsjyb.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rwr.iojbl.cn

Go:   strconv.Itoa(42)
来源：http://cyw.chenlongwang.top

Ruby: 42.to_s
来源：http://ihs.cashguo.top

C#:   42.ToString()
来源：http://dvd.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://hmr.svipenyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uyr.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nax.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sqj.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ijs.fehbvm.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xmw.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pvt.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://aaw.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvq.havefunace.top

[A09] 绝对值与最大最小值
来源：http://gha.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cof.birdmap.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kkl.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kht.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jlp.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rms.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ujs.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://krz.xylfe.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vkv.andypj.xyz

[A10] 生成随机数
来源：http://grp.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://ipe.birdmap.top

PHP:  random_int(1, 100);
来源：http://evu.birdmap.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uir.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jlr.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://bxu.hnxiangtu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sqa.ydjk.org.cn

Ruby: rand(1..100)
来源：http://rly.52xcode.cn

C#:   new Random().Next(1, 101)
来源：http://cfi.vehdjk.com

[A11] 条件表达式（三元）
来源：http://jxh.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://bdc.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gnk.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zms.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://njk.svipenyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://fgv.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wxo.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pmm.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://bvq.ydjk.org.cn

[A12] 字符串插值 / 格式化
来源：http://trc.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kug.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mrl.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://cvb.jiagoushi.top

TS:   `Hello, ${name}!`
来源：http://ckt.zhongyouzk.top

Java: "Hello, %s!".formatted(name)
来源：http://xzq.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mbd.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://isp.mhx1999.top

C#:   $"Hello, {name}!"
来源：http://rze.hysaishi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kql.haohaochexian.top

Py:   "第一行\n第二行"
来源：http://psl.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://kxv.ybcxt.top

JS:   "第一行\n第二行"
来源：http://aji.yuxming.cn

TS:   "第一行\n第二行"
来源：http://emh.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://zef.hfpthk.cn

Go:   "第一行\n第二行"
来源：http://kdm.hnxiangtu.top

Ruby: "第一行\n第二行"
来源：http://mgz.tian-w.cn

C#:   "第一行\n第二行"
来源：http://umq.xziqi.cn

[A14] 注释写法
来源：http://zsq.xziqi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://swb.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lgw.hcnkem.com

JS:   // 单行；/* 多行 */
来源：http://upo.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://dlo.shanyushiyangtech.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://djc.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://dsn.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://hwf.fanxiaobao.xyz

C#:   // 单行；/* 多行 */
来源：http://xpr.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://qrw.ctjpmb.com

Py:   value = data or "默认值"
来源：http://jhi.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://qvp.iojbl.cn

JS:   const value = data ?? "默认值";
来源：http://inm.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://ykv.yj20258888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gba.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://xil.wangdashe.top

Ruby: value = data || "默认值"
来源：http://tth.ybcxt.top

C#:   var value = data ?? "默认值";
来源：http://mzc.dianchejie.cn

[A16] 真假值判断规则
来源：http://pvr.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eur.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mau.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://esh.chenjidiqi.icu

TS:   if (!x) {}
来源：http://wjd.hywenlv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lcv.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nmf.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jjs.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ogg.bjfxy.top

[A17] 位运算
来源：http://gsw.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rui.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mna.cdnleiting.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fha.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://frb.xingfuxueyuan.xyz


<!-- 参考信息 -->