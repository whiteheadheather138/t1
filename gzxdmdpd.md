代发 wailian999

[U93] JS：模板字符串
来源：http://jyw.cdnleiting.top

`共 ${n} 条`
来源：http://iba.yfazqb.com

[U94] JS：箭头函数
来源：http://ach.cdnleiting.top

const double = x => x * 2;
来源：http://ydi.guannengcc.top

[U95] JS：Promise 包装
来源：http://zub.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://kyf.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://vrm.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ali.gzhubu.top

[U97] JS：并发请求
来源：http://cms.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://her.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://syo.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cyp.hfpthk.cn

[U99] JS：事件监听
来源：http://zix.havefunace.top

el.addEventListener("click", e => {})
来源：http://axh.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://fwi.ctjpmb.com

document.querySelector(".item")
来源：http://jes.fehbvm.com

[U101] JS：classList 操作
来源：http://esn.zdqjudy.top

el.classList.toggle("active")
来源：http://hbp.jinqigufen.top

[U102] JS：本地存储
来源：http://fwd.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qbj.tanke756.top

[U103] JS：定时器
来源：http://bhr.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jmv.yangfankeji.com

[U104] JS：防抖
来源：http://iun.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://arn.hnxiangtu.top

[U105] JS：节流
来源：http://rmt.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nnn.xinyue.icu

[U106] JS：日期格式化
来源：http://pdf.cheryme.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sye.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://yqd.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jft.yonumen.top

[U108] JS：随机整数
来源：http://ctr.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baf.feifeiyinyue.top

[U109] JS：数组分组
来源：http://ofh.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://xot.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://cwk.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jow.tianlin.xyz

[U111] JS：对象转 Map
来源：http://uxt.yj20258.top

new Map(Object.entries(obj))
来源：http://oaj.iojbl.cn

[U112] JS：字符串补位
来源：http://ajx.yangfankeji.com

"7".padStart(3, "0")
来源：http://igm.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://jdg.hesvh.cn

s.replaceAll("a", "b")
来源：http://lbx.yuxming.cn

[U114] JS：JSON 深比较
来源：http://ruk.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ayt.ivvv.top

[U115] JS：生成 UUID
来源：http://hxo.redwolf501.top

crypto.randomUUID()
来源：http://pyi.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://agg.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://wow.zdbjq.cn

[U117] JS：单元测试
来源：http://qrj.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://jrq.bbcook.cn

[U118] JS：开发服务器
来源：http://moi.wangdashe.top

npm i -D vite;  npx vite
来源：http://nui.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://mzq.shanyushiyangkeji.top

npx vite build
来源：http://sbg.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://fzw.tanke756.top

import.meta.env.VITE_API_URL
来源：http://btt.0kj1m.cn

================================================================================
来源：http://nts.c1oappe.top

统计汇总
来源：http://gvq.ctjpmb.com

================================================================================
来源：http://zxa.xuanzx.com

按语言统计（条）：
来源：http://rps.hcnkem.com

Python ......... 252
来源：http://qzo.zhengqikj.top

PHP ............ 252
来源：http://kpy.ppjwa.cn

JavaScript ..... 252
来源：http://eyd.gaohongyu789.top

TypeScript ..... 212
来源：http://lso.zhongyouzk.top

Java ........... 212
来源：http://api.gogol.net.cn

Go ............. 212
来源：http://ekq.xinyue.icu

Ruby ........... 212
来源：http://kis.zhixingplan.top

C# ............. 212
来源：http://xkd.wangshuangyany.cn

C .............. 30
来源：http://jfo.gzhubu.top

C++ ............ 30
来源：http://dmw.bbcook.cn

SQL ............ 90
来源：http://ulo.birdmap.top

Bash ........... 80
来源：http://suo.guannengcc.top

Kotlin ......... 15
来源：http://bla.jqgufenzy.top

Swift .......... 15
来源：http://van.ctjpmb.com

Lua ............ 10
来源：http://rnk.jinqigufen.top

Perl ........... 10
来源：http://wqj.zhixingplan.top

Scala .......... 10
来源：http://wse.snrcjt.cn

------------------------------------
来源：http://kei.dashuyun.cn

合计 ........... 2106 条
来源：http://lpm.aibaodan.cn

按章节统计：
来源：http://qna.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ebx.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uqm.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://frm.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wyl.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zox.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uqo.hcnkem.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://khx.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ryo.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zml.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ydr.52xcode.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://grt.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mdm.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nzc.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uhm.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mlw.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cqb.cucudq.cn

Q SQL 专题                              90
来源：http://ots.9152youxi.cn

R Bash 专题                             80
来源：http://bop.zhixingplan.top

S C / C++ 专题                          60
来源：http://nnd.yuxming.cn

T 其他语言补充                          60
来源：http://qhe.hnxiangtu.top

U 高频实用片段                         120
来源：http://nfp.tianlin.xyz

------------------------------------
来源：http://gwp.jiagoushi.top

合计                                  2106 条
来源：http://abs.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://ize.xziqi.cn

使用提醒
来源：http://obr.bjfxy.top

--------------------------------------------------------------------------------
来源：http://lkm.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://opa.sweek.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qms.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qqe.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pdi.aibaodan.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xgc.chenlongwang.top

—— 文件结束 ——
来源：http://rqw.fanxiaobao.xyz

================================================================================
来源：http://mkq.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://enr.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://zor.xziqi.cn

================================================================================
来源：http://gxn.epnwcf.com

【收录内容】
来源：http://hpp.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uvf.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lee.hammf.cn

SQL · Bash · C · C++
来源：http://hlf.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uxs.mhx1999.top

