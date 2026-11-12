代发 wailian999

[U85] JS：可选链
来源：http://dqm.c1oappe.top

a?.b?.c
来源：http://wgi.hcnkem.com

[U86] JS：空值合并
来源：http://qwr.aizwys.cn

a ?? b
来源：http://vjc.dianchejie.cn

[U87] JS：解构默认值
来源：http://hqz.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://rmz.gzhubu.top

[U88] JS：对象展开合并
来源：http://upi.haohaochexian.top

{ ...a, ...b }
来源：http://jiq.zhiwuduotai.top

[U89] JS：数组去重
来源：http://uzy.shuidangran.top

[...new Set(arr)]
来源：http://biy.mhx1999.top

[U90] JS：数字数组排序
来源：http://orb.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://yfz.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://ahj.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vbh.sweek.top

[U92] JS：深拷贝
来源：http://ugf.shangyingyoupin.top

structuredClone(obj)
来源：http://oid.shzxlz.cn

[U93] JS：模板字符串
来源：http://wep.zhixingplan.top

`共 ${n} 条`
来源：http://cdw.yj20258.top

[U94] JS：箭头函数
来源：http://vds.ehwqpu.com

const double = x => x * 2;
来源：http://tja.havefunace.top

[U95] JS：Promise 包装
来源：http://fnm.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://ymn.yvedp.cn

[U96] JS：async/await 与异常
来源：http://bpo.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zfl.tarul.cn

[U97] JS：并发请求
来源：http://tij.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://xwh.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://xrg.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mww.iojbl.cn

[U99] JS：事件监听
来源：http://ulu.guannengcc.top

el.addEventListener("click", e => {})
来源：http://drj.sweek.top

[U100] JS：DOM 查询
来源：http://lmk.ydzc1.top

document.querySelector(".item")
来源：http://znl.zhijiandao.cn

[U101] JS：classList 操作
来源：http://qfn.uphjek.com

el.classList.toggle("active")
来源：http://nvr.zhijiandao.cn

[U102] JS：本地存储
来源：http://jzn.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gql.snrcjt.cn

[U103] JS：定时器
来源：http://uix.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://efz.xylfe.cn

[U104] JS：防抖
来源：http://zrk.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcb.fengsongda.top

[U105] JS：节流
来源：http://cci.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gsm.cqqwz.cn

[U106] JS：日期格式化
来源：http://jia.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hzm.dashuyun.cn

[U107] JS：数字千分位
来源：http://jtm.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kdr.shangyingyoupin.top

[U108] JS：随机整数
来源：http://nao.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eql.jyoumei.cn

[U109] JS：数组分组
来源：http://gvw.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://har.jianghu66.top

[U110] JS：数组分块
来源：http://yue.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jni.yongpay.top

[U111] JS：对象转 Map
来源：http://mfy.dianchejie.cn

new Map(Object.entries(obj))
来源：http://ysv.dashuyun.cn

[U112] JS：字符串补位
来源：http://uyp.ydzc1.top

"7".padStart(3, "0")
来源：http://ofn.sysykeji.top

[U113] JS：正则替换全部
来源：http://yva.ivvv.top

s.replaceAll("a", "b")
来源：http://ezf.yueranfly.top

[U114] JS：JSON 深比较
来源：http://cnk.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hvu.xziqi.cn

[U115] JS：生成 UUID
来源：http://lqb.yj20258.top

crypto.randomUUID()
来源：http://vum.sweek.top

[U116] JS：类型检查（JSDoc）
来源：http://vfr.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://ory.jianghu66.top

[U117] JS：单元测试
来源：http://mwc.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://cnn.cashguo.top

[U118] JS：开发服务器
来源：http://jbg.xinyue.icu

npm i -D vite;  npx vite
来源：http://bgl.yangfankeji.com

[U119] JS：生产构建
来源：http://fqu.vehdjk.com

