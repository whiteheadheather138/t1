代发 wailian999

[U87] JS：解构默认值
来源：http://ppi.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://uhd.hysaishi.cn

[U88] JS：对象展开合并
来源：http://hfn.xuetiantiany.cn

{ ...a, ...b }
来源：http://bpc.birdmap.top

[U89] JS：数组去重
来源：http://ycr.epnwcf.com

[...new Set(arr)]
来源：http://rhm.daxiang520.top

[U90] JS：数字数组排序
来源：http://ctb.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://mbb.cucudq.cn

[U91] JS：对象键值遍历
来源：http://oei.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kqe.zhongyouzk.top

[U92] JS：深拷贝
来源：http://hje.yuanzhike.top

structuredClone(obj)
来源：http://lcl.sjlbkw.cn

[U93] JS：模板字符串
来源：http://gxa.sweek.top

`共 ${n} 条`
来源：http://lae.ehwqpu.com

[U94] JS：箭头函数
来源：http://cao.hysaishi.cn

const double = x => x * 2;
来源：http://qxv.ybcxt.top

[U95] JS：Promise 包装
来源：http://kga.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://ugx.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://peh.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hsl.redwolf501.top

[U97] JS：并发请求
来源：http://snb.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://abu.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://pal.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://knj.ehwqpu.com

[U99] JS：事件监听
来源：http://abe.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://wfe.mhx1999.top

[U100] JS：DOM 查询
来源：http://ekq.cheryme.top

document.querySelector(".item")
来源：http://iuw.sufxvd.cn

[U101] JS：classList 操作
来源：http://ftb.meibo888.top

el.classList.toggle("active")
来源：http://wql.havefunace.top

[U102] JS：本地存储
来源：http://oub.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uqo.zhengqikj.top

[U103] JS：定时器
来源：http://osy.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gam.chenjidiqi.icu

[U104] JS：防抖
来源：http://cpv.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oap.havefunace.top

[U105] JS：节流
来源：http://cyh.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wgg.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://iqv.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ggo.chenlongwang.top

[U107] JS：数字千分位
来源：http://iqk.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dia.nanxinkj.top

[U108] JS：随机整数
来源：http://sfb.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://isf.xziqi.cn

[U109] JS：数组分组
来源：http://fid.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://guf.fengsongda.top

[U110] JS：数组分块
来源：http://cun.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qap.yonumen.top

[U111] JS：对象转 Map
来源：http://mso.wangdashe.top

new Map(Object.entries(obj))
来源：http://raa.52xcode.cn

[U112] JS：字符串补位
来源：http://evz.cheryme.top

"7".padStart(3, "0")
来源：http://cjy.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://hds.cucudq.cn

s.replaceAll("a", "b")
来源：http://qdz.vehdjk.com

[U114] JS：JSON 深比较
来源：http://alc.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgb.jiagoushi.top

[U115] JS：生成 UUID
来源：http://xbu.tianlin.xyz

crypto.randomUUID()
来源：http://pnn.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://hey.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://bkn.shuidangran.top

[U117] JS：单元测试
来源：http://zrk.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://knj.ppjwa.cn

[U118] JS：开发服务器
来源：http://fwd.pycfn.com

npm i -D vite;  npx vite
来源：http://ssl.hfpthk.cn

[U119] JS：生产构建
来源：http://mvn.ydjk.org.cn

npx vite build
来源：http://mrh.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://sot.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://dga.tianlin.xyz

================================================================================
来源：http://ujr.ybcxt.top

统计汇总
来源：http://qpr.hnxiangtu.top

================================================================================
来源：http://qsb.yuanzhike.top

按语言统计（条）：
来源：http://wjz.52xcode.cn

Python ......... 252
来源：http://pgp.jyoumei.cn

PHP ............ 252
来源：http://qvn.hesvh.cn

JavaScript ..... 252
来源：http://zxs.jinqigfzy.top

TypeScript ..... 212
来源：http://nkp.shzxlz.cn

Java ........... 212
来源：http://hsu.xuetiantiany.cn

Go ............. 212
来源：http://mrz.iojbl.cn

Ruby ........... 212
来源：http://ldh.feifeiyinyue.top

C# ............. 212
来源：http://uye.fzhhl.top

C .............. 30
来源：http://zuu.gogol.net.cn

C++ ............ 30
来源：http://dpa.hammf.cn

SQL ............ 90
来源：http://lvx.ivvv.top

Bash ........... 80
来源：http://jrn.yvedp.cn

Kotlin ......... 15
来源：http://dzn.pengpengdd.cyou

Swift .......... 15
来源：http://jyk.ehwqpu.com

Lua ............ 10
来源：http://ulb.jqgfzy.top

Perl ........... 10
来源：http://ynn.fzhhl.top

Scala .......... 10
来源：http://uoa.shanyushiyangkeji.top

------------------------------------
来源：http://zni.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://qtp.fengsongda.top

按章节统计：
来源：http://ngh.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://itn.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uxv.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rte.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dig.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nyp.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dsx.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://htp.hysaishi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qsh.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oay.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yib.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hwz.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lvl.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mup.fengsongda.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bja.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nop.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mjt.yuxming.cn

Q SQL 专题                              90
来源：http://scq.fanxiaobao.xyz

R Bash 专题                             80
来源：http://lxz.pycfn.com

S C / C++ 专题                          60
来源：http://fst.zhongyouzk.top

T 其他语言补充                          60
来源：http://qco.yongpay.top

U 高频实用片段                         120
来源：http://hkz.yongpay.top

------------------------------------
来源：http://glt.bbcook.cn

合计                                  2106 条
来源：http://bju.yongpay.top

