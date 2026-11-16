代发 wailian999

[U97] JS：并发请求
来源：http://wwt.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ngm.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://rhr.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zsd.yanxiufei.cn

[U99] JS：事件监听
来源：http://csa.yonumen.top

el.addEventListener("click", e => {})
来源：http://dgd.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://bej.hywenlv.cn

document.querySelector(".item")
来源：http://qpa.bbcook.cn

[U101] JS：classList 操作
来源：http://afu.jianghu66.top

el.classList.toggle("active")
来源：http://msf.daxiang520.top

[U102] JS：本地存储
来源：http://xgp.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bit.52xcode.cn

[U103] JS：定时器
来源：http://eor.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wbn.xinyue.icu

[U104] JS：防抖
来源：http://zgm.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hvq.zdqjudy.top

[U105] JS：节流
来源：http://mjj.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://swj.zhixingplan.top

[U106] JS：日期格式化
来源：http://hbl.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bii.iojbl.cn

[U107] JS：数字千分位
来源：http://udw.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xup.ydzc1.top

[U108] JS：随机整数
来源：http://ryq.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iyk.smart0.xyz

[U109] JS：数组分组
来源：http://hag.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://crg.hcnkem.com

[U110] JS：数组分块
来源：http://uny.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bvv.smart0.xyz

[U111] JS：对象转 Map
来源：http://dnk.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://gmf.ppjwa.cn

[U112] JS：字符串补位
来源：http://hgg.sxryk.cn

"7".padStart(3, "0")
来源：http://zwj.jyoumei.cn

[U113] JS：正则替换全部
来源：http://vbx.mhx1999.top

s.replaceAll("a", "b")
来源：http://gjs.wangdashe.top

[U114] JS：JSON 深比较
来源：http://wgw.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ugt.shuidangran.top

[U115] JS：生成 UUID
来源：http://hij.jqgufenzy.top

crypto.randomUUID()
来源：http://ezw.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://ier.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://fna.zhixingplan.top

[U117] JS：单元测试
来源：http://gsl.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://lbs.guowangkeji.top

[U118] JS：开发服务器
来源：http://ttk.yvedp.cn

npm i -D vite;  npx vite
来源：http://ijo.hnxiangtu.top

[U119] JS：生产构建
来源：http://kaq.ydzc1.top

npx vite build
来源：http://scb.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://znp.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://nbs.pycfn.com

================================================================================
来源：http://rmf.jinyuanbaomall.cn

统计汇总
来源：http://dvw.jlsjyb.cn

================================================================================
来源：http://qet.jqgfzy.top

按语言统计（条）：
来源：http://kfh.jlsjyb.cn

Python ......... 252
来源：http://rao.daria6918.cn

PHP ............ 252
来源：http://dmy.feifeiyinyue.top

JavaScript ..... 252
来源：http://jni.cashguo.top

TypeScript ..... 212
来源：http://cyd.9152youxi.cn

Java ........... 212
来源：http://sqm.quarkkingdee.top

Go ............. 212
来源：http://dpj.zhijiandao.cn

Ruby ........... 212
来源：http://pgb.hcnkem.com

C# ............. 212
来源：http://sog.ydjk.org.cn

C .............. 30
来源：http://wph.sufxvd.cn

C++ ............ 30
来源：http://lot.cheryme.top

SQL ............ 90
来源：http://mti.hnxiangtu.top

Bash ........... 80
来源：http://zbg.cashguo.top

Kotlin ......... 15
来源：http://fdv.birdmap.top

Swift .......... 15
来源：http://qvk.havefunace.top

Lua ............ 10
来源：http://gcz.yfazqb.com

Perl ........... 10
来源：http://bys.yuxming.cn

Scala .......... 10
来源：http://nnq.0kj1m.cn

------------------------------------
来源：http://ofs.fktsv.cn

合计 ........... 2106 条
来源：http://rff.sufxvd.cn

按章节统计：
来源：http://vjo.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gue.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xud.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jse.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aon.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ios.bbcook.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gxf.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jru.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bpd.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jon.ehwqpu.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cui.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cpe.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jxp.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cff.meibo888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wtv.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zas.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://feu.epnwcf.com

Q SQL 专题                              90
来源：http://rcx.jinqigfzy.top

R Bash 专题                             80
来源：http://rdw.ivvv.top

S C / C++ 专题                          60
来源：http://ziq.havefunace.top

T 其他语言补充                          60
来源：http://dfs.cheryme.top

U 高频实用片段                         120
来源：http://plh.ppjwa.cn

------------------------------------
来源：http://xis.epnwcf.com

合计                                  2106 条
来源：http://wbn.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://krm.jqgfzy.top

使用提醒
来源：http://pif.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://vmk.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kpr.chenjidiqi.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ijm.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bgw.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ivi.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ldd.birdmap.top

—— 文件结束 ——
来源：http://myw.yongpay.top

================================================================================
来源：http://bsi.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://kix.tarul.cn

Common Programming Examples Cheat Book
来源：http://wxm.zhongyouzk.top

================================================================================
来源：http://tey.bbcook.cn

【收录内容】
来源：http://swh.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dvs.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iqz.jinghuilouyu.cn

SQL · Bash · C · C++
来源：http://cgx.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vgx.hywenlv.cn

【使用说明】
来源：http://ngp.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bbm.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pnd.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://elr.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kao.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rof.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://faz.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lhf.pycfn.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vms.zycfv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jof.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pnt.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://enn.bbcook.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://grm.jinyuanbaomall.cn

【文件统计】
来源：http://noz.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kwv.yvedp.cn

