代发 wailian999

[U101] JS：classList 操作
来源：http://uns.birdmap.top

el.classList.toggle("active")
来源：http://cif.gogol.net.cn

[U102] JS：本地存储
来源：http://thv.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dnn.feifeiyinyue.top

[U103] JS：定时器
来源：http://vws.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ani.hfpthk.cn

[U104] JS：防抖
来源：http://lwn.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hve.svipenyu.cn

[U105] JS：节流
来源：http://zvc.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rff.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://jpg.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cjn.gaohongyu789.top

[U107] JS：数字千分位
来源：http://wqf.xingfuxueyuan.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bbf.pycfn.com

[U108] JS：随机整数
来源：http://rhu.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rsw.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://sdj.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://mgy.zhongyouzk.top

[U110] JS：数组分块
来源：http://lcl.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hgw.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://zrx.gzhubu.top

new Map(Object.entries(obj))
来源：http://wsr.zdqjudy.top

[U112] JS：字符串补位
来源：http://lyh.jianghu66.top

"7".padStart(3, "0")
来源：http://nar.shuidangran.top

[U113] JS：正则替换全部
来源：http://npg.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://oqa.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://vxz.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qqm.hammf.cn

[U115] JS：生成 UUID
来源：http://msu.uphjek.com

crypto.randomUUID()
来源：http://ysi.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://gyj.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://zir.ctjpmb.com

[U117] JS：单元测试
来源：http://qna.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://wot.bbcook.cn

[U118] JS：开发服务器
来源：http://bdi.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://sxj.cashguo.top

[U119] JS：生产构建
来源：http://tqt.0kj1m.cn

npx vite build
来源：http://wji.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://aty.havefunace.top

import.meta.env.VITE_API_URL
来源：http://ilt.mhx1999.top

================================================================================
来源：http://olk.yj20258.top

统计汇总
来源：http://mys.hywenlv.cn

================================================================================
来源：http://jey.nanxinkj.top

按语言统计（条）：
来源：http://cmj.ivvv.top

Python ......... 252
来源：http://xee.zhengqikj.top

PHP ............ 252
来源：http://wmx.wangdashe.top

JavaScript ..... 252
来源：http://way.fengsongda.top

TypeScript ..... 212
来源：http://kjj.sjlbkw.cn

Java ........... 212
来源：http://zvk.xziqi.cn

Go ............. 212
来源：http://vrn.wangdashe.top

Ruby ........... 212
来源：http://dns.jinqigufen.top

C# ............. 212
来源：http://omy.jqgfzy.top

C .............. 30
来源：http://uox.gzhubu.top

C++ ............ 30
来源：http://hdx.shzxlz.cn

SQL ............ 90
来源：http://lub.xziqi.cn

Bash ........... 80
来源：http://sma.ydzc1.top

Kotlin ......... 15
来源：http://ivc.jinyuanbaomall.cn

Swift .......... 15
来源：http://vgj.sweek.top

Lua ............ 10
来源：http://kji.shangyingyoupin.top

Perl ........... 10
来源：http://oqk.nanxuanxn.top

Scala .......... 10
来源：http://dsp.aibaodan.cn

------------------------------------
来源：http://gph.yanxiufei.cn

合计 ........... 2106 条
来源：http://way.cucudq.cn

按章节统计：
来源：http://sxi.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rym.jianghu66.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gcv.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yeh.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ysu.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://owc.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mcv.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oao.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zbm.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://daz.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://exk.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://whw.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xbw.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rjz.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://thj.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jqz.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gwl.pengpengdd.cyou

Q SQL 专题                              90
来源：http://dcp.jqgfzy.top

R Bash 专题                             80
来源：http://juf.ydzc1.top

S C / C++ 专题                          60
来源：http://zds.xziqi.cn

T 其他语言补充                          60
来源：http://hqk.nanxuanxn.top

U 高频实用片段                         120
来源：http://wrr.cheryme.top

------------------------------------
来源：http://eus.tian-w.cn

合计                                  2106 条
来源：http://cpv.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://nbd.zhoulong.xyz

使用提醒
来源：http://dnz.daxiang520.top

--------------------------------------------------------------------------------
来源：http://lrz.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sni.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dfk.jinghuilouyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gtl.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bfp.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dlm.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://hrh.uphjek.com

================================================================================
来源：http://nio.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://afc.yvedp.cn

Common Programming Examples Cheat Book
来源：http://bbq.shuidangran.top

================================================================================
来源：http://cqb.yangfankeji.com

【收录内容】
来源：http://ouj.shuidangran.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kou.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dps.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://ybs.redwolf501.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://thy.yvedp.cn

【使用说明】
来源：http://dim.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jgx.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fnc.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uqa.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aov.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://itc.cheryme.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hzn.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://asx.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qih.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dtk.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ypt.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qud.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://prt.ydjk.org.cn

【文件统计】
来源：http://utf.yuanzhike.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pbc.shuidangran.top

--------------------------------------------------------------------------------
来源：http://gkq.guannengcc.top

目  录
来源：http://vzm.yj20258888.top

--------------------------------------------------------------------------------
来源：http://nkd.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nvj.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bgc.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oxz.chenlongwang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dwp.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://toz.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wzo.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wpf.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ofs.hnqzz.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cbb.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ihg.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://abd.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xcg.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://amw.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cco.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tdi.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rdb.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kri.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ezf.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yna.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwi.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jnv.tanke756.top

================================================================================
来源：http://stp.havefunace.top

