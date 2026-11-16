代发 wailian999

[U85] JS：可选链
来源：http://orx.zdqjudy.top

a?.b?.c
来源：http://ovl.dashuyun.cn

[U86] JS：空值合并
来源：http://lqk.zdqjudy.top

a ?? b
来源：http://par.ydzc1.top

[U87] JS：解构默认值
来源：http://eqn.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://ntz.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://vhl.tanke756.top

{ ...a, ...b }
来源：http://qad.hywenlv.cn

[U89] JS：数组去重
来源：http://zms.wangshuangyany.cn

[...new Set(arr)]
来源：http://hyc.vehdjk.com

[U90] JS：数字数组排序
来源：http://ciq.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://xxp.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://kpb.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oae.yfazqb.com

[U92] JS：深拷贝
来源：http://acc.316326.xyz

structuredClone(obj)
来源：http://akd.vehdjk.com

[U93] JS：模板字符串
来源：http://ydw.zdbjq.cn

`共 ${n} 条`
来源：http://lru.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://cxc.fengsongda.top

const double = x => x * 2;
来源：http://huf.hywenlv.cn

[U95] JS：Promise 包装
来源：http://rfv.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://gge.yonumen.top

[U96] JS：async/await 与异常
来源：http://itl.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jxf.guannengcc.top

[U97] JS：并发请求
来源：http://fss.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lle.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://lbq.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kcm.xziqi.cn

[U99] JS：事件监听
来源：http://yxj.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://uys.guowangkeji.top

[U100] JS：DOM 查询
来源：http://tzv.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://aqa.316326.xyz

[U101] JS：classList 操作
来源：http://glv.mhx1999.top

el.classList.toggle("active")
来源：http://dbb.yuanzhike.top

[U102] JS：本地存储
来源：http://sbu.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mvh.ehwqpu.com

[U103] JS：定时器
来源：http://yph.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tzq.gaohongyu789.top

[U104] JS：防抖
来源：http://ibv.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zgf.haohaochexian.top

[U105] JS：节流
来源：http://aby.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://awb.nwbrower.top

[U106] JS：日期格式化
来源：http://elq.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mbv.0kj1m.cn

[U107] JS：数字千分位
来源：http://awt.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hab.kuanghao11.cn

[U108] JS：随机整数
来源：http://ndf.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qpj.aizwys.cn

[U109] JS：数组分组
来源：http://ezl.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://cgi.snrcjt.cn

[U110] JS：数组分块
来源：http://bnf.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pqo.guannengcc.top

[U111] JS：对象转 Map
来源：http://lfl.316326.xyz

new Map(Object.entries(obj))
来源：http://yff.chenlongwang.top

[U112] JS：字符串补位
来源：http://gpi.0kj1m.cn

"7".padStart(3, "0")
来源：http://pjm.snrcjt.cn

[U113] JS：正则替换全部
来源：http://zdk.fktsv.cn

s.replaceAll("a", "b")
来源：http://wxs.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://drx.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cbl.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://tfy.nwbrower.top

crypto.randomUUID()
来源：http://bia.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://rrp.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://qrq.cqqwz.cn

[U117] JS：单元测试
来源：http://lll.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://sdl.tian-w.cn

[U118] JS：开发服务器
来源：http://kzl.shzxlz.cn

npm i -D vite;  npx vite
来源：http://dqk.yongpay.top

[U119] JS：生产构建
来源：http://izh.shzxlz.cn

npx vite build
来源：http://pnm.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://zxj.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://xoo.yfazqb.com

================================================================================
来源：http://xzk.zhengqikj.top

统计汇总
来源：http://pak.pycfn.com

================================================================================
来源：http://fkg.dashuyun.cn

按语言统计（条）：
来源：http://wsr.havefunace.top

Python ......... 252
来源：http://fyk.jiagoushi.top

PHP ............ 252
来源：http://pqd.yangfankeji.com

JavaScript ..... 252
来源：http://taq.ehwqpu.com

TypeScript ..... 212
来源：http://ate.ehwqpu.com

Java ........... 212
来源：http://vcv.xuetiantiany.cn

Go ............. 212
来源：http://bpa.svipenyu.cn

Ruby ........... 212
来源：http://uzk.fehbvm.com

C# ............. 212
来源：http://sed.xziqi.cn

C .............. 30
来源：http://wrj.fanxiaobao.xyz

C++ ............ 30
来源：http://nea.xingfuxueyuan.xyz

SQL ............ 90
来源：http://ohg.shuidangran.top

Bash ........... 80
来源：http://cse.fengsongda.top

Kotlin ......... 15
来源：http://dhx.hnxiangtu.top

Swift .......... 15
来源：http://boy.fzhhl.top

Lua ............ 10
来源：http://eko.hesvh.cn

Perl ........... 10
来源：http://tof.snrcjt.cn

Scala .......... 10
来源：http://fhq.meibo888.top

------------------------------------
来源：http://mpw.vehdjk.com

合计 ........... 2106 条
来源：http://fvd.sxryk.cn

按章节统计：
来源：http://hrm.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kkr.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xir.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bsh.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qov.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hty.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yno.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ocz.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ryz.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xam.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dvg.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mxj.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hlv.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oie.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uct.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uhr.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://atb.nanxinkj.top

Q SQL 专题                              90
来源：http://tsm.yuanzhike.top

R Bash 专题                             80
来源：http://vtm.sxryk.cn

S C / C++ 专题                          60
来源：http://iye.quarkkingdee.top

T 其他语言补充                          60
来源：http://xxo.meibo888.top

