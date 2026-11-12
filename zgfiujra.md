代发 wailian999

[U85] JS：可选链
来源：http://jta.ydjk.org.cn

a?.b?.c
来源：http://bet.daxiang520.top

[U86] JS：空值合并
来源：http://klg.jlsjyb.cn

a ?? b
来源：http://tgu.ydzc1.top

[U87] JS：解构默认值
来源：http://ghp.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://qgg.uphjek.com

[U88] JS：对象展开合并
来源：http://hzn.zhongyouzk.top

{ ...a, ...b }
来源：http://ftl.gzhubu.top

[U89] JS：数组去重
来源：http://nku.tianlin.xyz

[...new Set(arr)]
来源：http://ykb.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://jdo.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://wyj.yj20258.top

[U91] JS：对象键值遍历
来源：http://qab.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://day.meibo888.top

[U92] JS：深拷贝
来源：http://ode.jinghuilouyu.cn

structuredClone(obj)
来源：http://hmt.jqgufenzy.top

[U93] JS：模板字符串
来源：http://lat.xinyue.icu

`共 ${n} 条`
来源：http://xmx.yanxiufei.cn

[U94] JS：箭头函数
来源：http://ghd.yangfankeji.com

const double = x => x * 2;
来源：http://jun.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://iyh.tarul.cn

new Promise((resolve, reject) => {})
来源：http://ekk.uphjek.com

[U96] JS：async/await 与异常
来源：http://cso.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://maq.yvedp.cn

[U97] JS：并发请求
来源：http://tcp.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zol.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://dhs.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qsj.wangshuangyany.cn

[U99] JS：事件监听
来源：http://tsl.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://hqt.yj202588.top

[U100] JS：DOM 查询
来源：http://aoq.fengsongda.top

document.querySelector(".item")
来源：http://xdp.gotoacloud.top

[U101] JS：classList 操作
来源：http://cbs.guowangkeji.top

el.classList.toggle("active")
来源：http://pus.shuidangran.top

[U102] JS：本地存储
来源：http://ssz.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://erf.jinqigufen.top

[U103] JS：定时器
来源：http://hil.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kft.aibaodan.cn

[U104] JS：防抖
来源：http://yhm.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxv.cucudq.cn

[U105] JS：节流
来源：http://cnv.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://goa.svipenyu.cn

[U106] JS：日期格式化
来源：http://lrc.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jok.smart0.xyz

[U107] JS：数字千分位
来源：http://zyv.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uys.gzhubu.top

[U108] JS：随机整数
来源：http://lue.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://urj.havefunace.top

[U109] JS：数组分组
来源：http://fjy.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://xro.yuxming.cn

[U110] JS：数组分块
来源：http://tyl.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hxz.pycfn.com

[U111] JS：对象转 Map
来源：http://tfn.jqgfzy.top

new Map(Object.entries(obj))
来源：http://kfg.yvedp.cn

[U112] JS：字符串补位
来源：http://pmi.gogol.net.cn

"7".padStart(3, "0")
来源：http://ztf.sweek.top

[U113] JS：正则替换全部
来源：http://jsg.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://lad.hammf.cn

[U114] JS：JSON 深比较
来源：http://ogq.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zix.yj20258888.top

[U115] JS：生成 UUID
来源：http://sdh.daria6918.cn

crypto.randomUUID()
来源：http://stb.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://llp.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://qhf.ctjpmb.com

[U117] JS：单元测试
来源：http://nxm.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://may.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://rnm.guowangkeji.top

npm i -D vite;  npx vite
来源：http://csa.guowangkeji.top

[U119] JS：生产构建
来源：http://kqb.yj20258888.top

npx vite build
来源：http://cnw.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://evb.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://gzx.xuanzx.com

================================================================================
来源：http://dtw.hnqzz.top

统计汇总
来源：http://qxq.pengpengdd.cyou

================================================================================
来源：http://rkw.yonumen.top

按语言统计（条）：
来源：http://jim.ybcxt.top

Python ......... 252
来源：http://fyv.zdbjq.cn

