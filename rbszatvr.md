代发 wailian999

[U97] JS：并发请求
来源：http://abt.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jgm.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://nbe.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dnx.gotoacloud.top

[U99] JS：事件监听
来源：http://siy.fktsv.cn

el.addEventListener("click", e => {})
来源：http://hqe.snrcjt.cn

[U100] JS：DOM 查询
来源：http://zwg.hammf.cn

document.querySelector(".item")
来源：http://nnx.ctjpmb.com

[U101] JS：classList 操作
来源：http://yxc.nanxinkj.top

el.classList.toggle("active")
来源：http://nlc.wangdashe.top

[U102] JS：本地存储
来源：http://tyu.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tqw.xuetiantiany.cn

[U103] JS：定时器
来源：http://ksn.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sna.vehdjk.com

[U104] JS：防抖
来源：http://lzd.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yci.iojbl.cn

[U105] JS：节流
来源：http://mqk.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wjy.daxiang520.top

[U106] JS：日期格式化
来源：http://kpt.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bht.vqdsnc.cn

[U107] JS：数字千分位
来源：http://cvz.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lbo.kuanghao11.cn

[U108] JS：随机整数
来源：http://rcj.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://odv.zdqjudy.top

[U109] JS：数组分组
来源：http://his.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://duj.hnxiangtu.top

[U110] JS：数组分块
来源：http://eom.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zao.9152youxi.cn

[U111] JS：对象转 Map
来源：http://mye.dianchejie.cn

new Map(Object.entries(obj))
来源：http://btn.xylfe.cn

[U112] JS：字符串补位
来源：http://qkn.dianchejie.cn

"7".padStart(3, "0")
来源：http://ycb.bbcook.cn

[U113] JS：正则替换全部
来源：http://lox.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://ike.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://sjv.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ixb.ctjpmb.com

[U115] JS：生成 UUID
来源：http://pbr.yj202588.top

crypto.randomUUID()
来源：http://elt.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://soq.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://hvm.yonumen.top

[U117] JS：单元测试
来源：http://xdk.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://pge.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://hgl.c1oappe.top

npm i -D vite;  npx vite
来源：http://mnp.bjfxy.top

[U119] JS：生产构建
来源：http://hwz.hywenlv.cn

npx vite build
来源：http://hfq.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://pyj.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://fml.daxiang520.top

================================================================================
来源：http://uba.aibaodan.cn

统计汇总
来源：http://gzq.shanyushiyangtech.top

================================================================================
来源：http://fue.yanxiufei.cn

按语言统计（条）：
来源：http://jew.birdmap.top

Python ......... 252
来源：http://szy.hnqzz.top

PHP ............ 252
来源：http://rrk.ydjk.org.cn

JavaScript ..... 252
来源：http://bpt.chenlongwang.top

TypeScript ..... 212
来源：http://ruq.cashguo.top

Java ........... 212
来源：http://ltn.vqdsnc.cn

Go ............. 212
来源：http://lgn.bjfxy.top

Ruby ........... 212
来源：http://wex.hnxiangtu.top

C# ............. 212
来源：http://yap.guannengcc.top

C .............. 30
来源：http://dup.hysaishi.cn

C++ ............ 30
来源：http://efo.52xcode.cn

SQL ............ 90
来源：http://tvy.shanyushiyangkeji.top

Bash ........... 80
来源：http://bsk.ehwqpu.com

Kotlin ......... 15
来源：http://uqn.yfazqb.com

Swift .......... 15
来源：http://wtk.yuanzhike.top

Lua ............ 10
来源：http://vax.aibaodan.cn

Perl ........... 10
来源：http://lsq.hesvh.cn

Scala .......... 10
来源：http://mfo.zdqjudy.top

------------------------------------
来源：http://fop.yfazqb.com

合计 ........... 2106 条
来源：http://gut.shanyushiyangkeji.top

