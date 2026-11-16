代发 wailian999

[U95] JS：Promise 包装
来源：http://lji.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://rsl.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://pwo.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nus.cheryme.top

[U97] JS：并发请求
来源：http://tyq.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://sfo.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://mol.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ymq.ehwqpu.com

[U99] JS：事件监听
来源：http://yzu.fktsv.cn

el.addEventListener("click", e => {})
来源：http://yhw.fengsongda.top

[U100] JS：DOM 查询
来源：http://ffw.gogol.net.cn

document.querySelector(".item")
来源：http://ghw.jyoumei.cn

[U101] JS：classList 操作
来源：http://bsp.zdbjq.cn

el.classList.toggle("active")
来源：http://ivb.svipenyu.cn

[U102] JS：本地存储
来源：http://flt.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yrl.c1oappe.top

[U103] JS：定时器
来源：http://syi.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fgd.hywenlv.cn

[U104] JS：防抖
来源：http://rbq.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqs.birdmap.top

[U105] JS：节流
来源：http://cln.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jmn.ehwqpu.com

[U106] JS：日期格式化
来源：http://sip.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qcf.sxryk.cn

[U107] JS：数字千分位
来源：http://xtd.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://plw.sysykeji.top

[U108] JS：随机整数
来源：http://jrj.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qab.gogol.net.cn

[U109] JS：数组分组
来源：http://jii.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://qkz.dashuyun.cn

[U110] JS：数组分块
来源：http://eex.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gui.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://fet.pycfn.com

new Map(Object.entries(obj))
来源：http://cyy.zhengqikj.top

[U112] JS：字符串补位
来源：http://kvj.hywenlv.cn

"7".padStart(3, "0")
来源：http://cta.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://btv.bjfxy.top

s.replaceAll("a", "b")
来源：http://pic.hcnkem.com

[U114] JS：JSON 深比较
来源：http://qxe.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vwe.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://qyg.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://mqv.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://zmb.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://mtz.zhoulong.xyz

[U117] JS：单元测试
来源：http://xfp.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://kgh.pycfn.com

[U118] JS：开发服务器
来源：http://eie.tian-w.cn

npm i -D vite;  npx vite
来源：http://xqs.hnxiangtu.top

[U119] JS：生产构建
来源：http://qaw.316326.xyz

npx vite build
来源：http://lqo.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://bbv.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://ero.dashuyun.cn

================================================================================
来源：http://jkj.kuanghao11.cn

统计汇总
来源：http://cln.guannengcc.top

================================================================================
来源：http://noq.vqdsnc.cn

按语言统计（条）：
来源：http://nye.jinghuilouyu.cn

Python ......... 252
来源：http://auw.yuxming.cn

PHP ............ 252
来源：http://uhy.xylfe.cn

JavaScript ..... 252
来源：http://dhc.nwbrower.top

TypeScript ..... 212
来源：http://vxq.hysaishi.cn

Java ........... 212
来源：http://twt.gotoacloud.top

Go ............. 212
来源：http://unu.ydzc1.top

Ruby ........... 212
来源：http://jif.havefunace.top

C# ............. 212
来源：http://flm.zhongyouzk.top

C .............. 30
来源：http://luj.316326.xyz

C++ ............ 30
来源：http://iai.smart0.xyz

SQL ............ 90
来源：http://eep.9152youxi.cn

Bash ........... 80
来源：http://swq.jyoumei.cn

Kotlin ......... 15
来源：http://kds.sufxvd.cn

Swift .......... 15
来源：http://cll.fzhhl.top

Lua ............ 10
来源：http://lwn.uphjek.com

Perl ........... 10
来源：http://skq.yangfankeji.com

Scala .......... 10
来源：http://ffr.jinghuilouyu.cn

------------------------------------
来源：http://qkq.bjfxy.top

合计 ........... 2106 条
来源：http://foj.nanxinkj.top

按章节统计：
来源：http://bdq.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rog.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://olb.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ycp.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nqe.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aja.hesvh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wix.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eog.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rro.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ohf.epnwcf.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oaw.sxryk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wlr.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ytf.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://byi.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cmf.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pbh.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zou.shuidangran.top

Q SQL 专题                              90
来源：http://prm.shanyushiyangtech.top

R Bash 专题                             80
来源：http://rqf.cdnleiting.top

S C / C++ 专题                          60
来源：http://isw.cdnleiting.top

T 其他语言补充                          60
来源：http://uah.xinyue.icu

U 高频实用片段                         120
来源：http://bpf.yj20258.top

------------------------------------
来源：http://eki.aibaodan.cn

合计                                  2106 条
来源：http://uol.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://tih.sxryk.cn

使用提醒
来源：http://jal.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://tjf.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blx.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fsb.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vgy.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://txt.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xzw.c1oappe.top

—— 文件结束 ——
来源：http://pkb.yj202588.top

================================================================================
来源：http://fbl.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://npu.sysykeji.top

Common Programming Examples Cheat Book
来源：http://tbm.jlsjyb.cn

================================================================================
来源：http://eyb.shzxlz.cn

【收录内容】
来源：http://rts.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ehd.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wco.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://sdi.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hqj.kuanghao11.cn

【使用说明】
来源：http://rsd.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yxl.c1oappe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rly.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pbj.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kwa.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://mep.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wuq.vehdjk.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qgo.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ozk.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pey.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kkz.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qzb.ctjpmb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gbw.hywenlv.cn

【文件统计】
来源：http://pzq.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rkn.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://cvu.fengsongda.top

目  录
来源：http://wio.yj202588.top

