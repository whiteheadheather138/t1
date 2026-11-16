代发 wailian999

[U99] JS：事件监听
来源：http://rcb.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://fof.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://upj.cqqwz.cn

document.querySelector(".item")
来源：http://yht.bbcook.cn

[U101] JS：classList 操作
来源：http://tcq.zhixingplan.top

el.classList.toggle("active")
来源：http://zop.meibo888.top

[U102] JS：本地存储
来源：http://sfm.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ztu.gogol.net.cn

[U103] JS：定时器
来源：http://ukk.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kvo.havefunace.top

[U104] JS：防抖
来源：http://vwx.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnu.yj20258888.top

[U105] JS：节流
来源：http://mwv.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nzx.snrcjt.cn

[U106] JS：日期格式化
来源：http://obs.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zei.ydjk.org.cn

[U107] JS：数字千分位
来源：http://lyh.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bqf.hongshengwenyu.top

[U108] JS：随机整数
来源：http://pqo.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ssm.jqgfzy.top

[U109] JS：数组分组
来源：http://xkr.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://lfg.jinqigfzy.top

[U110] JS：数组分块
来源：http://aqb.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qig.zycfv.cn

[U111] JS：对象转 Map
来源：http://ini.9152youxi.cn

new Map(Object.entries(obj))
来源：http://cys.smart0.xyz

[U112] JS：字符串补位
来源：http://zbx.jqgufenzy.top

"7".padStart(3, "0")
来源：http://zrn.ydzc1.top

[U113] JS：正则替换全部
来源：http://gmq.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://rrt.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://mnv.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cbi.yueranfly.top

[U115] JS：生成 UUID
来源：http://dhp.yonumen.top

crypto.randomUUID()
来源：http://vzc.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://mlj.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://cbn.quarkkingdee.top

[U117] JS：单元测试
来源：http://vze.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://dme.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://bqg.hysaishi.cn

npm i -D vite;  npx vite
来源：http://nse.kuanghao11.cn

[U119] JS：生产构建
来源：http://xfp.haohaochexian.top

npx vite build
来源：http://nnr.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://lgs.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://lle.yvedp.cn

================================================================================
来源：http://ubi.gogol.net.cn

统计汇总
来源：http://ugx.daria6918.cn

================================================================================
来源：http://cqt.yvedp.cn

按语言统计（条）：
来源：http://fsa.xylfe.cn

Python ......... 252
来源：http://vzb.aibaodan.cn

PHP ............ 252
来源：http://bnc.fehbvm.com

JavaScript ..... 252
来源：http://xfn.zhixingplan.top

TypeScript ..... 212
来源：http://wcg.ybcxt.top

Java ........... 212
来源：http://yfb.fengsongda.top

Go ............. 212
来源：http://wde.haohaochexian.top

Ruby ........... 212
来源：http://nce.aibaodan.cn

C# ............. 212
来源：http://crr.hywenlv.cn

C .............. 30
来源：http://tay.gzhubu.top

C++ ............ 30
来源：http://hvw.shanyushiyangkeji.top

SQL ............ 90
来源：http://rqf.haohaochexian.top

Bash ........... 80
来源：http://apx.0kj1m.cn

Kotlin ......... 15
来源：http://yqo.yj202588.top

Swift .......... 15
来源：http://pyq.hongshengwenyu.top

Lua ............ 10
来源：http://mgs.wangdashe.top

Perl ........... 10
来源：http://vrb.dashuyun.cn

Scala .......... 10
来源：http://fnl.zycfv.cn

------------------------------------
来源：http://pjb.quarkkingdee.top

合计 ........... 2106 条
来源：http://ogr.hongshengwenyu.top

按章节统计：
来源：http://bez.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xtl.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pqn.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kgv.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kch.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cnv.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lfr.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kil.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://llp.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jgv.hcnkem.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zmb.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ugd.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vib.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mhg.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cih.jianghu66.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://waf.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mxt.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://iqg.sufxvd.cn

R Bash 专题                             80
来源：http://duy.zhixingplan.top

S C / C++ 专题                          60
来源：http://rzp.jqgufenzy.top

T 其他语言补充                          60
来源：http://zdu.birdmap.top

U 高频实用片段                         120
来源：http://fgr.ppjwa.cn

------------------------------------
来源：http://dwr.xuanzx.com

合计                                  2106 条
来源：http://gfr.smart0.xyz

--------------------------------------------------------------------------------
来源：http://nqe.tarul.cn

使用提醒
来源：http://vlj.jianghu66.top

--------------------------------------------------------------------------------
来源：http://pnn.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gwp.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gei.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nho.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jiw.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://whz.yangfankeji.com

—— 文件结束 ——
来源：http://jpl.daxiang520.top

================================================================================
来源：http://pms.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://gxl.tanke756.top

Common Programming Examples Cheat Book
来源：http://sfu.tian-w.cn

================================================================================
来源：http://pgx.yfazqb.com

【收录内容】
来源：http://fku.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wdd.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cav.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://fre.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hkf.jqgufenzy.top

【使用说明】
来源：http://knj.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bec.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xps.yangfankeji.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://krf.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qsw.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nlm.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cex.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lwm.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fiz.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rlf.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kfm.sufxvd.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qjg.tianlin.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://orn.hysaishi.cn

【文件统计】
来源：http://boz.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xok.tian-w.cn

--------------------------------------------------------------------------------
来源：http://mjd.yueranfly.top

目  录
来源：http://rrt.meibo888.top

--------------------------------------------------------------------------------
来源：http://xhl.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jdb.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fjd.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iss.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://shu.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yew.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yvb.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gvp.ehwqpu.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gby.fanxiaobao.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wdq.sweek.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ugo.meibo888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wiv.0kj1m.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nce.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lgu.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vtb.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bwe.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hle.tian-w.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bfl.yvedp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dvo.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uou.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://glb.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cki.yangfankeji.com

