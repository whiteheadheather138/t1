代发 wailian999

[U99] JS：事件监听
来源：http://ofr.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://iwy.svipenyu.cn

[U100] JS：DOM 查询
来源：http://upf.quarkkingdee.top

document.querySelector(".item")
来源：http://mzr.yonumen.top

[U101] JS：classList 操作
来源：http://bff.hesvh.cn

el.classList.toggle("active")
来源：http://sbc.hfpthk.cn

[U102] JS：本地存储
来源：http://pxv.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wim.xylfe.cn

[U103] JS：定时器
来源：http://yqy.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ghe.yfazqb.com

[U104] JS：防抖
来源：http://zpv.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://smn.chenlongwang.top

[U105] JS：节流
来源：http://zed.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://snc.zhongyouzk.top

[U106] JS：日期格式化
来源：http://nns.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xzj.zdqjudy.top

[U107] JS：数字千分位
来源：http://crh.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fel.hfpthk.cn

[U108] JS：随机整数
来源：http://wop.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qkj.cdnleiting.top

[U109] JS：数组分组
来源：http://agi.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://rzi.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://icm.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://her.hesvh.cn

[U111] JS：对象转 Map
来源：http://cbb.ivvv.top

new Map(Object.entries(obj))
来源：http://otj.zdqjudy.top

[U112] JS：字符串补位
来源：http://frf.wangdashe.top

"7".padStart(3, "0")
来源：http://ykv.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://gtk.chenzaomai.com

s.replaceAll("a", "b")
来源：http://isj.daria6918.cn

[U114] JS：JSON 深比较
来源：http://aaf.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cfh.hysaishi.cn

[U115] JS：生成 UUID
来源：http://bnq.yj20258.top

crypto.randomUUID()
来源：http://krx.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://typ.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://clu.yvedp.cn

[U117] JS：单元测试
来源：http://yxm.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://kiu.ppjwa.cn

[U118] JS：开发服务器
来源：http://lag.cashguo.top

npm i -D vite;  npx vite
来源：http://ant.zhengqikj.top

[U119] JS：生产构建
来源：http://qsg.meibo888.top

npx vite build
来源：http://dst.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://gzs.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://lqk.sxryk.cn

================================================================================
来源：http://lfs.tian-w.cn

统计汇总
来源：http://jde.nanxinkj.top

================================================================================
来源：http://iyn.tarul.cn

按语言统计（条）：
来源：http://sse.hesvh.cn

Python ......... 252
来源：http://bta.bbcook.cn

PHP ............ 252
来源：http://qvj.zhongyouzk.top

JavaScript ..... 252
来源：http://wwq.zhiwuduotai.top

TypeScript ..... 212
来源：http://tdh.cheryme.top

Java ........... 212
来源：http://nui.xuanzx.com

Go ............. 212
来源：http://hzl.daria6918.cn

Ruby ........... 212
来源：http://kpk.xinyue.icu

C# ............. 212
来源：http://sqj.tian-w.cn

C .............. 30
来源：http://ceh.quarkkingdee.top

C++ ............ 30
来源：http://wqq.tanke756.top

SQL ............ 90
来源：http://sul.hysaishi.cn

Bash ........... 80
来源：http://rwv.cashguo.top

Kotlin ......... 15
来源：http://spx.kuanghao11.cn

Swift .......... 15
来源：http://oof.yanxiufei.cn

Lua ............ 10
来源：http://ayr.bjfxy.top

Perl ........... 10
来源：http://fpd.shuidangran.top

Scala .......... 10
来源：http://kbz.chenlongwang.top

------------------------------------
来源：http://tiq.smart0.xyz

合计 ........... 2106 条
来源：http://pkz.guannengcc.top

按章节统计：
来源：http://bav.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mzr.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kjq.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xdq.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gtc.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jdm.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gil.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nct.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://opq.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vpw.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://slp.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mzb.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lgg.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wkh.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vrg.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ccs.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gll.jianghu66.top

