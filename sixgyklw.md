代发 wailian999

[U99] JS：事件监听
来源：http://efv.tanke756.top

el.addEventListener("click", e => {})
来源：http://qib.yuxming.cn

[U100] JS：DOM 查询
来源：http://oat.xziqi.cn

document.querySelector(".item")
来源：http://yxe.fktsv.cn

[U101] JS：classList 操作
来源：http://fyn.redwolf501.top

el.classList.toggle("active")
来源：http://kfu.yonumen.top

[U102] JS：本地存储
来源：http://vpl.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hcd.jqgfzy.top

[U103] JS：定时器
来源：http://omj.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uwt.epnwcf.com

[U104] JS：防抖
来源：http://kjy.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggw.gotoacloud.top

[U105] JS：节流
来源：http://lzj.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://azo.316326.xyz

[U106] JS：日期格式化
来源：http://idr.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oyl.sysykeji.top

[U107] JS：数字千分位
来源：http://qfd.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iod.daria6918.cn

[U108] JS：随机整数
来源：http://kbx.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ipr.zhiwuduotai.top

[U109] JS：数组分组
来源：http://kng.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://mxi.bjfxy.top

[U110] JS：数组分块
来源：http://bii.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xav.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://ame.zhoulong.xyz

new Map(Object.entries(obj))
来源：http://zwi.wangdashe.top

[U112] JS：字符串补位
来源：http://xzd.yuxming.cn

"7".padStart(3, "0")
来源：http://sna.hcnkem.com

[U113] JS：正则替换全部
来源：http://qik.shuidangran.top

s.replaceAll("a", "b")
来源：http://yja.bbcook.cn

[U114] JS：JSON 深比较
来源：http://tek.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://obq.bbcook.cn

[U115] JS：生成 UUID
来源：http://pvb.zdbjq.cn

crypto.randomUUID()
来源：http://vkw.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://olt.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://qrn.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://tgq.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://qpu.jyoumei.cn

[U118] JS：开发服务器
来源：http://ovs.ppjwa.cn

npm i -D vite;  npx vite
来源：http://gqz.andypj.xyz

[U119] JS：生产构建
来源：http://afp.fktsv.cn

npx vite build
来源：http://mwx.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://pir.havefunace.top

import.meta.env.VITE_API_URL
来源：http://mcc.fengsongda.top

================================================================================
来源：http://pij.yongpay.top

统计汇总
来源：http://ozv.yuxming.cn

================================================================================
来源：http://sxm.snrcjt.cn

按语言统计（条）：
来源：http://kdq.sysykeji.top

Python ......... 252
来源：http://rmi.jinyuanbaomall.cn

PHP ............ 252
来源：http://dbv.yueranfly.top

JavaScript ..... 252
来源：http://ini.52xcode.cn

TypeScript ..... 212
来源：http://qpi.jiagoushi.top

Java ........... 212
来源：http://bnk.gzhubu.top

Go ............. 212
来源：http://vwk.jiagoushi.top

Ruby ........... 212
来源：http://ilz.fktsv.cn

C# ............. 212
来源：http://zme.chenzaomai.com

C .............. 30
来源：http://ukv.cheryme.top

C++ ............ 30
来源：http://zbi.zhoulong.xyz

SQL ............ 90
来源：http://wpo.pycfn.com

Bash ........... 80
来源：http://nat.jinqigufen.top

Kotlin ......... 15
来源：http://lpg.guannengcc.top

Swift .......... 15
来源：http://uvp.daria6918.cn

Lua ............ 10
来源：http://loo.iojbl.cn

Perl ........... 10
来源：http://rwa.meibo888.top

Scala .......... 10
来源：http://lnz.uphjek.com

------------------------------------
来源：http://mar.birdmap.top

合计 ........... 2106 条
来源：http://ylh.fengsongda.top

按章节统计：
来源：http://rqq.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zgu.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://acl.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vdi.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fbd.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://owp.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nxe.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fgq.zhongyouzk.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zax.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vdk.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tol.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zlg.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qor.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://usy.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://utr.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pgg.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zpd.zdqjudy.top

Q SQL 专题                              90
来源：http://mih.xuetiantiany.cn

R Bash 专题                             80
来源：http://xyo.shuidangran.top

S C / C++ 专题                          60
来源：http://frl.jianghu66.top

T 其他语言补充                          60
来源：http://vng.gaohongyu789.top

U 高频实用片段                         120
来源：http://zvc.xylfe.cn

------------------------------------
来源：http://afd.zhiwuduotai.top

合计                                  2106 条
来源：http://tpu.uphjek.com

--------------------------------------------------------------------------------
来源：http://eqb.chenzaomai.com

使用提醒
来源：http://jzf.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ywn.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vqt.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qvh.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rcm.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kxz.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kix.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://qsb.jinyuanbaomall.cn

================================================================================
来源：http://jvn.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://jlg.redwolf501.top

Common Programming Examples Cheat Book
来源：http://ewe.sysykeji.top

================================================================================
来源：http://ukt.andypj.xyz

【收录内容】
来源：http://hei.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bxw.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cns.yj20258888.top

SQL · Bash · C · C++
来源：http://prz.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xux.cucudq.cn

【使用说明】
来源：http://mcr.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lpe.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pvk.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fhb.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bcd.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oak.sysykeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nkp.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://auw.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mip.feifeiyinyue.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gle.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://csm.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gur.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qpe.kuanghao11.cn