--------------------------------------------------------------------------------
来源：http://nti.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cgd.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zgq.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://asi.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sja.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iec.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://obf.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zbb.sxryk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cow.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mbc.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vic.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://syg.chenzaomai.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sgz.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zhx.guowangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ufc.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://poj.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bsv.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vge.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dvh.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pfk.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yug.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nty.yuxming.cn

================================================================================
来源：http://awp.c1oappe.top

A. 基础语法与类型
来源：http://gia.zhongyouzk.top

================================================================================
来源：http://txu.fehbvm.com

[A01] Hello World
来源：http://kai.daxiang520.top

Py:   print("Hello, World!")
来源：http://gyg.jqgufenzy.top

PHP:  echo "Hello, World!";
来源：http://ljl.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://rla.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hmu.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://gox.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://qqi.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://ues.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hzy.fengsongda.top

[A02] 变量声明与赋值
来源：http://mxz.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kiy.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://gdo.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://ane.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mrw.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://qel.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://ieo.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://oze.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mrh.uphjek.com

[A03] 常量定义
来源：http://ffw.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pxz.nanxuanxn.top

PHP:  const PI = 3.14159;
来源：http://ima.bbcook.cn

JS:   const PI = 3.14159;
来源：http://bgt.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://dpo.xziqi.cn

Java: static final double PI = 3.14159;
来源：http://pcm.shanyushiyangkeji.top

Go:   const PI = 3.14159
来源：http://fvb.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://mun.jinqigufen.top

C#:   const double PI = 3.14159;
来源：http://oai.jqgufenzy.top

[A04] 判断变量类型
来源：http://flb.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jvw.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wuw.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xqe.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://qvw.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://myz.jyoumei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aot.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ihf.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://spx.kuanghao11.cn

[A05] 整数除法与取模
来源：http://gzr.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yir.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xgp.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ele.jqgufenzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rdr.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://oug.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://zpa.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://isa.cashguo.top

C#:   7 / 2; 7 % 2
来源：http://tsg.shzxlz.cn

[A06] 字符串转数字
来源：http://opf.tanke756.top

Py:   int("42"); float("3.14")
来源：http://sac.bjfxy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sbk.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ckm.xziqi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pyt.ctjpmb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fdi.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qui.jqgfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ufv.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sci.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://cak.yj20258.top

Py:   str(42)
来源：http://azw.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://rdb.gzhubu.top

JS:   String(42); (42).toString()
来源：http://uei.tianlin.xyz

TS:   String(42)
来源：http://etv.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wsa.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://uuz.dashuyun.cn

Ruby: 42.to_s
来源：http://dey.nwbrower.top

C#:   42.ToString()
来源：http://tlh.zhijiandao.cn

[A08] 取整与四舍五入
来源：http://dym.vqdsnc.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yke.sysykeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zgd.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eff.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nry.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ixc.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://awg.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jdk.hammf.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kde.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://heu.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xga.sufxvd.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://igt.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tga.snrcjt.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cor.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ehj.wangdashe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dhh.sufxvd.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jmf.chenlongwang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vsr.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://ifp.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://cmz.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://ygs.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mwg.birdmap.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xgg.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://qmq.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mst.havefunace.top

Ruby: rand(1..100)
来源：http://caj.dianchejie.cn

C#:   new Random().Next(1, 101)
来源：http://wyx.hongshengwenyu.top

[A11] 条件表达式（三元）
来源：http://neb.xylfe.cn

Py:   "yes" if x > 0 else "no"
来源：http://cvv.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://yko.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kar.gotoacloud.top

TS:   x > 0 ? "yes" : "no"
来源：http://xwi.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://ktg.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qpc.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://esa.hcnkem.com

C#:   x > 0 ? "yes" : "no"
来源：http://rui.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://kmc.zhiwuduotai.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bau.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sgx.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://kgs.gotoacloud.top

TS:   `Hello, ${name}!`
来源：http://ogh.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://wab.dashuyun.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xzv.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://szg.aizwys.cn

C#:   $"Hello, {name}!"
来源：http://khn.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eyz.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://ewl.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://myp.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://ctl.c1oappe.top

TS:   "第一行\n第二行"
来源：http://wet.jinqigufen.top

Java: "第一行\n第二行"
来源：http://vit.ybcxt.top

Go:   "第一行\n第二行"
来源：http://lce.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://jzc.xinyue.icu

C#:   "第一行\n第二行"
来源：http://nvf.0kj1m.cn

[A14] 注释写法
来源：http://wcv.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xph.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fec.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://stx.kuanghao11.cn

TS:   // 单行；/* 多行 */
来源：http://gya.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ioa.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://ysk.fehbvm.com

Ruby: # 单行；=begin 多行 =end
来源：http://yje.ppjwa.cn

C#:   // 单行；/* 多行 */
来源：http://ymc.zhixingplan.top

[A15] 空值判断与默认值
来源：http://pgx.shzxlz.cn

Py:   value = data or "默认值"
来源：http://lhw.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://kaa.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://rqn.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://wqm.hesvh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://azv.pycfn.com

Go:   if data == "" { data = "默认值" }
来源：http://dgr.fehbvm.com

Ruby: value = data || "默认值"
来源：http://zaz.haohaochexian.top

C#:   var value = data ?? "默认值";
来源：http://qnk.hysaishi.cn

[A16] 真假值判断规则
来源：http://gzx.9152youxi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://olx.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yhu.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://seg.shuidangran.top

TS:   if (!x) {}
来源：http://kzo.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ofx.zhixingplan.top


<!-- 参考信息 -->