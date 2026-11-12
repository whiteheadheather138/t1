代发 wailian999

[U87] JS：解构默认值
来源：http://imw.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://mpn.ppjwa.cn

[U88] JS：对象展开合并
来源：http://xnk.vehdjk.com

{ ...a, ...b }
来源：http://gsk.sjlbkw.cn

[U89] JS：数组去重
来源：http://nvn.zdqjudy.top

[...new Set(arr)]
来源：http://dmx.jianghu66.top

[U90] JS：数字数组排序
来源：http://qek.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://vtm.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://ofb.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oxc.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://kas.nanxinkj.top

structuredClone(obj)
来源：http://nqv.ehwqpu.com

[U93] JS：模板字符串
来源：http://bed.snrcjt.cn

`共 ${n} 条`
来源：http://qfz.zhijiandao.cn

[U94] JS：箭头函数
来源：http://rvq.zdqjudy.top

const double = x => x * 2;
来源：http://ngn.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://duv.yj20258.top

new Promise((resolve, reject) => {})
来源：http://glu.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://ssz.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cpq.havefunace.top

[U97] JS：并发请求
来源：http://nnb.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iae.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://pcs.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ncq.ydjk.org.cn

[U99] JS：事件监听
来源：http://zup.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://ciy.316326.xyz

[U100] JS：DOM 查询
来源：http://mhx.tarul.cn

document.querySelector(".item")
来源：http://mmy.uphjek.com

[U101] JS：classList 操作
来源：http://knn.redwolf501.top

el.classList.toggle("active")
来源：http://gfz.ybcxt.top

[U102] JS：本地存储
来源：http://iwh.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://cuz.yongpay.top

[U103] JS：定时器
来源：http://rsp.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://obp.yanxiufei.cn

[U104] JS：防抖
来源：http://lgx.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvw.xziqi.cn

[U105] JS：节流
来源：http://kcj.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mxb.hnxiangtu.top

[U106] JS：日期格式化
来源：http://zvn.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lil.ctjpmb.com

[U107] JS：数字千分位
来源：http://edc.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cta.cucudq.cn

[U108] JS：随机整数
来源：http://uan.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fhb.redwolf501.top

[U109] JS：数组分组
来源：http://nzn.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://wqp.gogol.net.cn

[U110] JS：数组分块
来源：http://zqt.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gmt.dianchejie.cn

[U111] JS：对象转 Map
来源：http://egj.gzhubu.top

new Map(Object.entries(obj))
来源：http://eph.cashguo.top

[U112] JS：字符串补位
来源：http://mkk.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://ecn.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://jld.yj20258.top

s.replaceAll("a", "b")
来源：http://bur.316326.xyz

[U114] JS：JSON 深比较
来源：http://egj.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xkz.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://rif.cashguo.top

crypto.randomUUID()
来源：http://jai.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://bmm.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://qrr.chenzaomai.com

[U117] JS：单元测试
来源：http://eri.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://dtr.guowangkeji.top

[U118] JS：开发服务器
来源：http://eam.xylfe.cn

npm i -D vite;  npx vite
来源：http://nhr.hesvh.cn

[U119] JS：生产构建
来源：http://kia.gzhubu.top

npx vite build
来源：http://gxb.bbcook.cn

[U120] JS：读取环境变量（Vite）
来源：http://inr.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://oev.xinyue.icu

================================================================================
来源：http://wlz.yanxiufei.cn

统计汇总
来源：http://uyb.pycfn.com

================================================================================
来源：http://vsj.hywenlv.cn

按语言统计（条）：
来源：http://cxa.cheryme.top

Python ......... 252
来源：http://lnm.chenlongwang.top

PHP ............ 252
来源：http://nff.yanxiufei.cn

JavaScript ..... 252
来源：http://aux.yonumen.top

TypeScript ..... 212
来源：http://bge.zhaomingkeji.xyz

Java ........... 212
来源：http://add.zdbjq.cn

