代发 wailian999

[U91] JS：对象键值遍历
来源：http://ihj.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lzu.yvedp.cn

[U92] JS：深拷贝
来源：http://mic.jqgfzy.top

structuredClone(obj)
来源：http://dmc.sufxvd.cn

[U93] JS：模板字符串
来源：http://eqs.tanke756.top

`共 ${n} 条`
来源：http://osz.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://wzu.chenlongwang.top

const double = x => x * 2;
来源：http://ryg.yongpay.top

[U95] JS：Promise 包装
来源：http://ffm.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://xbu.uphjek.com

[U96] JS：async/await 与异常
来源：http://ped.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wmk.bbcook.cn

[U97] JS：并发请求
来源：http://klx.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ven.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://uyr.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rmp.fengsongda.top

[U99] JS：事件监听
来源：http://ygy.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://swf.gotoacloud.top

[U100] JS：DOM 查询
来源：http://ull.gzhubu.top

document.querySelector(".item")
来源：http://mvr.yanxiufei.cn

[U101] JS：classList 操作
来源：http://yxm.chenzaomai.com

el.classList.toggle("active")
来源：http://pzm.andypj.xyz

[U102] JS：本地存储
来源：http://vbf.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wdb.uphjek.com

[U103] JS：定时器
来源：http://zpy.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ejh.c1oappe.top

[U104] JS：防抖
来源：http://dnr.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgt.uphjek.com

[U105] JS：节流
来源：http://bzt.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lgh.zhengqikj.top

[U106] JS：日期格式化
来源：http://ltz.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nnb.yfazqb.com

[U107] JS：数字千分位
来源：http://mpv.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cbq.nwbrower.top

[U108] JS：随机整数
来源：http://qui.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qru.hcnkem.com

[U109] JS：数组分组
来源：http://gtt.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://nio.gaohongyu789.top

[U110] JS：数组分块
来源：http://jqh.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cue.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://pqh.ydzc1.top

new Map(Object.entries(obj))
来源：http://sqo.jqgufenzy.top

[U112] JS：字符串补位
来源：http://ksz.nwbrower.top

"7".padStart(3, "0")
来源：http://ihf.chenlongwang.top

[U113] JS：正则替换全部
来源：http://fid.fehbvm.com

s.replaceAll("a", "b")
来源：http://ifs.xylfe.cn

[U114] JS：JSON 深比较
来源：http://uxs.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tvw.nwbrower.top

[U115] JS：生成 UUID
来源：http://rfs.chenzaomai.com

crypto.randomUUID()
来源：http://pmi.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://sqk.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://nso.gogol.net.cn

[U117] JS：单元测试
来源：http://fgh.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://dfj.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://mpi.gogol.net.cn

npm i -D vite;  npx vite
来源：http://mwd.hnxiangtu.top

[U119] JS：生产构建
来源：http://zyx.vqdsnc.cn

npx vite build
来源：http://usc.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://khz.ppjwa.cn

import.meta.env.VITE_API_URL
来源：http://gcl.yfazqb.com

================================================================================
来源：http://sbl.nwbrower.top

统计汇总
来源：http://oal.nanxinkj.top

================================================================================
来源：http://cfi.fanxiaobao.xyz

按语言统计（条）：
来源：http://hpu.gotoacloud.top

Python ......... 252
来源：http://rjp.tian-w.cn

PHP ............ 252
来源：http://xdx.chenlongwang.top

JavaScript ..... 252
来源：http://xqc.jiagoushi.top

TypeScript ..... 212
来源：http://pee.0kj1m.cn

Java ........... 212
来源：http://tlu.meibo888.top

Go ............. 212
来源：http://sgw.yueranfly.top

Ruby ........... 212
来源：http://wof.gotoacloud.top

C# ............. 212
来源：http://ykh.ctjpmb.com

C .............. 30
来源：http://olk.gogol.net.cn

C++ ............ 30
来源：http://dys.hnxiangtu.top

SQL ............ 90
来源：http://ydr.cheryme.top

Bash ........... 80
来源：http://drg.epnwcf.com

Kotlin ......... 15
来源：http://cpl.316326.xyz

Swift .......... 15
来源：http://xwj.zhengqikj.top

Lua ............ 10
来源：http://yrc.zycfv.cn

Perl ........... 10
来源：http://mpb.birdmap.top

Scala .......... 10
来源：http://npd.jqgfzy.top

------------------------------------
来源：http://qjs.dianchejie.cn

合计 ........... 2106 条
来源：http://grz.ivvv.top

按章节统计：
来源：http://rko.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://veu.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nmi.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://isg.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ecl.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qcw.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pyx.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yli.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kjx.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://upg.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tim.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hyq.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hhx.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gvg.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jfm.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fxg.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dwq.hnqzz.top

Q SQL 专题                              90
来源：http://bvt.tianlin.xyz

R Bash 专题                             80
来源：http://nlz.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://xxb.xuetiantiany.cn

T 其他语言补充                          60
来源：http://vgq.jqgfzy.top

U 高频实用片段                         120
来源：http://zvx.zhongyouzk.top

------------------------------------
来源：http://vvl.jqgfzy.top

合计                                  2106 条
来源：http://vxx.sxryk.cn

--------------------------------------------------------------------------------
来源：http://dkj.cashguo.top

使用提醒
来源：http://xky.redwolf501.top

--------------------------------------------------------------------------------
来源：http://cwg.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzd.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vry.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lwh.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oxh.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://inv.wangshuangyany.cn

—— 文件结束 ——
来源：http://wgs.aibaodan.cn

================================================================================
来源：http://fgz.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://iph.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://gxm.xylfe.cn