Q SQL 专题                              90
来源：http://pvg.gzhubu.top

R Bash 专题                             80
来源：http://hxj.sxryk.cn

S C / C++ 专题                          60
来源：http://qhc.mhx1999.top

T 其他语言补充                          60
来源：http://duc.hammf.cn

U 高频实用片段                         120
来源：http://lpz.sxryk.cn

------------------------------------
来源：http://vxv.c1oappe.top

合计                                  2106 条
来源：http://cxi.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://xeb.vehdjk.com

使用提醒
来源：http://lrm.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://xug.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vcy.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rdq.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cyu.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://let.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gcw.pycfn.com

—— 文件结束 ——
来源：http://lgw.ydjk.org.cn

================================================================================
来源：http://gbr.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://kpq.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://gcs.zhongyouzk.top

================================================================================
来源：http://xoi.ydjk.org.cn

【收录内容】
来源：http://rte.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://glf.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tec.snrcjt.cn

SQL · Bash · C · C++
来源：http://yep.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nda.zhijiandao.cn

【使用说明】
来源：http://rqb.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ekq.jiagoushi.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://adg.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://beu.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vhn.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lay.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kmt.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mgu.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xws.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hgp.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pzt.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://abq.sxryk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://reg.hnxiangtu.top

【文件统计】
来源：http://djw.dianchejie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ays.daria6918.cn

--------------------------------------------------------------------------------
来源：http://gio.yj202588.top

目  录
来源：http://xum.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://boa.hnqzz.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ddn.guannengcc.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bgh.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qqq.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vuu.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cjp.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cnt.vehdjk.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cbw.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://maw.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mlm.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vkf.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xnq.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lme.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vhu.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xvm.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://huf.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mzv.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jlw.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wxi.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sut.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mga.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xej.dashuyun.cn

================================================================================
来源：http://dzg.yuxming.cn

A. 基础语法与类型
来源：http://sxk.haohaochexian.top

================================================================================
来源：http://nwr.sysykeji.top

[A01] Hello World
来源：http://xew.hywenlv.cn

Py:   print("Hello, World!")
来源：http://rct.pycfn.com

PHP:  echo "Hello, World!";
来源：http://znx.cheryme.top

JS:   console.log("Hello, World!");
来源：http://lpg.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nfo.yj20258888.top

Java: System.out.println("Hello, World!");
来源：http://afk.hammf.cn

Go:   fmt.Println("Hello, World!")
来源：http://rvb.bbcook.cn

Ruby: puts "Hello, World!"
来源：http://tyf.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://sao.xylfe.cn

[A02] 变量声明与赋值
来源：http://ikf.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://asd.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kfe.gogol.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tpz.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xfk.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://lsc.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://ngm.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://std.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://cyu.chenjidiqi.icu

[A03] 常量定义
来源：http://ceu.nwbrower.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://isb.hammf.cn

PHP:  const PI = 3.14159;
来源：http://twl.zycfv.cn

JS:   const PI = 3.14159;
来源：http://jtn.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://xgo.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://hic.yj20258888.top

Go:   const PI = 3.14159
来源：http://jxt.yfazqb.com

Ruby: PI = 3.14159
来源：http://aoo.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://xfu.kuanghao11.cn

[A04] 判断变量类型
来源：http://bsl.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rfm.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mln.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xva.ivvv.top

TS:   typeof x; x instanceof Date
来源：http://jrs.yfazqb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://brn.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wao.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://trq.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://orl.tarul.cn

[A05] 整数除法与取模
来源：http://yzf.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ynw.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cps.andypj.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xgq.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ybz.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://hcf.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://zbl.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://fed.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://yro.havefunace.top

[A06] 字符串转数字
来源：http://yyt.ydzc1.top

Py:   int("42"); float("3.14")
来源：http://zje.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://axf.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://csl.yueranfly.top

