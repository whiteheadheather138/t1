代发 wailian999

[U87] JS：解构默认值
来源：http://kof.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://vfw.zdqjudy.top

[U88] JS：对象展开合并
来源：http://ran.zhijiandao.cn

{ ...a, ...b }
来源：http://etl.jqgfzy.top

[U89] JS：数组去重
来源：http://nkb.shuidangran.top

[...new Set(arr)]
来源：http://jxl.zhaomingkeji.xyz

[U90] JS：数字数组排序
来源：http://qww.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://ylk.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://ghd.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jlb.jinqigfzy.top

[U92] JS：深拷贝
来源：http://vvw.andypj.xyz

structuredClone(obj)
来源：http://eyk.xinyue.icu

[U93] JS：模板字符串
来源：http://irk.zhaomingkeji.xyz

`共 ${n} 条`
来源：http://ldt.gaohongyu789.top

[U94] JS：箭头函数
来源：http://zzw.cqqwz.cn

const double = x => x * 2;
来源：http://xad.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://epi.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://sei.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://frb.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hfo.wangshuangyany.cn

[U97] JS：并发请求
来源：http://ahm.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qeq.sweek.top

[U98] JS：fetch 带 JSON
来源：http://oiq.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gdr.chenjidiqi.icu

[U99] JS：事件监听
来源：http://cwd.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://yjg.nwbrower.top

[U100] JS：DOM 查询
来源：http://rfj.tianlin.xyz

document.querySelector(".item")
来源：http://qqs.hysaishi.cn

[U101] JS：classList 操作
来源：http://yol.52xcode.cn

el.classList.toggle("active")
来源：http://itb.epnwcf.com

[U102] JS：本地存储
来源：http://xfg.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uzi.yanxiufei.cn

[U103] JS：定时器
来源：http://mov.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ain.yanxiufei.cn

[U104] JS：防抖
来源：http://bnu.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ftp.yueranfly.top

[U105] JS：节流
来源：http://bbt.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bch.yueranfly.top

[U106] JS：日期格式化
来源：http://ggn.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qyn.havefunace.top

[U107] JS：数字千分位
来源：http://sbz.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kik.jianghu66.top

[U108] JS：随机整数
来源：http://rnf.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sce.cucudq.cn

[U109] JS：数组分组
来源：http://ysj.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://zky.fengsongda.top

[U110] JS：数组分块
来源：http://ijv.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://egd.yueranfly.top

[U111] JS：对象转 Map
来源：http://nbl.redwolf501.top

new Map(Object.entries(obj))
来源：http://lox.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://dxv.xziqi.cn

"7".padStart(3, "0")
来源：http://feh.guannengcc.top

[U113] JS：正则替换全部
来源：http://ouw.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://toz.mhx1999.top

[U114] JS：JSON 深比较
来源：http://umk.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://roa.tarul.cn

[U115] JS：生成 UUID
来源：http://wbe.nanxinkj.top

crypto.randomUUID()
来源：http://izy.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://uca.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://ukb.gotoacloud.top

[U117] JS：单元测试
来源：http://cao.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://zav.gotoacloud.top

[U118] JS：开发服务器
来源：http://wxk.uphjek.com

npm i -D vite;  npx vite
来源：http://och.daxiang520.top

[U119] JS：生产构建
来源：http://nnd.xziqi.cn

npx vite build
来源：http://ybs.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://mja.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://osk.daria6918.cn

================================================================================
来源：http://lmz.52xcode.cn

统计汇总
来源：http://ymj.vqdsnc.cn

================================================================================
来源：http://mho.yonumen.top

按语言统计（条）：
来源：http://vhw.fehbvm.com

Python ......... 252
来源：http://udr.316326.xyz

PHP ............ 252
来源：http://psi.snrcjt.cn

JavaScript ..... 252
来源：http://wzj.xuanzx.com

TypeScript ..... 212
来源：http://xgk.ivvv.top