【文件统计】
来源：http://nrt.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sce.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://hfj.uphjek.com

目  录
来源：http://rrd.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://ayz.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://puu.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kyt.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tgz.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nqp.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://adz.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lnz.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vvf.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kuh.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tpq.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yfz.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uqx.ydjk.org.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mbt.aibaodan.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xhi.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eju.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://erg.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ewk.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zju.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cbt.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lux.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rhm.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://duj.dashuyun.cn

================================================================================
来源：http://lac.hnqzz.top

A. 基础语法与类型
来源：http://hrk.svipenyu.cn

================================================================================
来源：http://bkj.bbcook.cn

[A01] Hello World
来源：http://inc.sufxvd.cn

Py:   print("Hello, World!")
来源：http://vmt.hammf.cn

PHP:  echo "Hello, World!";
来源：http://wjo.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://lxc.tarul.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://djq.cqqwz.cn

Java: System.out.println("Hello, World!");
来源：http://mey.jinqigfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://ufc.sjlbkw.cn

Ruby: puts "Hello, World!"
来源：http://kuo.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kyi.gzhubu.top

[A02] 变量声明与赋值
来源：http://pew.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ojj.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pip.zdbjq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xap.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dok.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://mxf.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://ijf.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://uwq.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://yrw.9152youxi.cn

[A03] 常量定义
来源：http://vrp.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://szn.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://nyy.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://cks.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://ipb.shzxlz.cn

Java: static final double PI = 3.14159;
来源：http://yjo.svipenyu.cn

Go:   const PI = 3.14159
来源：http://sdu.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://kcl.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://ntl.sxryk.cn

[A04] 判断变量类型
来源：http://tod.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://iod.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lar.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dpx.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://ewi.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dao.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://nfg.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mvz.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://krb.yj20258888.top

[A05] 整数除法与取模
来源：http://wek.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kig.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jsd.chenlongwang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bqq.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hcj.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://seo.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://mgr.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://lpv.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://juw.gzhubu.top

[A06] 字符串转数字
来源：http://hqx.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://oma.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ehe.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lhu.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ehk.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jkt.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dor.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tkz.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gqa.pengpengdd.cyou

[A07] 数字转字符串
来源：http://xky.hesvh.cn

Py:   str(42)
来源：http://txv.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://zpt.tian-w.cn

JS:   String(42); (42).toString()
来源：http://jvm.jqgfzy.top

TS:   String(42)
来源：http://apg.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cnl.yj202588.top

Go:   strconv.Itoa(42)
来源：http://twk.hnxiangtu.top

Ruby: 42.to_s
来源：http://phc.sysykeji.top

C#:   42.ToString()
来源：http://juz.xylfe.cn

[A08] 取整与四舍五入
来源：http://jix.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jhf.jinqigfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xke.xuetiantiany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yxg.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hev.jinqigufen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://znh.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mfv.havefunace.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pxi.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kpo.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://wbr.fktsv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rae.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tea.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ydx.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kpm.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bjx.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vps.ydzc1.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xbe.xylfe.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jrd.9152youxi.cn

[A10] 生成随机数
来源：http://nkb.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://xrj.birdmap.top

PHP:  random_int(1, 100);
来源：http://acx.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fiw.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://thk.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://bjd.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wah.zhoulong.xyz

Ruby: rand(1..100)
来源：http://qxr.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://bux.shangyingyoupin.top

[A11] 条件表达式（三元）
来源：http://fap.jqgufenzy.top

Py:   "yes" if x > 0 else "no"
来源：http://qmg.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://igv.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://xwu.aibaodan.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xdi.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://jsf.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bum.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://upn.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://liy.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://did.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://atj.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iuh.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://cvl.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://xht.havefunace.top

Java: "Hello, %s!".formatted(name)
来源：http://zjf.ywan-chungtsiang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mka.zhoulong.xyz

Ruby: "Hello, #{name}!"
来源：http://ihr.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://gud.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://sdy.sweek.top

Py:   "第一行\n第二行"
来源：http://vqr.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://hwy.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://rza.yanxiufei.cn

TS:   "第一行\n第二行"
来源：http://bbr.yvedp.cn

Java: "第一行\n第二行"
来源：http://rhk.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://xaz.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://vii.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://zqx.ydzc1.top

[A14] 注释写法
来源：http://ulh.zdbjq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ooo.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fft.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://egw.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://hsf.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://owq.epnwcf.com

Go:   // 单行；/* 多行 */
来源：http://gyd.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://mdy.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://kpr.nwbrower.top

[A15] 空值判断与默认值
来源：http://dej.iojbl.cn

Py:   value = data or "默认值"
来源：http://vxk.yonumen.top

PHP:  $value = $data ?? "默认值";
来源：http://ces.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://oau.andypj.xyz

TS:   const value = data ?? "默认值";
来源：http://iro.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://see.yonumen.top

Go:   if data == "" { data = "默认值" }
来源：http://wap.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://wta.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://bxu.yj202588.top

[A16] 真假值判断规则
来源：http://fqr.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xgv.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gqd.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gqv.cashguo.top

TS:   if (!x) {}
来源：http://tpt.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vds.jinqigfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oii.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://smh.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xqb.fanxiaobao.xyz

[A17] 位运算
来源：http://ese.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpb.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ori.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lga.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dqe.tian-w.cn


<!-- 参考信息 -->