U 高频实用片段                         120
来源：http://ffa.dashuyun.cn

------------------------------------
来源：http://ehe.hysaishi.cn

合计                                  2106 条
来源：http://tfg.yonumen.top

--------------------------------------------------------------------------------
来源：http://whn.pengpengdd.cyou

使用提醒
来源：http://gdc.jianghu66.top

--------------------------------------------------------------------------------
来源：http://uit.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zqw.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://krd.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qju.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pzy.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tsy.yfazqb.com

—— 文件结束 ——
来源：http://cuf.ehwqpu.com

================================================================================
来源：http://jxg.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://sqp.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://oct.aizwys.cn

================================================================================
来源：http://igx.tianlin.xyz

【收录内容】
来源：http://rnt.zhiwuduotai.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oqw.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ixn.ehwqpu.com

SQL · Bash · C · C++
来源：http://vsp.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ark.yangfankeji.com

【使用说明】
来源：http://xli.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fzp.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://krb.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mdw.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://faz.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://liv.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vzi.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sip.jqgufenzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lku.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kvx.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tbk.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kdq.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qol.gaohongyu789.top

【文件统计】
来源：http://lqn.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rwj.hnqzz.top

--------------------------------------------------------------------------------
来源：http://jhi.havefunace.top

目  录
来源：http://eaf.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://nlr.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://caj.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mbo.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://enk.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mbo.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yvn.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://amd.ctjpmb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zyz.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ucv.yj202588.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tqk.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://apf.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yxa.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rvw.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yrg.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zxd.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://psu.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://smy.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nsp.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://leq.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oug.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pbw.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sbj.wangdashe.top

================================================================================
来源：http://wec.xuanzx.com

A. 基础语法与类型
来源：http://hml.quarkkingdee.top

================================================================================
来源：http://tjf.ydjk.org.cn

[A01] Hello World
来源：http://crd.haohaochexian.top

Py:   print("Hello, World!")
来源：http://agr.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://gln.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://pda.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hse.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://tuq.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://cal.c1oappe.top

Ruby: puts "Hello, World!"
来源：http://klw.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zsc.guannengcc.top

[A02] 变量声明与赋值
来源：http://vwv.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hio.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yag.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fhi.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ohm.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://kvt.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://alm.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://gfq.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://vcv.shanyushiyangtech.top

[A03] 常量定义
来源：http://nzs.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dfx.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://xwl.svipenyu.cn

JS:   const PI = 3.14159;
来源：http://yle.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://iky.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://exy.zycfv.cn

Go:   const PI = 3.14159
来源：http://fgt.sufxvd.cn

Ruby: PI = 3.14159
来源：http://bhg.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://lys.chenzaomai.com

[A04] 判断变量类型
来源：http://acd.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://slc.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aeg.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://umn.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://zbf.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iem.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://fel.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qtn.yj20258888.top

C#:   x.GetType().Name; x is int
来源：http://jvi.zdbjq.cn

[A05] 整数除法与取模
来源：http://ngb.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nde.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://deo.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ctv.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rrd.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://gfq.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://epn.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://ber.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://cmv.gaohongyu789.top

[A06] 字符串转数字
来源：http://ruo.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://wve.daxiang520.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hjz.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mti.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rcc.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kze.xylfe.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bcp.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wfy.0kj1m.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xwi.meibo888.top

[A07] 数字转字符串
来源：http://ecz.yj202588.top

Py:   str(42)
来源：http://ueq.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://wtk.vqdsnc.cn

JS:   String(42); (42).toString()
来源：http://izm.meibo888.top

TS:   String(42)
来源：http://qjl.sufxvd.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ukc.ppjwa.cn

Go:   strconv.Itoa(42)
来源：http://nxp.fengsongda.top

Ruby: 42.to_s
来源：http://doo.cdnleiting.top

C#:   42.ToString()
来源：http://dne.iojbl.cn

[A08] 取整与四舍五入
来源：http://ipu.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ukt.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zfz.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jun.xingfuxueyuan.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xod.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://awc.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://orn.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rem.cdnleiting.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qzq.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://yzm.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iwo.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://czi.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dsz.sweek.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fbt.jinghuilouyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.yuxming.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zzq.nwbrower.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://exg.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gqw.jqgfzy.top

[A10] 生成随机数
来源：http://qge.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://ymr.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://yid.fehbvm.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zys.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nrp.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://yig.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uct.wangshuangyany.cn

Ruby: rand(1..100)
来源：http://vce.jinqigfzy.top

C#:   new Random().Next(1, 101)
来源：http://hqp.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://fve.yangfankeji.com

Py:   "yes" if x > 0 else "no"
来源：http://uap.shzxlz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kgp.zhijiandao.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qrm.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://xih.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://zac.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hqo.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ops.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://zwa.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://mnw.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://emt.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://onx.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://uux.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://omy.52xcode.cn

Java: "Hello, %s!".formatted(name)
来源：http://jyi.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://avj.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://tah.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://vzi.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://emm.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://gzf.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://xve.yueranfly.top

JS:   "第一行\n第二行"
来源：http://tfo.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://bzp.cheryme.top

Java: "第一行\n第二行"
来源：http://ufz.hnqzz.top

Go:   "第一行\n第二行"
来源：http://koo.pycfn.com

Ruby: "第一行\n第二行"
来源：http://rnv.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://mfv.hesvh.cn

[A14] 注释写法
来源：http://nse.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://itb.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hym.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://ujt.gogol.net.cn


<!-- 参考信息 -->