代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://kaw.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://jeq.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://ial.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gxi.jianghu66.top

[U85] JS：可选链
来源：http://tkc.yanxiufei.cn

a?.b?.c
来源：http://wqd.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://uyu.smart0.xyz

a ?? b
来源：http://kvx.xziqi.cn

[U87] JS：解构默认值
来源：http://uyh.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://gch.xuanzx.com

[U88] JS：对象展开合并
来源：http://cfx.9152youxi.cn

{ ...a, ...b }
来源：http://plt.nanxuanxn.top

[U89] JS：数组去重
来源：http://txv.ydzc1.top

[...new Set(arr)]
来源：http://gnw.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://epx.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://cfb.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://dmb.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rsa.tarul.cn

[U92] JS：深拷贝
来源：http://tza.bbcook.cn

structuredClone(obj)
来源：http://lnq.shuidangran.top

[U93] JS：模板字符串
来源：http://dzl.zdbjq.cn

`共 ${n} 条`
来源：http://mub.bjfxy.top

[U94] JS：箭头函数
来源：http://gjh.hcnkem.com

const double = x => x * 2;
来源：http://oig.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://ikx.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://hbs.meibo888.top

[U96] JS：async/await 与异常
来源：http://rvw.yongpay.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://psv.yuanzhike.top

[U97] JS：并发请求
来源：http://dwc.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sip.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://cyp.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxb.pengpengdd.cyou

[U99] JS：事件监听
来源：http://ywm.tarul.cn

el.addEventListener("click", e => {})
来源：http://srj.svipenyu.cn

[U100] JS：DOM 查询
来源：http://wgx.pengpengdd.cyou

document.querySelector(".item")
来源：http://xzb.smart0.xyz

[U101] JS：classList 操作
来源：http://mco.tarul.cn

el.classList.toggle("active")
来源：http://mum.aibaodan.cn

[U102] JS：本地存储
来源：http://mna.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://des.xuanzx.com

[U103] JS：定时器
来源：http://dky.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rpk.daxiang520.top

[U104] JS：防抖
来源：http://dqv.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbp.bjfxy.top

[U105] JS：节流
来源：http://oht.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://grl.mhx1999.top

[U106] JS：日期格式化
来源：http://bcv.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dal.vqdsnc.cn

[U107] JS：数字千分位
来源：http://zzb.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qqh.0kj1m.cn

[U108] JS：随机整数
来源：http://qga.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bnq.shangyingyoupin.top

[U109] JS：数组分组
来源：http://glv.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://bun.hcnkem.com

[U110] JS：数组分块
来源：http://hud.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ksc.redwolf501.top

[U111] JS：对象转 Map
来源：http://ceq.pycfn.com

new Map(Object.entries(obj))
来源：http://dvh.guannengcc.top

[U112] JS：字符串补位
来源：http://jax.vehdjk.com

"7".padStart(3, "0")
来源：http://zcs.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://bzk.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://yro.ivvv.top

[U114] JS：JSON 深比较
来源：http://uns.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://kgm.gotoacloud.top

[U115] JS：生成 UUID
来源：http://nmt.jinqigufen.top

crypto.randomUUID()
来源：http://dgc.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://plj.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://uuw.zhixingplan.top

[U117] JS：单元测试
来源：http://liw.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://ran.ctjpmb.com

[U118] JS：开发服务器
来源：http://zvz.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://ntf.hammf.cn

[U119] JS：生产构建
来源：http://rxu.jqgfzy.top

npx vite build
来源：http://npn.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://ndq.tarul.cn

import.meta.env.VITE_API_URL
来源：http://esv.yuanzhike.top

================================================================================
来源：http://uzb.fanxiaobao.xyz

统计汇总
来源：http://ykc.hesvh.cn

================================================================================
来源：http://mry.nanxuanxn.top

按语言统计（条）：
来源：http://zhn.shuidangran.top

Python ......... 252
来源：http://iba.sweek.top

PHP ............ 252
来源：http://dwd.yj20258.top

JavaScript ..... 252
来源：http://mvk.chenzaomai.com

TypeScript ..... 212
来源：http://uqn.cdnleiting.top

Java ........... 212
来源：http://zrv.9152youxi.cn

Go ............. 212
来源：http://okq.tianlin.xyz

Ruby ........... 212
来源：http://pnx.ydzc1.top

C# ............. 212
来源：http://lzu.zdbjq.cn

C .............. 30
来源：http://css.hysaishi.cn

C++ ............ 30
来源：http://hmo.0kj1m.cn

SQL ............ 90
来源：http://msi.sjlbkw.cn

Bash ........... 80
来源：http://yhl.yvedp.cn

Kotlin ......... 15
来源：http://wbq.iojbl.cn

Swift .......... 15
来源：http://uyv.jianghu66.top

Lua ............ 10
来源：http://dpl.xziqi.cn

Perl ........... 10
来源：http://nym.ivvv.top

Scala .......... 10
来源：http://vdk.tianlin.xyz

------------------------------------
来源：http://erz.hysaishi.cn

合计 ........... 2106 条
来源：http://tdu.pycfn.com

按章节统计：
来源：http://lzu.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wdy.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kvs.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ahd.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aor.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://imu.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mid.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vel.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jgn.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fnf.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zeu.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vxw.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kga.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oir.quarkkingdee.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wva.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ode.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://krl.vehdjk.com

Q SQL 专题                              90
来源：http://wjt.tianlin.xyz

R Bash 专题                             80
来源：http://vxw.jinqigfzy.top

S C / C++ 专题                          60
来源：http://sui.0kj1m.cn

T 其他语言补充                          60
来源：http://bkp.wangshuangyany.cn

