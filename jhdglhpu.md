代发 wailian999

[U95] JS：Promise 包装
来源：http://uwx.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://dnk.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://wuv.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ias.shuidangran.top

[U97] JS：并发请求
来源：http://gim.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ewa.sweek.top

[U98] JS：fetch 带 JSON
来源：http://tdf.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mpq.9152youxi.cn

[U99] JS：事件监听
来源：http://jyy.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://paw.fktsv.cn

[U100] JS：DOM 查询
来源：http://khw.tarul.cn

document.querySelector(".item")
来源：http://rsx.xuanzx.com

[U101] JS：classList 操作
来源：http://dsi.tian-w.cn

el.classList.toggle("active")
来源：http://opb.xinyue.icu

[U102] JS：本地存储
来源：http://tmx.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://klm.ehwqpu.com

[U103] JS：定时器
来源：http://bzo.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zie.zhixingplan.top

[U104] JS：防抖
来源：http://yyt.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kqn.jqgufenzy.top

[U105] JS：节流
来源：http://fkq.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yma.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://nkq.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gqt.hysaishi.cn

[U107] JS：数字千分位
来源：http://mjt.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vbi.zhiwuduotai.top

[U108] JS：随机整数
来源：http://abl.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://edn.fengsongda.top

[U109] JS：数组分组
来源：http://rfs.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://gqe.vehdjk.com

[U110] JS：数组分块
来源：http://qnl.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vim.hfpthk.cn

[U111] JS：对象转 Map
来源：http://ixy.ehwqpu.com

new Map(Object.entries(obj))
来源：http://qdj.c1oappe.top

[U112] JS：字符串补位
来源：http://rdh.9152youxi.cn

"7".padStart(3, "0")
来源：http://nyq.sufxvd.cn

[U113] JS：正则替换全部
来源：http://qjq.xziqi.cn

s.replaceAll("a", "b")
来源：http://hvv.nwbrower.top

[U114] JS：JSON 深比较
来源：http://atq.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hyt.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://kxo.yuxming.cn

crypto.randomUUID()
来源：http://vtk.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://gsd.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://wnh.zdqjudy.top

[U117] JS：单元测试
来源：http://obv.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://zpr.sysykeji.top

[U118] JS：开发服务器
来源：http://rin.hfpthk.cn

npm i -D vite;  npx vite
来源：http://wql.yangfankeji.com

[U119] JS：生产构建
来源：http://bxk.smart0.xyz

npx vite build
来源：http://fqx.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://ofh.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://cpk.c1oappe.top

================================================================================
来源：http://hap.wangshuangyany.cn

统计汇总
来源：http://jyx.sufxvd.cn

================================================================================
来源：http://wcv.ppjwa.cn

按语言统计（条）：
来源：http://tzi.redwolf501.top

Python ......... 252
来源：http://lyp.ydzc1.top

PHP ............ 252
来源：http://gfx.dashuyun.cn

JavaScript ..... 252
来源：http://uth.hfpthk.cn

TypeScript ..... 212
来源：http://waq.uphjek.com

Java ........... 212
来源：http://ngd.sweek.top

Go ............. 212
来源：http://ewk.ehwqpu.com

Ruby ........... 212
来源：http://rqq.9152youxi.cn

C# ............. 212
来源：http://qst.shzxlz.cn

C .............. 30
来源：http://dsg.chenjidiqi.icu

C++ ............ 30
来源：http://pmc.hongshengwenyu.top

SQL ............ 90
来源：http://qqz.meibo888.top

Bash ........... 80
来源：http://trt.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://qvx.bbcook.cn

Swift .......... 15
来源：http://bxd.guannengcc.top

Lua ............ 10
来源：http://uuq.zhoulong.xyz

Perl ........... 10
来源：http://ygy.guowangkeji.top

Scala .......... 10
来源：http://rzk.uphjek.com

------------------------------------
来源：http://fuy.daria6918.cn

合计 ........... 2106 条
来源：http://hjz.vehdjk.com

按章节统计：
来源：http://dvd.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://urw.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mlg.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vlg.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gzu.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fgm.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://spx.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zey.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qly.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ejy.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jrs.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dob.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yec.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gvl.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eyl.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qat.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ikx.jqgfzy.top

Q SQL 专题                              90
来源：http://ril.xziqi.cn

R Bash 专题                             80
来源：http://qpx.tanke756.top

S C / C++ 专题                          60
来源：http://wsb.316326.xyz

T 其他语言补充                          60
来源：http://hsr.yonumen.top

U 高频实用片段                         120
来源：http://jcv.cucudq.cn

------------------------------------
来源：http://yeh.smart0.xyz

合计                                  2106 条
来源：http://hll.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://hpc.ctjpmb.com

使用提醒
来源：http://uja.zycfv.cn

--------------------------------------------------------------------------------
来源：http://day.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ghh.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wql.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qhv.xuanzx.com

在旧版本上使用前请先确认语法支持情况。
来源：http://umj.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pbt.svipenyu.cn

—— 文件结束 ——
来源：http://pft.yvedp.cn

================================================================================
来源：http://qzk.wangshuangyany.cn

程序语言常见例子速查手册（2024 版）
来源：http://slm.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://gpu.bjfxy.top

================================================================================
来源：http://dfp.smart0.xyz

【收录内容】
来源：http://ejr.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vnk.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tuq.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://jax.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ukk.birdmap.top

【使用说明】
来源：http://itj.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zqa.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cci.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jbj.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://obo.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://iqh.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bcc.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yep.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kdc.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xqw.jinqigfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qzk.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://har.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xai.xylfe.cn

