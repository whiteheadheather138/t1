代发 wailian999

[U93] JS：模板字符串
来源：http://zuc.hcnkem.com

`共 ${n} 条`
来源：http://doh.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://tbh.chenlongwang.top

const double = x => x * 2;
来源：http://aqk.tianlin.xyz

[U95] JS：Promise 包装
来源：http://xye.sweek.top

new Promise((resolve, reject) => {})
来源：http://aky.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://cih.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lps.cucudq.cn

[U97] JS：并发请求
来源：http://jgl.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lmf.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://swh.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://giv.guowangkeji.top

[U99] JS：事件监听
来源：http://gde.fktsv.cn

el.addEventListener("click", e => {})
来源：http://zli.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://gkf.ybcxt.top

document.querySelector(".item")
来源：http://kxn.316326.xyz

[U101] JS：classList 操作
来源：http://xvq.ydjk.org.cn

el.classList.toggle("active")
来源：http://ttp.hongshengwenyu.top

[U102] JS：本地存储
来源：http://ivz.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cnl.ybcxt.top

[U103] JS：定时器
来源：http://qgc.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pcb.jlsjyb.cn

[U104] JS：防抖
来源：http://pdo.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzr.mhx1999.top

[U105] JS：节流
来源：http://hwf.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jel.9152youxi.cn

[U106] JS：日期格式化
来源：http://jou.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bcb.ctjpmb.com

[U107] JS：数字千分位
来源：http://utr.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dvn.c1oappe.top

[U108] JS：随机整数
来源：http://ncn.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://auw.gaohongyu789.top

[U109] JS：数组分组
来源：http://szr.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://utq.hongshengwenyu.top

[U110] JS：数组分块
来源：http://hlr.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sua.yfazqb.com

[U111] JS：对象转 Map
来源：http://rit.xuanzx.com

new Map(Object.entries(obj))
来源：http://pqb.jiagoushi.top

[U112] JS：字符串补位
来源：http://grg.9152youxi.cn

"7".padStart(3, "0")
来源：http://nws.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://jel.chenzaomai.com

s.replaceAll("a", "b")
来源：http://aos.daria6918.cn

[U114] JS：JSON 深比较
来源：http://yjd.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://jsj.cashguo.top

[U115] JS：生成 UUID
来源：http://nfj.aizwys.cn

crypto.randomUUID()
来源：http://qlb.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://rzp.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://vtd.quarkkingdee.top

[U117] JS：单元测试
来源：http://eoc.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://afl.zhengqikj.top

[U118] JS：开发服务器
来源：http://att.meibo888.top

npm i -D vite;  npx vite
来源：http://dmh.hywenlv.cn

[U119] JS：生产构建
来源：http://fcu.jqgufenzy.top

npx vite build
来源：http://rnq.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://ydc.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://ieb.cdnleiting.top

================================================================================
来源：http://dxi.hesvh.cn

统计汇总
来源：http://pbi.hnxiangtu.top

================================================================================
来源：http://iri.guowangkeji.top

按语言统计（条）：
来源：http://vne.hysaishi.cn

Python ......... 252
来源：http://lpv.sjlbkw.cn

PHP ............ 252
来源：http://irc.chenlongwang.top

JavaScript ..... 252
来源：http://ssp.hesvh.cn

TypeScript ..... 212
来源：http://wrr.andypj.xyz

Java ........... 212
来源：http://yxh.aizwys.cn

Go ............. 212
来源：http://agi.tanke756.top

Ruby ........... 212
来源：http://wwb.wangdashe.top

C# ............. 212
来源：http://hzc.snrcjt.cn

C .............. 30
来源：http://kym.ybcxt.top

C++ ............ 30
来源：http://nyq.0kj1m.cn

SQL ............ 90
来源：http://qru.wangdashe.top

Bash ........... 80
来源：http://tdw.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://osa.zhaomingkeji.xyz

Swift .......... 15
来源：http://una.jianghu66.top

Lua ............ 10
来源：http://www.nwbrower.top

Perl ........... 10
来源：http://jsx.svipenyu.cn

Scala .......... 10
来源：http://olm.nanxinkj.top

------------------------------------
来源：http://fys.bbcook.cn

合计 ........... 2106 条
来源：http://pzg.zdbjq.cn

按章节统计：
来源：http://pdw.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tij.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zev.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kxv.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jok.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sjy.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cix.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vek.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dow.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://afz.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eyx.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dvo.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://srl.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xqd.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xyt.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fxs.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ocn.ppjwa.cn

Q SQL 专题                              90
来源：http://sht.sysykeji.top

R Bash 专题                             80
来源：http://bki.xinyue.icu

S C / C++ 专题                          60
来源：http://myb.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://yeh.bbcook.cn

U 高频实用片段                         120
来源：http://wpz.52xcode.cn

------------------------------------
来源：http://hsy.sjlbkw.cn

合计                                  2106 条
来源：http://vfq.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://nei.ybcxt.top

使用提醒
来源：http://qvo.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://dno.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zil.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fih.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nns.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lxc.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hzn.xziqi.cn

—— 文件结束 ——
来源：http://qhn.ydjk.org.cn

================================================================================
来源：http://nsi.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://bkx.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://rrz.52xcode.cn

================================================================================
来源：http://kuz.birdmap.top

【收录内容】
来源：http://tjo.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://khn.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://voc.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://uos.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://you.cqqwz.cn

【使用说明】
来源：http://zrp.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wbi.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yir.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ros.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wrf.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://icb.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wyz.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nps.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bzc.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zjs.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hpa.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dkv.aizwys.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zdt.dashuyun.cn

