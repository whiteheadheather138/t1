代发 wailian999

[U89] JS：数组去重
来源：http://smm.aibaodan.cn

[...new Set(arr)]
来源：http://ntm.tanke756.top

[U90] JS：数字数组排序
来源：http://nnc.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://yag.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://ysz.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lzw.shzxlz.cn

[U92] JS：深拷贝
来源：http://otw.sysykeji.top

structuredClone(obj)
来源：http://vsm.ydzc1.top

[U93] JS：模板字符串
来源：http://ebk.zdbjq.cn

`共 ${n} 条`
来源：http://azd.smart0.xyz

[U94] JS：箭头函数
来源：http://bod.zhijiandao.cn

const double = x => x * 2;
来源：http://dzr.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://rpc.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://nqc.xylfe.cn

[U96] JS：async/await 与异常
来源：http://suw.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yxs.daxiang520.top

[U97] JS：并发请求
来源：http://uwq.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://sbz.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://kkr.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zmg.hcnkem.com

[U99] JS：事件监听
来源：http://qmt.shuidangran.top

el.addEventListener("click", e => {})
来源：http://qbd.xylfe.cn

[U100] JS：DOM 查询
来源：http://vck.jinqigufen.top

document.querySelector(".item")
来源：http://ysd.nwbrower.top

[U101] JS：classList 操作
来源：http://dqi.dianchejie.cn

el.classList.toggle("active")
来源：http://rbx.sxryk.cn

[U102] JS：本地存储
来源：http://wln.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jfl.jiagoushi.top

[U103] JS：定时器
来源：http://jhr.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wqs.jinqigfzy.top

[U104] JS：防抖
来源：http://ttt.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ced.dashuyun.cn

[U105] JS：节流
来源：http://pdz.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ybw.gogol.net.cn

[U106] JS：日期格式化
来源：http://aav.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vbc.snrcjt.cn

[U107] JS：数字千分位
来源：http://cmn.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ekg.hongshengwenyu.top

[U108] JS：随机整数
来源：http://nfy.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cko.gaohongyu789.top

[U109] JS：数组分组
来源：http://pgh.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://fpj.zycfv.cn

[U110] JS：数组分块
来源：http://wnp.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cwp.chenlongwang.top

[U111] JS：对象转 Map
来源：http://hvn.zycfv.cn

new Map(Object.entries(obj))
来源：http://zut.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://nqr.fehbvm.com

"7".padStart(3, "0")
来源：http://lgs.fehbvm.com

[U113] JS：正则替换全部
来源：http://mzl.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://cco.yfazqb.com

[U114] JS：JSON 深比较
来源：http://esm.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://jcz.hcnkem.com

[U115] JS：生成 UUID
来源：http://kqn.0kj1m.cn

crypto.randomUUID()
来源：http://fac.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://mwe.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://mvk.redwolf501.top

[U117] JS：单元测试
来源：http://zkg.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://hqp.jqgufenzy.top

[U118] JS：开发服务器
来源：http://vko.cucudq.cn

npm i -D vite;  npx vite
来源：http://ybn.gaohongyu789.top

[U119] JS：生产构建
来源：http://gnk.nanxuanxn.top

npx vite build
来源：http://swj.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://cuq.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://dmn.cdnleiting.top

================================================================================
来源：http://jvt.gzhubu.top

统计汇总
来源：http://aid.jinqigufen.top

================================================================================
来源：http://eyo.zhijiandao.cn

按语言统计（条）：
来源：http://fni.redwolf501.top

Python ......... 252
来源：http://fkx.yongpay.top

PHP ............ 252
来源：http://tmt.yj20258.top

JavaScript ..... 252
来源：http://krf.hfpthk.cn

TypeScript ..... 212
来源：http://qsg.jinqigufen.top

Java ........... 212
来源：http://qsl.xziqi.cn

Go ............. 212
来源：http://bmp.gzhubu.top

Ruby ........... 212
来源：http://uhe.cheryme.top

C# ............. 212
来源：http://lfl.ydzc1.top

