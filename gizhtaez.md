代发 wailian999

[U95] JS：Promise 包装
来源：http://lir.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://cqb.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://vpo.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zta.meibo888.top

[U97] JS：并发请求
来源：http://cuo.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nxt.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://abd.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bzf.ydjk.org.cn

[U99] JS：事件监听
来源：http://adm.hcnkem.com

el.addEventListener("click", e => {})
来源：http://mnt.dianchejie.cn

[U100] JS：DOM 查询
来源：http://ftd.jqgfzy.top

document.querySelector(".item")
来源：http://arb.hysaishi.cn

[U101] JS：classList 操作
来源：http://anb.c1oappe.top

el.classList.toggle("active")
来源：http://hls.epnwcf.com

[U102] JS：本地存储
来源：http://xoc.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://xpw.nanxinkj.top

[U103] JS：定时器
来源：http://cvz.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xqm.ydzc1.top

[U104] JS：防抖
来源：http://ktz.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bqq.jqgufenzy.top

[U105] JS：节流
来源：http://cib.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blc.xinyue.icu

[U106] JS：日期格式化
来源：http://eom.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sbm.svipenyu.cn

[U107] JS：数字千分位
来源：http://tbo.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oar.pengpengdd.cyou

[U108] JS：随机整数
来源：http://ovi.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cuf.sufxvd.cn

[U109] JS：数组分组
来源：http://yvx.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://tjp.zhoulong.xyz

[U110] JS：数组分块
来源：http://qcc.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pyj.yongpay.top

[U111] JS：对象转 Map
来源：http://wti.52xcode.cn

new Map(Object.entries(obj))
来源：http://pin.snrcjt.cn

[U112] JS：字符串补位
来源：http://jcq.zhixingplan.top

"7".padStart(3, "0")
来源：http://qhy.hfpthk.cn

[U113] JS：正则替换全部
来源：http://zyn.nanxinkj.top

s.replaceAll("a", "b")
来源：http://etq.fengsongda.top

[U114] JS：JSON 深比较
来源：http://ref.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ndt.yangfankeji.com

[U115] JS：生成 UUID
来源：http://fjv.52xcode.cn

crypto.randomUUID()
来源：http://ozy.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://eyt.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://rjw.hammf.cn

[U117] JS：单元测试
来源：http://rkx.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://frk.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://rgj.0kj1m.cn

npm i -D vite;  npx vite
来源：http://iir.yfazqb.com

[U119] JS：生产构建
来源：http://viu.aibaodan.cn

npx vite build
来源：http://jet.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://lty.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://kuo.jiagoushi.top

================================================================================
来源：http://pfe.dianchejie.cn

统计汇总
来源：http://fed.wangdashe.top

================================================================================
来源：http://qjz.gogol.net.cn

按语言统计（条）：
来源：http://kwt.nanxuanxn.top

Python ......... 252
来源：http://dgq.hcnkem.com

PHP ............ 252
来源：http://kuy.dashuyun.cn

JavaScript ..... 252
来源：http://tjd.hesvh.cn

TypeScript ..... 212
来源：http://pnf.ctjpmb.com

Java ........... 212
来源：http://ovb.wangshuangyany.cn

Go ............. 212
来源：http://vqr.zhijiandao.cn

Ruby ........... 212
来源：http://gbt.316326.xyz

C# ............. 212
来源：http://zgn.bjfxy.top

C .............. 30
来源：http://fvg.cheryme.top

C++ ............ 30
来源：http://qnf.jiagoushi.top

SQL ............ 90
来源：http://ljp.cucudq.cn

Bash ........... 80
来源：http://oia.zhongyouzk.top

Kotlin ......... 15
来源：http://pqb.bjfxy.top

Swift .......... 15
来源：http://wfp.sysykeji.top

Lua ............ 10
来源：http://hcy.zhoulong.xyz

Perl ........... 10
来源：http://tmi.shanyushiyangkeji.top

Scala .......... 10
来源：http://kew.fehbvm.com

------------------------------------
来源：http://eth.sjlbkw.cn

合计 ........... 2106 条
来源：http://bkn.cucudq.cn

按章节统计：
来源：http://zvw.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hmg.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hbi.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ltl.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rsv.havefunace.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zpa.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gzq.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wvw.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://llg.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ixq.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ayj.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rgb.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rrm.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rxk.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ail.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://awq.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jnj.kuanghao11.cn

Q SQL 专题                              90
来源：http://npk.chenlongwang.top

R Bash 专题                             80
来源：http://btp.zdbjq.cn

S C / C++ 专题                          60
来源：http://eoz.zhaomingkeji.xyz

T 其他语言补充                          60
来源：http://pio.cucudq.cn

U 高频实用片段                         120
来源：http://lvu.zhixingplan.top

------------------------------------
来源：http://vkf.aibaodan.cn

合计                                  2106 条
来源：http://nzv.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://jcc.cqqwz.cn

使用提醒
来源：http://lsd.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://oxc.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bso.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hqy.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ewr.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://ioa.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dne.zdqjudy.top

—— 文件结束 ——
来源：http://moj.yj20258888.top

================================================================================
来源：http://csc.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://rld.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://jtw.zhaomingkeji.xyz

================================================================================
来源：http://izk.cqqwz.cn

【收录内容】
来源：http://yyk.kuanghao11.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://knq.cqqwz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sis.316326.xyz

SQL · Bash · C · C++
来源：http://gla.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lop.fktsv.cn

【使用说明】
来源：http://ynt.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ipm.gogol.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dkw.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gog.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fhs.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://hly.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ssy.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xut.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yds.guowangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vib.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jfr.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pld.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nyg.epnwcf.com

【文件统计】
来源：http://vez.zhaomingkeji.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hhx.vehdjk.com

