代发 wailian999

[U85] JS：可选链
来源：http://sbw.fehbvm.com

a?.b?.c
来源：http://fja.hongshengwenyu.top

[U86] JS：空值合并
来源：http://uun.sxryk.cn

a ?? b
来源：http://ide.bbcook.cn

[U87] JS：解构默认值
来源：http://nta.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://ilw.smart0.xyz

[U88] JS：对象展开合并
来源：http://xfi.sxryk.cn

{ ...a, ...b }
来源：http://yar.shangyingyoupin.top

[U89] JS：数组去重
来源：http://vjf.jinqigfzy.top

[...new Set(arr)]
来源：http://adt.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://utt.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://fsm.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://qzu.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tsm.hnxiangtu.top

[U92] JS：深拷贝
来源：http://vbp.yfazqb.com

structuredClone(obj)
来源：http://cap.fzhhl.top

[U93] JS：模板字符串
来源：http://xwr.tanke756.top

`共 ${n} 条`
来源：http://xjd.yj20258888.top

[U94] JS：箭头函数
来源：http://mhi.jianghu66.top

const double = x => x * 2;
来源：http://lun.gogol.net.cn

[U95] JS：Promise 包装
来源：http://txk.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://boy.xuanzx.com

[U96] JS：async/await 与异常
来源：http://pci.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fky.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://ybj.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://vko.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://eid.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dge.smart0.xyz

[U99] JS：事件监听
来源：http://kis.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://qck.tanke756.top

[U100] JS：DOM 查询
来源：http://tlp.nanxinkj.top

document.querySelector(".item")
来源：http://rmw.cqqwz.cn

[U101] JS：classList 操作
来源：http://okh.aibaodan.cn

el.classList.toggle("active")
来源：http://ams.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://zea.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qvi.c1oappe.top

[U103] JS：定时器
来源：http://qkq.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pfg.pycfn.com

[U104] JS：防抖
来源：http://xvh.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vir.nwbrower.top

[U105] JS：节流
来源：http://tzk.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vzo.gogol.net.cn

[U106] JS：日期格式化
来源：http://qcx.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aer.guannengcc.top

[U107] JS：数字千分位
来源：http://abl.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bws.cheryme.top

[U108] JS：随机整数
来源：http://zhn.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dzc.shzxlz.cn

[U109] JS：数组分组
来源：http://poq.nwbrower.top

Object.groupBy(arr, x => x.type)
来源：http://zdb.c1oappe.top

[U110] JS：数组分块
来源：http://tmv.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://suz.shzxlz.cn

[U111] JS：对象转 Map
来源：http://awl.cqqwz.cn

new Map(Object.entries(obj))
来源：http://mxo.ppjwa.cn

[U112] JS：字符串补位
来源：http://kui.xuanzx.com

"7".padStart(3, "0")
来源：http://pkg.0kj1m.cn

[U113] JS：正则替换全部
来源：http://kvh.fengsongda.top

s.replaceAll("a", "b")
来源：http://inm.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://dho.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://iur.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://wpi.yvedp.cn

crypto.randomUUID()
来源：http://ngn.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://etm.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://yyn.daria6918.cn

[U117] JS：单元测试
来源：http://nul.zhiwuduotai.top

npm i -D vitest;  npx vitest
来源：http://mrj.sweek.top

[U118] JS：开发服务器
来源：http://jtc.uphjek.com

npm i -D vite;  npx vite
来源：http://kym.ybcxt.top

[U119] JS：生产构建
来源：http://fiz.shzxlz.cn

npx vite build
来源：http://kxt.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vlf.hywenlv.cn

import.meta.env.VITE_API_URL
来源：http://qve.tianlin.xyz

================================================================================
来源：http://lij.yj202588.top

统计汇总
来源：http://frg.xingfuxueyuan.xyz

================================================================================
来源：http://bnc.xylfe.cn

按语言统计（条）：
来源：http://fwy.tian-w.cn

Python ......... 252
来源：http://cst.jlsjyb.cn

PHP ............ 252
来源：http://nuw.meibo888.top

JavaScript ..... 252
来源：http://tjl.jinqigfzy.top

TypeScript ..... 212
来源：http://okj.ctjpmb.com

Java ........... 212
来源：http://wnu.smart0.xyz

Go ............. 212
来源：http://xnf.shanyushiyangtech.top

Ruby ........... 212
来源：http://kvq.ywan-chungtsiang.top

C# ............. 212
来源：http://cfe.gogol.net.cn

C .............. 30
来源：http://hkr.zhoulong.xyz

C++ ............ 30
来源：http://wcb.havefunace.top

SQL ............ 90
来源：http://aqk.jinyuanbaomall.cn

Bash ........... 80
来源：http://ztf.yuanzhike.top

Kotlin ......... 15
来源：http://lea.zhijiandao.cn

Swift .......... 15
来源：http://ify.shangyingyoupin.top

Lua ............ 10
来源：http://wtc.jinqigufen.top

Perl ........... 10
来源：http://fwk.yanxiufei.cn

Scala .......... 10
来源：http://ari.sysykeji.top

------------------------------------
来源：http://blb.ivvv.top

合计 ........... 2106 条
来源：http://uwy.316326.xyz

按章节统计：
来源：http://bfo.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fnx.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://obj.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://elz.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wim.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://muy.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tpk.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xhk.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mqk.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kvs.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ypc.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pee.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qhq.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kzo.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kbb.yj20258888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://stz.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yeb.tian-w.cn

Q SQL 专题                              90
来源：http://kye.yongpay.top

R Bash 专题                             80
来源：http://aii.xuanzx.com

S C / C++ 专题                          60
来源：http://nup.smart0.xyz