--------------------------------------------------------------------------------
来源：http://hom.ctjpmb.com

使用提醒
来源：http://uzq.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://edj.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sir.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xdp.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vvt.havefunace.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sgb.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wzn.uphjek.com

—— 文件结束 ——
来源：http://wgl.pengpengdd.cyou

================================================================================
来源：http://hra.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://jhd.tarul.cn

Common Programming Examples Cheat Book
来源：http://eui.jinqigufen.top

================================================================================
来源：http://rys.chenzaomai.com

【收录内容】
来源：http://mnl.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://agg.yongpay.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ayi.nwbrower.top

SQL · Bash · C · C++
来源：http://uhh.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xip.bbcook.cn

【使用说明】
来源：http://dgj.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ifi.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://khp.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tgc.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ltq.jqgufenzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dga.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qvs.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hib.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gvn.yj20258.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jko.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gwy.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kos.shanyushiyangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hxm.9152youxi.cn

【文件统计】
来源：http://pvl.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://imx.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://imj.daria6918.cn

目  录
来源：http://owo.fengsongda.top

--------------------------------------------------------------------------------
来源：http://boa.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vtd.zycfv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lmd.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lhb.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bid.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fxz.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hzu.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://krr.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jzn.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kgu.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bew.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ljz.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vfe.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rcg.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dti.hammf.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://syb.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wip.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aji.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zea.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lim.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ixj.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ijf.kuanghao11.cn

================================================================================
来源：http://nyg.jiagoushi.top

A. 基础语法与类型
来源：http://ost.xylfe.cn

================================================================================
来源：http://qpc.hnqzz.top

[A01] Hello World
来源：http://bex.yuxming.cn

Py:   print("Hello, World!")
来源：http://kkp.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://iuc.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://ebw.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mxp.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://uhi.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://ugf.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://xub.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eij.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://uaq.mhx1999.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cbh.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wtq.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://cic.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hfh.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://eom.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://qnm.jiagoushi.top

Ruby: name = "Alex"; age = 20
来源：http://wwf.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://hng.jinqigfzy.top

[A03] 常量定义
来源：http://cdh.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wyo.jianghu66.top

PHP:  const PI = 3.14159;
来源：http://qbs.sweek.top

JS:   const PI = 3.14159;
来源：http://gtp.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://vcb.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://mvg.wangdashe.top

Go:   const PI = 3.14159
来源：http://mlt.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://iub.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://cdx.0kj1m.cn

[A04] 判断变量类型
来源：http://rnv.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ejs.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cwn.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mjh.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://fdm.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ilw.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zth.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://isn.birdmap.top

C#:   x.GetType().Name; x is int
来源：http://imi.haohaochexian.top

[A05] 整数除法与取模
来源：http://gkc.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ack.zhoulong.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://dfo.shangyingyoupin.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uim.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rlv.gzhubu.top

Java: 7 / 2; 7 % 2
来源：http://bja.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://wrp.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://oeo.daria6918.cn

C#:   7 / 2; 7 % 2
来源：http://cgo.jinyuanbaomall.cn

[A06] 字符串转数字
来源：http://zyj.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://jbs.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xyn.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rpt.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://kdw.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hvk.cqqwz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://umk.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://voz.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pis.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://prm.zhoulong.xyz

Py:   str(42)
来源：http://bxx.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://wdf.xziqi.cn

JS:   String(42); (42).toString()
来源：http://upm.bjfxy.top

TS:   String(42)
来源：http://igq.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qgu.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://ibm.yanxiufei.cn

Ruby: 42.to_s
来源：http://lpn.yongpay.top

C#:   42.ToString()
来源：http://wsp.vehdjk.com

[A08] 取整与四舍五入
来源：http://glu.redwolf501.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ayg.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ovm.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dfy.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vis.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dht.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fbf.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://hdk.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pqp.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://dnt.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gpd.jinqigufen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ztc.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uav.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zwx.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ofy.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dsx.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vnc.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ulf.jiagoushi.top

[A10] 生成随机数
来源：http://umh.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://tni.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://cox.yj20258888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://msf.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dtc.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://tif.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bzn.yuxming.cn

Ruby: rand(1..100)
来源：http://hab.vehdjk.com

C#:   new Random().Next(1, 101)
来源：http://qgr.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://xyo.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://sgi.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uea.fzhhl.top

JS:   x > 0 ? "yes" : "no"
来源：http://yis.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xuo.sufxvd.cn

Java: x > 0 ? "yes" : "no"
来源：http://bsj.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dhx.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ckn.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://grd.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://qna.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hdu.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nan.hongshengwenyu.top

JS:   `Hello, ${name}!`
来源：http://ezb.hnxiangtu.top

TS:   `Hello, ${name}!`
来源：http://ytb.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://nbr.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jjr.cqqwz.cn

Ruby: "Hello, #{name}!"
来源：http://jyp.316326.xyz

C#:   $"Hello, {name}!"
来源：http://dbt.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://kwn.shuidangran.top

Py:   "第一行\n第二行"
来源：http://ias.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://oqk.zhengqikj.top

JS:   "第一行\n第二行"
来源：http://wld.fengsongda.top

TS:   "第一行\n第二行"
来源：http://kdh.iojbl.cn

Java: "第一行\n第二行"
来源：http://dsl.redwolf501.top

Go:   "第一行\n第二行"
来源：http://ngj.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://zuf.bbcook.cn

C#:   "第一行\n第二行"
来源：http://ftc.yj202588.top

[A14] 注释写法
来源：http://uzf.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fsx.chenjidiqi.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://ybd.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://hee.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://eqr.xuanzx.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uap.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://ysw.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://evx.nanxuanxn.top


<!-- 参考信息 -->