A. 基础语法与类型
来源：http://eca.feifeiyinyue.top

================================================================================
来源：http://qgk.pycfn.com

[A01] Hello World
来源：http://nor.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://blk.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://koj.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://dkt.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wjk.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://wkg.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://hjm.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://phs.tarul.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xmt.yj20258.top

[A02] 变量声明与赋值
来源：http://jhe.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ncm.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mtu.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://mzh.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hhu.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://lpi.yvedp.cn

Go:   name := "Alex"; age := 20
来源：http://xpe.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://vzu.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://vjo.nanxuanxn.top

[A03] 常量定义
来源：http://ixd.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://juo.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://rbh.fehbvm.com

JS:   const PI = 3.14159;
来源：http://jxy.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://lcf.hfpthk.cn

Java: static final double PI = 3.14159;
来源：http://eiv.xziqi.cn

Go:   const PI = 3.14159
来源：http://pwv.yuanzhike.top

Ruby: PI = 3.14159
来源：http://wrp.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://hdr.wangshuangyany.cn

[A04] 判断变量类型
来源：http://ifq.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pca.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xtk.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ubs.andypj.xyz

TS:   typeof x; x instanceof Date
来源：http://fqe.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ryi.gaohongyu789.top

Go:   reflect.TypeOf(x).Name()
来源：http://hxs.fanxiaobao.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://nmm.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://gml.mhx1999.top

[A05] 整数除法与取模
来源：http://ydi.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://syx.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hpg.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://piw.c1oappe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jxv.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://egw.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://qfs.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://gbn.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://glt.xinyue.icu

[A06] 字符串转数字
来源：http://msh.tanke756.top

Py:   int("42"); float("3.14")
来源：http://bih.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hqm.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bqx.yj20258.top

TS:   parseInt("42", 10); Number("42")
来源：http://idz.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sdg.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nvo.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ymq.xylfe.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pum.zdqjudy.top

[A07] 数字转字符串
来源：http://djd.chenzaomai.com

Py:   str(42)
来源：http://zel.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://erq.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://iss.gotoacloud.top

TS:   String(42)
来源：http://ozd.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kao.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://cma.cdnleiting.top

Ruby: 42.to_s
来源：http://qys.aibaodan.cn

C#:   42.ToString()
来源：http://nlb.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://btb.aibaodan.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jbi.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jkx.hcnkem.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ghj.ydjk.org.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://csx.redwolf501.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zaf.ywan-chungtsiang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sdm.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qea.ctjpmb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://erx.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://ahd.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cde.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oui.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vxk.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nuy.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://evl.chenzaomai.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://abd.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dtm.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lio.yuanzhike.top

[A10] 生成随机数
来源：http://dhm.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://css.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://deu.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ueb.xziqi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jli.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://hky.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pjc.ywan-chungtsiang.top

Ruby: rand(1..100)
来源：http://jmt.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://beq.ivvv.top

[A11] 条件表达式（三元）
来源：http://ude.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://wem.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yyn.bbcook.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gbp.redwolf501.top

TS:   x > 0 ? "yes" : "no"
来源：http://jnu.jiagoushi.top

Java: x > 0 ? "yes" : "no"
来源：http://lqc.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qkn.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://syt.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://xed.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://kwh.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ywt.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wah.svipenyu.cn

JS:   `Hello, ${name}!`
来源：http://hjm.tanke756.top

TS:   `Hello, ${name}!`
来源：http://osm.snrcjt.cn

Java: "Hello, %s!".formatted(name)
来源：http://psw.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nyh.birdmap.top

Ruby: "Hello, #{name}!"
来源：http://ddh.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://uch.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dgm.kuanghao11.cn

Py:   "第一行\n第二行"
来源：http://mlt.ppjwa.cn

PHP:  "第一行\n第二行"
来源：http://nqh.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://clj.tarul.cn

TS:   "第一行\n第二行"
来源：http://xsv.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://kmi.zhengqikj.top

Go:   "第一行\n第二行"
来源：http://qwn.cqqwz.cn

Ruby: "第一行\n第二行"
来源：http://mlx.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://lbu.zhoulong.xyz

[A14] 注释写法
来源：http://mtt.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://uqb.zhongyouzk.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ngs.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://coq.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://ckg.meibo888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pqo.jinqigufen.top

Go:   // 单行；/* 多行 */
来源：http://chk.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ldz.hysaishi.cn

C#:   // 单行；/* 多行 */
来源：http://jwo.fengsongda.top

[A15] 空值判断与默认值
来源：http://uva.cucudq.cn

Py:   value = data or "默认值"
来源：http://xqm.sweek.top

PHP:  $value = $data ?? "默认值";
来源：http://zei.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://pkr.sufxvd.cn

TS:   const value = data ?? "默认值";
来源：http://koh.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uhp.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://tef.vehdjk.com

Ruby: value = data || "默认值"
来源：http://lwv.sweek.top

C#:   var value = data ?? "默认值";
来源：http://ygc.yangfankeji.com

[A16] 真假值判断规则
来源：http://iqa.yfazqb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yza.hammf.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eoc.svipenyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://apj.jyoumei.cn

TS:   if (!x) {}
来源：http://age.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pox.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mzp.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://gxq.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zwm.xinyue.icu

[A17] 位运算
来源：http://nzj.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mbd.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jso.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldj.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zlu.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhk.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ltv.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mga.hfpthk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zdf.feifeiyinyue.top


<!-- 参考信息 -->