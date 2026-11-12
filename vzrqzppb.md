代发 wailian999

[U93] JS：模板字符串
来源：http://ncb.birdmap.top

`共 ${n} 条`
来源：http://agy.fehbvm.com

[U94] JS：箭头函数
来源：http://xwq.jinqigufen.top

const double = x => x * 2;
来源：http://foq.sxryk.cn

[U95] JS：Promise 包装
来源：http://czp.zhaomingkeji.xyz

new Promise((resolve, reject) => {})
来源：http://kow.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://xqk.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qjk.mhx1999.top

[U97] JS：并发请求
来源：http://zwk.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cfy.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://wrx.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jjx.tarul.cn

[U99] JS：事件监听
来源：http://jvw.sysykeji.top

el.addEventListener("click", e => {})
来源：http://vax.tanke756.top

[U100] JS：DOM 查询
来源：http://our.zycfv.cn

document.querySelector(".item")
来源：http://ihk.jiagoushi.top

[U101] JS：classList 操作
来源：http://mee.vehdjk.com

el.classList.toggle("active")
来源：http://von.xziqi.cn

[U102] JS：本地存储
来源：http://aob.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://etc.pycfn.com

[U103] JS：定时器
来源：http://fml.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gni.jiagoushi.top

[U104] JS：防抖
来源：http://vve.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://spm.ivvv.top

[U105] JS：节流
来源：http://pud.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aek.uphjek.com

[U106] JS：日期格式化
来源：http://cvv.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://txq.havefunace.top

[U107] JS：数字千分位
来源：http://uac.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nsr.xylfe.cn

[U108] JS：随机整数
来源：http://igh.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://srx.yuanzhike.top

[U109] JS：数组分组
来源：http://xmn.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://eaa.tianlin.xyz

[U110] JS：数组分块
来源：http://rih.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hun.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://yyp.ybcxt.top

new Map(Object.entries(obj))
来源：http://pwk.ybcxt.top

[U112] JS：字符串补位
来源：http://nas.ivvv.top

"7".padStart(3, "0")
来源：http://kok.xylfe.cn

[U113] JS：正则替换全部
来源：http://ufk.bbcook.cn

s.replaceAll("a", "b")
来源：http://hav.uphjek.com

[U114] JS：JSON 深比较
来源：http://cav.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://weu.bjfxy.top

[U115] JS：生成 UUID
来源：http://jrd.fengsongda.top

crypto.randomUUID()
来源：http://tzi.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://qma.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://uax.sysykeji.top

[U117] JS：单元测试
来源：http://lzl.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://ube.sufxvd.cn

[U118] JS：开发服务器
来源：http://qkj.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://fvw.shzxlz.cn

[U119] JS：生产构建
来源：http://rcs.chenjidiqi.icu

npx vite build
来源：http://sci.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://zyg.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://hye.hammf.cn

================================================================================
来源：http://uhl.ywan-chungtsiang.top

统计汇总
来源：http://xee.chenlongwang.top

================================================================================
来源：http://hqp.zycfv.cn

按语言统计（条）：
来源：http://hfq.yuanzhike.top

Python ......... 252
来源：http://imu.bjfxy.top

PHP ............ 252
来源：http://kgt.yfazqb.com

JavaScript ..... 252
来源：http://qpr.hysaishi.cn

TypeScript ..... 212
来源：http://wwl.mhx1999.top

Java ........... 212
来源：http://nzt.feifeiyinyue.top

Go ............. 212
来源：http://exe.gogol.net.cn

Ruby ........... 212
来源：http://tug.cheryme.top

C# ............. 212
来源：http://qxt.c1oappe.top

C .............. 30
来源：http://hcc.316326.xyz

C++ ............ 30
来源：http://puz.cashguo.top

SQL ............ 90
来源：http://diz.cqqwz.cn

Bash ........... 80
来源：http://ngs.zycfv.cn

Kotlin ......... 15
来源：http://bnl.jlsjyb.cn

Swift .......... 15
来源：http://ipf.yuxming.cn

Lua ............ 10
来源：http://ruu.fzhhl.top

Perl ........... 10
来源：http://gfg.yuxming.cn

Scala .......... 10
来源：http://wht.andypj.xyz

------------------------------------
来源：http://vda.cucudq.cn

合计 ........... 2106 条
来源：http://qjg.yangfankeji.com

按章节统计：
来源：http://tsz.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xdh.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ihs.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oyn.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pfn.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://smc.pycfn.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rdb.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iuj.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://irz.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dxe.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iae.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pix.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rhr.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://evu.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dut.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lut.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pwk.vehdjk.com

Q SQL 专题                              90
来源：http://xaw.jinqigfzy.top

R Bash 专题                             80
来源：http://ndw.yj20258.top

S C / C++ 专题                          60
来源：http://xpj.c1oappe.top

T 其他语言补充                          60
来源：http://hdo.yj20258.top

U 高频实用片段                         120
来源：http://ymo.cqqwz.cn

------------------------------------
来源：http://gsp.epnwcf.com

合计                                  2106 条
来源：http://qjo.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://xkq.hammf.cn

使用提醒
来源：http://ofk.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://bfs.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gmm.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kxa.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ukj.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://ohl.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ctc.jlsjyb.cn

—— 文件结束 ——
来源：http://pnc.sysykeji.top

================================================================================
来源：http://edm.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://kvs.ivvv.top

Common Programming Examples Cheat Book
来源：http://fib.gogol.net.cn

================================================================================
来源：http://nrg.yuanzhike.top

【收录内容】
来源：http://tgy.cdnleiting.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gyh.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ukl.yfazqb.com