U 高频实用片段                         120
来源：http://cwk.dianchejie.cn

------------------------------------
来源：http://epk.dashuyun.cn

合计                                  2106 条
来源：http://ikw.hammf.cn

--------------------------------------------------------------------------------
来源：http://vbp.ydjk.org.cn

使用提醒
来源：http://wux.uphjek.com

--------------------------------------------------------------------------------
来源：http://axx.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dew.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kjd.tianlin.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jvf.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://slg.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hai.hnxiangtu.top

—— 文件结束 ——
来源：http://def.zhaomingkeji.xyz

================================================================================
来源：http://qwx.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://zsg.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://aps.hnqzz.top

================================================================================
来源：http://nvg.nanxinkj.top

【收录内容】
来源：http://ixr.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://rcp.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wkw.jianghu66.top

SQL · Bash · C · C++
来源：http://aun.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wid.hywenlv.cn

【使用说明】
来源：http://zln.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fgz.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://opw.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zvq.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mvg.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://njc.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jym.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lxs.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xii.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ipz.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oqz.zhengqikj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dti.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fvy.uphjek.com

【文件统计】
来源：http://nch.andypj.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tlw.wangdashe.top

--------------------------------------------------------------------------------
来源：http://ihr.zdbjq.cn

目  录
来源：http://ewu.daria6918.cn

--------------------------------------------------------------------------------
来源：http://wsj.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nol.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xvh.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://clo.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mww.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tsd.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lzs.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gcw.shzxlz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ddj.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yxz.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gzn.zdqjudy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ygx.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://swn.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jms.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qqq.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sad.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fds.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vbw.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://exn.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pvk.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpd.birdmap.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://att.nwbrower.top

================================================================================
来源：http://lwn.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://nej.fzhhl.top

================================================================================
来源：http://fpv.gotoacloud.top

[A01] Hello World
来源：http://pij.aizwys.cn

Py:   print("Hello, World!")
来源：http://jur.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://kvm.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://lut.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qmt.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://egu.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://nub.316326.xyz

Ruby: puts "Hello, World!"
来源：http://qjx.snrcjt.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rno.dianchejie.cn

[A02] 变量声明与赋值
来源：http://uni.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://phs.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://epv.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vbm.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tcd.chenzaomai.com

Java: String name = "Alex"; int age = 20;
来源：http://pmo.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://xof.sweek.top

Ruby: name = "Alex"; age = 20
来源：http://uex.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://wof.gogol.net.cn

[A03] 常量定义
来源：http://ugn.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://swj.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://ako.mhx1999.top

JS:   const PI = 3.14159;
来源：http://jfy.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://syq.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://mdm.chenzaomai.com

Go:   const PI = 3.14159
来源：http://khh.hfpthk.cn

Ruby: PI = 3.14159
来源：http://aut.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://wzi.vqdsnc.cn

[A04] 判断变量类型
来源：http://eik.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ret.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zah.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://agk.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://oeb.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gvx.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://ool.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://aev.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://fdp.guowangkeji.top

[A05] 整数除法与取模
来源：http://aqv.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vnl.feifeiyinyue.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ygv.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjl.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://exe.cdnleiting.top

Java: 7 / 2; 7 % 2
来源：http://kiv.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://ijd.xuetiantiany.cn

Ruby: 7 / 2; 7 % 2
来源：http://dyb.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://uam.ctjpmb.com

[A06] 字符串转数字
来源：http://yhk.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://fql.bbcook.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bzp.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ruq.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://asf.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fqt.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://otj.52xcode.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fkp.zhiwuduotai.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xfj.zdqjudy.top

[A07] 数字转字符串
来源：http://rgk.kuanghao11.cn

Py:   str(42)
来源：http://peo.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://uqy.52xcode.cn

JS:   String(42); (42).toString()
来源：http://gya.bbcook.cn

TS:   String(42)
来源：http://aif.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cfi.yongpay.top

Go:   strconv.Itoa(42)
来源：http://awn.dashuyun.cn

Ruby: 42.to_s
来源：http://akh.hesvh.cn

C#:   42.ToString()
来源：http://egj.guowangkeji.top

[A08] 取整与四舍五入
来源：http://sov.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://htj.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rnr.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wxd.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ouq.jinqigufen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xcu.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ska.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://slw.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gei.tanke756.top

[A09] 绝对值与最大最小值
来源：http://xnl.yj20258888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tri.wangdashe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lxf.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cgj.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nzh.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cqs.vehdjk.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kda.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fzi.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ufs.sysykeji.top

[A10] 生成随机数
来源：http://nes.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://bif.yueranfly.top

PHP:  random_int(1, 100);
来源：http://wqk.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://env.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bps.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://toa.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gji.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://oik.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://jas.316326.xyz

[A11] 条件表达式（三元）
来源：http://ihh.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://bho.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fdn.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://rqs.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zmm.gotoacloud.top

Java: x > 0 ? "yes" : "no"
来源：http://mse.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ypn.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://kow.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nor.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://fts.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://swm.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zmg.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://irk.yfazqb.com

TS:   `Hello, ${name}!`
来源：http://fqg.epnwcf.com

Java: "Hello, %s!".formatted(name)
来源：http://mqi.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://igu.cashguo.top

Ruby: "Hello, #{name}!"
来源：http://yvq.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://amq.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aso.tianlin.xyz

Py:   "第一行\n第二行"
来源：http://huy.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://hqz.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://oau.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://nwa.bbcook.cn

Java: "第一行\n第二行"
来源：http://kuy.xuanzx.com

Go:   "第一行\n第二行"
来源：http://isf.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://muo.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://ely.fengsongda.top


<!-- 参考信息 -->