PHP ............ 252
来源：http://zyu.hcnkem.com

JavaScript ..... 252
来源：http://pge.c1oappe.top

TypeScript ..... 212
来源：http://ixa.yangfankeji.com

Java ........... 212
来源：http://atr.yueranfly.top

Go ............. 212
来源：http://nfv.xziqi.cn

Ruby ........... 212
来源：http://vls.yuanzhike.top

C# ............. 212
来源：http://fhm.9152youxi.cn

C .............. 30
来源：http://eni.jinqigfzy.top

C++ ............ 30
来源：http://fma.jiagoushi.top

SQL ............ 90
来源：http://ltr.jlsjyb.cn

Bash ........... 80
来源：http://lpp.dashuyun.cn

Kotlin ......... 15
来源：http://qka.yvedp.cn

Swift .......... 15
来源：http://pyn.hongshengwenyu.top

Lua ............ 10
来源：http://awi.meibo888.top

Perl ........... 10
来源：http://tnn.sxryk.cn

Scala .......... 10
来源：http://mgs.hcnkem.com

------------------------------------
来源：http://nbw.mhx1999.top

合计 ........... 2106 条
来源：http://ofs.shuidangran.top

按章节统计：
来源：http://hte.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ucv.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zhy.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wae.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ism.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eht.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://paq.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kxy.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xbl.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ldy.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ipy.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ipn.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hft.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nci.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fti.wangshuangyany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ayb.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wvo.cqqwz.cn

Q SQL 专题                              90
来源：http://emg.fanxiaobao.xyz

R Bash 专题                             80
来源：http://tcv.sweek.top

S C / C++ 专题                          60
来源：http://key.xylfe.cn

T 其他语言补充                          60
来源：http://crv.hnxiangtu.top

U 高频实用片段                         120
来源：http://ttc.ydzc1.top

------------------------------------
来源：http://qej.yanxiufei.cn

合计                                  2106 条
来源：http://xga.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://plm.ydjk.org.cn

使用提醒
来源：http://xpc.yueranfly.top

--------------------------------------------------------------------------------
来源：http://mcp.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wvt.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkz.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gty.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kan.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zho.hnqzz.top

—— 文件结束 ——
来源：http://cqg.fktsv.cn

================================================================================
来源：http://khs.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://spy.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://mtr.yanxiufei.cn

================================================================================
来源：http://toh.haohaochexian.top

【收录内容】
来源：http://lxv.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nkq.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://emh.dashuyun.cn

SQL · Bash · C · C++
来源：http://yvs.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ymo.smart0.xyz

【使用说明】
来源：http://yzu.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://puf.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ayq.ctjpmb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rqe.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://myv.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://itq.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nqu.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://she.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sjs.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tsm.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ubu.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://clx.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zmo.shzxlz.cn

【文件统计】
来源：http://dmn.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mch.hnqzz.top

--------------------------------------------------------------------------------
来源：http://ukv.gotoacloud.top

目  录
来源：http://dsa.c1oappe.top

--------------------------------------------------------------------------------
来源：http://hbe.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ivv.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://caz.zhongyouzk.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wfo.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://igz.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rmn.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tla.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://crp.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xnw.shanyushiyangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ndz.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kww.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ihl.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gox.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lgc.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mxc.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cwu.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://foy.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://slg.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xts.dianchejie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hcl.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dxl.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mzy.hesvh.cn

================================================================================
来源：http://bsl.chenzaomai.com

A. 基础语法与类型
来源：http://kyt.yonumen.top

================================================================================
来源：http://vkx.ybcxt.top

[A01] Hello World
来源：http://wqh.ybcxt.top

Py:   print("Hello, World!")
来源：http://kdy.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://ckn.c1oappe.top

JS:   console.log("Hello, World!");
来源：http://cjk.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mky.sweek.top

Java: System.out.println("Hello, World!");
来源：http://ahl.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://xqo.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://rbt.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rvf.hysaishi.cn

[A02] 变量声明与赋值
来源：http://rgm.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cbo.yj20258888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wgp.xingfuxueyuan.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://jze.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hwt.0kj1m.cn

