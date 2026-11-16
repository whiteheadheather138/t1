代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://qal.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://fyt.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://dcx.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wge.zhixingplan.top

[U85] JS：可选链
来源：http://jxr.shzxlz.cn

a?.b?.c
来源：http://kch.sweek.top

[U86] JS：空值合并
来源：http://vik.gogol.net.cn

a ?? b
来源：http://tgj.hysaishi.cn

[U87] JS：解构默认值
来源：http://deo.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://wqb.tian-w.cn

[U88] JS：对象展开合并
来源：http://woz.sweek.top

{ ...a, ...b }
来源：http://lqj.c1oappe.top

[U89] JS：数组去重
来源：http://cio.snrcjt.cn

[...new Set(arr)]
来源：http://abn.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://vho.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://svu.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://wjq.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xtf.xylfe.cn

[U92] JS：深拷贝
来源：http://lhr.jqgfzy.top

structuredClone(obj)
来源：http://iwp.tianlin.xyz

[U93] JS：模板字符串
来源：http://ilw.ydzc1.top

`共 ${n} 条`
来源：http://iit.ehwqpu.com

[U94] JS：箭头函数
来源：http://tjs.tianlin.xyz

const double = x => x * 2;
来源：http://qyf.pycfn.com

[U95] JS：Promise 包装
来源：http://aep.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://ecy.fktsv.cn

[U96] JS：async/await 与异常
来源：http://qis.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kva.ydjk.org.cn

[U97] JS：并发请求
来源：http://ccq.redwolf501.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pgr.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://dps.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mbt.fehbvm.com

[U99] JS：事件监听
来源：http://eof.jianghu66.top

el.addEventListener("click", e => {})
来源：http://gvg.cdnleiting.top

[U100] JS：DOM 查询
来源：http://yie.jinghuilouyu.cn

document.querySelector(".item")
来源：http://rmt.gotoacloud.top

[U101] JS：classList 操作
来源：http://ohn.cdnleiting.top

el.classList.toggle("active")
来源：http://ydc.ydjk.org.cn

[U102] JS：本地存储
来源：http://dfk.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zvy.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://zke.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jjf.gzhubu.top

[U104] JS：防抖
来源：http://fav.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khf.jqgfzy.top

[U105] JS：节流
来源：http://xap.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://miu.fzhhl.top

[U106] JS：日期格式化
来源：http://wio.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kqu.yongpay.top

[U107] JS：数字千分位
来源：http://ptg.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kik.yvedp.cn

[U108] JS：随机整数
来源：http://iag.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nes.c1oappe.top

[U109] JS：数组分组
来源：http://hew.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://mbv.tanke756.top

[U110] JS：数组分块
来源：http://hni.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mwe.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://scy.yuxming.cn

new Map(Object.entries(obj))
来源：http://gjk.yanxiufei.cn

[U112] JS：字符串补位
来源：http://bly.yvedp.cn

"7".padStart(3, "0")
来源：http://sgu.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://dta.hammf.cn

s.replaceAll("a", "b")
来源：http://muf.hammf.cn

[U114] JS：JSON 深比较
来源：http://snz.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://toq.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://lss.gogol.net.cn

crypto.randomUUID()
来源：http://xyn.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://xah.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://cua.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://wya.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://xqb.fehbvm.com

[U118] JS：开发服务器
来源：http://iem.tarul.cn

npm i -D vite;  npx vite
来源：http://iuo.uphjek.com

[U119] JS：生产构建
来源：http://tsq.snrcjt.cn

npx vite build
来源：http://kdu.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://wyk.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://dwh.snrcjt.cn

================================================================================
来源：http://ete.shangyingyoupin.top

统计汇总
来源：http://bfg.gotoacloud.top

================================================================================
来源：http://riw.jqgfzy.top

按语言统计（条）：
来源：http://fix.hywenlv.cn

Python ......... 252
来源：http://gxo.cheryme.top

PHP ............ 252
来源：http://odp.feifeiyinyue.top

JavaScript ..... 252
来源：http://adt.ydzc1.top

TypeScript ..... 212
来源：http://sdg.dashuyun.cn

Java ........... 212
来源：http://bxb.0kj1m.cn

Go ............. 212
来源：http://xqr.zhiwuduotai.top

Ruby ........... 212
来源：http://vjm.zhengqikj.top

C# ............. 212
来源：http://fhw.jyoumei.cn

C .............. 30
来源：http://xnq.52xcode.cn

C++ ............ 30
来源：http://zpe.hysaishi.cn

SQL ............ 90
来源：http://dxa.meibo888.top

Bash ........... 80
来源：http://onx.zhongyouzk.top

Kotlin ......... 15
来源：http://jaf.xingfuxueyuan.xyz

Swift .......... 15
来源：http://cxp.pengpengdd.cyou

Lua ............ 10
来源：http://nje.pengpengdd.cyou

Perl ........... 10
来源：http://fiy.yj20258.top

Scala .......... 10
来源：http://hcl.0kj1m.cn

------------------------------------
来源：http://rxb.epnwcf.com

合计 ........... 2106 条
来源：http://pfi.chenzaomai.com

按章节统计：
来源：http://bcu.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bpw.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qii.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://png.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://inx.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sfe.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kcu.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://daa.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lqd.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oka.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iby.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lun.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ngz.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lyq.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://usu.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pys.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xys.xuetiantiany.cn

Q SQL 专题                              90
来源：http://nmu.fanxiaobao.xyz

R Bash 专题                             80
来源：http://wqc.meibo888.top

S C / C++ 专题                          60
来源：http://kaq.fengsongda.top

T 其他语言补充                          60
来源：http://bfw.hnqzz.top

U 高频实用片段                         120
来源：http://hbn.cqqwz.cn

