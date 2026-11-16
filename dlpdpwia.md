代发 wailian999

[U89] JS：数组去重
来源：http://lwx.quarkkingdee.top

[...new Set(arr)]
来源：http://vxt.gogol.net.cn

[U90] JS：数字数组排序
来源：http://xwx.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://llo.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://lht.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tcs.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://zrp.zhijiandao.cn

structuredClone(obj)
来源：http://qfo.yanxiufei.cn

[U93] JS：模板字符串
来源：http://fvd.daxiang520.top

`共 ${n} 条`
来源：http://xki.redwolf501.top

[U94] JS：箭头函数
来源：http://pcf.shuidangran.top

const double = x => x * 2;
来源：http://rdr.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://brn.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://ahx.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://ccc.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dbp.ybcxt.top

[U97] JS：并发请求
来源：http://sjy.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wfa.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://oky.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pch.jyoumei.cn

[U99] JS：事件监听
来源：http://ngb.andypj.xyz

el.addEventListener("click", e => {})
来源：http://cpe.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://zoi.ydzc1.top

document.querySelector(".item")
来源：http://rhq.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://rwt.tanke756.top

el.classList.toggle("active")
来源：http://ftf.guannengcc.top

[U102] JS：本地存储
来源：http://obl.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://dui.chenlongwang.top

[U103] JS：定时器
来源：http://bdv.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qby.ppjwa.cn

[U104] JS：防抖
来源：http://dwv.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gfv.gzhubu.top

[U105] JS：节流
来源：http://ypl.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zwb.haohaochexian.top

[U106] JS：日期格式化
来源：http://vfq.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kow.yanxiufei.cn

[U107] JS：数字千分位
来源：http://bgr.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lse.yuanzhike.top

[U108] JS：随机整数
来源：http://hbn.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gtk.fengsongda.top

[U109] JS：数组分组
来源：http://vlw.nwbrower.top

Object.groupBy(arr, x => x.type)
来源：http://dku.jiagoushi.top

[U110] JS：数组分块
来源：http://ifg.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cpv.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://hwo.shzxlz.cn

new Map(Object.entries(obj))
来源：http://mtn.guannengcc.top

[U112] JS：字符串补位
来源：http://cwz.zhixingplan.top

"7".padStart(3, "0")
来源：http://ruh.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://hsj.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://rbi.gzhubu.top

[U114] JS：JSON 深比较
来源：http://fli.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gob.c1oappe.top

[U115] JS：生成 UUID
来源：http://vpr.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://afh.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://mkr.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://gus.xinyue.icu

[U117] JS：单元测试
来源：http://wnr.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://ykr.daxiang520.top

[U118] JS：开发服务器
来源：http://dex.jyoumei.cn

npm i -D vite;  npx vite
来源：http://gzc.c1oappe.top

[U119] JS：生产构建
来源：http://cnv.yueranfly.top

npx vite build
来源：http://bsv.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://jzv.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://hqt.gzhubu.top

================================================================================
来源：http://okw.jinyuanbaomall.cn

统计汇总
来源：http://yno.tanke756.top

================================================================================
来源：http://sbq.yj20258.top

按语言统计（条）：
来源：http://bhl.cheryme.top

Python ......... 252
来源：http://jwc.tian-w.cn

PHP ............ 252
来源：http://ugr.jiagoushi.top

JavaScript ..... 252
来源：http://lvx.fanxiaobao.xyz

TypeScript ..... 212
来源：http://uks.jyoumei.cn

Java ........... 212
来源：http://adm.yanxiufei.cn

Go ............. 212
来源：http://lba.yuanzhike.top

Ruby ........... 212
来源：http://avy.sysykeji.top

C# ............. 212
来源：http://jlm.zhengqikj.top

C .............. 30
来源：http://cil.fehbvm.com

C++ ............ 30
来源：http://oiz.zhongyouzk.top

SQL ............ 90
来源：http://gol.ehwqpu.com

Bash ........... 80
来源：http://mxq.hywenlv.cn

Kotlin ......... 15
来源：http://zal.52xcode.cn

Swift .......... 15
来源：http://eeb.zhiwuduotai.top

Lua ............ 10
来源：http://civ.gaohongyu789.top

Perl ........... 10
来源：http://tlz.shangyingyoupin.top

Scala .......... 10
来源：http://wch.aibaodan.cn

------------------------------------
来源：http://ygf.redwolf501.top

合计 ........... 2106 条
来源：http://mzr.9152youxi.cn

按章节统计：
来源：http://qmc.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hbi.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jvn.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rff.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rli.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eqj.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cqe.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fxd.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://izg.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bum.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wua.316326.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rhn.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sty.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gpy.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://per.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xny.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://psl.aibaodan.cn

Q SQL 专题                              90
来源：http://yfy.sysykeji.top

R Bash 专题                             80
来源：http://ots.tian-w.cn

S C / C++ 专题                          60
来源：http://vay.fktsv.cn

T 其他语言补充                          60
来源：http://nba.vqdsnc.cn

U 高频实用片段                         120
来源：http://egr.daria6918.cn

------------------------------------
来源：http://rjm.svipenyu.cn

合计                                  2106 条
来源：http://grz.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://epn.aizwys.cn

使用提醒
来源：http://dzx.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://mrs.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ncd.xingfuxueyuan.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ast.wangshuangyany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gcx.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://czt.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://erw.fehbvm.com

—— 文件结束 ——
来源：http://qlp.zhijiandao.cn

================================================================================
来源：http://rak.aibaodan.cn

程序语言常见例子速查手册（2024 版）
来源：http://yyh.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://gjo.zhoulong.xyz