C .............. 30
来源：http://xft.jyoumei.cn

C++ ............ 30
来源：http://xik.ctjpmb.com

SQL ............ 90
来源：http://jce.mhx1999.top

Bash ........... 80
来源：http://ktj.smart0.xyz

Kotlin ......... 15
来源：http://old.ywan-chungtsiang.top

Swift .......... 15
来源：http://dee.cheryme.top

Lua ............ 10
来源：http://pts.hysaishi.cn

Perl ........... 10
来源：http://pje.jinqigfzy.top

Scala .......... 10
来源：http://tok.zycfv.cn

------------------------------------
来源：http://mtf.fzhhl.top

合计 ........... 2106 条
来源：http://dmx.hongshengwenyu.top

按章节统计：
来源：http://grl.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://odj.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ngq.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zoc.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://czb.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qxl.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hpt.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qzl.wangshuangyany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kgl.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://arr.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aym.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wzj.hywenlv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pnj.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hhg.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zjk.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jeg.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wdz.52xcode.cn

Q SQL 专题                              90
来源：http://byp.daria6918.cn

R Bash 专题                             80
来源：http://mtn.hammf.cn

S C / C++ 专题                          60
来源：http://nvk.haohaochexian.top

T 其他语言补充                          60
来源：http://qli.hongshengwenyu.top

U 高频实用片段                         120
来源：http://uwq.smart0.xyz

------------------------------------
来源：http://och.ctjpmb.com

合计                                  2106 条
来源：http://jbq.cashguo.top

--------------------------------------------------------------------------------
来源：http://txj.sufxvd.cn

使用提醒
来源：http://dgz.tanke756.top

--------------------------------------------------------------------------------
来源：http://fid.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gky.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xov.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jfb.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dtn.zhongyouzk.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zvq.ctjpmb.com

—— 文件结束 ——
来源：http://wjn.shanyushiyangkeji.top

================================================================================
来源：http://ftx.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://xzk.jinghuilouyu.cn

Common Programming Examples Cheat Book
来源：http://ylv.xinyue.icu

================================================================================
来源：http://mxl.zhiwuduotai.top

【收录内容】
来源：http://fzx.xingfuxueyuan.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://yew.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jhr.dianchejie.cn

SQL · Bash · C · C++
来源：http://fju.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zqj.tarul.cn

【使用说明】
来源：http://iqv.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://epw.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jvn.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://phs.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fnv.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zki.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lvl.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iyg.zdqjudy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cko.sweek.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qdz.yfazqb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://upw.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rod.c1oappe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ska.yj20258888.top

【文件统计】
来源：http://pms.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jrs.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://jod.zdqjudy.top

目  录
来源：http://ufg.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://cnv.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mig.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uig.andypj.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://htp.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xtv.yvedp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hxq.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://anv.shuidangran.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zyz.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dne.tian-w.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://thq.sjlbkw.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rmk.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nwu.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ggv.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ntg.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gez.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vau.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://olf.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fwk.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wix.wangshuangyany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://edm.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ioo.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://deg.shanyushiyangkeji.top

================================================================================
来源：http://gkd.jinghuilouyu.cn

A. 基础语法与类型
来源：http://xkr.hywenlv.cn

================================================================================
来源：http://hvt.jinghuilouyu.cn

[A01] Hello World
来源：http://lnb.9152youxi.cn

Py:   print("Hello, World!")
来源：http://unn.fengsongda.top

PHP:  echo "Hello, World!";
来源：http://slh.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://vyk.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cmq.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://hbr.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://xfu.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://zht.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mnn.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://ygf.chenjidiqi.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ldk.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://xby.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yqi.52xcode.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gvt.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://qtn.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://qro.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://ubv.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ata.jinghuilouyu.cn

[A03] 常量定义
来源：http://dhm.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ivh.yuanzhike.top

PHP:  const PI = 3.14159;
来源：http://uyc.zycfv.cn

JS:   const PI = 3.14159;
来源：http://oxr.zhaomingkeji.xyz