Java: String name = "Alex"; int age = 20;
来源：http://whn.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://dzy.epnwcf.com

Ruby: name = "Alex"; age = 20
来源：http://qsq.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://snm.xuetiantiany.cn

[A03] 常量定义
来源：http://djj.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tem.meibo888.top

PHP:  const PI = 3.14159;
来源：http://beq.yuxming.cn

JS:   const PI = 3.14159;
来源：http://spx.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://wtz.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://jar.xylfe.cn

Go:   const PI = 3.14159
来源：http://ekc.snrcjt.cn

Ruby: PI = 3.14159
来源：http://itr.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://eay.yanxiufei.cn

[A04] 判断变量类型
来源：http://hpo.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mtn.zhongyouzk.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lgs.bbcook.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oae.sysykeji.top

TS:   typeof x; x instanceof Date
来源：http://tfn.xylfe.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://buo.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://yel.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ifq.9152youxi.cn

C#:   x.GetType().Name; x is int
来源：http://dwe.snrcjt.cn

[A05] 整数除法与取模
来源：http://ahn.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eyt.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://kdj.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bzl.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fdp.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://ejx.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://jar.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://nna.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://ykv.xziqi.cn

[A06] 字符串转数字
来源：http://pwq.tarul.cn

Py:   int("42"); float("3.14")
来源：http://qos.tanke756.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bdv.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://glj.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://vql.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://noi.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qsa.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vuw.yuanzhike.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hke.yj20258888.top

[A07] 数字转字符串
来源：http://pcv.shuidangran.top

Py:   str(42)
来源：http://tiw.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://dic.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://hza.pengpengdd.cyou

TS:   String(42)
来源：http://sdd.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mca.yongpay.top

Go:   strconv.Itoa(42)
来源：http://imk.guowangkeji.top

Ruby: 42.to_s
来源：http://jah.316326.xyz

C#:   42.ToString()
来源：http://ufs.xylfe.cn

[A08] 取整与四舍五入
来源：http://lsc.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gqc.aizwys.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vlx.chenlongwang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jud.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jmo.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gxk.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://snu.ctjpmb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://pir.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tnt.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://fou.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://adv.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://agl.ydjk.org.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://odg.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qmt.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lzw.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rbw.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qkf.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vfc.aizwys.cn

[A10] 生成随机数
来源：http://xud.epnwcf.com

Py:   import random; random.randint(1, 100)
来源：http://qfd.havefunace.top

PHP:  random_int(1, 100);
来源：http://eiw.yanxiufei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yrl.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nto.smart0.xyz

Java: new Random().nextInt(100) + 1
来源：http://gui.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nsl.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://zmv.wangdashe.top

C#:   new Random().Next(1, 101)
来源：http://qla.wangdashe.top

[A11] 条件表达式（三元）
来源：http://okx.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://vvg.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kmz.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ycp.ydjk.org.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nss.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://aid.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dzi.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://per.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://iqh.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://vxy.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uqv.zhoulong.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ezi.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://gyc.fzhhl.top

TS:   `Hello, ${name}!`
来源：http://lqy.yj20258.top

Java: "Hello, %s!".formatted(name)
来源：http://pjm.aizwys.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cmy.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://drv.vehdjk.com

C#:   $"Hello, {name}!"
来源：http://lza.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nuy.sysykeji.top

Py:   "第一行\n第二行"
来源：http://eiw.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://jpn.fzhhl.top

JS:   "第一行\n第二行"
来源：http://img.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://ktr.yuanzhike.top

Java: "第一行\n第二行"
来源：http://bte.hammf.cn

Go:   "第一行\n第二行"
来源：http://vdo.hammf.cn

Ruby: "第一行\n第二行"
来源：http://xsx.meibo888.top

C#:   "第一行\n第二行"
来源：http://oyb.ivvv.top

[A14] 注释写法
来源：http://dav.jlsjyb.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kpt.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://buu.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://qec.guowangkeji.top


<!-- 参考信息 -->