================================================================================
来源：http://lxa.dashuyun.cn

A. 基础语法与类型
来源：http://vse.sxryk.cn

================================================================================
来源：http://isg.tianlin.xyz

[A01] Hello World
来源：http://pmi.vqdsnc.cn

Py:   print("Hello, World!")
来源：http://dut.zdqjudy.top

PHP:  echo "Hello, World!";
来源：http://xfu.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://lcb.tarul.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pkp.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://nqw.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://uvx.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://hxx.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ese.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://hti.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ofp.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yfa.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sxv.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xme.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://dfb.dashuyun.cn

Go:   name := "Alex"; age := 20
来源：http://oax.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://sbf.ydjk.org.cn

C#:   string name = "Alex"; int age = 20;
来源：http://udj.shanyushiyangtech.top

[A03] 常量定义
来源：http://ufz.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dmd.cheryme.top

PHP:  const PI = 3.14159;
来源：http://euk.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://gqg.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://ztz.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://diy.ydzc1.top

Go:   const PI = 3.14159
来源：http://vep.zhengqikj.top

Ruby: PI = 3.14159
来源：http://gso.ivvv.top

C#:   const double PI = 3.14159;
来源：http://wch.meibo888.top

[A04] 判断变量类型
来源：http://mex.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ifo.zdqjudy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://itk.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://upi.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://kyf.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ysg.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://ppm.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://jkn.jinqigfzy.top

C#:   x.GetType().Name; x is int
来源：http://cej.ydjk.org.cn

[A05] 整数除法与取模
来源：http://fcl.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cwy.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rws.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hgm.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bwg.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://evp.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://zwp.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://ggs.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://equ.guannengcc.top

[A06] 字符串转数字
来源：http://peu.pycfn.com

Py:   int("42"); float("3.14")
来源：http://zdh.gzhubu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jjv.uphjek.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ieu.redwolf501.top

TS:   parseInt("42", 10); Number("42")
来源：http://ymw.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nng.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rch.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://qix.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eif.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://kgq.fktsv.cn

Py:   str(42)
来源：http://dve.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://ksw.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://jbg.cdnleiting.top

TS:   String(42)
来源：http://erm.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ycb.gaohongyu789.top

Go:   strconv.Itoa(42)
来源：http://oyu.zhengqikj.top

Ruby: 42.to_s
来源：http://zhc.yuxming.cn

C#:   42.ToString()
来源：http://uwp.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://ybh.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zph.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://azz.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tnd.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jqr.jinqigufen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wuq.vehdjk.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xha.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://sdg.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qvs.hammf.cn

[A09] 绝对值与最大最小值
来源：http://yvf.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://btm.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://duc.daria6918.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jeb.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ccc.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wef.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ryx.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tku.ydjk.org.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ohn.chenlongwang.top

[A10] 生成随机数
来源：http://ado.gzhubu.top

Py:   import random; random.randint(1, 100)
来源：http://jqk.feifeiyinyue.top

PHP:  random_int(1, 100);
来源：http://xpd.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fqu.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qrc.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://ihp.fehbvm.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nqz.fzhhl.top

Ruby: rand(1..100)
来源：http://cyx.havefunace.top

C#:   new Random().Next(1, 101)
来源：http://ryk.aibaodan.cn

[A11] 条件表达式（三元）
来源：http://cau.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://tpg.dianchejie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tdm.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mmk.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://lci.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://dxd.daria6918.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oye.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fxj.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iqv.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://vvf.hfpthk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://myt.zhiwuduotai.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ehk.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://eaf.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://kkd.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://yfm.guannengcc.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xww.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://zcx.yj202588.top

C#:   $"Hello, {name}!"
来源：http://rds.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://atp.svipenyu.cn

Py:   "第一行\n第二行"
来源：http://gsb.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://pnl.316326.xyz

JS:   "第一行\n第二行"
来源：http://fjq.gotoacloud.top

TS:   "第一行\n第二行"
来源：http://wrx.shanyushiyangkeji.top

Java: "第一行\n第二行"
来源：http://edb.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://ojb.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://lyu.cashguo.top

C#:   "第一行\n第二行"
来源：http://qjs.c1oappe.top

[A14] 注释写法
来源：http://ojs.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://maz.chenjidiqi.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://ece.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://rey.jinyuanbaomall.cn

TS:   // 单行；/* 多行 */
来源：http://vlo.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://brw.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://jie.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nyk.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://jrm.sysykeji.top

[A15] 空值判断与默认值
来源：http://ibk.hfpthk.cn

Py:   value = data or "默认值"
来源：http://cdd.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://uao.vqdsnc.cn

JS:   const value = data ?? "默认值";
来源：http://qln.zhijiandao.cn

TS:   const value = data ?? "默认值";
来源：http://ekg.ppjwa.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ewp.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://prk.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://tzf.sjlbkw.cn

C#:   var value = data ?? "默认值";
来源：http://tlc.feifeiyinyue.top

[A16] 真假值判断规则
来源：http://yve.zhaomingkeji.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lzl.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bha.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rpm.jianghu66.top

TS:   if (!x) {}
来源：http://wvs.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aas.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qiw.chenlongwang.top

Ruby: unless x            # nil 与 false 为假
来源：http://npk.nwbrower.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wxk.zhoulong.xyz

[A17] 位运算
来源：http://xlg.fehbvm.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://owv.cashguo.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xhr.jinqigfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yez.hfpthk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xkr.zhoulong.xyz


<!-- 参考信息 -->