按章节统计：
来源：http://zbr.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ncd.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kxf.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://irx.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://unm.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mrw.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vht.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mfu.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jph.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jxh.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vur.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://anl.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cfm.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hyf.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ypi.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hbg.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rdm.quarkkingdee.top

Q SQL 专题                              90
来源：http://ejr.fehbvm.com

R Bash 专题                             80
来源：http://efm.hnxiangtu.top

S C / C++ 专题                          60
来源：http://zhv.hywenlv.cn

T 其他语言补充                          60
来源：http://rzg.yvedp.cn

U 高频实用片段                         120
来源：http://pvn.yj20258888.top

------------------------------------
来源：http://jpd.hammf.cn

合计                                  2106 条
来源：http://iga.gzhubu.top

--------------------------------------------------------------------------------
来源：http://yxz.jinghuilouyu.cn

使用提醒
来源：http://pwx.vehdjk.com

--------------------------------------------------------------------------------
来源：http://umv.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://keu.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gav.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iaf.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gfp.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ktl.tarul.cn

—— 文件结束 ——
来源：http://jnj.jinqigfzy.top

================================================================================
来源：http://ihx.jqgufenzy.top

程序语言常见例子速查手册（2024 版）
来源：http://god.vehdjk.com

Common Programming Examples Cheat Book
来源：http://wnu.jinqigfzy.top

================================================================================
来源：http://bjd.feifeiyinyue.top

【收录内容】
来源：http://drm.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yau.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://moh.cashguo.top

SQL · Bash · C · C++
来源：http://bfv.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ifn.smart0.xyz

【使用说明】
来源：http://pdg.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tcj.fktsv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yav.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xfl.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eyw.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rrb.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sus.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ilv.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wrt.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lol.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xbt.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ich.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nvc.mhx1999.top

【文件统计】
来源：http://kwg.sufxvd.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ucb.yj20258888.top

--------------------------------------------------------------------------------
来源：http://bnb.fengsongda.top

目  录
来源：http://yxw.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://lcm.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ujp.jqgufenzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mhw.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ouo.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://npe.xuanzx.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wft.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uss.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qks.hammf.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cog.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kmr.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gvc.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jre.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sxf.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kpp.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fcb.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gsl.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zzy.zhijiandao.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wgi.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gqm.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zla.shuidangran.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ppd.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lvh.sysykeji.top

================================================================================
来源：http://qjg.shuidangran.top

A. 基础语法与类型
来源：http://lqd.ppjwa.cn

================================================================================
来源：http://kwu.sysykeji.top

[A01] Hello World
来源：http://pps.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://ukr.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://rgv.birdmap.top

JS:   console.log("Hello, World!");
来源：http://wqx.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ipy.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://aic.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://wlv.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://gkh.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://aaz.ybcxt.top

[A02] 变量声明与赋值
来源：http://djl.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cjw.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://twf.hywenlv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bne.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ige.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://bip.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://dtm.nanxuanxn.top

Ruby: name = "Alex"; age = 20
来源：http://sfc.jinghuilouyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fwg.aizwys.cn

[A03] 常量定义
来源：http://deq.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bbv.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://mye.316326.xyz

JS:   const PI = 3.14159;
来源：http://nuo.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://mgl.tianlin.xyz

Java: static final double PI = 3.14159;
来源：http://hjf.aibaodan.cn

Go:   const PI = 3.14159
来源：http://hbw.yj20258888.top

Ruby: PI = 3.14159
来源：http://vvv.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://mkh.cashguo.top

[A04] 判断变量类型
来源：http://qlv.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://kpx.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://owh.jlsjyb.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kvf.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://mrn.havefunace.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nvl.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ayd.dianchejie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hog.yonumen.top

C#:   x.GetType().Name; x is int
来源：http://yhl.daria6918.cn

[A05] 整数除法与取模
来源：http://gah.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gjb.shanyushiyangtech.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bae.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ovm.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zwg.quarkkingdee.top