npx vite build
来源：http://czp.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://yvx.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://fqh.316326.xyz

================================================================================
来源：http://fqo.zhijiandao.cn

统计汇总
来源：http://rwq.kuanghao11.cn

================================================================================
来源：http://aio.ehwqpu.com

按语言统计（条）：
来源：http://hpu.snrcjt.cn

Python ......... 252
来源：http://lrb.gotoacloud.top

PHP ............ 252
来源：http://plq.cucudq.cn

JavaScript ..... 252
来源：http://gpy.jiagoushi.top

TypeScript ..... 212
来源：http://ofq.shanyushiyangkeji.top

Java ........... 212
来源：http://jqe.hesvh.cn

Go ............. 212
来源：http://scc.ehwqpu.com

Ruby ........... 212
来源：http://qap.gotoacloud.top

C# ............. 212
来源：http://igy.0kj1m.cn

C .............. 30
来源：http://bbe.hysaishi.cn

C++ ............ 30
来源：http://aat.cucudq.cn

SQL ............ 90
来源：http://snv.gaohongyu789.top

Bash ........... 80
来源：http://uqf.nanxinkj.top

Kotlin ......... 15
来源：http://xmh.daria6918.cn

Swift .......... 15
来源：http://wmm.cucudq.cn

Lua ............ 10
来源：http://ejy.zhaomingkeji.xyz

Perl ........... 10
来源：http://vyl.hesvh.cn

Scala .......... 10
来源：http://qlv.dashuyun.cn

------------------------------------
来源：http://nia.zhoulong.xyz

合计 ........... 2106 条
来源：http://jpv.sysykeji.top

按章节统计：
来源：http://fqf.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://onb.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://csi.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wrh.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gkw.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://omf.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jfs.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xtl.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ejt.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ldv.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://owo.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tts.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mse.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tda.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kta.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lhg.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yya.sweek.top

Q SQL 专题                              90
来源：http://ajy.yanxiufei.cn

R Bash 专题                             80
来源：http://hdk.fktsv.cn

S C / C++ 专题                          60
来源：http://qoq.9152youxi.cn

T 其他语言补充                          60
来源：http://cmu.ivvv.top

U 高频实用片段                         120
来源：http://fyi.chenjidiqi.icu

------------------------------------
来源：http://okf.uphjek.com

合计                                  2106 条
来源：http://kvv.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://wuq.pengpengdd.cyou

使用提醒
来源：http://sgx.ivvv.top

--------------------------------------------------------------------------------
来源：http://kkn.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uey.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eyz.yueranfly.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oog.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yib.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wop.hesvh.cn

—— 文件结束 ——
来源：http://lzi.xingfuxueyuan.xyz

================================================================================
来源：http://uck.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://aur.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://wau.ppjwa.cn

================================================================================
来源：http://ikl.andypj.xyz

【收录内容】
来源：http://wdn.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://djh.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bfv.gzhubu.top

SQL · Bash · C · C++
来源：http://aqu.hcnkem.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fhr.sweek.top

【使用说明】
来源：http://sxw.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wjs.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wqw.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uws.ybcxt.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://arx.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hkx.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kkc.hammf.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://izi.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qrj.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iiq.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yfh.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lba.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ehy.aibaodan.cn

【文件统计】
来源：http://sls.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xcj.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://uyf.yuxming.cn

目  录
来源：http://bji.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://ywk.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wvr.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lzf.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gzs.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kui.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hmn.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fyf.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zjb.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gpy.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ujw.hfpthk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hwa.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gny.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tto.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ojy.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qqm.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://peo.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tge.snrcjt.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qms.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://exs.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://boe.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lqb.hcnkem.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ujm.jyoumei.cn

================================================================================
来源：http://zbv.tianlin.xyz

A. 基础语法与类型
来源：http://wfk.hammf.cn

================================================================================
来源：http://rtq.chenlongwang.top

[A01] Hello World
来源：http://vgk.zdbjq.cn