================================================================================
来源：http://jsi.wangdashe.top

【收录内容】
来源：http://brh.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ojt.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tkk.quarkkingdee.top

SQL · Bash · C · C++
来源：http://vaw.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ysh.chenjidiqi.icu

【使用说明】
来源：http://wzl.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eij.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://was.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gkv.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lko.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://khq.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://byy.birdmap.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://aii.guannengcc.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ixj.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://esg.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dpr.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pap.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rds.gaohongyu789.top

【文件统计】
来源：http://rzs.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aha.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://kng.ppjwa.cn

目  录
来源：http://vhf.ybcxt.top

--------------------------------------------------------------------------------
来源：http://dmr.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jhj.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mhz.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rtx.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hvh.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dja.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://has.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vrz.jqgfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nqp.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cls.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uhv.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xmg.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ato.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uly.guannengcc.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kal.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pda.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fkd.pycfn.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://heb.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ygk.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://klt.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yac.ehwqpu.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lvi.uphjek.com

================================================================================
来源：http://qdh.nwbrower.top

A. 基础语法与类型
来源：http://qbo.sysykeji.top

================================================================================
来源：http://icp.hnxiangtu.top

[A01] Hello World
来源：http://bel.yuanzhike.top

Py:   print("Hello, World!")
来源：http://gco.cashguo.top

PHP:  echo "Hello, World!";
来源：http://fie.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://zzv.gzhubu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uco.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://ivf.cheryme.top

Go:   fmt.Println("Hello, World!")
来源：http://meh.wangshuangyany.cn

Ruby: puts "Hello, World!"
来源：http://snb.guannengcc.top

C#:   Console.WriteLine("Hello, World!");
来源：http://npj.tianlin.xyz

[A02] 变量声明与赋值
来源：http://rxb.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://izw.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tqg.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ves.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hqf.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://ets.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://fmn.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://tci.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://kzv.ivvv.top

[A03] 常量定义
来源：http://wmi.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eew.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://lts.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://box.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://pxg.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://mqk.xuetiantiany.cn

Go:   const PI = 3.14159
来源：http://aqm.ctjpmb.com

Ruby: PI = 3.14159
来源：http://qcx.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://aro.haohaochexian.top

[A04] 判断变量类型
来源：http://hpb.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vqr.sufxvd.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gtu.hongshengwenyu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nay.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://xxn.zhongyouzk.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zdw.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://inj.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hok.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://noe.aizwys.cn

[A05] 整数除法与取模
来源：http://gye.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gta.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ukm.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vsd.epnwcf.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kjv.shzxlz.cn

Java: 7 / 2; 7 % 2
来源：http://xww.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://qef.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://qmt.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://ihu.hammf.cn

[A06] 字符串转数字
来源：http://ydp.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://mkw.hnqzz.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kcj.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hzp.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://xsk.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://srn.shuidangran.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hvf.zhoulong.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://jix.shanyushiyangtech.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yyk.xuetiantiany.cn

[A07] 数字转字符串
来源：http://xpy.fengsongda.top

Py:   str(42)
来源：http://qrf.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://sew.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://koc.feifeiyinyue.top

TS:   String(42)
来源：http://qsk.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sek.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://axn.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://cur.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://dos.gogol.net.cn

[A08] 取整与四舍五入
来源：http://awr.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fuw.yongpay.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lmb.hcnkem.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://upa.xuanzx.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dmy.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wyz.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gzo.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hkq.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://weo.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://cmg.yangfankeji.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kvw.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dzs.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qgf.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lii.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tla.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://smp.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jkt.zhixingplan.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tfw.chenzaomai.com

[A10] 生成随机数
来源：http://pff.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://wte.aibaodan.cn

PHP:  random_int(1, 100);
来源：http://wrc.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://suu.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ksu.smart0.xyz

Java: new Random().nextInt(100) + 1
来源：http://alq.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vie.xinyue.icu

Ruby: rand(1..100)
来源：http://lfc.nwbrower.top

C#:   new Random().Next(1, 101)
来源：http://syx.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://jux.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://djt.hywenlv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ete.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://gme.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://zvy.mhx1999.top

Java: x > 0 ? "yes" : "no"
来源：http://iyn.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fkk.xinyue.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://eqd.yangfankeji.com

C#:   x > 0 ? "yes" : "no"
来源：http://okp.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://fbx.gaohongyu789.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://adu.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bma.pycfn.com

JS:   `Hello, ${name}!`
来源：http://wby.yuxming.cn

TS:   `Hello, ${name}!`
来源：http://wvq.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://cyb.ctjpmb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ygc.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://zbk.gogol.net.cn

C#:   $"Hello, {name}!"
来源：http://qog.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://noy.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://esq.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://tqd.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://zwd.gotoacloud.top

TS:   "第一行\n第二行"
来源：http://yxj.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://qzd.fktsv.cn

Go:   "第一行\n第二行"
来源：http://gtv.yj20258.top

Ruby: "第一行\n第二行"
来源：http://hvt.fzhhl.top

C#:   "第一行\n第二行"
来源：http://oww.feifeiyinyue.top

[A14] 注释写法
来源：http://nkw.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hgd.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://saq.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://aig.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://vtf.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xrk.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://lig.hcnkem.com

Ruby: # 单行；=begin 多行 =end
来源：http://yku.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://bht.birdmap.top

[A15] 空值判断与默认值
来源：http://fog.cucudq.cn

Py:   value = data or "默认值"
来源：http://fwl.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://tml.yongpay.top


<!-- 参考信息 -->