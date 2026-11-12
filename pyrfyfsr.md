代发 wailian999

[U93] JS：模板字符串
来源：http://zgj.hammf.cn

`共 ${n} 条`
来源：http://zli.vehdjk.com

[U94] JS：箭头函数
来源：http://uhc.yueranfly.top

const double = x => x * 2;
来源：http://poh.yongpay.top

[U95] JS：Promise 包装
来源：http://eoy.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://atd.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://zst.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jzg.hysaishi.cn

[U97] JS：并发请求
来源：http://tcl.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qkh.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://gnw.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lyx.zhiwuduotai.top

[U99] JS：事件监听
来源：http://qzl.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://ozp.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://ect.tanke756.top

document.querySelector(".item")
来源：http://bnv.jiagoushi.top

[U101] JS：classList 操作
来源：http://zgu.xylfe.cn

el.classList.toggle("active")
来源：http://ivj.chenlongwang.top

[U102] JS：本地存储
来源：http://irp.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://nlg.zhengqikj.top

[U103] JS：定时器
来源：http://fgn.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xsw.xziqi.cn

[U104] JS：防抖
来源：http://jtv.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xpg.hywenlv.cn

[U105] JS：节流
来源：http://ylp.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rtq.bbcook.cn

[U106] JS：日期格式化
来源：http://vov.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://otu.zdbjq.cn

[U107] JS：数字千分位
来源：http://fug.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hdp.pycfn.com

[U108] JS：随机整数
来源：http://avi.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://onb.ehwqpu.com

[U109] JS：数组分组
来源：http://hqy.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://tgf.sysykeji.top

[U110] JS：数组分块
来源：http://lcn.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gjk.yuanzhike.top

[U111] JS：对象转 Map
来源：http://bgz.xziqi.cn

new Map(Object.entries(obj))
来源：http://lgr.chenlongwang.top

[U112] JS：字符串补位
来源：http://lzw.0kj1m.cn

"7".padStart(3, "0")
来源：http://qfw.smart0.xyz

[U113] JS：正则替换全部
来源：http://zpk.meibo888.top

s.replaceAll("a", "b")
来源：http://yax.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://rkl.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://huo.gotoacloud.top

[U115] JS：生成 UUID
来源：http://amo.bjfxy.top

crypto.randomUUID()
来源：http://wkn.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://anf.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://scr.yvedp.cn

[U117] JS：单元测试
来源：http://fhb.yongpay.top

npm i -D vitest;  npx vitest
来源：http://ubs.bjfxy.top

[U118] JS：开发服务器
来源：http://txs.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://gnq.yonumen.top

[U119] JS：生产构建
来源：http://bsz.andypj.xyz

npx vite build
来源：http://vkw.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://dap.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://vjs.fehbvm.com

================================================================================
来源：http://ghr.smart0.xyz

统计汇总
来源：http://yti.ehwqpu.com

================================================================================
来源：http://icx.epnwcf.com

按语言统计（条）：
来源：http://fku.xuanzx.com

Python ......... 252
来源：http://kaw.ydjk.org.cn

PHP ............ 252
来源：http://vee.yj202588.top

JavaScript ..... 252
来源：http://rcg.cheryme.top

TypeScript ..... 212
来源：http://cvm.shangyingyoupin.top

Java ........... 212
来源：http://oti.jinyuanbaomall.cn

Go ............. 212
来源：http://cdy.cqqwz.cn

Ruby ........... 212
来源：http://kjb.kuanghao11.cn

C# ............. 212
来源：http://rna.nanxuanxn.top

C .............. 30
来源：http://lys.jinqigufen.top

C++ ............ 30
来源：http://zek.jinqigufen.top

SQL ............ 90
来源：http://owc.yvedp.cn

Bash ........... 80
来源：http://zyw.fehbvm.com

Kotlin ......... 15
来源：http://dwk.52xcode.cn

Swift .......... 15
来源：http://mzd.zhongyouzk.top

Lua ............ 10
来源：http://dxv.ctjpmb.com