Py:   print("Hello, World!")
来源：http://rxt.ywan-chungtsiang.top

PHP:  echo "Hello, World!";
来源：http://dml.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://rin.zhoulong.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ojg.hongshengwenyu.top

Java: System.out.println("Hello, World!");
来源：http://mcv.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://fkx.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://xpr.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ied.zhixingplan.top

[A02] 变量声明与赋值
来源：http://gfg.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qpu.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qfm.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xbb.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xpz.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://hzr.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://kfc.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://xpc.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://azr.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://uek.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kjl.fzhhl.top

PHP:  const PI = 3.14159;
来源：http://bha.jianghu66.top

JS:   const PI = 3.14159;
来源：http://faa.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://hfe.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://enh.ehwqpu.com

Go:   const PI = 3.14159
来源：http://lzp.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://gng.havefunace.top

C#:   const double PI = 3.14159;
来源：http://ndm.chenzaomai.com

[A04] 判断变量类型
来源：http://qvu.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jtu.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tdw.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ndi.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://dzd.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yrf.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ibd.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jse.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://gue.yongpay.top

[A05] 整数除法与取模
来源：http://hzi.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wyx.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vqy.tanke756.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eoh.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ebc.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://evq.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://aof.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://fmz.meibo888.top

C#:   7 / 2; 7 % 2
来源：http://kpr.sysykeji.top

[A06] 字符串转数字
来源：http://eht.hysaishi.cn

Py:   int("42"); float("3.14")
来源：http://fnf.wangshuangyany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ujf.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eqm.nanxuanxn.top

TS:   parseInt("42", 10); Number("42")
来源：http://ecc.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zba.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zum.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qgz.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xbn.yonumen.top

[A07] 数字转字符串
来源：http://vwl.ydzc1.top

Py:   str(42)
来源：http://ugh.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://eqt.snrcjt.cn

JS:   String(42); (42).toString()
来源：http://qah.jinghuilouyu.cn

TS:   String(42)
来源：http://vyc.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mxg.yuxming.cn

Go:   strconv.Itoa(42)
来源：http://yea.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://ajz.sweek.top

C#:   42.ToString()
来源：http://ftq.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://xyh.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://spd.aizwys.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kue.gogol.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zlq.ybcxt.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ely.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://alz.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rdo.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hno.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://idw.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://pbs.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lty.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rgo.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sax.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://osc.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rsl.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dmw.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kde.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mpc.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://wii.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://wjd.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://xit.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://glw.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qkt.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://vxg.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tzh.jyoumei.cn

Ruby: rand(1..100)
来源：http://zxn.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://eur.yfazqb.com

[A11] 条件表达式（三元）
来源：http://dsv.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://mtu.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sru.redwolf501.top

JS:   x > 0 ? "yes" : "no"
来源：http://dgj.nanxuanxn.top

TS:   x > 0 ? "yes" : "no"
来源：http://rnm.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://hzw.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dcz.zhoulong.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://dlw.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://yse.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://gmv.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hpo.aibaodan.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://teu.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://hdx.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://aao.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://izm.nanxuanxn.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hrm.jqgufenzy.top

Ruby: "Hello, #{name}!"
来源：http://ign.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://jrn.tarul.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jpe.sxryk.cn

Py:   "第一行\n第二行"
来源：http://hvl.ppjwa.cn

PHP:  "第一行\n第二行"
来源：http://yum.wangshuangyany.cn

JS:   "第一行\n第二行"
来源：http://oon.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://gmc.andypj.xyz

Java: "第一行\n第二行"
来源：http://ptd.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://hfx.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://xak.nanxuanxn.top

C#:   "第一行\n第二行"
来源：http://fxc.xziqi.cn

[A14] 注释写法
来源：http://gbu.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://asd.havefunace.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zrq.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://equ.shanyushiyangtech.top


<!-- 参考信息 -->