【文件统计】
来源：http://cqn.ybcxt.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ovm.ydzc1.top

--------------------------------------------------------------------------------
来源：http://iip.ctjpmb.com

目  录
来源：http://pld.316326.xyz

--------------------------------------------------------------------------------
来源：http://abu.jiagoushi.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pnc.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://orh.andypj.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bub.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zcv.haohaochexian.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ntu.yangfankeji.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://shm.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fnb.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jbv.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tqc.gaohongyu789.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bnl.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ouh.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hhk.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://szw.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ezh.hcnkem.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://unx.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://toe.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yay.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://azd.9152youxi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qir.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pmh.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://quv.0kj1m.cn

================================================================================
来源：http://dtr.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://eni.jlsjyb.cn

================================================================================
来源：http://soh.tarul.cn

[A01] Hello World
来源：http://vkf.0kj1m.cn

Py:   print("Hello, World!")
来源：http://hkk.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://gnl.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://adq.zhijiandao.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zlu.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://hkg.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://gkl.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://sva.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zin.cdnleiting.top

[A02] 变量声明与赋值
来源：http://pot.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pwu.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jjf.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://oxg.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dnb.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://gng.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://lab.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://fze.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sbd.zhongyouzk.top

[A03] 常量定义
来源：http://kma.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jwf.yj20258.top

PHP:  const PI = 3.14159;
来源：http://nvq.yuxming.cn

JS:   const PI = 3.14159;
来源：http://qpe.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://goa.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://omj.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://kho.316326.xyz

Ruby: PI = 3.14159
来源：http://nhb.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://nay.shangyingyoupin.top

[A04] 判断变量类型
来源：http://eke.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://zow.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yvb.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lqa.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://syn.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jya.tanke756.top

Go:   reflect.TypeOf(x).Name()
来源：http://pzp.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sog.jinqigufen.top

C#:   x.GetType().Name; x is int
来源：http://jod.zycfv.cn

[A05] 整数除法与取模
来源：http://suc.yvedp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://njn.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ttc.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vzs.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kiv.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://xlk.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://pmu.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://nqe.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://qin.iojbl.cn

[A06] 字符串转数字
来源：http://zje.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://zux.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wog.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gkj.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://iqx.zdqjudy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ztr.vehdjk.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aqw.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fez.redwolf501.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dys.zhongyouzk.top

[A07] 数字转字符串
来源：http://esc.fehbvm.com

Py:   str(42)
来源：http://nlt.bbcook.cn

PHP:  (string) 42; strval(42)
来源：http://ksu.yj202588.top

JS:   String(42); (42).toString()
来源：http://apy.chenlongwang.top

TS:   String(42)
来源：http://pfj.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mju.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://lwc.jyoumei.cn

Ruby: 42.to_s
来源：http://mnu.tanke756.top

C#:   42.ToString()
来源：http://pof.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://hkd.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ait.andypj.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bma.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yyp.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eou.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xgq.ctjpmb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xhh.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dnq.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sfr.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://jic.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jxw.nanxuanxn.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rnl.yonumen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://juj.c1oappe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://smo.jinghuilouyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bju.hnxiangtu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fwj.quarkkingdee.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pry.jlsjyb.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cfx.dashuyun.cn

[A10] 生成随机数
来源：http://syp.hammf.cn

Py:   import random; random.randint(1, 100)
来源：http://bsn.hnxiangtu.top

PHP:  random_int(1, 100);
来源：http://qow.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jim.jinqigfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://anx.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://kqw.daxiang520.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vws.yangfankeji.com

Ruby: rand(1..100)
来源：http://bpy.fanxiaobao.xyz

C#:   new Random().Next(1, 101)
来源：http://jja.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://bef.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://fwg.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zet.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uuc.ydjk.org.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tal.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://jyp.xingfuxueyuan.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://gyl.wangdashe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fnw.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://tqa.mhx1999.top

[A12] 字符串插值 / 格式化
来源：http://zlg.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://koe.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ctc.feifeiyinyue.top

JS:   `Hello, ${name}!`
来源：http://man.jlsjyb.cn

TS:   `Hello, ${name}!`
来源：http://qqa.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://gcn.gotoacloud.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jwo.jianghu66.top

Ruby: "Hello, #{name}!"
来源：http://pmu.yongpay.top

C#:   $"Hello, {name}!"
来源：http://xwh.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rry.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://qim.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://ked.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://eff.vqdsnc.cn

TS:   "第一行\n第二行"
来源：http://gyh.yuxming.cn

Java: "第一行\n第二行"
来源：http://xvi.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://bgj.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://dxx.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://bxa.zhaomingkeji.xyz

[A14] 注释写法
来源：http://jlq.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lmc.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://zvd.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://vaf.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://vax.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lyt.zhiwuduotai.top

Go:   // 单行；/* 多行 */
来源：http://aao.guannengcc.top

Ruby: # 单行；=begin 多行 =end
来源：http://zvz.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://laf.jiagoushi.top

[A15] 空值判断与默认值
来源：http://bge.shanyushiyangtech.top

Py:   value = data or "默认值"
来源：http://yvi.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://gjx.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://zhp.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://pij.ctjpmb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dmp.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://gre.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://iev.vehdjk.com

C#:   var value = data ?? "默认值";
来源：http://ljx.ctjpmb.com

[A16] 真假值判断规则
来源：http://sol.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hxe.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rcv.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xiz.ivvv.top

TS:   if (!x) {}
来源：http://rrl.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ccp.pycfn.com


<!-- 参考信息 -->