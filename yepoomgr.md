代发 wailian999

[U85] JS：可选链
来源：http://mhc.yj20258.top

a?.b?.c
来源：http://vgi.daria6918.cn

[U86] JS：空值合并
来源：http://zxv.bbcook.cn

a ?? b
来源：http://ori.daria6918.cn

[U87] JS：解构默认值
来源：http://rmj.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://hat.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://szx.xuetiantiany.cn

{ ...a, ...b }
来源：http://rhr.hesvh.cn

[U89] JS：数组去重
来源：http://lcx.fehbvm.com

[...new Set(arr)]
来源：http://nwz.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://tzc.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://apo.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://cgc.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pry.bbcook.cn

[U92] JS：深拷贝
来源：http://pni.andypj.xyz

structuredClone(obj)
来源：http://imq.yj20258888.top

[U93] JS：模板字符串
来源：http://yxy.hywenlv.cn

`共 ${n} 条`
来源：http://okb.xylfe.cn

[U94] JS：箭头函数
来源：http://crr.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://ezd.52xcode.cn

[U95] JS：Promise 包装
来源：http://rjh.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://rbg.yonumen.top

[U96] JS：async/await 与异常
来源：http://ykg.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ozt.xinyue.icu

[U97] JS：并发请求
来源：http://edu.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rey.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://lkz.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xpg.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://poi.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://lhv.aibaodan.cn

[U100] JS：DOM 查询
来源：http://hfc.hfpthk.cn

document.querySelector(".item")
来源：http://vyj.yueranfly.top

[U101] JS：classList 操作
来源：http://qfa.yuanzhike.top

el.classList.toggle("active")
来源：http://qis.316326.xyz

[U102] JS：本地存储
来源：http://irk.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ebc.yangfankeji.com

[U103] JS：定时器
来源：http://fog.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qie.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://izq.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggy.316326.xyz

[U105] JS：节流
来源：http://zdx.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mco.bjfxy.top

[U106] JS：日期格式化
来源：http://tcb.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fhb.jyoumei.cn

[U107] JS：数字千分位
来源：http://xhx.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ccs.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://sjc.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://obh.9152youxi.cn

[U109] JS：数组分组
来源：http://tnl.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://huq.yueranfly.top

[U110] JS：数组分块
来源：http://cav.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gxf.yuanzhike.top

[U111] JS：对象转 Map
来源：http://lub.cqqwz.cn

new Map(Object.entries(obj))
来源：http://rps.xuanzx.com

[U112] JS：字符串补位
来源：http://zzj.andypj.xyz

"7".padStart(3, "0")
来源：http://fyj.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://han.c1oappe.top

s.replaceAll("a", "b")
来源：http://kfp.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://eop.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hia.gzhubu.top

[U115] JS：生成 UUID
来源：http://jwt.ehwqpu.com

crypto.randomUUID()
来源：http://tkl.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://awu.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://goo.fktsv.cn

[U117] JS：单元测试
来源：http://ztc.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://gwv.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://wow.cqqwz.cn

npm i -D vite;  npx vite
来源：http://vut.feifeiyinyue.top

[U119] JS：生产构建
来源：http://cgy.yonumen.top

npx vite build
来源：http://mlr.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://nji.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://lxi.gaohongyu789.top

================================================================================
来源：http://pdw.bbcook.cn

统计汇总
来源：http://atr.cdnleiting.top

================================================================================
来源：http://asu.yangfankeji.com

按语言统计（条）：
来源：http://lok.yangfankeji.com

Python ......... 252
来源：http://zpa.cheryme.top

PHP ............ 252
来源：http://uwc.xinyue.icu

JavaScript ..... 252
来源：http://asl.tanke756.top

TypeScript ..... 212
来源：http://gfu.tian-w.cn

Java ........... 212
来源：http://mki.jinqigfzy.top

Go ............. 212
来源：http://pij.chenlongwang.top

Ruby ........... 212
来源：http://pqy.hnxiangtu.top

C# ............. 212
来源：http://hzf.cucudq.cn

C .............. 30
来源：http://zsy.hywenlv.cn

C++ ............ 30
来源：http://ckl.ydjk.org.cn

SQL ............ 90
来源：http://eym.zhaomingkeji.xyz

Bash ........... 80
来源：http://oxl.cashguo.top

Kotlin ......... 15
来源：http://ldq.chenzaomai.com

Swift .......... 15
来源：http://tpy.fktsv.cn

Lua ............ 10
来源：http://jvu.yanxiufei.cn

Perl ........... 10
来源：http://inj.ywan-chungtsiang.top

Scala .......... 10
来源：http://ecw.cucudq.cn

------------------------------------
来源：http://qee.chenlongwang.top

合计 ........... 2106 条
来源：http://rwi.yanxiufei.cn

按章节统计：
来源：http://lok.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bie.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xuc.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oby.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kca.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lxh.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mfk.daxiang520.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jcl.zhijiandao.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hwy.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qjc.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bgt.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nfx.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://voj.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fbt.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sae.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tzc.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rjd.pengpengdd.cyou

Q SQL 专题                              90
来源：http://yaf.gaohongyu789.top

R Bash 专题                             80
来源：http://lxc.yongpay.top

S C / C++ 专题                          60
来源：http://yiu.zycfv.cn

T 其他语言补充                          60
来源：http://wod.cucudq.cn

U 高频实用片段                         120
来源：http://eld.c1oappe.top

------------------------------------
来源：http://xkm.cucudq.cn

合计                                  2106 条
来源：http://qmi.xylfe.cn

--------------------------------------------------------------------------------
来源：http://feo.dashuyun.cn

使用提醒
来源：http://aot.meibo888.top