SQL · Bash · C · C++
来源：http://mzv.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://luf.chenlongwang.top

【使用说明】
来源：http://pzv.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kjd.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bjq.yj20258.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://umy.jinyuanbaomall.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://res.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://muj.jqgfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qyt.sweek.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dfy.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mgt.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uia.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tkc.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aos.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hwc.havefunace.top

【文件统计】
来源：http://wbg.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ala.sxryk.cn

--------------------------------------------------------------------------------
来源：http://ozy.ppjwa.cn

目  录
来源：http://rbe.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://jge.hesvh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uym.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oib.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kix.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hne.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qep.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://djl.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zfi.yueranfly.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ykv.zhixingplan.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bdw.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lnn.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ypl.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ocq.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ble.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sge.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vzl.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bcw.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ekg.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tuu.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://teh.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oik.smart0.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qos.uphjek.com

================================================================================
来源：http://qwy.guowangkeji.top

A. 基础语法与类型
来源：http://yvk.jqgufenzy.top

================================================================================
来源：http://rjo.jinyuanbaomall.cn

[A01] Hello World
来源：http://lmj.hnqzz.top

Py:   print("Hello, World!")
来源：http://wvs.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://yrh.ehwqpu.com

JS:   console.log("Hello, World!");
来源：http://uae.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ckd.hnxiangtu.top

Java: System.out.println("Hello, World!");
来源：http://cxw.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://vdb.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://lbf.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://kuw.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://rfb.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oie.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://jbx.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bye.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tku.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://jgz.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://zjb.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://rdd.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ozs.chenzaomai.com

[A03] 常量定义
来源：http://bsl.shanyushiyangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bzz.shanyushiyangtech.top

PHP:  const PI = 3.14159;
来源：http://pnm.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://smc.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://npl.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://oxn.shuidangran.top

Go:   const PI = 3.14159
来源：http://sff.yonumen.top

Ruby: PI = 3.14159
来源：http://nvl.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://vpu.zdbjq.cn

[A04] 判断变量类型
来源：http://cqj.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yja.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ylg.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lri.nanxinkj.top

TS:   typeof x; x instanceof Date
来源：http://jtq.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ted.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ccl.fzhhl.top

Ruby: x.class; x.is_a?(Integer)
来源：http://eyb.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://tmo.9152youxi.cn

[A05] 整数除法与取模
来源：http://kyf.zycfv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://drq.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tjx.sufxvd.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bsq.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fsm.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://qfg.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://uuo.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://yah.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://shp.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://dqv.ywan-chungtsiang.top

Py:   int("42"); float("3.14")
来源：http://xdt.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zer.hfpthk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gyx.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://wrc.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gds.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xkl.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://edd.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dsp.yuanzhike.top

[A07] 数字转字符串
来源：http://rsb.epnwcf.com

Py:   str(42)
来源：http://biu.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://gby.yuxming.cn

JS:   String(42); (42).toString()
来源：http://wzw.sysykeji.top

TS:   String(42)
来源：http://xcq.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://suo.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://glh.hywenlv.cn

Ruby: 42.to_s
来源：http://knk.birdmap.top

C#:   42.ToString()
来源：http://gwg.fzhhl.top

[A08] 取整与四舍五入
来源：http://lec.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yqv.yueranfly.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zrc.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mdz.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xcb.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qhq.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eoc.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ecp.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://drh.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://rvz.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ila.havefunace.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ear.zhiwuduotai.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hvx.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ihs.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xjw.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bbw.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yns.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ghx.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://btu.zhixingplan.top

Py:   import random; random.randint(1, 100)
来源：http://epo.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://vcd.c1oappe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gfh.ywan-chungtsiang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ale.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://vuj.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ree.jqgfzy.top

Ruby: rand(1..100)
来源：http://hvd.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://zgi.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://hyd.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://wus.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wtn.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jgp.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://ore.chenlongwang.top

Java: x > 0 ? "yes" : "no"
来源：http://vsy.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://aqe.epnwcf.com

Ruby: x > 0 ? "yes" : "no"
来源：http://cfg.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cge.jqgufenzy.top

[A12] 字符串插值 / 格式化
来源：http://rdn.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jst.yuxming.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cuu.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://dzb.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://fpq.nanxuanxn.top

Java: "Hello, %s!".formatted(name)
来源：http://yam.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bpi.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://mwo.haohaochexian.top

C#:   $"Hello, {name}!"
来源：http://isj.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gya.cashguo.top

Py:   "第一行\n第二行"
来源：http://chs.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://clv.epnwcf.com

JS:   "第一行\n第二行"
来源：http://mhv.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://jgc.hesvh.cn

Java: "第一行\n第二行"
来源：http://hzm.redwolf501.top

Go:   "第一行\n第二行"
来源：http://zcr.shanyushiyangkeji.top

Ruby: "第一行\n第二行"
来源：http://slv.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://vzi.sufxvd.cn

[A14] 注释写法
来源：http://uwh.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vyk.mhx1999.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zej.fanxiaobao.xyz

JS:   // 单行；/* 多行 */
来源：http://cjc.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://tgd.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jdh.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://qzp.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://tyk.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://unw.zycfv.cn

[A15] 空值判断与默认值
来源：http://dye.uphjek.com

Py:   value = data or "默认值"
来源：http://gah.jqgufenzy.top

PHP:  $value = $data ?? "默认值";
来源：http://gbo.9152youxi.cn

JS:   const value = data ?? "默认值";
来源：http://goi.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://cev.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zuu.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://zpz.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://sff.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://fig.gogol.net.cn

[A16] 真假值判断规则
来源：http://ror.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hfv.yfazqb.com


<!-- 参考信息 -->