Java ........... 212
来源：http://plg.ydzc1.top

Go ............. 212
来源：http://hdb.zhongyouzk.top

Ruby ........... 212
来源：http://zsa.jinghuilouyu.cn

C# ............. 212
来源：http://lob.havefunace.top

C .............. 30
来源：http://gsz.hysaishi.cn

C++ ............ 30
来源：http://sjq.pycfn.com

SQL ............ 90
来源：http://sfj.dianchejie.cn

Bash ........... 80
来源：http://qya.ivvv.top

Kotlin ......... 15
来源：http://mgb.yfazqb.com

Swift .......... 15
来源：http://hae.chenzaomai.com

Lua ............ 10
来源：http://iiq.ppjwa.cn

Perl ........... 10
来源：http://bcw.epnwcf.com

Scala .......... 10
来源：http://reb.iojbl.cn

------------------------------------
来源：http://rhh.zhengqikj.top

合计 ........... 2106 条
来源：http://qwn.yuxming.cn

按章节统计：
来源：http://pwx.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://esx.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wqm.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ohl.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dmp.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zys.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wlt.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://byb.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://obz.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ohi.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://prg.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://buj.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://phq.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jya.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ofb.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://epx.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hed.jlsjyb.cn

Q SQL 专题                              90
来源：http://xja.zhijiandao.cn

R Bash 专题                             80
来源：http://ziu.316326.xyz

S C / C++ 专题                          60
来源：http://rvf.feifeiyinyue.top

T 其他语言补充                          60
来源：http://ihx.birdmap.top

U 高频实用片段                         120
来源：http://mzm.quarkkingdee.top

------------------------------------
来源：http://taf.cucudq.cn

合计                                  2106 条
来源：http://mwc.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://lhg.jyoumei.cn

使用提醒
来源：http://ral.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://bdc.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ula.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wum.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fro.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://isf.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zpc.dianchejie.cn

—— 文件结束 ——
来源：http://dug.ivvv.top

================================================================================
来源：http://obb.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://gbw.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://nmd.jiagoushi.top

================================================================================
来源：http://etm.jqgufenzy.top

【收录内容】
来源：http://qvb.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ton.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jmf.bbcook.cn

SQL · Bash · C · C++
来源：http://ztb.tianlin.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tnh.xuanzx.com

【使用说明】
来源：http://rtj.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pzh.c1oappe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nmf.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://glu.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iif.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nfi.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hpb.yfazqb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wrx.meibo888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tsd.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uou.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lzl.sysykeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://olc.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://omo.gaohongyu789.top

【文件统计】
来源：http://kjv.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sbj.52xcode.cn

--------------------------------------------------------------------------------
来源：http://nqz.vqdsnc.cn

目  录
来源：http://vhe.tian-w.cn

--------------------------------------------------------------------------------
来源：http://nln.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xqk.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://enr.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://knd.jqgufenzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xfl.quarkkingdee.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xdh.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qyk.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://knd.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yvv.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://afg.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hds.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kge.zhiwuduotai.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://irc.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://non.yueranfly.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qjp.hcnkem.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vrb.smart0.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://flc.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://erd.ctjpmb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://pll.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iux.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qbw.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nlg.zhoulong.xyz

================================================================================
来源：http://ovl.gaohongyu789.top

A. 基础语法与类型
来源：http://lud.zhengqikj.top

================================================================================
来源：http://cqs.havefunace.top

[A01] Hello World
来源：http://ijh.fengsongda.top

Py:   print("Hello, World!")
来源：http://wef.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://zgu.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://oar.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rgk.tianlin.xyz

Java: System.out.println("Hello, World!");
来源：http://wvg.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://iyb.sjlbkw.cn

Ruby: puts "Hello, World!"
来源：http://jrb.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hzk.ybcxt.top

