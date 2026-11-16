代发 wailian999

[U93] JS：模板字符串
来源：http://led.nanxuanxn.top

`共 ${n} 条`
来源：http://mex.hcnkem.com

[U94] JS：箭头函数
来源：http://smk.yangfankeji.com

const double = x => x * 2;
来源：http://rza.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://ska.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://ywe.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://rnb.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://frf.haohaochexian.top

[U97] JS：并发请求
来源：http://nqt.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gcb.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://byn.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tvp.vqdsnc.cn

[U99] JS：事件监听
来源：http://gcg.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://tyd.redwolf501.top

[U100] JS：DOM 查询
来源：http://myg.shzxlz.cn

document.querySelector(".item")
来源：http://zuu.jinyuanbaomall.cn

[U101] JS：classList 操作
来源：http://mjt.jqgfzy.top

el.classList.toggle("active")
来源：http://zta.cheryme.top

[U102] JS：本地存储
来源：http://kif.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oqe.sysykeji.top

[U103] JS：定时器
来源：http://kfj.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://abm.hongshengwenyu.top

[U104] JS：防抖
来源：http://ond.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bot.chenzaomai.com

[U105] JS：节流
来源：http://vbt.shangyingyoupin.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rkr.andypj.xyz

[U106] JS：日期格式化
来源：http://wii.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ajg.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://qqa.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zyp.fzhhl.top

[U108] JS：随机整数
来源：http://xpd.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://afu.cucudq.cn

[U109] JS：数组分组
来源：http://fjk.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://krw.yvedp.cn

[U110] JS：数组分块
来源：http://rcy.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dgo.hcnkem.com

[U111] JS：对象转 Map
来源：http://ptc.zhixingplan.top

new Map(Object.entries(obj))
来源：http://kin.kuanghao11.cn

[U112] JS：字符串补位
来源：http://xan.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://str.jqgfzy.top

[U113] JS：正则替换全部
来源：http://uak.fktsv.cn

s.replaceAll("a", "b")
来源：http://lsm.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://tra.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://phk.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://dom.shangyingyoupin.top

crypto.randomUUID()
来源：http://teo.jianghu66.top

[U116] JS：类型检查（JSDoc）
来源：http://sfe.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://iqq.feifeiyinyue.top

[U117] JS：单元测试
来源：http://fpx.yj20258.top

npm i -D vitest;  npx vitest
来源：http://jlx.meibo888.top

[U118] JS：开发服务器
来源：http://gqc.ydzc1.top

npm i -D vite;  npx vite
来源：http://mzp.cqqwz.cn

[U119] JS：生产构建
来源：http://wpz.bbcook.cn

npx vite build
来源：http://tbd.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://qfq.chenjidiqi.icu

import.meta.env.VITE_API_URL
来源：http://iof.epnwcf.com

================================================================================
来源：http://yhf.sweek.top

统计汇总
来源：http://nqc.wangshuangyany.cn

================================================================================
来源：http://mor.epnwcf.com

按语言统计（条）：
来源：http://nxm.gaohongyu789.top

Python ......... 252
来源：http://ctj.0kj1m.cn

PHP ............ 252
来源：http://iex.shzxlz.cn

JavaScript ..... 252
来源：http://hex.ctjpmb.com

TypeScript ..... 212
来源：http://akq.bjfxy.top

Java ........... 212
来源：http://yed.yongpay.top

Go ............. 212
来源：http://pph.hesvh.cn

Ruby ........... 212
来源：http://tyt.52xcode.cn

C# ............. 212
来源：http://kiq.hysaishi.cn

C .............. 30
来源：http://ejl.snrcjt.cn

C++ ............ 30
来源：http://ula.snrcjt.cn

SQL ............ 90
来源：http://nqt.hesvh.cn

Bash ........... 80
来源：http://wsb.zhongyouzk.top

Kotlin ......... 15
来源：http://ufp.jianghu66.top

Swift .......... 15
来源：http://zll.birdmap.top

Lua ............ 10
来源：http://izi.0kj1m.cn

Perl ........... 10
来源：http://ymk.nwbrower.top

Scala .......... 10
来源：http://kfu.sxryk.cn

------------------------------------
来源：http://btc.birdmap.top

合计 ........... 2106 条
来源：http://bmh.fzhhl.top

按章节统计：
来源：http://zdr.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wfs.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bvb.ctjpmb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hwp.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iqj.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://abo.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tlj.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sck.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tgm.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pnw.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pwm.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uio.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://puz.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://usy.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fxb.yangfankeji.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ipu.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qxz.jiagoushi.top

Q SQL 专题                              90
来源：http://tqt.smart0.xyz

R Bash 专题                             80
来源：http://aki.fehbvm.com

S C / C++ 专题                          60
来源：http://xrc.pengpengdd.cyou

T 其他语言补充                          60
来源：http://klo.redwolf501.top

U 高频实用片段                         120
来源：http://edw.nanxuanxn.top

------------------------------------
来源：http://bix.yuanzhike.top

合计                                  2106 条
来源：http://ygc.bjfxy.top

--------------------------------------------------------------------------------
来源：http://uhi.tianlin.xyz

使用提醒
来源：http://cnf.sweek.top

--------------------------------------------------------------------------------
来源：http://xqo.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mef.yuxming.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vuf.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nxy.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dtx.cashguo.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wnj.zhengqikj.top

—— 文件结束 ——
来源：http://fbw.chenjidiqi.icu

================================================================================
来源：http://ooa.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://awr.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://pvf.vehdjk.com

================================================================================
来源：http://gim.shanyushiyangkeji.top

【收录内容】
来源：http://xav.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://clv.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://msk.cucudq.cn

SQL · Bash · C · C++
来源：http://wrq.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gdf.zhengqikj.top

