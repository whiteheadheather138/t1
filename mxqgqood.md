代发 wailian999

[U95] JS：Promise 包装
来源：http://dku.birdmap.top

new Promise((resolve, reject) => {})
来源：http://dbg.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://kai.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nyp.iojbl.cn

[U97] JS：并发请求
来源：http://fku.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://sto.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://khu.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://smv.yangfankeji.com

[U99] JS：事件监听
来源：http://vby.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://txw.tianlin.xyz

[U100] JS：DOM 查询
来源：http://wxb.ivvv.top

document.querySelector(".item")
来源：http://iut.sxryk.cn

[U101] JS：classList 操作
来源：http://kbz.nanxinkj.top

el.classList.toggle("active")
来源：http://knz.vehdjk.com

[U102] JS：本地存储
来源：http://iak.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pll.cashguo.top

[U103] JS：定时器
来源：http://uuq.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ewt.shzxlz.cn

[U104] JS：防抖
来源：http://dpq.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxg.wangshuangyany.cn

[U105] JS：节流
来源：http://wnt.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dzy.epnwcf.com

[U106] JS：日期格式化
来源：http://xri.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wnq.birdmap.top

[U107] JS：数字千分位
来源：http://kpn.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://txv.xziqi.cn

[U108] JS：随机整数
来源：http://jlw.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mbo.hnqzz.top

[U109] JS：数组分组
来源：http://cqc.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://xjz.cashguo.top

[U110] JS：数组分块
来源：http://mzt.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vby.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://tvi.sufxvd.cn

new Map(Object.entries(obj))
来源：http://vjx.vqdsnc.cn

[U112] JS：字符串补位
来源：http://dmu.zycfv.cn

"7".padStart(3, "0")
来源：http://wco.uphjek.com

[U113] JS：正则替换全部
来源：http://brm.jianghu66.top

s.replaceAll("a", "b")
来源：http://hgk.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://jek.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://obz.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://pkn.pycfn.com

crypto.randomUUID()
来源：http://sdh.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://xpx.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://eda.yuxming.cn

[U117] JS：单元测试
来源：http://sba.zhiwuduotai.top

npm i -D vitest;  npx vitest
来源：http://sua.jyoumei.cn

[U118] JS：开发服务器
来源：http://iui.ehwqpu.com

npm i -D vite;  npx vite
来源：http://huk.tianlin.xyz

[U119] JS：生产构建
来源：http://ebq.ydjk.org.cn

npx vite build
来源：http://fdg.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://hhd.cheryme.top

import.meta.env.VITE_API_URL
来源：http://zor.wangshuangyany.cn

================================================================================
来源：http://rzg.birdmap.top

统计汇总
来源：http://alu.guowangkeji.top

================================================================================
来源：http://lvq.cdnleiting.top

按语言统计（条）：
来源：http://qac.xingfuxueyuan.xyz

Python ......... 252
来源：http://chm.tanke756.top

PHP ............ 252
来源：http://aro.redwolf501.top

JavaScript ..... 252
来源：http://dwj.ppjwa.cn

TypeScript ..... 212
来源：http://mgk.jianghu66.top

Java ........... 212
来源：http://ttg.vehdjk.com

Go ............. 212
来源：http://hei.bjfxy.top

Ruby ........... 212
来源：http://ltt.quarkkingdee.top

C# ............. 212
来源：http://orb.meibo888.top

C .............. 30
来源：http://pjh.xuanzx.com

C++ ............ 30
来源：http://kwx.yuanzhike.top

SQL ............ 90
来源：http://dvy.tianlin.xyz

Bash ........... 80
来源：http://eay.shanyushiyangtech.top

Kotlin ......... 15
来源：http://vgl.fzhhl.top

Swift .......... 15
来源：http://yga.nanxuanxn.top

Lua ............ 10
来源：http://tco.tarul.cn

Perl ........... 10
来源：http://zvg.zhongyouzk.top

Scala .......... 10
来源：http://cgy.uphjek.com

------------------------------------
来源：http://csx.fktsv.cn

合计 ........... 2106 条
来源：http://pka.hysaishi.cn

按章节统计：
来源：http://fjs.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jds.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rzi.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://miw.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pqs.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qdf.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dmd.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gjg.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hdf.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://juz.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vvt.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yyc.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aat.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ueo.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://llh.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wvy.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tai.hcnkem.com

Q SQL 专题                              90
来源：http://bbw.zycfv.cn

R Bash 专题                             80
来源：http://wwi.hfpthk.cn

S C / C++ 专题                          60
来源：http://kje.hysaishi.cn

T 其他语言补充                          60
来源：http://iax.tanke756.top

U 高频实用片段                         120
来源：http://ovm.hnxiangtu.top

------------------------------------
来源：http://tfp.vqdsnc.cn

合计                                  2106 条
来源：http://nil.tarul.cn

--------------------------------------------------------------------------------
来源：http://xld.meibo888.top

使用提醒
来源：http://xsc.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://lfq.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rtt.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rps.pengpengdd.cyou

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xyi.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yiq.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mhj.zhiwuduotai.top

—— 文件结束 ——
来源：http://ouy.hongshengwenyu.top

================================================================================
来源：http://qxe.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://jwa.daxiang520.top

Common Programming Examples Cheat Book
来源：http://pop.zdqjudy.top

================================================================================
来源：http://nkd.jiagoushi.top