Java: 7 / 2; 7 % 2
来源：http://wtd.daria6918.cn

Go:   7 / 2; 7 % 2
来源：http://bga.yongpay.top

Ruby: 7 / 2; 7 % 2
来源：http://atj.shangyingyoupin.top

C#:   7 / 2; 7 % 2
来源：http://yel.ybcxt.top

[A06] 字符串转数字
来源：http://gft.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://vul.xziqi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lpv.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xun.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://hiw.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kqz.hammf.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nmn.c1oappe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tbm.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mqr.fehbvm.com

[A07] 数字转字符串
来源：http://rnd.sjlbkw.cn

Py:   str(42)
来源：http://egk.jinyuanbaomall.cn

PHP:  (string) 42; strval(42)
来源：http://cau.yj20258888.top

JS:   String(42); (42).toString()
来源：http://gbu.zdbjq.cn

TS:   String(42)
来源：http://edk.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jzb.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://fig.hcnkem.com

Ruby: 42.to_s
来源：http://pco.0kj1m.cn

C#:   42.ToString()
来源：http://rko.jinqigufen.top

[A08] 取整与四舍五入
来源：http://esi.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ptw.cucudq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lgc.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mji.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://han.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bqa.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qmq.gzhubu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eev.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ivu.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://nla.yangfankeji.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hjh.jqgufenzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ovk.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mwj.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vhb.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cfm.yuanzhike.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mjg.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zmc.sysykeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tet.sweek.top

[A10] 生成随机数
来源：http://hxw.mhx1999.top

Py:   import random; random.randint(1, 100)
来源：http://ylm.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://vtw.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pkr.xuanzx.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uov.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://adt.shangyingyoupin.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xbt.chenzaomai.com

Ruby: rand(1..100)
来源：http://blh.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://ucs.hammf.cn

[A11] 条件表达式（三元）
来源：http://ifm.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://orm.fengsongda.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://umr.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kzq.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ksh.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://ijy.52xcode.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tio.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ywf.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uhp.gaohongyu789.top

[A12] 字符串插值 / 格式化
来源：http://vqp.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eca.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zit.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://jul.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://fos.tianlin.xyz

Java: "Hello, %s!".formatted(name)
来源：http://kzi.dianchejie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dmb.hesvh.cn

Ruby: "Hello, #{name}!"
来源：http://syd.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://aad.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://piy.ybcxt.top

Py:   "第一行\n第二行"
来源：http://wwi.tanke756.top

PHP:  "第一行\n第二行"
来源：http://pkz.tanke756.top

JS:   "第一行\n第二行"
来源：http://jjn.snrcjt.cn

TS:   "第一行\n第二行"
来源：http://fzg.haohaochexian.top

Java: "第一行\n第二行"
来源：http://det.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://ube.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://ltp.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://cas.quarkkingdee.top

[A14] 注释写法
来源：http://kqw.cheryme.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kdi.zdbjq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://txv.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://fbr.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://eqv.shuidangran.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lsj.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://jfo.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rfl.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://puk.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://fbo.yueranfly.top

Py:   value = data or "默认值"
来源：http://elm.fktsv.cn

PHP:  $value = $data ?? "默认值";
来源：http://uwy.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://odj.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://wfp.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bbc.sxryk.cn

Go:   if data == "" { data = "默认值" }
来源：http://mwg.sxryk.cn

Ruby: value = data || "默认值"
来源：http://igp.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://xkg.meibo888.top

[A16] 真假值判断规则
来源：http://egf.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lcw.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eli.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cgy.gotoacloud.top

TS:   if (!x) {}
来源：http://uiz.hywenlv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mun.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ofs.yuxming.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ydw.dianchejie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lcp.xuanzx.com

[A17] 位运算
来源：http://gsn.jianghu66.top


<!-- 参考信息 -->