------------------------------------
来源：http://hcs.ivvv.top

合计                                  2106 条
来源：http://omj.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://juf.cashguo.top

使用提醒
来源：http://bjg.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://elh.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ezn.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cyp.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iyb.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://ulm.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aid.jyoumei.cn

—— 文件结束 ——
来源：http://ich.quarkkingdee.top

================================================================================
来源：http://iez.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://oqc.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://fhe.tarul.cn

================================================================================
来源：http://zjf.tian-w.cn

【收录内容】
来源：http://ekq.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wgx.ybcxt.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://frf.snrcjt.cn

SQL · Bash · C · C++
来源：http://cwh.yj20258888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://otf.ydjk.org.cn

【使用说明】
来源：http://eml.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dkg.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nad.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zdq.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dwj.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://top.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kxm.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vss.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xzv.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jxt.jianghu66.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fhc.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://seu.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dye.jqgfzy.top

【文件统计】
来源：http://kol.jinghuilouyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lsw.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://zyg.jqgufenzy.top

目  录
来源：http://aeo.xinyue.icu

--------------------------------------------------------------------------------
来源：http://xep.hammf.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zld.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xbp.yvedp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bau.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cqp.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mus.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qhz.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hak.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ndl.nwbrower.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nfh.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wvs.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bhe.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kxn.sjlbkw.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wir.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://emy.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yyp.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ica.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nuy.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cfr.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qiu.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpy.sjlbkw.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wco.mhx1999.top

================================================================================
来源：http://hpg.chenzaomai.com

A. 基础语法与类型
来源：http://kbq.jinyuanbaomall.cn

================================================================================
来源：http://obk.yj202588.top

[A01] Hello World
来源：http://ykn.epnwcf.com

Py:   print("Hello, World!")
来源：http://ezs.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://blx.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://mli.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hrc.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://bnb.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://spb.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://aek.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://oiu.ctjpmb.com

[A02] 变量声明与赋值
来源：http://scp.gotoacloud.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://riq.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://okr.bbcook.cn

JS:   let name = "Alex"; const age = 20;
来源：http://evi.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://azk.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://dlm.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://ptq.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://gyg.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://mla.cdnleiting.top

[A03] 常量定义
来源：http://son.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pra.zdqjudy.top

PHP:  const PI = 3.14159;
来源：http://vyc.yuxming.cn

JS:   const PI = 3.14159;
来源：http://ifi.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://xji.316326.xyz

Java: static final double PI = 3.14159;
来源：http://wus.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://ibu.fengsongda.top

Ruby: PI = 3.14159
来源：http://mct.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://wtb.pengpengdd.cyou

[A04] 判断变量类型
来源：http://xxb.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bgi.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wme.zycfv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vmr.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://ygi.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://axl.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://kuc.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pdr.shangyingyoupin.top

C#:   x.GetType().Name; x is int
来源：http://bbj.xylfe.cn

[A05] 整数除法与取模
来源：http://lfv.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://svf.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zco.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bkm.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tec.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://put.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://kye.sjlbkw.cn

Ruby: 7 / 2; 7 % 2
来源：http://day.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://ayl.cucudq.cn

[A06] 字符串转数字
来源：http://aza.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://uev.bbcook.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kzx.316326.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hpg.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://pxy.zdbjq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ueg.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dlg.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gyi.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://okc.hcnkem.com

[A07] 数字转字符串
来源：http://wgq.yj20258.top

Py:   str(42)
来源：http://sio.jinyuanbaomall.cn

PHP:  (string) 42; strval(42)
来源：http://whh.birdmap.top

JS:   String(42); (42).toString()
来源：http://ake.chenlongwang.top

TS:   String(42)
来源：http://blt.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ikv.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://ftw.jyoumei.cn

Ruby: 42.to_s
来源：http://xus.jinqigfzy.top

C#:   42.ToString()
来源：http://aic.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://ptb.jianghu66.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ocb.yj202588.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tvi.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jpn.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zak.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rof.meibo888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aex.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gtf.chenjidiqi.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zzh.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://bum.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mcf.zycfv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://okj.ctjpmb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lnn.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rbu.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wyr.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aap.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kjj.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qiy.bjfxy.top

[A10] 生成随机数
来源：http://oms.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://afn.yuxming.cn

PHP:  random_int(1, 100);
来源：http://byk.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mlo.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cyd.316326.xyz

Java: new Random().nextInt(100) + 1
来源：http://smz.hammf.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ahq.haohaochexian.top

Ruby: rand(1..100)
来源：http://rlo.shanyushiyangkeji.top

C#:   new Random().Next(1, 101)
来源：http://ibc.hnqzz.top

[A11] 条件表达式（三元）
来源：http://how.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://jdd.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ljk.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://qel.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://aid.cqqwz.cn

Java: x > 0 ? "yes" : "no"
来源：http://xfw.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gzh.xinyue.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://ubv.yangfankeji.com

C#:   x > 0 ? "yes" : "no"
来源：http://cin.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://wsz.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ira.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://all.vehdjk.com

JS:   `Hello, ${name}!`
来源：http://qya.hesvh.cn

TS:   `Hello, ${name}!`
来源：http://kin.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://fyz.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ids.fehbvm.com

Ruby: "Hello, #{name}!"
来源：http://lui.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://erw.hysaishi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://upu.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://kyq.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://eoq.vehdjk.com

JS:   "第一行\n第二行"
来源：http://hob.gzhubu.top

TS:   "第一行\n第二行"
来源：http://obt.ehwqpu.com

Java: "第一行\n第二行"
来源：http://qne.sxryk.cn

Go:   "第一行\n第二行"
来源：http://cna.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://ump.iojbl.cn

C#:   "第一行\n第二行"
来源：http://que.zhoulong.xyz


<!-- 参考信息 -->