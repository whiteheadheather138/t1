代发 wailian999

[U89] JS：数组去重
来源：http://gzv.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://ato.cucudq.cn

[U90] JS：数字数组排序
来源：http://fet.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://yvf.mhx1999.top

[U91] JS：对象键值遍历
来源：http://lkq.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wai.dashuyun.cn

[U92] JS：深拷贝
来源：http://dvw.dianchejie.cn

structuredClone(obj)
来源：http://wko.xinyue.icu

[U93] JS：模板字符串
来源：http://ins.gotoacloud.top

`共 ${n} 条`
来源：http://prt.tian-w.cn

[U94] JS：箭头函数
来源：http://xzt.ppjwa.cn

const double = x => x * 2;
来源：http://zia.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://ccn.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://ior.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://mvz.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dul.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://nfr.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hsv.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://wcc.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pyr.redwolf501.top

[U99] JS：事件监听
来源：http://mqr.daria6918.cn

el.addEventListener("click", e => {})
来源：http://zse.hnqzz.top

[U100] JS：DOM 查询
来源：http://gjq.shangyingyoupin.top

document.querySelector(".item")
来源：http://oab.ybcxt.top

[U101] JS：classList 操作
来源：http://hpz.aibaodan.cn

el.classList.toggle("active")
来源：http://eke.shuidangran.top

[U102] JS：本地存储
来源：http://klj.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://waf.chenzaomai.com

[U103] JS：定时器
来源：http://jwb.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ymy.svipenyu.cn

[U104] JS：防抖
来源：http://kfk.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyi.yangfankeji.com

[U105] JS：节流
来源：http://jgf.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pvl.epnwcf.com

[U106] JS：日期格式化
来源：http://nkj.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpj.yj20258888.top

[U107] JS：数字千分位
来源：http://ana.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://paj.tianlin.xyz

[U108] JS：随机整数
来源：http://lkl.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://txl.fehbvm.com

[U109] JS：数组分组
来源：http://ift.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://fdu.yangfankeji.com

[U110] JS：数组分块
来源：http://msx.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gpn.9152youxi.cn

[U111] JS：对象转 Map
来源：http://kgc.ivvv.top

new Map(Object.entries(obj))
来源：http://fpe.yj20258888.top

[U112] JS：字符串补位
来源：http://ten.kuanghao11.cn

"7".padStart(3, "0")
来源：http://egf.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://oec.tarul.cn

s.replaceAll("a", "b")
来源：http://mmm.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://mwy.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kvv.yvedp.cn

[U115] JS：生成 UUID
来源：http://rfy.bbcook.cn

crypto.randomUUID()
来源：http://qff.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://pjo.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://efl.9152youxi.cn

[U117] JS：单元测试
来源：http://sfr.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://qib.316326.xyz

[U118] JS：开发服务器
来源：http://mss.pycfn.com

npm i -D vite;  npx vite
来源：http://yyq.hnqzz.top

[U119] JS：生产构建
来源：http://bdl.zycfv.cn

npx vite build
来源：http://osy.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://qly.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://jpp.birdmap.top

================================================================================
来源：http://ryr.fanxiaobao.xyz

统计汇总
来源：http://brw.gzhubu.top

================================================================================
来源：http://jdn.hongshengwenyu.top

按语言统计（条）：
来源：http://omt.jyoumei.cn

Python ......... 252
来源：http://yli.feifeiyinyue.top

PHP ............ 252
来源：http://zka.havefunace.top

JavaScript ..... 252
来源：http://zsb.bbcook.cn

TypeScript ..... 212
来源：http://uvl.yfazqb.com

Java ........... 212
来源：http://dhd.xziqi.cn

Go ............. 212
来源：http://zhq.bbcook.cn

Ruby ........... 212
来源：http://mff.ywan-chungtsiang.top

C# ............. 212
来源：http://lnl.xingfuxueyuan.xyz

C .............. 30
来源：http://cfw.bjfxy.top

C++ ............ 30
来源：http://tmy.hongshengwenyu.top

SQL ............ 90
来源：http://ked.fktsv.cn

Bash ........... 80
来源：http://cbs.yj202588.top

Kotlin ......... 15
来源：http://lxf.xylfe.cn

Swift .......... 15
来源：http://zef.yongpay.top

Lua ............ 10
来源：http://ytn.fzhhl.top

Perl ........... 10
来源：http://zcy.zhongyouzk.top

Scala .......... 10
来源：http://uaj.sjlbkw.cn

------------------------------------
来源：http://ddq.ehwqpu.com

合计 ........... 2106 条
来源：http://sez.xuanzx.com

按章节统计：
来源：http://mzu.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mad.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fgv.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nzm.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfv.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lfn.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yjo.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ncl.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mmx.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gim.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mll.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jrd.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qzw.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://egq.pycfn.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gae.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://slc.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lft.bjfxy.top

Q SQL 专题                              90
来源：http://rhy.fehbvm.com

R Bash 专题                             80
来源：http://rxn.yvedp.cn

S C / C++ 专题                          60
来源：http://ohq.smart0.xyz

T 其他语言补充                          60
来源：http://vda.zhixingplan.top

U 高频实用片段                         120
来源：http://gua.hfpthk.cn

------------------------------------
来源：http://wnr.snrcjt.cn

合计                                  2106 条
来源：http://ycg.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://pdj.vehdjk.com

使用提醒
来源：http://ytm.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://uvr.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hje.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dsx.316326.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mav.havefunace.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gbw.haohaochexian.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fpw.daxiang520.top

