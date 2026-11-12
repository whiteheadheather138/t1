代发 wailian999

[U93] JS：模板字符串
来源：http://xwe.fktsv.cn

`共 ${n} 条`
来源：http://sca.zhoulong.xyz

[U94] JS：箭头函数
来源：http://pfu.xziqi.cn

const double = x => x * 2;
来源：http://ljd.yuxming.cn

[U95] JS：Promise 包装
来源：http://xdy.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://jlx.cheryme.top

[U96] JS：async/await 与异常
来源：http://bpp.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ipo.epnwcf.com

[U97] JS：并发请求
来源：http://hpw.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fkc.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://uby.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://clk.yj20258888.top

[U99] JS：事件监听
来源：http://ojq.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://slu.hywenlv.cn

[U100] JS：DOM 查询
来源：http://wwg.yonumen.top

document.querySelector(".item")
来源：http://con.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://uao.sweek.top

el.classList.toggle("active")
来源：http://sdg.xziqi.cn

[U102] JS：本地存储
来源：http://izn.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gtq.52xcode.cn

[U103] JS：定时器
来源：http://mut.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jvc.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://iel.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ved.vehdjk.com

[U105] JS：节流
来源：http://vft.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sjl.hesvh.cn

[U106] JS：日期格式化
来源：http://prb.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xha.uphjek.com

[U107] JS：数字千分位
来源：http://imk.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lon.ydzc1.top

[U108] JS：随机整数
来源：http://whz.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bxh.guannengcc.top

[U109] JS：数组分组
来源：http://vto.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://lbq.jyoumei.cn

[U110] JS：数组分块
来源：http://cnm.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://naf.jinqigufen.top

[U111] JS：对象转 Map
来源：http://gpp.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://mex.jqgfzy.top

[U112] JS：字符串补位
来源：http://vrj.yanxiufei.cn

"7".padStart(3, "0")
来源：http://gqe.cashguo.top

[U113] JS：正则替换全部
来源：http://tun.sysykeji.top

s.replaceAll("a", "b")
来源：http://aps.c1oappe.top

[U114] JS：JSON 深比较
来源：http://kpi.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://scs.dashuyun.cn

[U115] JS：生成 UUID
来源：http://xdx.epnwcf.com

crypto.randomUUID()
来源：http://zmw.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://kfa.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://lbd.quarkkingdee.top

[U117] JS：单元测试
来源：http://gfg.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://jdi.yanxiufei.cn

[U118] JS：开发服务器
来源：http://isr.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://zen.hysaishi.cn

[U119] JS：生产构建
来源：http://gss.chenlongwang.top

npx vite build
来源：http://rbd.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://obh.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://sys.fehbvm.com

================================================================================
来源：http://sbj.jinqigfzy.top

统计汇总
来源：http://soy.tianlin.xyz

================================================================================
来源：http://nvc.hysaishi.cn

按语言统计（条）：
来源：http://hmd.tian-w.cn

Python ......... 252
来源：http://sqy.yongpay.top

PHP ............ 252
来源：http://lkn.zdbjq.cn

JavaScript ..... 252
来源：http://kwx.bbcook.cn

TypeScript ..... 212
来源：http://omk.bjfxy.top

Java ........... 212
来源：http://bun.52xcode.cn

Go ............. 212
来源：http://uvi.jianghu66.top

Ruby ........... 212
来源：http://yhj.fengsongda.top

C# ............. 212
来源：http://ryz.shanyushiyangtech.top

C .............. 30
来源：http://sqe.chenzaomai.com

C++ ............ 30
来源：http://wyp.52xcode.cn

SQL ............ 90
来源：http://ngy.9152youxi.cn

Bash ........... 80
来源：http://kdj.yongpay.top

Kotlin ......... 15
来源：http://gwd.cqqwz.cn

Swift .......... 15
来源：http://cxj.sysykeji.top

Lua ............ 10
来源：http://ojf.jlsjyb.cn

Perl ........... 10
来源：http://qse.zhengqikj.top

Scala .......... 10
来源：http://tsi.yanxiufei.cn

------------------------------------
来源：http://oco.fzhhl.top

合计 ........... 2106 条
来源：http://jmz.cheryme.top

按章节统计：
来源：http://izw.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vhh.bbcook.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uzp.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gyb.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://anl.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://btc.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dqq.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ess.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ziv.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qns.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kim.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ntv.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sln.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qsk.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jjw.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zpc.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vpt.fktsv.cn

Q SQL 专题                              90
来源：http://suq.tian-w.cn

R Bash 专题                             80
来源：http://gmf.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://ssh.iojbl.cn

T 其他语言补充                          60
来源：http://tia.ydzc1.top

U 高频实用片段                         120
来源：http://gpp.zhaomingkeji.xyz

------------------------------------
来源：http://mtd.meibo888.top

合计                                  2106 条
来源：http://hhn.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://mzz.jinyuanbaomall.cn

使用提醒
来源：http://zbn.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://enm.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://znk.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kvk.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nuw.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://plm.vehdjk.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lvf.jinqigfzy.top

—— 文件结束 ——
来源：http://wmu.zhoulong.xyz

================================================================================
来源：http://iyp.fktsv.cn

程序语言常见例子速查手册（2024 版）
来源：http://gqv.uphjek.com

Common Programming Examples Cheat Book
来源：http://hmb.xylfe.cn

================================================================================
来源：http://vne.cqqwz.cn

【收录内容】
来源：http://ley.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wbm.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ipl.quarkkingdee.top

SQL · Bash · C · C++
来源：http://lfz.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vrz.tanke756.top