【使用说明】
来源：http://oyp.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://izt.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lsq.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://buw.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ift.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wnn.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kkz.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://stw.xylfe.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qys.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pst.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yic.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://obr.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://otq.yongpay.top

【文件统计】
来源：http://wno.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xlg.zycfv.cn

--------------------------------------------------------------------------------
来源：http://ikm.zhengqikj.top

目  录
来源：http://fsq.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://jcl.jinghuilouyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kqk.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://whc.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://auv.ywan-chungtsiang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tnf.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mmu.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hml.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jjq.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zhx.tanke756.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ujq.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hjp.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://khh.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dbv.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xvg.9152youxi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lmk.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://knn.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ixz.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://waz.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kod.bbcook.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mst.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ksy.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://evz.yanxiufei.cn

================================================================================
来源：http://mgs.andypj.xyz

A. 基础语法与类型
来源：http://iky.svipenyu.cn

================================================================================
来源：http://aaz.pycfn.com

[A01] Hello World
来源：http://hlv.dianchejie.cn

Py:   print("Hello, World!")
来源：http://obv.redwolf501.top

PHP:  echo "Hello, World!";
来源：http://xks.tarul.cn

JS:   console.log("Hello, World!");
来源：http://zps.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://owv.hnxiangtu.top

Java: System.out.println("Hello, World!");
来源：http://wbe.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://dvk.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://mrd.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://szb.c1oappe.top

[A02] 变量声明与赋值
来源：http://zrf.yuxming.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hxp.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zgg.bbcook.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xuj.fzhhl.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uxl.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://kml.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://zbt.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://kfd.meibo888.top

C#:   string name = "Alex"; int age = 20;
来源：http://mbi.fanxiaobao.xyz

[A03] 常量定义
来源：http://bvr.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jul.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://vnf.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://eyy.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://sss.gzhubu.top

Java: static final double PI = 3.14159;
来源：http://kdp.pycfn.com

Go:   const PI = 3.14159
来源：http://uzy.cqqwz.cn

Ruby: PI = 3.14159
来源：http://fqx.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://vqt.yj202588.top

[A04] 判断变量类型
来源：http://ktt.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yxm.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://drh.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hve.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://lpy.gzhubu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yiq.xinyue.icu

Go:   reflect.TypeOf(x).Name()
来源：http://mtb.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gru.svipenyu.cn

C#:   x.GetType().Name; x is int
来源：http://eje.gzhubu.top

[A05] 整数除法与取模
来源：http://yzp.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iea.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ukn.hywenlv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://isr.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wkz.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://kvs.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://heb.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://nfe.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://olf.yvedp.cn

[A06] 字符串转数字
来源：http://pzj.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://wlt.jinqigfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wdp.xylfe.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wrh.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://svl.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fvv.cheryme.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sye.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://hbi.cheryme.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://loq.andypj.xyz

[A07] 数字转字符串
来源：http://jyu.yfazqb.com

Py:   str(42)
来源：http://sxe.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://bfe.shuidangran.top

JS:   String(42); (42).toString()
来源：http://bbj.zhongyouzk.top

TS:   String(42)
来源：http://qjn.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dzo.yj202588.top

Go:   strconv.Itoa(42)
来源：http://pod.zhongyouzk.top

Ruby: 42.to_s
来源：http://rjc.chenzaomai.com

C#:   42.ToString()
来源：http://cyp.xinyue.icu

[A08] 取整与四舍五入
来源：http://hjq.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://upb.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yya.tarul.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hvv.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uys.shanyushiyangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lrf.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ith.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pzj.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qjv.pycfn.com

[A09] 绝对值与最大最小值
来源：http://thc.yangfankeji.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sik.havefunace.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oor.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tfs.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://khd.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pmo.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iln.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vqj.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://guv.xinyue.icu

[A10] 生成随机数
来源：http://nsd.nwbrower.top

Py:   import random; random.randint(1, 100)
来源：http://qxg.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://vbq.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uri.yueranfly.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gxd.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://gtp.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yxr.yj20258.top

Ruby: rand(1..100)
来源：http://zzn.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://len.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://vpv.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://dyl.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ysp.aibaodan.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lxo.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qff.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://njo.tianlin.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://cei.shangyingyoupin.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fte.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://ser.nanxuanxn.top

[A12] 字符串插值 / 格式化
来源：http://ziw.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ryg.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uxr.ctjpmb.com

JS:   `Hello, ${name}!`
来源：http://vby.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://qed.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://alh.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fbx.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://wlv.haohaochexian.top

C#:   $"Hello, {name}!"
来源：http://kgu.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hpw.yuxming.cn

Py:   "第一行\n第二行"
来源：http://eyz.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://nln.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://vei.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://ueg.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://hbl.cheryme.top

Go:   "第一行\n第二行"
来源：http://mwk.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://mlt.pengpengdd.cyou

C#:   "第一行\n第二行"
来源：http://por.andypj.xyz

[A14] 注释写法
来源：http://jwa.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rps.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://sjv.nanxuanxn.top

JS:   // 单行；/* 多行 */
来源：http://gvh.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://dnb.jlsjyb.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jkj.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://okt.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://dww.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://mrb.jqgfzy.top

[A15] 空值判断与默认值
来源：http://slh.daria6918.cn

Py:   value = data or "默认值"
来源：http://hgf.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://yyw.zdqjudy.top

JS:   const value = data ?? "默认值";
来源：http://xxc.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://xwv.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wiu.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://xvc.fzhhl.top

Ruby: value = data || "默认值"
来源：http://yqe.pycfn.com

C#:   var value = data ?? "默认值";
来源：http://ngl.svipenyu.cn

[A16] 真假值判断规则
来源：http://lga.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oyz.jinqigfzy.top


<!-- 参考信息 -->