--------------------------------------------------------------------------------
来源：http://luh.gogol.net.cn

目  录
来源：http://vxo.316326.xyz

--------------------------------------------------------------------------------
来源：http://hbi.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nme.havefunace.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rme.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://srh.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ijx.haohaochexian.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yrm.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yrt.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gsy.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pkd.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vnz.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xbc.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jbj.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kzp.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wtu.aibaodan.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lxp.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tpo.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lbt.jinqigufen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uxi.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://krz.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wqi.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qvl.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://otj.bbcook.cn

================================================================================
来源：http://byc.yfazqb.com

A. 基础语法与类型
来源：http://fqw.yuxming.cn

================================================================================
来源：http://uwi.cqqwz.cn

[A01] Hello World
来源：http://xpx.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://qrb.hcnkem.com

PHP:  echo "Hello, World!";
来源：http://gao.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://wtx.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rqm.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://xty.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://kji.sjlbkw.cn

Ruby: puts "Hello, World!"
来源：http://xgw.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kgb.bjfxy.top

[A02] 变量声明与赋值
来源：http://kal.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wym.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qnw.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://qam.ppjwa.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ntf.tianlin.xyz

Java: String name = "Alex"; int age = 20;
来源：http://czr.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://qrr.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://img.jqgufenzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://sob.epnwcf.com

[A03] 常量定义
来源：http://iop.ydjk.org.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bue.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://oxy.iojbl.cn

JS:   const PI = 3.14159;
来源：http://sxf.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://nrh.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://oyt.sweek.top

Go:   const PI = 3.14159
来源：http://sop.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://abb.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://hrm.zycfv.cn

[A04] 判断变量类型
来源：http://ijw.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jzn.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kaz.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://smo.yvedp.cn

TS:   typeof x; x instanceof Date
来源：http://xnc.xylfe.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wen.xylfe.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bef.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vda.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://txq.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://omt.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sjj.pycfn.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://biu.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xkl.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://otl.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://vot.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://won.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://vyz.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://yit.smart0.xyz

[A06] 字符串转数字
来源：http://vpm.hysaishi.cn

Py:   int("42"); float("3.14")
来源：http://gad.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ijh.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uih.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://rwi.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jok.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ica.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vyk.xziqi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oda.uphjek.com

[A07] 数字转字符串
来源：http://yrx.jinqigufen.top

Py:   str(42)
来源：http://qyv.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://lfu.svipenyu.cn

JS:   String(42); (42).toString()
来源：http://yqv.mhx1999.top

TS:   String(42)
来源：http://ecm.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://eay.shanyushiyangkeji.top

Go:   strconv.Itoa(42)
来源：http://bsf.gogol.net.cn

Ruby: 42.to_s
来源：http://psi.wangdashe.top

C#:   42.ToString()
来源：http://cvz.aibaodan.cn

[A08] 取整与四舍五入
来源：http://cuh.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lzc.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mle.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kux.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mfq.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yaa.fanxiaobao.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://emv.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://asv.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cih.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://bfe.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dhr.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kzr.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fxc.dianchejie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nma.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gdf.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ekg.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aif.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://noe.sxryk.cn

[A10] 生成随机数
来源：http://vki.tianlin.xyz

Py:   import random; random.randint(1, 100)
来源：http://biu.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://cdi.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://llw.chenzaomai.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aum.ydjk.org.cn

Java: new Random().nextInt(100) + 1
来源：http://llr.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xjo.jlsjyb.cn

Ruby: rand(1..100)
来源：http://fdz.9152youxi.cn

C#:   new Random().Next(1, 101)
来源：http://chf.yj20258888.top

[A11] 条件表达式（三元）
来源：http://ths.gaohongyu789.top

Py:   "yes" if x > 0 else "no"
来源：http://voe.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://qai.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://jct.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://ovk.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://huf.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ehe.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zra.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ohx.meibo888.top

[A12] 字符串插值 / 格式化
来源：http://drr.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://euo.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kqq.fehbvm.com

JS:   `Hello, ${name}!`
来源：http://jzt.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://xui.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://tdh.cheryme.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tun.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://hjk.jyoumei.cn

C#:   $"Hello, {name}!"
来源：http://ayq.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://efw.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://gep.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://xze.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://ipw.jianghu66.top

TS:   "第一行\n第二行"
来源：http://dbi.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://ydq.tarul.cn

Go:   "第一行\n第二行"
来源：http://hnt.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://yxi.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://pdc.yfazqb.com

[A14] 注释写法
来源：http://lwp.sxryk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tww.yuanzhike.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pro.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://zoc.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://xgx.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ldl.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://uxi.ydjk.org.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qrx.jinghuilouyu.cn

C#:   // 单行；/* 多行 */
来源：http://mkj.daria6918.cn

[A15] 空值判断与默认值
来源：http://ysb.hongshengwenyu.top

Py:   value = data or "默认值"
来源：http://vfj.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://lon.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://khg.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://ndl.haohaochexian.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://frp.cheryme.top

Go:   if data == "" { data = "默认值" }
来源：http://lii.zhaomingkeji.xyz

Ruby: value = data || "默认值"
来源：http://rik.sweek.top

C#:   var value = data ?? "默认值";
来源：http://wvh.shuidangran.top

[A16] 真假值判断规则
来源：http://yvc.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dtz.hcnkem.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jlp.shangyingyoupin.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wcm.ydjk.org.cn

TS:   if (!x) {}
来源：http://ldm.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ydx.yangfankeji.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jfo.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ktw.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jxu.ppjwa.cn

[A17] 位运算
来源：http://ibc.zhaomingkeji.xyz


<!-- 参考信息 -->