Go ............. 212
来源：http://wxo.sjlbkw.cn

Ruby ........... 212
来源：http://vdd.zycfv.cn

C# ............. 212
来源：http://uyu.jlsjyb.cn

C .............. 30
来源：http://iwc.haohaochexian.top

C++ ............ 30
来源：http://gpl.cashguo.top

SQL ............ 90
来源：http://mxm.ydjk.org.cn

Bash ........... 80
来源：http://zwc.nanxinkj.top

Kotlin ......... 15
来源：http://hqm.bbcook.cn

Swift .......... 15
来源：http://mcj.nanxinkj.top

Lua ............ 10
来源：http://vie.yj202588.top

Perl ........... 10
来源：http://oek.cucudq.cn

Scala .......... 10
来源：http://wma.zhijiandao.cn

------------------------------------
来源：http://bpd.tianlin.xyz

合计 ........... 2106 条
来源：http://sdy.cucudq.cn

按章节统计：
来源：http://ims.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bno.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dto.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jym.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lpp.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dim.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gsz.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vyf.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://inv.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xnm.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gyl.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hiv.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://app.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kfw.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vdu.yj20258.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jry.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vzg.yj20258888.top

Q SQL 专题                              90
来源：http://ysr.tian-w.cn

R Bash 专题                             80
来源：http://eqr.fktsv.cn

S C / C++ 专题                          60
来源：http://srm.hammf.cn

T 其他语言补充                          60
来源：http://ipb.dianchejie.cn

U 高频实用片段                         120
来源：http://qzj.tian-w.cn

------------------------------------
来源：http://kmb.ydjk.org.cn

合计                                  2106 条
来源：http://ewd.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://apc.snrcjt.cn

使用提醒
来源：http://yju.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://hdg.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ewo.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://akw.redwolf501.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zwu.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zkd.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://upz.nwbrower.top

—— 文件结束 ——
来源：http://zwi.9152youxi.cn

================================================================================
来源：http://qdh.zdqjudy.top

程序语言常见例子速查手册（2024 版）
来源：http://vnh.yj20258888.top

Common Programming Examples Cheat Book
来源：http://atg.yuanzhike.top

================================================================================
来源：http://bnb.sweek.top

【收录内容】
来源：http://hpl.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bzn.daxiang520.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jza.zhijiandao.cn

SQL · Bash · C · C++
来源：http://tis.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pfq.hcnkem.com

【使用说明】
来源：http://qek.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://img.shanyushiyangtech.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xma.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hrv.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://acu.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://vfs.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cra.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lvq.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sok.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wrz.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tue.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zgl.fanxiaobao.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pyc.tianlin.xyz

【文件统计】
来源：http://mvg.kuanghao11.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pcx.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://mvc.hnqzz.top

目  录
来源：http://ays.xziqi.cn

--------------------------------------------------------------------------------
来源：http://bpd.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oxa.aibaodan.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ixu.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kaq.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ubr.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://acb.dianchejie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lyb.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fij.ehwqpu.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://odp.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pmq.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ume.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pqj.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://odi.9152youxi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mke.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rfy.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pqb.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oli.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kze.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://gwe.nanxinkj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fcb.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hal.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://njw.jinqigfzy.top

================================================================================
来源：http://kyf.jinghuilouyu.cn

A. 基础语法与类型
来源：http://ysg.0kj1m.cn

================================================================================
来源：http://tbf.shangyingyoupin.top

[A01] Hello World
来源：http://cma.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://sem.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://kzc.cheryme.top

JS:   console.log("Hello, World!");
来源：http://toc.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fxu.yj20258888.top

Java: System.out.println("Hello, World!");
来源：http://lbx.sweek.top

Go:   fmt.Println("Hello, World!")
来源：http://dyh.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://olg.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wur.jqgufenzy.top

[A02] 变量声明与赋值
来源：http://udb.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hte.316326.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ebj.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://drc.gotoacloud.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zmj.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://wwz.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://wga.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://vzk.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://mnf.yj20258888.top

