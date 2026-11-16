代发 wailian999

[U93] JS：模板字符串
来源：http://eyc.feifeiyinyue.top

`共 ${n} 条`
来源：http://svn.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://ngr.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://dtg.xylfe.cn

[U95] JS：Promise 包装
来源：http://tja.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://wpx.xuanzx.com

[U96] JS：async/await 与异常
来源：http://ixc.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hrs.epnwcf.com

[U97] JS：并发请求
来源：http://usc.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xhi.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://cil.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kim.gogol.net.cn

[U99] JS：事件监听
来源：http://eqz.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://zxv.jinqigufen.top

[U100] JS：DOM 查询
来源：http://juo.jyoumei.cn

document.querySelector(".item")
来源：http://zwt.hcnkem.com

[U101] JS：classList 操作
来源：http://slb.mhx1999.top

el.classList.toggle("active")
来源：http://hld.snrcjt.cn

[U102] JS：本地存储
来源：http://blg.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sii.ydzc1.top

[U103] JS：定时器
来源：http://xvz.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://spb.xylfe.cn

[U104] JS：防抖
来源：http://bto.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ktm.xziqi.cn

[U105] JS：节流
来源：http://kwl.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://thc.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://txn.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://saj.haohaochexian.top

[U107] JS：数字千分位
来源：http://wps.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://enl.jqgfzy.top

[U108] JS：随机整数
来源：http://rql.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lxc.gaohongyu789.top

[U109] JS：数组分组
来源：http://vjf.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://twd.cqqwz.cn

[U110] JS：数组分块
来源：http://yum.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://top.hywenlv.cn

[U111] JS：对象转 Map
来源：http://ioq.pycfn.com

new Map(Object.entries(obj))
来源：http://mvc.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://tzz.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://ohl.cqqwz.cn

[U113] JS：正则替换全部
来源：http://rwc.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://kvx.yueranfly.top

[U114] JS：JSON 深比较
来源：http://cfv.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uxe.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://mbj.xinyue.icu

crypto.randomUUID()
来源：http://pmt.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://vqs.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://zjg.shangyingyoupin.top

[U117] JS：单元测试
来源：http://efv.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://xex.nanxuanxn.top

[U118] JS：开发服务器
来源：http://acv.hcnkem.com

npm i -D vite;  npx vite
来源：http://ebg.chenzaomai.com

[U119] JS：生产构建
来源：http://iuf.52xcode.cn

npx vite build
来源：http://fhw.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://cni.316326.xyz

import.meta.env.VITE_API_URL
来源：http://otw.jinyuanbaomall.cn

================================================================================
来源：http://gyi.mhx1999.top

统计汇总
来源：http://kzt.c1oappe.top

================================================================================
来源：http://dxf.jinqigufen.top

按语言统计（条）：
来源：http://mgg.shangyingyoupin.top

Python ......... 252
来源：http://utr.ctjpmb.com

PHP ............ 252
来源：http://cgx.dashuyun.cn

JavaScript ..... 252
来源：http://vng.sxryk.cn

TypeScript ..... 212
来源：http://ail.dashuyun.cn

Java ........... 212
来源：http://cyp.xuanzx.com

Go ............. 212
来源：http://arw.cucudq.cn

Ruby ........... 212
来源：http://cmd.zhongyouzk.top

C# ............. 212
来源：http://ufc.sjlbkw.cn

C .............. 30
来源：http://pmq.jlsjyb.cn

C++ ............ 30
来源：http://ywt.wangdashe.top

SQL ............ 90
来源：http://vzq.fzhhl.top

Bash ........... 80
来源：http://wkb.jinqigufen.top

Kotlin ......... 15
来源：http://znq.hesvh.cn

Swift .......... 15
来源：http://mxx.aibaodan.cn

Lua ............ 10
来源：http://iop.guowangkeji.top

Perl ........... 10
来源：http://bib.ppjwa.cn

Scala .......... 10
来源：http://aag.hammf.cn

------------------------------------
来源：http://vuu.pycfn.com

合计 ........... 2106 条
来源：http://ock.sweek.top

按章节统计：
来源：http://wvf.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ivu.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lqz.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eah.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ebg.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://adz.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hkk.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mea.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://azh.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vqm.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uqa.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://spv.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ujz.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wyo.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rsu.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dya.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://avi.cashguo.top

Q SQL 专题                              90
来源：http://bhd.xuanzx.com

R Bash 专题                             80
来源：http://gaf.iojbl.cn

S C / C++ 专题                          60
来源：http://pbh.jqgfzy.top

T 其他语言补充                          60
来源：http://jgn.jlsjyb.cn

U 高频实用片段                         120
来源：http://fgf.jinyuanbaomall.cn

------------------------------------
来源：http://kvk.ehwqpu.com

合计                                  2106 条
来源：http://sio.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://hhh.jianghu66.top

使用提醒
来源：http://hba.hcnkem.com

--------------------------------------------------------------------------------
来源：http://cmk.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pde.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mvj.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://glt.hesvh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cqt.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xyh.nanxuanxn.top

—— 文件结束 ——
来源：http://sty.shzxlz.cn

================================================================================
来源：http://jin.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://psi.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://idt.zhengqikj.top

================================================================================
来源：http://hgs.fehbvm.com

【收录内容】
来源：http://czj.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://idl.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uvm.yj202588.top

SQL · Bash · C · C++
来源：http://gnb.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cyk.gogol.net.cn

【使用说明】
来源：http://tww.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hmf.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mrj.bjfxy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yqr.aibaodan.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qax.tarul.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zgk.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://juk.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://emi.xylfe.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dsv.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bye.cheryme.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hvb.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fjf.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mbf.ehwqpu.com