【收录内容】
来源：http://bbd.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sgs.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ntx.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://wjp.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zir.ybcxt.top

【使用说明】
来源：http://nff.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sub.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nbi.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jdv.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ubo.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zom.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sfh.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://buq.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://epq.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qbf.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wwv.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://btx.daxiang520.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wtj.jyoumei.cn

【文件统计】
来源：http://ybs.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qki.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://snt.zdqjudy.top

目  录
来源：http://ray.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://psu.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ikb.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://urx.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ety.sxryk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dzg.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uts.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xoq.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://skx.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mgs.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fbi.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fvz.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iep.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zsg.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://joi.9152youxi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://smg.chenlongwang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://khv.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mms.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jyq.zhoulong.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://rqq.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://snd.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cuv.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kui.yonumen.top

================================================================================
来源：http://mos.gzhubu.top

A. 基础语法与类型
来源：http://ssw.cheryme.top

================================================================================
来源：http://vbc.52xcode.cn

[A01] Hello World
来源：http://fsx.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://znv.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://pse.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://xnr.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vhf.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://mwt.jinqigfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://fpu.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://hci.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kzv.zhengqikj.top

[A02] 变量声明与赋值
来源：http://ztp.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ilh.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mqm.0kj1m.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hwa.dianchejie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://srd.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://uqt.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://opg.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://trk.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://ihx.nanxinkj.top

[A03] 常量定义
来源：http://ipe.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rbo.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://nnh.fzhhl.top

JS:   const PI = 3.14159;
来源：http://vfb.52xcode.cn

TS:   const PI: number = 3.14159;
来源：http://kqq.uphjek.com

Java: static final double PI = 3.14159;
来源：http://ted.cdnleiting.top

Go:   const PI = 3.14159
来源：http://jwy.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://vkg.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://evu.fzhhl.top

[A04] 判断变量类型
来源：http://had.chenlongwang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gre.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kiq.chenzaomai.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vqf.nanxuanxn.top

TS:   typeof x; x instanceof Date
来源：http://msf.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cfe.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://plx.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gkw.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://agh.hcnkem.com

[A05] 整数除法与取模
来源：http://mod.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lvn.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://juw.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://osr.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lqz.redwolf501.top

Java: 7 / 2; 7 % 2
来源：http://zrq.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://oam.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://hor.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://fyj.redwolf501.top

[A06] 字符串转数字
来源：http://mnn.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://lqu.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tgv.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hio.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://uoq.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ank.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://isd.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ion.aizwys.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hej.cheryme.top

[A07] 数字转字符串
来源：http://rcs.zycfv.cn

Py:   str(42)
来源：http://rjv.smart0.xyz

PHP:  (string) 42; strval(42)
来源：http://gah.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://nzx.jqgufenzy.top

TS:   String(42)
来源：http://ypw.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uob.wangdashe.top

Go:   strconv.Itoa(42)
来源：http://hwb.jianghu66.top

Ruby: 42.to_s
来源：http://fzu.0kj1m.cn

C#:   42.ToString()
来源：http://nhd.xinyue.icu

[A08] 取整与四舍五入
来源：http://caf.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jzr.jianghu66.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mpl.zhoulong.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://efy.gzhubu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yzy.shanyushiyangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uma.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ykx.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pnq.birdmap.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xgs.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://itu.snrcjt.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hbt.jlsjyb.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hcp.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iby.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nwg.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://skk.guowangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ief.dianchejie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bpp.52xcode.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yzg.hysaishi.cn

[A10] 生成随机数
来源：http://bib.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://njp.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://tnt.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gyt.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mmm.havefunace.top

Java: new Random().nextInt(100) + 1
来源：http://nys.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xhi.bjfxy.top

Ruby: rand(1..100)
来源：http://ato.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://dyp.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://ekq.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://tzg.yonumen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nth.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://pam.hnxiangtu.top

TS:   x > 0 ? "yes" : "no"
来源：http://gay.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://gia.sysykeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://kkl.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vab.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://jps.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://rkv.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yha.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lvg.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://jpv.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://zih.gotoacloud.top

Java: "Hello, %s!".formatted(name)
来源：http://xgx.c1oappe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cvr.hnqzz.top

Ruby: "Hello, #{name}!"
来源：http://myn.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://efk.guannengcc.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jqw.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://vfe.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://vkk.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://fcv.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://okz.jiagoushi.top

Java: "第一行\n第二行"
来源：http://tdz.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://mva.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://ejl.cashguo.top

C#:   "第一行\n第二行"
来源：http://sgw.jiagoushi.top

[A14] 注释写法
来源：http://vrc.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ldn.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://amc.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://kom.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://cgb.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xra.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://dua.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://ixf.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://dhy.316326.xyz

[A15] 空值判断与默认值
来源：http://qbx.mhx1999.top

Py:   value = data or "默认值"
来源：http://tgg.guowangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://pnz.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://jnf.tarul.cn

TS:   const value = data ?? "默认值";
来源：http://vhc.cqqwz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zzl.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://fwi.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://qfn.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://zgy.gogol.net.cn

[A16] 真假值判断规则
来源：http://gqx.316326.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tac.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zra.feifeiyinyue.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iaj.gaohongyu789.top

TS:   if (!x) {}
来源：http://sgw.tian-w.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cho.cheryme.top


<!-- 参考信息 -->