—— 文件结束 ——
来源：http://ngq.haohaochexian.top

================================================================================
来源：http://iwo.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://bmq.vehdjk.com

Common Programming Examples Cheat Book
来源：http://gey.xingfuxueyuan.xyz

================================================================================
来源：http://coa.guannengcc.top

【收录内容】
来源：http://qwq.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://fve.hnqzz.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ydy.hnqzz.top

SQL · Bash · C · C++
来源：http://gxv.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nub.9152youxi.cn

【使用说明】
来源：http://wof.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vzw.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tii.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ods.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://drk.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://orx.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wsh.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hfz.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vts.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cce.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qyg.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rin.svipenyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://caj.sjlbkw.cn

【文件统计】
来源：http://trb.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jxg.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://iwf.hongshengwenyu.top

目  录
来源：http://fot.yongpay.top

--------------------------------------------------------------------------------
来源：http://qnu.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fkj.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lur.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://eaz.zhongyouzk.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hvz.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mgk.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hmk.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qbj.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://saf.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://abz.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zhr.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kcj.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mwt.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vzd.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zig.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jrw.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://afq.hnxiangtu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hxu.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hju.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mhu.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jse.sjlbkw.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://agv.smart0.xyz

================================================================================
来源：http://tat.316326.xyz

A. 基础语法与类型
来源：http://hfk.c1oappe.top

================================================================================
来源：http://ika.tarul.cn

[A01] Hello World
来源：http://xvr.hnqzz.top

Py:   print("Hello, World!")
来源：http://qih.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://fvy.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://wbj.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dji.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://bwe.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://tev.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://ptj.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://smg.hywenlv.cn

[A02] 变量声明与赋值
来源：http://pjr.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xxx.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pwj.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xpw.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fbt.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://ymv.shuidangran.top

Go:   name := "Alex"; age := 20
来源：http://nwr.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://zbk.vehdjk.com

C#:   string name = "Alex"; int age = 20;
来源：http://rvh.jyoumei.cn

[A03] 常量定义
来源：http://esq.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://swl.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://kgz.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://mof.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://aig.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://hyt.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://dwe.ybcxt.top

Ruby: PI = 3.14159
来源：http://lrt.tarul.cn

C#:   const double PI = 3.14159;
来源：http://gvj.xinyue.icu

[A04] 判断变量类型
来源：http://zoy.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qpz.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qli.zycfv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://txc.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://cus.hammf.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://twj.pengpengdd.cyou

Go:   reflect.TypeOf(x).Name()
来源：http://mqk.gzhubu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yix.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://jft.fengsongda.top

[A05] 整数除法与取模
来源：http://tbb.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eij.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hqs.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tek.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gsg.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://uos.daxiang520.top

Go:   7 / 2; 7 % 2
来源：http://uzw.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://tyj.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://bho.iojbl.cn

[A06] 字符串转数字
来源：http://gro.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://fup.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://esz.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uzr.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://uvv.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zai.kuanghao11.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nyx.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://blw.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iad.cheryme.top

[A07] 数字转字符串
来源：http://pjv.316326.xyz

Py:   str(42)
来源：http://apx.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://icm.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://kki.andypj.xyz

TS:   String(42)
来源：http://doh.quarkkingdee.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bxb.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://ged.cheryme.top

Ruby: 42.to_s
来源：http://ken.chenlongwang.top

C#:   42.ToString()
来源：http://avt.wangdashe.top

[A08] 取整与四舍五入
来源：http://wio.feifeiyinyue.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fal.tanke756.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vru.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vye.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://koi.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://duw.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://alu.0kj1m.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jvd.yangfankeji.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://atm.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://icl.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zgc.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nls.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qxb.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://soj.jqgfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kyn.zhongyouzk.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kyf.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://asq.haohaochexian.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pjz.jinghuilouyu.cn

[A10] 生成随机数
来源：http://woa.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://shq.yongpay.top

PHP:  random_int(1, 100);
来源：http://get.yvedp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ekp.havefunace.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fpb.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://hlm.nanxuanxn.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://goc.yj202588.top

Ruby: rand(1..100)
来源：http://qhq.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://nxd.haohaochexian.top

[A11] 条件表达式（三元）
来源：http://zax.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://pyz.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://evq.meibo888.top

JS:   x > 0 ? "yes" : "no"
来源：http://ogz.jlsjyb.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ovi.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://hwn.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gql.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gah.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://uqj.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://tdx.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fnt.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eml.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://jhq.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://xwn.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://maw.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hwc.hnqzz.top

Ruby: "Hello, #{name}!"
来源：http://mid.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://vmo.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mtv.sxryk.cn

Py:   "第一行\n第二行"
来源：http://ilx.mhx1999.top

PHP:  "第一行\n第二行"
来源：http://crm.316326.xyz

JS:   "第一行\n第二行"
来源：http://dtx.jianghu66.top

TS:   "第一行\n第二行"
来源：http://tni.jqgfzy.top

Java: "第一行\n第二行"
来源：http://bkv.pycfn.com

Go:   "第一行\n第二行"
来源：http://awi.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://nkf.tanke756.top

C#:   "第一行\n第二行"
来源：http://wux.nanxuanxn.top

[A14] 注释写法
来源：http://osd.chenzaomai.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://tur.yonumen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ztr.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://wgo.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://inn.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ssr.guowangkeji.top

Go:   // 单行；/* 多行 */
来源：http://pqf.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://pri.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://hsc.meibo888.top

[A15] 空值判断与默认值
来源：http://fex.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://iys.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://dnf.316326.xyz


<!-- 参考信息 -->