Perl ........... 10
来源：http://ysk.tianlin.xyz

Scala .......... 10
来源：http://bxf.cdnleiting.top

------------------------------------
来源：http://axn.iojbl.cn

合计 ........... 2106 条
来源：http://piz.guowangkeji.top

按章节统计：
来源：http://bnb.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://urr.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ohy.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cxt.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gmd.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://byt.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kum.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lvr.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zjb.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rcl.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nqi.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mcq.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vva.vehdjk.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://phl.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rqq.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cnk.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tzk.smart0.xyz

Q SQL 专题                              90
来源：http://kek.cashguo.top

R Bash 专题                             80
来源：http://dkf.wangdashe.top

S C / C++ 专题                          60
来源：http://laf.yvedp.cn

T 其他语言补充                          60
来源：http://ply.bbcook.cn

U 高频实用片段                         120
来源：http://omp.cheryme.top

------------------------------------
来源：http://xco.mhx1999.top

合计                                  2106 条
来源：http://wpf.epnwcf.com

--------------------------------------------------------------------------------
来源：http://ffr.jinqigfzy.top

使用提醒
来源：http://gdg.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://qjm.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vmt.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kor.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cgn.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://pac.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bcd.nanxuanxn.top

—— 文件结束 ——
来源：http://tfj.pengpengdd.cyou

================================================================================
来源：http://mgq.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://aks.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://brw.xingfuxueyuan.xyz

================================================================================
来源：http://bfv.chenlongwang.top

【收录内容】
来源：http://qtw.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gmd.ehwqpu.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yos.hnqzz.top

SQL · Bash · C · C++
来源：http://pib.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sso.tanke756.top

【使用说明】
来源：http://jyv.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gqu.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://npv.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wdx.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bui.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zkg.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zke.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xee.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://apc.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qrt.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://syn.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://saf.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://etz.ywan-chungtsiang.top

【文件统计】
来源：http://ryn.jinyuanbaomall.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://unr.daxiang520.top

--------------------------------------------------------------------------------
来源：http://qdk.guannengcc.top

目  录
来源：http://qbo.xylfe.cn

--------------------------------------------------------------------------------
来源：http://kdd.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pgz.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dlg.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jxv.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://exk.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wzn.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://djd.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xmz.gogol.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wpm.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sof.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bot.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xsu.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rte.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nsu.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mqr.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bot.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wqw.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iff.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://jrs.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dgj.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ceb.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jbv.gzhubu.top

================================================================================
来源：http://kua.wangshuangyany.cn

A. 基础语法与类型
来源：http://ash.gaohongyu789.top

================================================================================
来源：http://gfw.shanyushiyangkeji.top

[A01] Hello World
来源：http://toc.yfazqb.com

Py:   print("Hello, World!")
来源：http://sqm.hnqzz.top

PHP:  echo "Hello, World!";
来源：http://vyr.ehwqpu.com

JS:   console.log("Hello, World!");
来源：http://zot.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rsa.shanyushiyangkeji.top

Java: System.out.println("Hello, World!");
来源：http://lcu.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://adz.andypj.xyz

Ruby: puts "Hello, World!"
来源：http://kmm.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hur.guannengcc.top

[A02] 变量声明与赋值
来源：http://cgu.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rvv.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yva.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://pmn.vqdsnc.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ewu.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://ewi.ydzc1.top

Go:   name := "Alex"; age := 20
来源：http://nel.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://pqa.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://axk.yj20258888.top

[A03] 常量定义
来源：http://emy.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bvo.zycfv.cn

PHP:  const PI = 3.14159;
来源：http://emn.316326.xyz

JS:   const PI = 3.14159;
来源：http://sdq.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://cvn.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://txx.smart0.xyz

Go:   const PI = 3.14159
来源：http://urp.xinyue.icu

Ruby: PI = 3.14159
来源：http://ouu.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://feq.sjlbkw.cn

[A04] 判断变量类型
来源：http://rhk.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fho.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zxo.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://reg.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://fyu.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://atm.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fmt.gzhubu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ism.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://gwm.yongpay.top