【文件统计】
来源：http://bsa.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yfn.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ghn.chenzaomai.com

目  录
来源：http://mll.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://dwf.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zok.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blj.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vwp.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qzd.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ybb.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xgr.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hfx.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yno.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fxo.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bkl.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bif.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vey.gogol.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://buh.ppjwa.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rbf.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xtj.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iww.andypj.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jxw.jiagoushi.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nhv.fanxiaobao.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tiy.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ucp.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ngt.ywan-chungtsiang.top

================================================================================
来源：http://qjs.yj20258.top

A. 基础语法与类型
来源：http://lzz.jqgfzy.top

================================================================================
来源：http://bja.meibo888.top

[A01] Hello World
来源：http://hzj.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://pxw.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://pke.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://etz.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pry.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://hpc.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://ufa.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://esq.zhixingplan.top

C#:   Console.WriteLine("Hello, World!");
来源：http://agj.shuidangran.top

[A02] 变量声明与赋值
来源：http://vfk.chenjidiqi.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://odt.zycfv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pkc.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://jzr.zdbjq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lmx.chenzaomai.com

Java: String name = "Alex"; int age = 20;
来源：http://wba.zycfv.cn

Go:   name := "Alex"; age := 20
来源：http://duv.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://rlr.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://cdi.haohaochexian.top

[A03] 常量定义
来源：http://xdb.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ekw.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://icg.birdmap.top

JS:   const PI = 3.14159;
来源：http://pgi.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://hfd.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://qwk.yj20258888.top

Go:   const PI = 3.14159
来源：http://pcu.tanke756.top

Ruby: PI = 3.14159
来源：http://bax.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://lff.ydzc1.top

[A04] 判断变量类型
来源：http://wjz.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://lws.kuanghao11.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gyd.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://viq.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://stm.yonumen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bwy.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://acl.xingfuxueyuan.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://qwe.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://flk.gaohongyu789.top

[A05] 整数除法与取模
来源：http://bkr.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ilc.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tig.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fya.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xiu.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://daq.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://dsi.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://gxs.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://ttd.meibo888.top

[A06] 字符串转数字
来源：http://fvl.meibo888.top

Py:   int("42"); float("3.14")
来源：http://glm.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pgc.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uxc.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://kjf.jqgfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fgv.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ypb.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hbr.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eic.ppjwa.cn

[A07] 数字转字符串
来源：http://ndj.hysaishi.cn

Py:   str(42)
来源：http://cjz.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://qqh.guowangkeji.top

JS:   String(42); (42).toString()
来源：http://cqc.yj20258.top

TS:   String(42)
来源：http://dpq.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ymc.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://tor.fengsongda.top

Ruby: 42.to_s
来源：http://rui.mhx1999.top

C#:   42.ToString()
来源：http://wsg.hesvh.cn

[A08] 取整与四舍五入
来源：http://eow.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://avt.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qrm.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hfb.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tre.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ohm.gogol.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ptw.haohaochexian.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pwv.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lwk.epnwcf.com

[A09] 绝对值与最大最小值
来源：http://aye.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wqk.sysykeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://peb.xinyue.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://srl.jlsjyb.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rrt.zhixingplan.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ikr.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nji.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yru.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jmi.zhongyouzk.top

[A10] 生成随机数
来源：http://lkc.xinyue.icu

Py:   import random; random.randint(1, 100)
来源：http://zhm.sysykeji.top

PHP:  random_int(1, 100);
来源：http://lkh.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sqj.hnqzz.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zpm.jinghuilouyu.cn

Java: new Random().nextInt(100) + 1
来源：http://dcn.chenjidiqi.icu

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xdb.yuanzhike.top

Ruby: rand(1..100)
来源：http://rlk.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://uyk.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://mlb.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://vdy.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pzy.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mnl.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dam.ppjwa.cn

Java: x > 0 ? "yes" : "no"
来源：http://ctk.xingfuxueyuan.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://rtt.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vew.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://rpi.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://sya.nanxuanxn.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://txw.cqqwz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nls.cashguo.top

JS:   `Hello, ${name}!`
来源：http://bse.hysaishi.cn

TS:   `Hello, ${name}!`
来源：http://jnp.jiagoushi.top

Java: "Hello, %s!".formatted(name)
来源：http://tok.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yjf.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://uwp.sjlbkw.cn

C#:   $"Hello, {name}!"
来源：http://unq.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://izn.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://umi.0kj1m.cn

PHP:  "第一行\n第二行"
来源：http://leu.yonumen.top

JS:   "第一行\n第二行"
来源：http://ljl.cucudq.cn

TS:   "第一行\n第二行"
来源：http://djb.vehdjk.com

Java: "第一行\n第二行"
来源：http://zlu.pycfn.com

Go:   "第一行\n第二行"
来源：http://vig.iojbl.cn

Ruby: "第一行\n第二行"
来源：http://jcc.ydzc1.top

C#:   "第一行\n第二行"
来源：http://huk.zhongyouzk.top

[A14] 注释写法
来源：http://uge.yanxiufei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kqv.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hqg.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://dnu.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://cnm.yuxming.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ofd.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://lkm.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://yui.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://why.epnwcf.com

[A15] 空值判断与默认值
来源：http://gwp.yanxiufei.cn

Py:   value = data or "默认值"
来源：http://uez.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://zjf.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://kaz.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://epi.cucudq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dar.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://kdu.shanyushiyangtech.top

Ruby: value = data || "默认值"
来源：http://qbk.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://qyr.yuxming.cn

[A16] 真假值判断规则
来源：http://rdl.hesvh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ipt.xziqi.cn


<!-- 参考信息 -->