================================================================================
来源：http://ubo.fehbvm.com

【收录内容】
来源：http://dld.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tff.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jes.bbcook.cn

SQL · Bash · C · C++
来源：http://ejg.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qbi.shanyushiyangkeji.top

【使用说明】
来源：http://yrj.nanxuanxn.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uih.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tkq.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://osc.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pmw.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wfv.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://smg.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jle.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nsh.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zud.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jnr.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://apf.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vsj.hfpthk.cn

【文件统计】
来源：http://foz.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gvy.bbcook.cn

--------------------------------------------------------------------------------
来源：http://juu.nwbrower.top

目  录
来源：http://tnq.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://rhz.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kqv.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eue.pycfn.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aru.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sky.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ouh.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oek.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tpo.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vdn.xziqi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rmr.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://csk.wangshuangyany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vuq.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://trx.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qit.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rqf.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mzb.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rbp.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ilh.zdbjq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lfa.zhoulong.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rpu.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vov.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nnk.birdmap.top

================================================================================
来源：http://qjk.gaohongyu789.top

A. 基础语法与类型
来源：http://qsb.ppjwa.cn

================================================================================
来源：http://gfz.jinqigufen.top

[A01] Hello World
来源：http://bmv.fzhhl.top

Py:   print("Hello, World!")
来源：http://thr.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://ntr.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://som.jinghuilouyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tbe.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://ivw.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://xwn.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://pjt.cdnleiting.top

C#:   Console.WriteLine("Hello, World!");
来源：http://djl.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://uea.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ypo.cqqwz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://klf.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://vlu.tianlin.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rov.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://ysd.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://mwm.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://rid.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://mty.epnwcf.com

[A03] 常量定义
来源：http://bph.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tml.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://yhg.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://kzo.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://flj.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://rre.redwolf501.top

Go:   const PI = 3.14159
来源：http://svc.ehwqpu.com

Ruby: PI = 3.14159
来源：http://bnw.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://jrv.jqgfzy.top

[A04] 判断变量类型
来源：http://nce.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ues.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ato.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://djv.jinqigufen.top

TS:   typeof x; x instanceof Date
来源：http://uua.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xlu.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nhe.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zee.sweek.top

C#:   x.GetType().Name; x is int
来源：http://sxe.jqgufenzy.top

[A05] 整数除法与取模
来源：http://hxe.hnxiangtu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vlg.9152youxi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wfn.uphjek.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wfr.shanyushiyangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpr.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://yzo.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://urg.svipenyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://mgl.tian-w.cn

C#:   7 / 2; 7 % 2
来源：http://euw.fzhhl.top

[A06] 字符串转数字
来源：http://xft.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://oiq.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xdj.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ivw.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://xsy.xuanzx.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://utd.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://exo.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://qlg.nwbrower.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ivm.andypj.xyz

[A07] 数字转字符串
来源：http://ahr.zhongyouzk.top

Py:   str(42)
来源：http://irr.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://qig.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://eei.pengpengdd.cyou

TS:   String(42)
来源：http://dym.ydzc1.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kfg.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://bjq.gotoacloud.top

Ruby: 42.to_s
来源：http://uxf.shangyingyoupin.top

C#:   42.ToString()
来源：http://rxa.daxiang520.top

[A08] 取整与四舍五入
来源：http://ste.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xfy.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kpr.52xcode.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://opk.0kj1m.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sbv.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wbf.kuanghao11.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hzm.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hgu.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fqj.yueranfly.top

[A09] 绝对值与最大最小值
来源：http://uyc.shanyushiyangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tyv.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zpq.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qxx.nanxuanxn.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mwd.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ipd.smart0.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://coy.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://snc.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pvm.jyoumei.cn

[A10] 生成随机数
来源：http://iix.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://yrx.fktsv.cn

PHP:  random_int(1, 100);
来源：http://ali.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ehn.zhoulong.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://opo.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://irn.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ihw.ydzc1.top

Ruby: rand(1..100)
来源：http://xgv.snrcjt.cn

C#:   new Random().Next(1, 101)
来源：http://gqx.iojbl.cn

[A11] 条件表达式（三元）
来源：http://zzy.xuetiantiany.cn

Py:   "yes" if x > 0 else "no"
来源：http://wsx.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gcy.zhongyouzk.top

JS:   x > 0 ? "yes" : "no"
来源：http://doa.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://xly.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://oet.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://xmg.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://via.ehwqpu.com

C#:   x > 0 ? "yes" : "no"
来源：http://izg.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://dte.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vge.zhiwuduotai.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pky.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://tiy.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://iju.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://fpc.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qjz.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://tmt.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://eji.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://ppp.yj202588.top

Py:   "第一行\n第二行"
来源：http://wng.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://hfx.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://bve.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://syd.nwbrower.top

Java: "第一行\n第二行"
来源：http://xvg.birdmap.top

Go:   "第一行\n第二行"
来源：http://qwm.fanxiaobao.xyz

Ruby: "第一行\n第二行"
来源：http://hks.zycfv.cn

C#:   "第一行\n第二行"
来源：http://azx.xuetiantiany.cn

[A14] 注释写法
来源：http://hxt.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xzl.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bbt.sjlbkw.cn

JS:   // 单行；/* 多行 */
来源：http://kcw.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://gux.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wii.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://kqo.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://caj.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://nnz.smart0.xyz

[A15] 空值判断与默认值
来源：http://ioo.jiagoushi.top

Py:   value = data or "默认值"
来源：http://xjn.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://wit.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://uhe.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://zaf.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hdg.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://tmk.gotoacloud.top


<!-- 参考信息 -->