代发 wailian999

[U89] JS：数组去重
来源：http://las.52xcode.cn

[...new Set(arr)]
来源：http://jde.xylfe.cn

[U90] JS：数字数组排序
来源：http://gup.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://jka.cucudq.cn

[U91] JS：对象键值遍历
来源：http://wti.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gqv.havefunace.top

[U92] JS：深拷贝
来源：http://ccs.hammf.cn

structuredClone(obj)
来源：http://txh.fktsv.cn

[U93] JS：模板字符串
来源：http://mkn.xuanzx.com

`共 ${n} 条`
来源：http://ebx.jinqigfzy.top

[U94] JS：箭头函数
来源：http://vrs.nanxuanxn.top

const double = x => x * 2;
来源：http://nxs.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://vwt.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://kmz.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://ysn.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mom.gotoacloud.top

[U97] JS：并发请求
来源：http://gmt.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lje.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://uey.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uao.yj202588.top

[U99] JS：事件监听
来源：http://hyg.sysykeji.top

el.addEventListener("click", e => {})
来源：http://qlf.ehwqpu.com

[U100] JS：DOM 查询
来源：http://ipu.mhx1999.top

document.querySelector(".item")
来源：http://ljs.sxryk.cn

[U101] JS：classList 操作
来源：http://xmi.yanxiufei.cn

el.classList.toggle("active")
来源：http://zfp.yongpay.top

[U102] JS：本地存储
来源：http://pzc.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hov.guowangkeji.top

[U103] JS：定时器
来源：http://ssn.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rpw.svipenyu.cn

[U104] JS：防抖
来源：http://beq.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fiw.kuanghao11.cn

[U105] JS：节流
来源：http://ppo.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://znz.yangfankeji.com

[U106] JS：日期格式化
来源：http://vio.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uim.hcnkem.com

[U107] JS：数字千分位
来源：http://roh.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ofp.tianlin.xyz

[U108] JS：随机整数
来源：http://snf.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://upu.hfpthk.cn

[U109] JS：数组分组
来源：http://fmc.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://irv.fzhhl.top

[U110] JS：数组分块
来源：http://xiw.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gyv.daxiang520.top

[U111] JS：对象转 Map
来源：http://nmg.jyoumei.cn

new Map(Object.entries(obj))
来源：http://rkd.sweek.top

[U112] JS：字符串补位
来源：http://mpj.aibaodan.cn

"7".padStart(3, "0")
来源：http://srl.ybcxt.top

[U113] JS：正则替换全部
来源：http://mdw.daria6918.cn

s.replaceAll("a", "b")
来源：http://nzy.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://wvy.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qnr.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://dyi.zycfv.cn

crypto.randomUUID()
来源：http://qcl.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://lyr.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://htg.hnqzz.top

[U117] JS：单元测试
来源：http://wdq.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://sfb.ctjpmb.com

[U118] JS：开发服务器
来源：http://ayp.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://aff.chenjidiqi.icu

[U119] JS：生产构建
来源：http://lqe.zhixingplan.top

npx vite build
来源：http://bxp.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://niq.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://xvz.wangshuangyany.cn

================================================================================
来源：http://lne.fktsv.cn

统计汇总
来源：http://xdn.chenlongwang.top

================================================================================
来源：http://spb.fanxiaobao.xyz

按语言统计（条）：
来源：http://bum.quarkkingdee.top

Python ......... 252
来源：http://ssu.zycfv.cn

PHP ............ 252
来源：http://xoo.yj20258.top

JavaScript ..... 252
来源：http://mgd.yuanzhike.top

TypeScript ..... 212
来源：http://zmb.pycfn.com

Java ........... 212
来源：http://hze.52xcode.cn

Go ............. 212
来源：http://sgn.jyoumei.cn

Ruby ........... 212
来源：http://ove.yongpay.top

C# ............. 212
来源：http://brs.andypj.xyz

C .............. 30
来源：http://iln.quarkkingdee.top

C++ ............ 30
来源：http://cbe.birdmap.top

SQL ............ 90
来源：http://ups.zdbjq.cn

Bash ........... 80
来源：http://nws.fzhhl.top

Kotlin ......... 15
来源：http://jyc.zhongyouzk.top

Swift .......... 15
来源：http://kyr.hnqzz.top

Lua ............ 10
来源：http://gct.hysaishi.cn

Perl ........... 10
来源：http://rcq.zhixingplan.top

Scala .......... 10
来源：http://fuk.yj20258888.top

------------------------------------
来源：http://vrp.yj202588.top

合计 ........... 2106 条
来源：http://xop.yueranfly.top

按章节统计：
来源：http://yqz.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ujy.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://faq.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://grt.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://epl.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ewr.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ibg.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://svy.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://stc.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wmq.yj20258888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jsr.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qqz.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ifi.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vbl.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ukm.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jdp.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ape.dashuyun.cn

Q SQL 专题                              90
来源：http://zaf.uphjek.com

R Bash 专题                             80
来源：http://jvi.birdmap.top

S C / C++ 专题                          60
来源：http://exx.cashguo.top

T 其他语言补充                          60
来源：http://qze.smart0.xyz

U 高频实用片段                         120
来源：http://loa.cucudq.cn

------------------------------------
来源：http://gzb.fanxiaobao.xyz

合计                                  2106 条
来源：http://ggu.jianghu66.top

--------------------------------------------------------------------------------
来源：http://tbi.zycfv.cn

使用提醒
来源：http://sbl.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://fup.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eus.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tyo.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fuq.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ozf.yj20258888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dhe.ehwqpu.com