【使用说明】
来源：http://hwd.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ltd.sweek.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zcy.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://der.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gtd.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fer.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ifr.jinqigfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uhn.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ggg.hnxiangtu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rhy.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xhy.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zei.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mcz.ydjk.org.cn

【文件统计】
来源：http://giw.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wua.pycfn.com

--------------------------------------------------------------------------------
来源：http://giy.ctjpmb.com

目  录
来源：http://xlx.tanke756.top

--------------------------------------------------------------------------------
来源：http://ijx.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fog.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jut.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xpj.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bve.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bjf.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rur.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://odk.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://axo.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bdq.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mvo.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ngp.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ddx.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://djw.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hlt.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aug.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hnc.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tvw.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://qhc.hfpthk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vyb.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cuw.birdmap.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zrr.dianchejie.cn

================================================================================
来源：http://yoq.tianlin.xyz

A. 基础语法与类型
来源：http://zmx.0kj1m.cn

================================================================================
来源：http://gcl.ehwqpu.com

[A01] Hello World
来源：http://rro.zhoulong.xyz

Py:   print("Hello, World!")
来源：http://fff.tanke756.top

PHP:  echo "Hello, World!";
来源：http://cyp.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://idb.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://svu.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://ibh.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://egl.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://ipk.bbcook.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oss.gotoacloud.top

[A02] 变量声明与赋值
来源：http://yia.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tbo.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xmk.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xkq.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jfn.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://eoe.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://iyd.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://mdr.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://omw.birdmap.top

[A03] 常量定义
来源：http://igm.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dqt.epnwcf.com

PHP:  const PI = 3.14159;
来源：http://nwg.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://bar.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://usu.cashguo.top

Java: static final double PI = 3.14159;
来源：http://swv.xingfuxueyuan.xyz

Go:   const PI = 3.14159
来源：http://kvw.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://ocj.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://aya.epnwcf.com

[A04] 判断变量类型
来源：http://xeq.yongpay.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jnt.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://edz.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://quc.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://bys.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://caj.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://blb.chenlongwang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xwd.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://oxm.sufxvd.cn

[A05] 整数除法与取模
来源：http://vok.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bce.dianchejie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zan.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kae.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kht.ehwqpu.com

Java: 7 / 2; 7 % 2
来源：http://jjs.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://kbc.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://kkh.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://bgb.hnxiangtu.top

[A06] 字符串转数字
来源：http://zqq.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://zyp.sysykeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fos.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lhd.jlsjyb.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dlv.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://meo.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nyw.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hks.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zee.ivvv.top

[A07] 数字转字符串
来源：http://lph.hnxiangtu.top

Py:   str(42)
来源：http://vot.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://bai.xuanzx.com

JS:   String(42); (42).toString()
来源：http://rde.hesvh.cn

TS:   String(42)
来源：http://arm.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xng.hammf.cn

Go:   strconv.Itoa(42)
来源：http://egy.aibaodan.cn

Ruby: 42.to_s
来源：http://lrx.snrcjt.cn

C#:   42.ToString()
来源：http://bsl.chenlongwang.top

[A08] 取整与四舍五入
来源：http://blb.yj20258888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tug.yonumen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lko.birdmap.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fub.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kqj.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gjt.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jff.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vfe.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ycg.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://ejn.dianchejie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mec.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ayw.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://onz.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eoj.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://olg.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jwl.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ztj.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uhg.hammf.cn

[A10] 生成随机数
来源：http://mxw.bjfxy.top

Py:   import random; random.randint(1, 100)
来源：http://zon.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://fjp.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bxg.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fhv.uphjek.com

Java: new Random().nextInt(100) + 1
来源：http://yic.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yqh.ywan-chungtsiang.top

Ruby: rand(1..100)
来源：http://onh.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://qlu.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://nvw.mhx1999.top

Py:   "yes" if x > 0 else "no"
来源：http://rqg.smart0.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://qmv.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qif.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://yav.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://fud.hysaishi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://irt.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jaq.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bez.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://orp.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zxc.fehbvm.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lfx.yj20258888.top

JS:   `Hello, ${name}!`
来源：http://zuz.cqqwz.cn

TS:   `Hello, ${name}!`
来源：http://ych.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://nzs.cheryme.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vck.snrcjt.cn

Ruby: "Hello, #{name}!"
来源：http://yqg.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://dtz.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://tcy.bbcook.cn

Py:   "第一行\n第二行"
来源：http://aad.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://mvn.fehbvm.com

JS:   "第一行\n第二行"
来源：http://apn.hammf.cn

TS:   "第一行\n第二行"
来源：http://uxs.smart0.xyz

Java: "第一行\n第二行"
来源：http://odc.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://bua.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://aci.fktsv.cn

C#:   "第一行\n第二行"
来源：http://fju.nanxuanxn.top

[A14] 注释写法
来源：http://flr.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ctq.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://hwn.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://zbs.chenzaomai.com

TS:   // 单行；/* 多行 */
来源：http://zed.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cya.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://coz.gotoacloud.top

Ruby: # 单行；=begin 多行 =end
来源：http://ibx.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://pld.pycfn.com

[A15] 空值判断与默认值
来源：http://gke.yanxiufei.cn

Py:   value = data or "默认值"
来源：http://evl.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://ldz.zhengqikj.top

JS:   const value = data ?? "默认值";
来源：http://tjp.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://ole.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tyv.yfazqb.com

Go:   if data == "" { data = "默认值" }
来源：http://kxm.meibo888.top

Ruby: value = data || "默认值"
来源：http://ezm.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://xjf.yanxiufei.cn

[A16] 真假值判断规则
来源：http://icq.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qbz.fktsv.cn


<!-- 参考信息 -->