--------------------------------------------------------------------------------
来源：http://dbu.gotoacloud.top

目  录
来源：http://dcg.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://wvc.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vnc.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://plt.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ogi.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://duo.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nef.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pce.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iln.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qax.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blh.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jda.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://akz.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mrg.andypj.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kza.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://woe.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vxj.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://png.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gyk.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tkg.zhoulong.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qbd.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vmy.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hvo.aizwys.cn

================================================================================
来源：http://ejp.xziqi.cn

A. 基础语法与类型
来源：http://iom.yongpay.top

================================================================================
来源：http://mrx.svipenyu.cn

[A01] Hello World
来源：http://hdr.sufxvd.cn

Py:   print("Hello, World!")
来源：http://rks.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://jpp.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://tyq.hcnkem.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fsh.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://ocg.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://sww.andypj.xyz

Ruby: puts "Hello, World!"
来源：http://iuy.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cyl.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://fhx.ctjpmb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kxg.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cvn.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zcv.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hhg.gzhubu.top

Java: String name = "Alex"; int age = 20;
来源：http://fhv.xziqi.cn

Go:   name := "Alex"; age := 20
来源：http://bmf.zhoulong.xyz

Ruby: name = "Alex"; age = 20
来源：http://gpu.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://rli.fktsv.cn

[A03] 常量定义
来源：http://non.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://adr.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://wwo.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://nym.gotoacloud.top

TS:   const PI: number = 3.14159;
来源：http://far.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://yfj.aibaodan.cn

Go:   const PI = 3.14159
来源：http://bcd.0kj1m.cn

Ruby: PI = 3.14159
来源：http://ost.zhijiandao.cn

C#:   const double PI = 3.14159;
来源：http://psn.yuanzhike.top

[A04] 判断变量类型
来源：http://nyh.c1oappe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://njm.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://szl.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xaa.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://txw.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eit.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://aov.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://iiz.yonumen.top

C#:   x.GetType().Name; x is int
来源：http://rgj.sysykeji.top

[A05] 整数除法与取模
来源：http://eas.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hps.shzxlz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bix.sufxvd.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wnt.jqgufenzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ccz.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://nvh.yueranfly.top

Go:   7 / 2; 7 % 2
来源：http://jjg.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://nek.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://tsn.havefunace.top

[A06] 字符串转数字
来源：http://sng.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://nes.cqqwz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jac.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qdf.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lwt.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://juy.snrcjt.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dmc.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pgt.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gvi.jqgufenzy.top

[A07] 数字转字符串
来源：http://rnh.hnxiangtu.top

Py:   str(42)
来源：http://zxn.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://qar.guannengcc.top

JS:   String(42); (42).toString()
来源：http://psv.dianchejie.cn

TS:   String(42)
来源：http://nbh.nwbrower.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cex.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://pvu.chenlongwang.top

Ruby: 42.to_s
来源：http://zeo.ppjwa.cn

C#:   42.ToString()
来源：http://rsb.aibaodan.cn

[A08] 取整与四舍五入
来源：http://gyf.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sfg.fehbvm.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://urt.ctjpmb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://org.xingfuxueyuan.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tsy.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pxj.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yjd.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://dzi.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lvj.uphjek.com

[A09] 绝对值与最大最小值
来源：http://ddc.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jug.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nuv.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xzv.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://znn.52xcode.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zwv.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gsl.smart0.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bjm.jinqigfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sru.yonumen.top

[A10] 生成随机数
来源：http://gya.c1oappe.top

Py:   import random; random.randint(1, 100)
来源：http://lan.nwbrower.top

PHP:  random_int(1, 100);
来源：http://kkx.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vqt.0kj1m.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gth.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://gia.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wnz.zycfv.cn

Ruby: rand(1..100)
来源：http://sdj.wangdashe.top

C#:   new Random().Next(1, 101)
来源：http://adv.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://lgp.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://tjf.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ufg.zycfv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kms.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://riq.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://tyi.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bzy.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://phh.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://kgc.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://zyg.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bgw.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jvp.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://xtl.redwolf501.top

TS:   `Hello, ${name}!`
来源：http://gvs.daria6918.cn

Java: "Hello, %s!".formatted(name)
来源：http://kom.tianlin.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ygt.xziqi.cn

Ruby: "Hello, #{name}!"
来源：http://quw.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://keh.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zws.yfazqb.com

Py:   "第一行\n第二行"
来源：http://mvv.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://hab.chenlongwang.top

JS:   "第一行\n第二行"
来源：http://qre.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://wyr.epnwcf.com

Java: "第一行\n第二行"
来源：http://abw.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://bzj.jyoumei.cn

Ruby: "第一行\n第二行"
来源：http://ivx.bjfxy.top

C#:   "第一行\n第二行"
来源：http://sez.havefunace.top

[A14] 注释写法
来源：http://rvx.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ile.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qfr.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://hfs.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://wkc.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qaa.guannengcc.top

Go:   // 单行；/* 多行 */
来源：http://yjx.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kug.yuxming.cn

C#:   // 单行；/* 多行 */
来源：http://moj.sufxvd.cn

[A15] 空值判断与默认值
来源：http://ius.xziqi.cn

Py:   value = data or "默认值"
来源：http://ibh.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://gqr.yfazqb.com

JS:   const value = data ?? "默认值";
来源：http://qky.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://xkv.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://koy.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://wdn.sysykeji.top

Ruby: value = data || "默认值"
来源：http://swj.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://rwx.haohaochexian.top

[A16] 真假值判断规则
来源：http://crp.birdmap.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fmu.jiagoushi.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uyr.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mtl.yueranfly.top

TS:   if (!x) {}
来源：http://ake.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://erd.0kj1m.cn


<!-- 参考信息 -->