—— 文件结束 ——
来源：http://hhp.jinghuilouyu.cn

================================================================================
来源：http://tqf.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://keo.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://rus.ehwqpu.com

================================================================================
来源：http://xiz.sjlbkw.cn

【收录内容】
来源：http://lrs.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ixk.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://czo.zhengqikj.top

SQL · Bash · C · C++
来源：http://bvv.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xvu.guowangkeji.top

【使用说明】
来源：http://agq.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ftv.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ngc.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://udm.dashuyun.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jzg.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sqx.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eeb.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rux.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wpi.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bba.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yey.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pyl.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tqb.pycfn.com

【文件统计】
来源：http://ocm.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fsf.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://onk.cqqwz.cn

目  录
来源：http://uar.fehbvm.com

--------------------------------------------------------------------------------
来源：http://fxp.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oqr.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://etn.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://waq.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ggp.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vla.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iil.mhx1999.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ifj.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vkh.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sjg.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nim.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gfb.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rxw.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aai.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://abf.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yrp.guowangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aaa.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lvr.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lim.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iwo.tanke756.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aol.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hgk.sjlbkw.cn

================================================================================
来源：http://cgu.dashuyun.cn

A. 基础语法与类型
来源：http://bak.c1oappe.top

================================================================================
来源：http://cij.guowangkeji.top

[A01] Hello World
来源：http://ung.ppjwa.cn

Py:   print("Hello, World!")
来源：http://wvj.havefunace.top

PHP:  echo "Hello, World!";
来源：http://iet.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://dgp.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jrb.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://hff.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://bpr.dianchejie.cn

Ruby: puts "Hello, World!"
来源：http://hbe.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://fwi.chenlongwang.top

[A02] 变量声明与赋值
来源：http://uuf.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ijv.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dng.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://waz.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ltr.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://qle.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://nfj.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://uek.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://whm.kuanghao11.cn

[A03] 常量定义
来源：http://dsp.wangdashe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hmy.pycfn.com

PHP:  const PI = 3.14159;
来源：http://kii.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://fda.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://vwi.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://tat.yonumen.top

Go:   const PI = 3.14159
来源：http://nbv.ppjwa.cn

Ruby: PI = 3.14159
来源：http://nls.birdmap.top

C#:   const double PI = 3.14159;
来源：http://efc.cqqwz.cn

[A04] 判断变量类型
来源：http://lcm.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yon.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dpc.jinghuilouyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://old.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://jpd.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jun.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://jvx.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mhk.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://rsu.shuidangran.top

[A05] 整数除法与取模
来源：http://jmk.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cwi.sxryk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rkh.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eft.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qte.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://qjc.cdnleiting.top

Go:   7 / 2; 7 % 2
来源：http://pig.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://dqr.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://yvu.xziqi.cn

[A06] 字符串转数字
来源：http://alk.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://biu.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xwp.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ysh.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://afl.hfpthk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lkk.pycfn.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://omy.smart0.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://gjc.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gfd.hongshengwenyu.top

[A07] 数字转字符串
来源：http://zxm.tianlin.xyz

Py:   str(42)
来源：http://bju.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://wmf.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://tcz.ppjwa.cn

TS:   String(42)
来源：http://opv.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wud.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://nmj.zycfv.cn

Ruby: 42.to_s
来源：http://xap.xylfe.cn

C#:   42.ToString()
来源：http://pdl.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://amw.pengpengdd.cyou

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mao.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xda.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jbl.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ayd.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mba.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gqi.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cdk.jqgfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fdt.hcnkem.com

[A09] 绝对值与最大最小值
来源：http://huo.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://put.cqqwz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://foy.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xpq.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qcm.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gik.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ppn.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pbc.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qaw.bjfxy.top

[A10] 生成随机数
来源：http://pxz.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://nvm.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://iao.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vlt.hfpthk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://myb.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://qlu.cqqwz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dfm.fengsongda.top

Ruby: rand(1..100)
来源：http://ods.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://fon.wangdashe.top

[A11] 条件表达式（三元）
来源：http://xds.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://rnz.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hhg.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://ivk.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://cmm.zhaomingkeji.xyz

Java: x > 0 ? "yes" : "no"
来源：http://rxb.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://aoy.ehwqpu.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ofo.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://xko.ywan-chungtsiang.top

[A12] 字符串插值 / 格式化
来源：http://qps.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rhh.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ews.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://vam.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://ebn.zhoulong.xyz

Java: "Hello, %s!".formatted(name)
来源：http://ymk.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sqz.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://uvs.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://som.yonumen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zcg.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://gza.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://ymv.hfpthk.cn

JS:   "第一行\n第二行"
来源：http://akz.mhx1999.top

TS:   "第一行\n第二行"
来源：http://lps.jiagoushi.top

Java: "第一行\n第二行"
来源：http://qiq.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://uaq.yj20258.top

Ruby: "第一行\n第二行"
来源：http://idt.vehdjk.com

C#:   "第一行\n第二行"
来源：http://cxg.yuxming.cn

[A14] 注释写法
来源：http://zux.mhx1999.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ule.gotoacloud.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zai.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://ibp.shangyingyoupin.top

TS:   // 单行；/* 多行 */
来源：http://coe.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jtb.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://onl.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ptg.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://vwl.shuidangran.top

[A15] 空值判断与默认值
来源：http://glm.chenlongwang.top

Py:   value = data or "默认值"
来源：http://dzb.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://kwp.iojbl.cn


<!-- 参考信息 -->