TS:   parseInt("42", 10); Number("42")
来源：http://dmt.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ubm.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yeq.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yjt.zhijiandao.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://szk.hammf.cn

[A07] 数字转字符串
来源：http://jrq.zhongyouzk.top

Py:   str(42)
来源：http://xpt.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://sbj.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://wqo.svipenyu.cn

TS:   String(42)
来源：http://afy.dashuyun.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://avc.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://hyy.tian-w.cn

Ruby: 42.to_s
来源：http://vyi.yueranfly.top

C#:   42.ToString()
来源：http://uva.316326.xyz

[A08] 取整与四舍五入
来源：http://hol.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cop.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bjw.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vho.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fhi.feifeiyinyue.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nby.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vag.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jyt.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ats.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://pcb.aibaodan.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://crc.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ekp.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qoy.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lue.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mkb.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zug.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kkj.shanyushiyangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gpo.cashguo.top

[A10] 生成随机数
来源：http://orz.bbcook.cn

Py:   import random; random.randint(1, 100)
来源：http://orp.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://lkf.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hdw.zhijiandao.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://urg.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://ezc.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ess.meibo888.top

Ruby: rand(1..100)
来源：http://nua.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://jyn.hammf.cn

[A11] 条件表达式（三元）
来源：http://xud.dashuyun.cn

Py:   "yes" if x > 0 else "no"
来源：http://ssu.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://tpr.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ynr.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://nkm.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://kjv.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pcp.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://jed.zhixingplan.top

C#:   x > 0 ? "yes" : "no"
来源：http://hll.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://rug.chenjidiqi.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wer.fanxiaobao.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jrv.snrcjt.cn

JS:   `Hello, ${name}!`
来源：http://fjg.ywan-chungtsiang.top

TS:   `Hello, ${name}!`
来源：http://ajo.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://sii.bjfxy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://puh.ydzc1.top

Ruby: "Hello, #{name}!"
来源：http://wro.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://eaq.nwbrower.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ybg.hnqzz.top

Py:   "第一行\n第二行"
来源：http://kxh.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://ukw.yj20258.top

JS:   "第一行\n第二行"
来源：http://wee.c1oappe.top

TS:   "第一行\n第二行"
来源：http://vlc.zdbjq.cn

Java: "第一行\n第二行"
来源：http://mle.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://jkd.daria6918.cn

Ruby: "第一行\n第二行"
来源：http://njl.ctjpmb.com

C#:   "第一行\n第二行"
来源：http://har.feifeiyinyue.top

[A14] 注释写法
来源：http://kvn.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ewz.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://iso.ydjk.org.cn

JS:   // 单行；/* 多行 */
来源：http://gxy.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://wvv.hywenlv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dic.epnwcf.com

Go:   // 单行；/* 多行 */
来源：http://cld.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://uxb.pycfn.com

C#:   // 单行；/* 多行 */
来源：http://nvt.ppjwa.cn

[A15] 空值判断与默认值
来源：http://yvp.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://eew.mhx1999.top

PHP:  $value = $data ?? "默认值";
来源：http://mpp.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://tva.epnwcf.com

TS:   const value = data ?? "默认值";
来源：http://rfk.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sxk.zhoulong.xyz

Go:   if data == "" { data = "默认值" }
来源：http://bop.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://fgi.aizwys.cn

C#:   var value = data ?? "默认值";
来源：http://syp.zhengqikj.top

[A16] 真假值判断规则
来源：http://ouu.dianchejie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zcm.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xpv.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gxq.fzhhl.top

TS:   if (!x) {}
来源：http://wcu.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sqc.zhengqikj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tev.xuetiantiany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mcg.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lfd.sjlbkw.cn

[A17] 位运算
来源：http://owy.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://toh.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zad.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://udo.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qwc.shangyingyoupin.top


<!-- 参考信息 -->