TS:   const PI: number = 3.14159;
来源：http://fsk.hfpthk.cn

Java: static final double PI = 3.14159;
来源：http://hwj.yongpay.top

Go:   const PI = 3.14159
来源：http://fuw.tanke756.top

Ruby: PI = 3.14159
来源：http://coq.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://swg.jyoumei.cn

[A04] 判断变量类型
来源：http://wod.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nnn.jinyuanbaomall.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://elf.cheryme.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cmp.52xcode.cn

TS:   typeof x; x instanceof Date
来源：http://xwg.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://psz.chenlongwang.top

Go:   reflect.TypeOf(x).Name()
来源：http://wvn.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yod.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://kuz.chenlongwang.top

[A05] 整数除法与取模
来源：http://zcc.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rft.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://tye.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gpj.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jvr.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://rmn.chenjidiqi.icu

Go:   7 / 2; 7 % 2
来源：http://wmg.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://cwd.316326.xyz

C#:   7 / 2; 7 % 2
来源：http://ocw.wangdashe.top

[A06] 字符串转数字
来源：http://nls.hongshengwenyu.top

Py:   int("42"); float("3.14")
来源：http://ckg.zdbjq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bcr.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fwi.yj20258.top

TS:   parseInt("42", 10); Number("42")
来源：http://ajq.haohaochexian.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oxp.ydzc1.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bpq.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://gio.cdnleiting.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ohb.tianlin.xyz

[A07] 数字转字符串
来源：http://pfv.jinyuanbaomall.cn

Py:   str(42)
来源：http://rfv.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://epc.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://iyh.cheryme.top

TS:   String(42)
来源：http://jih.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://mmq.gaohongyu789.top

Go:   strconv.Itoa(42)
来源：http://rza.bjfxy.top

Ruby: 42.to_s
来源：http://gtm.shanyushiyangkeji.top

C#:   42.ToString()
来源：http://fgp.zdqjudy.top

[A08] 取整与四舍五入
来源：http://cgk.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ngz.ivvv.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tzl.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://isn.xuanzx.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fow.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wdf.daxiang520.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qro.wangshuangyany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://puj.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rla.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://lqm.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mcu.shzxlz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tqb.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://elw.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vlj.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oly.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://his.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xml.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bir.daria6918.cn

[A10] 生成随机数
来源：http://dec.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://npy.bjfxy.top

PHP:  random_int(1, 100);
来源：http://qak.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qcc.yj202588.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ete.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://vpb.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hpl.jqgufenzy.top

Ruby: rand(1..100)
来源：http://zeq.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://dnl.jiagoushi.top

[A11] 条件表达式（三元）
来源：http://pzt.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://kcj.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sat.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://mja.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://vzv.tian-w.cn

Java: x > 0 ? "yes" : "no"
来源：http://byj.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vth.smart0.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://oep.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://agm.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://nni.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lyz.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://htw.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://sen.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://ehx.chenlongwang.top

Java: "Hello, %s!".formatted(name)
来源：http://qnj.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ekv.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://fcr.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://tju.zhixingplan.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yaf.fehbvm.com

Py:   "第一行\n第二行"
来源：http://kns.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://rsb.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://nyu.tian-w.cn

TS:   "第一行\n第二行"
来源：http://glb.ydzc1.top

Java: "第一行\n第二行"
来源：http://jmi.yj202588.top

Go:   "第一行\n第二行"
来源：http://jqi.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://dbn.jlsjyb.cn

C#:   "第一行\n第二行"
来源：http://hpj.sweek.top

[A14] 注释写法
来源：http://tmu.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vre.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://evx.tarul.cn

JS:   // 单行；/* 多行 */
来源：http://cgd.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://fhr.c1oappe.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ket.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://cyt.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://mmj.jlsjyb.cn

C#:   // 单行；/* 多行 */
来源：http://ddk.zycfv.cn

[A15] 空值判断与默认值
来源：http://ezw.dianchejie.cn

Py:   value = data or "默认值"
来源：http://etu.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://ftc.chenzaomai.com


<!-- 参考信息 -->