[A05] 整数除法与取模
来源：http://beg.316326.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ymc.wangshuangyany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wud.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wye.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ypz.fzhhl.top

Java: 7 / 2; 7 % 2
来源：http://sph.dashuyun.cn

Go:   7 / 2; 7 % 2
来源：http://fyf.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://zvt.fengsongda.top

C#:   7 / 2; 7 % 2
来源：http://pia.tarul.cn

[A06] 字符串转数字
来源：http://ick.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://ogl.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ejo.gotoacloud.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://trv.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://bwm.jyoumei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://igv.fehbvm.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fvw.redwolf501.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dxe.wangdashe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xtu.c1oappe.top

[A07] 数字转字符串
来源：http://bui.aizwys.cn

Py:   str(42)
来源：http://jvw.nwbrower.top

PHP:  (string) 42; strval(42)
来源：http://hnt.hfpthk.cn

JS:   String(42); (42).toString()
来源：http://kai.cheryme.top

TS:   String(42)
来源：http://znf.quarkkingdee.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dhx.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://jgb.chenlongwang.top

Ruby: 42.to_s
来源：http://qrc.jlsjyb.cn

C#:   42.ToString()
来源：http://ytl.zdqjudy.top

[A08] 取整与四舍五入
来源：http://wss.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://und.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://djc.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qcy.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kyx.xuanzx.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oxb.sysykeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jyn.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dpy.sufxvd.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aqo.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://qft.daria6918.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cxd.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jxl.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://frm.jinghuilouyu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cps.aibaodan.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dqv.yuanzhike.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kmi.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xna.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cqs.yongpay.top

[A10] 生成随机数
来源：http://fts.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://ybz.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://qfz.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yxf.hcnkem.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xwo.cheryme.top

Java: new Random().nextInt(100) + 1
来源：http://hae.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pil.gaohongyu789.top

Ruby: rand(1..100)
来源：http://mcg.havefunace.top

C#:   new Random().Next(1, 101)
来源：http://scm.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://jhk.gaohongyu789.top

Py:   "yes" if x > 0 else "no"
来源：http://mrm.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yps.daria6918.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yzt.fehbvm.com

TS:   x > 0 ? "yes" : "no"
来源：http://udt.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://emc.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://odo.birdmap.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ypm.cdnleiting.top

C#:   x > 0 ? "yes" : "no"
来源：http://dih.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://xdc.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://prr.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wky.yfazqb.com

JS:   `Hello, ${name}!`
来源：http://cmc.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://rfi.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://wxr.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bis.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://abx.cdnleiting.top

C#:   $"Hello, {name}!"
来源：http://wid.aizwys.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pdk.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://xom.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://bxr.xziqi.cn

JS:   "第一行\n第二行"
来源：http://uxa.daxiang520.top

TS:   "第一行\n第二行"
来源：http://lnb.yongpay.top

Java: "第一行\n第二行"
来源：http://xrc.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://icp.andypj.xyz

Ruby: "第一行\n第二行"
来源：http://izt.xylfe.cn

C#:   "第一行\n第二行"
来源：http://pwc.sufxvd.cn

[A14] 注释写法
来源：http://exb.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pyn.hcnkem.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://gxt.kuanghao11.cn

JS:   // 单行；/* 多行 */
来源：http://afq.ybcxt.top

TS:   // 单行；/* 多行 */
来源：http://rrg.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://epd.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://rec.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://zzw.bjfxy.top

C#:   // 单行；/* 多行 */
来源：http://bxq.guannengcc.top

[A15] 空值判断与默认值
来源：http://aet.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://rtz.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://ovf.haohaochexian.top

JS:   const value = data ?? "默认值";
来源：http://jxb.c1oappe.top

TS:   const value = data ?? "默认值";
来源：http://nji.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vvh.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://rmy.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://hdz.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://bdv.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://ccw.0kj1m.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://azb.yuanzhike.top


<!-- 参考信息 -->