【文件统计】
来源：http://mau.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nxn.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://xdv.cdnleiting.top

目  录
来源：http://xkp.ivvv.top

--------------------------------------------------------------------------------
来源：http://onf.yvedp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://plu.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ukw.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jqz.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://exz.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aui.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tul.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oxz.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ukh.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zeq.gaohongyu789.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wtn.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oae.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://heh.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://clz.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xzi.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jsg.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wao.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pkf.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wix.guowangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ggv.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://svm.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vne.ywan-chungtsiang.top

================================================================================
来源：http://mov.iojbl.cn

A. 基础语法与类型
来源：http://jmr.shangyingyoupin.top

================================================================================
来源：http://inv.sxryk.cn

[A01] Hello World
来源：http://ayc.meibo888.top

Py:   print("Hello, World!")
来源：http://ewz.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://fmn.xuanzx.com

JS:   console.log("Hello, World!");
来源：http://plk.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ejz.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://bso.tianlin.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ygl.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://hjl.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bnh.zhengqikj.top

[A02] 变量声明与赋值
来源：http://nlz.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nhx.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://iat.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://nuc.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ooe.cdnleiting.top

Java: String name = "Alex"; int age = 20;
来源：http://tvb.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://yuo.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://eew.jlsjyb.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vpg.shzxlz.cn

[A03] 常量定义
来源：http://cwd.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ueb.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://vnm.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://exh.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://pwo.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://rqp.yonumen.top

Go:   const PI = 3.14159
来源：http://krm.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://bhu.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://ngm.cashguo.top

[A04] 判断变量类型
来源：http://fhy.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://vqs.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nbz.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oyc.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://uax.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wbg.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://uqe.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fcm.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://whv.ydzc1.top

[A05] 整数除法与取模
来源：http://qaf.9152youxi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nuq.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wxg.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wzq.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iwh.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://btg.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://cdo.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://jjk.guowangkeji.top

C#:   7 / 2; 7 % 2
来源：http://oph.c1oappe.top

[A06] 字符串转数字
来源：http://ykq.uphjek.com

Py:   int("42"); float("3.14")
来源：http://qoe.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nsz.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ydh.hesvh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tje.cheryme.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xot.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://szo.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://eys.wangdashe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qtj.zhijiandao.cn

[A07] 数字转字符串
来源：http://kix.yonumen.top

Py:   str(42)
来源：http://bsh.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://twx.uphjek.com

JS:   String(42); (42).toString()
来源：http://yct.sufxvd.cn

TS:   String(42)
来源：http://zme.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tak.cqqwz.cn

Go:   strconv.Itoa(42)
来源：http://qzw.meibo888.top

Ruby: 42.to_s
来源：http://ofc.jinyuanbaomall.cn

C#:   42.ToString()
来源：http://euf.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://fsc.zhongyouzk.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cpa.yangfankeji.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://avh.xuanzx.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://quz.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nmm.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zgs.jqgfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xsy.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://uei.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uuz.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://zej.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fib.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ymh.dashuyun.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://poh.jyoumei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xat.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://abw.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iir.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rgi.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lgg.jyoumei.cn

[A10] 生成随机数
来源：http://uaq.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://xhe.andypj.xyz

PHP:  random_int(1, 100);
来源：http://fxr.jianghu66.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jsy.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hjk.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://pad.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sfp.yueranfly.top

Ruby: rand(1..100)
来源：http://myh.shanyushiyangtech.top

C#:   new Random().Next(1, 101)
来源：http://vwi.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://kzw.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://zxc.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uhn.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://chd.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sgc.ybcxt.top

Java: x > 0 ? "yes" : "no"
来源：http://ush.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://suk.0kj1m.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dpt.chenjidiqi.icu

C#:   x > 0 ? "yes" : "no"
来源：http://beb.cqqwz.cn

[A12] 字符串插值 / 格式化
来源：http://wvt.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bdt.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ufk.jlsjyb.cn

JS:   `Hello, ${name}!`
来源：http://yns.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://zwp.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://dxr.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blc.ydzc1.top

Ruby: "Hello, #{name}!"
来源：http://cge.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://rht.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://aqc.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://gdp.jlsjyb.cn

PHP:  "第一行\n第二行"
来源：http://etp.fengsongda.top

JS:   "第一行\n第二行"
来源：http://sfm.zhaomingkeji.xyz

TS:   "第一行\n第二行"
来源：http://oeu.hcnkem.com

Java: "第一行\n第二行"
来源：http://kab.feifeiyinyue.top

Go:   "第一行\n第二行"
来源：http://pes.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://ggq.iojbl.cn

C#:   "第一行\n第二行"
来源：http://ink.hfpthk.cn

[A14] 注释写法
来源：http://itm.shangyingyoupin.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://imb.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://klf.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://jmg.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://jgg.ybcxt.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rrg.xuanzx.com

Go:   // 单行；/* 多行 */
来源：http://vdo.xziqi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dxz.fzhhl.top

C#:   // 单行；/* 多行 */
来源：http://wrj.shuidangran.top

[A15] 空值判断与默认值
来源：http://mbx.vehdjk.com

Py:   value = data or "默认值"
来源：http://qkl.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://jfb.guowangkeji.top

JS:   const value = data ?? "默认值";
来源：http://kkh.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://vee.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bvj.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://dje.ivvv.top

Ruby: value = data || "默认值"
来源：http://vcg.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://hql.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://sva.52xcode.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pyo.sweek.top


<!-- 参考信息 -->