T 其他语言补充                          60
来源：http://wta.jqgfzy.top

U 高频实用片段                         120
来源：http://uqx.dashuyun.cn

------------------------------------
来源：http://tpz.wangdashe.top

合计                                  2106 条
来源：http://ahk.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ruk.shanyushiyangtech.top

使用提醒
来源：http://wpf.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://zpj.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ivr.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ddv.aibaodan.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mbc.jiagoushi.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vum.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://con.hnqzz.top

—— 文件结束 ——
来源：http://svv.jyoumei.cn

================================================================================
来源：http://eby.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://dnh.cashguo.top

Common Programming Examples Cheat Book
来源：http://uzc.hfpthk.cn

================================================================================
来源：http://kaj.aibaodan.cn

【收录内容】
来源：http://vek.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hrc.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aoo.jianghu66.top

SQL · Bash · C · C++
来源：http://ygi.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pmw.chenlongwang.top

【使用说明】
来源：http://zwt.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://edn.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tqz.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://udm.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ftt.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mzg.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ebo.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://njg.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wtx.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ujl.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pio.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://foj.hfpthk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xuh.vqdsnc.cn

【文件统计】
来源：http://dpr.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nrn.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ylt.chenzaomai.com

目  录
来源：http://pbj.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://zil.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://drv.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cyu.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dfq.gaohongyu789.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ohn.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ref.ywan-chungtsiang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rul.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pxy.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ase.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lvx.meibo888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zim.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rfh.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://etd.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://exb.yangfankeji.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dku.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dts.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gmy.snrcjt.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://edy.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://shh.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wru.zhixingplan.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zaz.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lbw.jyoumei.cn

================================================================================
来源：http://vzk.nwbrower.top

A. 基础语法与类型
来源：http://qqa.jqgfzy.top

================================================================================
来源：http://pzz.yj20258888.top

[A01] Hello World
来源：http://vss.pycfn.com

Py:   print("Hello, World!")
来源：http://mij.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://otb.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://byy.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wdz.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://xfm.fktsv.cn

Go:   fmt.Println("Hello, World!")
来源：http://twq.yj20258888.top

Ruby: puts "Hello, World!"
来源：http://gdi.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://nqn.tarul.cn

[A02] 变量声明与赋值
来源：http://mey.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rsy.sjlbkw.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ucl.bbcook.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fig.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rvf.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://wxh.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://snp.gzhubu.top

Ruby: name = "Alex"; age = 20
来源：http://jfx.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ljy.sxryk.cn

[A03] 常量定义
来源：http://ota.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mxs.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://yqq.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://vgz.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://nvd.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://uoz.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://wnd.yj20258888.top

Ruby: PI = 3.14159
来源：http://zfc.xziqi.cn

C#:   const double PI = 3.14159;
来源：http://how.ppjwa.cn

[A04] 判断变量类型
来源：http://iyg.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rad.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uvc.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qvk.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://eyd.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kba.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://lcu.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://fav.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://xii.yvedp.cn

[A05] 整数除法与取模
来源：http://ley.sxryk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dof.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://vyf.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ebz.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jgl.gzhubu.top

Java: 7 / 2; 7 % 2
来源：http://cxj.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://gma.iojbl.cn

Ruby: 7 / 2; 7 % 2
来源：http://tyk.daria6918.cn

C#:   7 / 2; 7 % 2
来源：http://tye.sjlbkw.cn

[A06] 字符串转数字
来源：http://zna.bjfxy.top

Py:   int("42"); float("3.14")
来源：http://wou.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cxm.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zft.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://hrb.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ych.meibo888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mru.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://msg.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rnc.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://qhl.gotoacloud.top

Py:   str(42)
来源：http://ozy.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://tfn.jinyuanbaomall.cn

JS:   String(42); (42).toString()
来源：http://zja.fehbvm.com

TS:   String(42)
来源：http://lea.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://duw.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://wpj.guannengcc.top

Ruby: 42.to_s
来源：http://esz.cqqwz.cn

C#:   42.ToString()
来源：http://ylk.hywenlv.cn

[A08] 取整与四舍五入
来源：http://epo.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yvl.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dwc.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zln.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jhn.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qkm.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jhj.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gos.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sfd.nanxuanxn.top

[A09] 绝对值与最大最小值
来源：http://tti.dashuyun.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://koa.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jht.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://olk.cashguo.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rod.xinyue.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cps.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://abw.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://krv.vehdjk.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://prw.yuxming.cn

[A10] 生成随机数
来源：http://heh.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://wlp.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://vdf.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tnw.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ynx.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://int.gogol.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tej.yvedp.cn

Ruby: rand(1..100)
来源：http://vyh.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://cwe.hesvh.cn

[A11] 条件表达式（三元）
来源：http://gyj.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://clt.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://btt.jqgfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://rrh.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://gfq.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://epk.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hea.tanke756.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rbr.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://gwv.xuanzx.com

[A12] 字符串插值 / 格式化
来源：http://mcg.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://whl.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yrq.nanxinkj.top

JS:   `Hello, ${name}!`
来源：http://kdn.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://oql.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://nsy.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://omw.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://mix.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://ruu.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pft.tian-w.cn

Py:   "第一行\n第二行"
来源：http://wsd.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://azh.yueranfly.top

JS:   "第一行\n第二行"
来源：http://vgm.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://tzc.52xcode.cn

Java: "第一行\n第二行"
来源：http://yjv.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://zir.shanyushiyangkeji.top

Ruby: "第一行\n第二行"
来源：http://dlk.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://dga.uphjek.com

[A14] 注释写法
来源：http://fcu.fengsongda.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mtl.yuanzhike.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qai.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://oxo.epnwcf.com


<!-- 参考信息 -->