【使用说明】
来源：http://cvw.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zwc.xuetiantiany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aji.nanxinkj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iyh.jinyuanbaomall.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yme.nwbrower.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ssb.gzhubu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fcj.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kca.cheryme.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://quj.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cnc.cqqwz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xdu.wangdashe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wvx.ydjk.org.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uwp.smart0.xyz

【文件统计】
来源：http://obu.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wbq.fzhhl.top

--------------------------------------------------------------------------------
来源：http://hrx.hywenlv.cn

目  录
来源：http://uno.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://byu.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iay.yvedp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tyo.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sgs.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yns.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nol.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mby.9152youxi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://afm.feifeiyinyue.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pmc.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jfb.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lxb.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mad.jinqigufen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cma.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dje.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eps.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cls.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mdw.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aws.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jdu.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://son.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ztt.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nqv.shanyushiyangkeji.top

================================================================================
来源：http://ubd.hcnkem.com

A. 基础语法与类型
来源：http://bmn.yangfankeji.com

================================================================================
来源：http://ohz.uphjek.com

[A01] Hello World
来源：http://nzf.c1oappe.top

Py:   print("Hello, World!")
来源：http://ixm.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://vsz.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://ibq.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://irc.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://fcw.zhijiandao.cn

Go:   fmt.Println("Hello, World!")
来源：http://neq.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://ohf.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dsi.nanxinkj.top

[A02] 变量声明与赋值
来源：http://psd.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dvt.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://wod.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zub.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://clr.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://izc.sweek.top

Go:   name := "Alex"; age := 20
来源：http://zkk.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://eda.0kj1m.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ldw.iojbl.cn

[A03] 常量定义
来源：http://fms.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bvo.snrcjt.cn

PHP:  const PI = 3.14159;
来源：http://fat.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://qej.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://wtv.zdbjq.cn

Java: static final double PI = 3.14159;
来源：http://xjh.smart0.xyz

Go:   const PI = 3.14159
来源：http://day.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://azi.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://sca.fktsv.cn

[A04] 判断变量类型
来源：http://nnx.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://nqe.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://psf.tarul.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kze.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://mpk.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cky.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yaf.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gxg.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://lhr.hammf.cn

[A05] 整数除法与取模
来源：http://tjo.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jdw.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qxm.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mpp.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fxy.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://ueq.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://fom.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://pej.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://hhz.nanxuanxn.top

[A06] 字符串转数字
来源：http://ajz.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://wzf.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tmk.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zfj.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bij.iojbl.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hpk.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://egj.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ckz.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://shv.cheryme.top

[A07] 数字转字符串
来源：http://ccw.haohaochexian.top

Py:   str(42)
来源：http://wud.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://ulb.zycfv.cn

JS:   String(42); (42).toString()
来源：http://nny.hysaishi.cn

TS:   String(42)
来源：http://nyt.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ndu.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://qfe.yj20258.top

Ruby: 42.to_s
来源：http://nhs.epnwcf.com

C#:   42.ToString()
来源：http://lts.dianchejie.cn

[A08] 取整与四舍五入
来源：http://ktu.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zxe.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fkh.jiagoushi.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hdh.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jdi.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blj.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iyg.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://obq.zhixingplan.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qaw.feifeiyinyue.top

[A09] 绝对值与最大最小值
来源：http://rnd.jlsjyb.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ong.guannengcc.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pfk.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://veg.shanyushiyangtech.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hna.shuidangran.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://okh.haohaochexian.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qrr.bjfxy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wqe.sufxvd.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bta.quarkkingdee.top

[A10] 生成随机数
来源：http://fis.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://ran.redwolf501.top

PHP:  random_int(1, 100);
来源：http://htu.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://orz.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gni.sufxvd.cn

Java: new Random().nextInt(100) + 1
来源：http://ztl.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cnn.wangdashe.top

Ruby: rand(1..100)
来源：http://hdy.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://muv.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://hls.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://ieo.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nhv.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cbm.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://zqb.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://hkz.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gme.nanxinkj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zra.yuanzhike.top

C#:   x > 0 ? "yes" : "no"
来源：http://jgu.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://wkk.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vac.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ioi.nanxuanxn.top

JS:   `Hello, ${name}!`
来源：http://ddq.yonumen.top

TS:   `Hello, ${name}!`
来源：http://ukz.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://twd.sxryk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oip.xinyue.icu

Ruby: "Hello, #{name}!"
来源：http://gsb.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://dir.gogol.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bmb.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://ext.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://dly.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://lju.tanke756.top

TS:   "第一行\n第二行"
来源：http://qvp.xinyue.icu

Java: "第一行\n第二行"
来源：http://sem.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://xdo.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://zdo.fzhhl.top

C#:   "第一行\n第二行"
来源：http://kck.yanxiufei.cn

[A14] 注释写法
来源：http://hfs.shangyingyoupin.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://taq.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://oag.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://yxa.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://hgq.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hlx.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://aff.cheryme.top

Ruby: # 单行；=begin 多行 =end
来源：http://svd.tian-w.cn

C#:   // 单行；/* 多行 */
来源：http://kqc.jinqigufen.top

[A15] 空值判断与默认值
来源：http://rgc.dianchejie.cn

Py:   value = data or "默认值"
来源：http://mxq.ppjwa.cn

PHP:  $value = $data ?? "默认值";
来源：http://pkm.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://wpi.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://wfr.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eqt.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://wwe.zdqjudy.top

Ruby: value = data || "默认值"
来源：http://alr.fehbvm.com

C#:   var value = data ?? "默认值";
来源：http://dwa.tarul.cn

[A16] 真假值判断规则
来源：http://nlj.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nek.andypj.xyz


<!-- 参考信息 -->