--------------------------------------------------------------------------------
来源：http://wyu.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sqs.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qur.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://upi.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://igt.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nud.zycfv.cn

—— 文件结束 ——
来源：http://yls.zdqjudy.top

================================================================================
来源：http://pak.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://eqx.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://kwu.jinqigfzy.top

================================================================================
来源：http://ius.c1oappe.top

【收录内容】
来源：http://kmk.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mfj.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pad.sufxvd.cn

SQL · Bash · C · C++
来源：http://jsb.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aeo.hysaishi.cn

【使用说明】
来源：http://cxk.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://onc.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oss.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rzc.316326.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://idr.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://azh.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vdi.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mnn.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hvs.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pev.gotoacloud.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hne.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dzr.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://plu.jlsjyb.cn

【文件统计】
来源：http://jpp.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tfw.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://xzm.gaohongyu789.top

目  录
来源：http://tbk.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://zbs.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xaw.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zhv.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vqc.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lco.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vnk.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wdx.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://idw.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nsh.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lsx.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tju.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vzj.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zze.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ysd.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jwg.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tfj.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://azj.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jll.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sia.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://icv.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gvm.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dgr.chenlongwang.top

================================================================================
来源：http://trt.hnxiangtu.top

A. 基础语法与类型
来源：http://izz.kuanghao11.cn

================================================================================
来源：http://tvf.ppjwa.cn

[A01] Hello World
来源：http://zel.gzhubu.top

Py:   print("Hello, World!")
来源：http://gjc.cheryme.top

PHP:  echo "Hello, World!";
来源：http://nms.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://tny.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://knt.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://jrb.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://umr.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://mzr.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dei.tianlin.xyz

[A02] 变量声明与赋值
来源：http://lvg.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tam.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://liv.xylfe.cn

JS:   let name = "Alex"; const age = 20;
来源：http://siv.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://obs.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://nhp.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://cjx.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://hjh.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://wzz.guannengcc.top

[A03] 常量定义
来源：http://qvf.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yqe.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://det.uphjek.com

JS:   const PI = 3.14159;
来源：http://alt.yanxiufei.cn

TS:   const PI: number = 3.14159;
来源：http://zmj.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://ztm.cdnleiting.top

Go:   const PI = 3.14159
来源：http://vbf.hammf.cn

Ruby: PI = 3.14159
来源：http://fxm.ybcxt.top

C#:   const double PI = 3.14159;
来源：http://alr.nwbrower.top

[A04] 判断变量类型
来源：http://pdu.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ibs.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tnm.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qyl.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://lrh.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fnl.xinyue.icu

Go:   reflect.TypeOf(x).Name()
来源：http://qym.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tgb.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://eob.chenlongwang.top

[A05] 整数除法与取模
来源：http://ivj.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://asw.zhongyouzk.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lsb.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ljr.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uzp.yangfankeji.com

Java: 7 / 2; 7 % 2
来源：http://cor.sjlbkw.cn

Go:   7 / 2; 7 % 2
来源：http://rxp.jqgufenzy.top

Ruby: 7 / 2; 7 % 2
来源：http://dxq.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://cop.zdbjq.cn

[A06] 字符串转数字
来源：http://jlk.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://idx.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kwx.meibo888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lzu.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://zex.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qvy.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://scj.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://jha.aizwys.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sxt.ctjpmb.com

[A07] 数字转字符串
来源：http://ahn.0kj1m.cn

Py:   str(42)
来源：http://uui.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://dij.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://yjz.shuidangran.top

TS:   String(42)
来源：http://pkb.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eqm.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://box.sxryk.cn

Ruby: 42.to_s
来源：http://fqr.yueranfly.top

C#:   42.ToString()
来源：http://cmt.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://llu.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wgl.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nhm.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hxl.zhoulong.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jxn.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zsq.jqgufenzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bvd.quarkkingdee.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qts.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gsz.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://rho.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hoh.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xcs.daria6918.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dni.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gkl.52xcode.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uif.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uip.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mzu.tian-w.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cmz.yj20258.top

[A10] 生成随机数
来源：http://wjo.smart0.xyz

Py:   import random; random.randint(1, 100)
来源：http://taa.xinyue.icu

PHP:  random_int(1, 100);
来源：http://hqq.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dgs.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nqv.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://zik.316326.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nqx.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://mfm.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://vcy.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://tpy.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://cla.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lhq.yuanzhike.top

JS:   x > 0 ? "yes" : "no"
来源：http://mgx.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tbn.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://rhd.zdbjq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bmc.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xtk.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gnv.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://ikz.quarkkingdee.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zsu.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://diq.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://pqn.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://plx.ivvv.top

Java: "Hello, %s!".formatted(name)
来源：http://epx.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eih.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://sob.hongshengwenyu.top

C#:   $"Hello, {name}!"
来源：http://wwa.hammf.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://knb.tianlin.xyz

Py:   "第一行\n第二行"
来源：http://vpg.ctjpmb.com

PHP:  "第一行\n第二行"
来源：http://ska.tanke756.top

JS:   "第一行\n第二行"
来源：http://asa.c1oappe.top

TS:   "第一行\n第二行"
来源：http://bri.havefunace.top

Java: "第一行\n第二行"
来源：http://wsa.fktsv.cn

Go:   "第一行\n第二行"
来源：http://vcn.jlsjyb.cn

Ruby: "第一行\n第二行"
来源：http://drw.smart0.xyz

C#:   "第一行\n第二行"
来源：http://yei.zhijiandao.cn

[A14] 注释写法
来源：http://fox.nanxinkj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fbb.gotoacloud.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://oyf.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://lkn.cashguo.top


<!-- 参考信息 -->