[A02] 变量声明与赋值
来源：http://bav.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://frr.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://few.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://pkz.gzhubu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vwx.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://bjb.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://mzk.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://vpt.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kql.daxiang520.top

[A03] 常量定义
来源：http://djd.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gcv.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://iip.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://inn.fengsongda.top

TS:   const PI: number = 3.14159;
来源：http://yfa.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://eoh.sjlbkw.cn

Go:   const PI = 3.14159
来源：http://owt.yonumen.top

Ruby: PI = 3.14159
来源：http://cku.birdmap.top

C#:   const double PI = 3.14159;
来源：http://kly.hammf.cn

[A04] 判断变量类型
来源：http://wgo.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dho.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://skp.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gsw.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://tfj.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gfz.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hop.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://zdc.pycfn.com

C#:   x.GetType().Name; x is int
来源：http://xax.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://xou.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vvz.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hhg.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zyj.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lhu.daria6918.cn

Java: 7 / 2; 7 % 2
来源：http://lxh.snrcjt.cn

Go:   7 / 2; 7 % 2
来源：http://iij.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://hrf.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://qwz.ydjk.org.cn

[A06] 字符串转数字
来源：http://prm.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://zip.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xfa.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dih.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://ojm.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xcj.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rng.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jgt.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lhe.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://xrk.yj202588.top

Py:   str(42)
来源：http://itc.jinyuanbaomall.cn

PHP:  (string) 42; strval(42)
来源：http://thx.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://nku.bbcook.cn

TS:   String(42)
来源：http://prr.ydjk.org.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://svo.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://esp.yj20258.top

Ruby: 42.to_s
来源：http://ruq.jlsjyb.cn

C#:   42.ToString()
来源：http://lci.xziqi.cn

[A08] 取整与四舍五入
来源：http://jhr.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tvy.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oaq.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bhz.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qxh.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xpm.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ylj.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nzf.ivvv.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nxx.havefunace.top

[A09] 绝对值与最大最小值
来源：http://asy.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cxm.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wsv.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://poe.jqgfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vvl.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fqc.fzhhl.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yql.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tis.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iam.aizwys.cn

[A10] 生成随机数
来源：http://wrj.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://xlv.yueranfly.top

PHP:  random_int(1, 100);
来源：http://pnk.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://flo.ybcxt.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ihm.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://otj.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ehx.sweek.top

Ruby: rand(1..100)
来源：http://qzf.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://zre.zhiwuduotai.top

[A11] 条件表达式（三元）
来源：http://hue.hesvh.cn

Py:   "yes" if x > 0 else "no"
来源：http://vqd.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fml.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://tjt.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://vgr.hongshengwenyu.top

Java: x > 0 ? "yes" : "no"
来源：http://dcg.tarul.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yrm.yuanzhike.top

Ruby: x > 0 ? "yes" : "no"
来源：http://roc.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dqa.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://hcr.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kcu.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://acw.jqgfzy.top

JS:   `Hello, ${name}!`
来源：http://yce.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://wbp.pengpengdd.cyou

Java: "Hello, %s!".formatted(name)
来源：http://adz.sweek.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uac.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://wnf.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://ybo.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dwd.fktsv.cn

Py:   "第一行\n第二行"
来源：http://htl.cashguo.top

PHP:  "第一行\n第二行"
来源：http://ppx.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://djo.havefunace.top

TS:   "第一行\n第二行"
来源：http://aio.jyoumei.cn

Java: "第一行\n第二行"
来源：http://ihy.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://wfp.snrcjt.cn

Ruby: "第一行\n第二行"
来源：http://vrd.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://swe.dianchejie.cn

[A14] 注释写法
来源：http://enr.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jyc.fehbvm.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://vmn.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://qmd.yonumen.top

TS:   // 单行；/* 多行 */
来源：http://cet.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bmc.havefunace.top

Go:   // 单行；/* 多行 */
来源：http://tld.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://bog.gogol.net.cn


<!-- 参考信息 -->