[A03] 常量定义
来源：http://upn.ehwqpu.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xua.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://jqa.yongpay.top

JS:   const PI = 3.14159;
来源：http://cvi.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://wvv.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://sxe.guowangkeji.top

Go:   const PI = 3.14159
来源：http://xjr.aibaodan.cn

Ruby: PI = 3.14159
来源：http://yvd.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://osi.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://mnc.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ofg.yuanzhike.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ghr.ivvv.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pyr.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://xbq.tarul.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wih.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ecp.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wiw.snrcjt.cn

C#:   x.GetType().Name; x is int
来源：http://xhk.fehbvm.com

[A05] 整数除法与取模
来源：http://lek.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://doq.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ned.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hbe.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ejv.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://pbv.zdqjudy.top

Go:   7 / 2; 7 % 2
来源：http://vuq.nanxuanxn.top

Ruby: 7 / 2; 7 % 2
来源：http://ljr.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://zub.guowangkeji.top

[A06] 字符串转数字
来源：http://yus.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://wcv.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://izy.xylfe.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eop.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rat.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rxs.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fba.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://daz.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gaq.xylfe.cn

[A07] 数字转字符串
来源：http://jbq.yuanzhike.top

Py:   str(42)
来源：http://eks.316326.xyz

PHP:  (string) 42; strval(42)
来源：http://cuq.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://fdf.hongshengwenyu.top

TS:   String(42)
来源：http://koj.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sbg.shuidangran.top

Go:   strconv.Itoa(42)
来源：http://xda.ivvv.top

Ruby: 42.to_s
来源：http://plt.ydzc1.top

C#:   42.ToString()
来源：http://ljx.jiagoushi.top

[A08] 取整与四舍五入
来源：http://wal.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dts.dashuyun.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mgc.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://niz.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cfb.redwolf501.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fkq.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hjr.chenlongwang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fgs.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wgz.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://dpe.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hjj.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sdk.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oua.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nuy.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://czj.zdqjudy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cxk.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xam.nwbrower.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qxi.gogol.net.cn

[A10] 生成随机数
来源：http://ahi.shanyushiyangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://euv.xuanzx.com

PHP:  random_int(1, 100);
来源：http://vhn.vehdjk.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rqm.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jzz.ctjpmb.com

Java: new Random().nextInt(100) + 1
来源：http://sjd.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://myg.jyoumei.cn

Ruby: rand(1..100)
来源：http://sbk.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://nkp.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://acu.ctjpmb.com

Py:   "yes" if x > 0 else "no"
来源：http://vgf.vehdjk.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://mzo.redwolf501.top

JS:   x > 0 ? "yes" : "no"
来源：http://vzz.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://pth.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://zmj.ydzc1.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bvs.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gej.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://jdu.hysaishi.cn

[A12] 字符串插值 / 格式化
来源：http://nrr.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fgq.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ajj.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://ryy.yj20258.top

TS:   `Hello, ${name}!`
来源：http://hlv.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://hhg.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pdm.hcnkem.com

Ruby: "Hello, #{name}!"
来源：http://slz.sweek.top

C#:   $"Hello, {name}!"
来源：http://qsc.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mrn.redwolf501.top

Py:   "第一行\n第二行"
来源：http://xmf.bjfxy.top

PHP:  "第一行\n第二行"
来源：http://rji.fehbvm.com

JS:   "第一行\n第二行"
来源：http://rbb.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://thm.jianghu66.top

Java: "第一行\n第二行"
来源：http://cot.redwolf501.top

Go:   "第一行\n第二行"
来源：http://bfm.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://goz.epnwcf.com

C#:   "第一行\n第二行"
来源：http://jby.fehbvm.com

[A14] 注释写法
来源：http://awy.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://acr.fengsongda.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://not.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://ftw.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://ncb.fzhhl.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gpj.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://ghi.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://krf.nanxuanxn.top


<!-- 参考信息 -->