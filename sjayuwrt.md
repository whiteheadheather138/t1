代发 wailian999

[U97] JS：并发请求
来源：http://bbx.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ngh.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://gun.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dlh.zhixingplan.top

[U99] JS：事件监听
来源：http://cly.hcnkem.com

el.addEventListener("click", e => {})
来源：http://ciq.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://ana.gogol.net.cn

document.querySelector(".item")
来源：http://bxj.ybcxt.top

[U101] JS：classList 操作
来源：http://avc.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://tyt.hcnkem.com

[U102] JS：本地存储
来源：http://kyd.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dcp.zhongyouzk.top

[U103] JS：定时器
来源：http://evl.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tii.wangdashe.top

[U104] JS：防抖
来源：http://qfz.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ivx.hcnkem.com

[U105] JS：节流
来源：http://qff.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zai.cashguo.top

[U106] JS：日期格式化
来源：http://tuc.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://crs.zhijiandao.cn

[U107] JS：数字千分位
来源：http://odi.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://suf.gotoacloud.top

[U108] JS：随机整数
来源：http://mlt.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zer.hnqzz.top

[U109] JS：数组分组
来源：http://qeg.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://xzi.zhongyouzk.top

[U110] JS：数组分块
来源：http://zmv.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://akj.yj20258888.top

[U111] JS：对象转 Map
来源：http://hxz.svipenyu.cn

new Map(Object.entries(obj))
来源：http://jsn.ppjwa.cn

[U112] JS：字符串补位
来源：http://dfn.gaohongyu789.top

"7".padStart(3, "0")
来源：http://xto.xziqi.cn

[U113] JS：正则替换全部
来源：http://qic.snrcjt.cn

s.replaceAll("a", "b")
来源：http://qjv.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://fev.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vzq.hesvh.cn

[U115] JS：生成 UUID
来源：http://tjn.fanxiaobao.xyz

crypto.randomUUID()
来源：http://ezr.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://aif.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://lbs.ctjpmb.com

[U117] JS：单元测试
来源：http://llm.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://qzr.sjlbkw.cn

[U118] JS：开发服务器
来源：http://erl.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://jux.ppjwa.cn

[U119] JS：生产构建
来源：http://gwq.guowangkeji.top

npx vite build
来源：http://ffl.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://wcl.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://jeu.yj20258.top

================================================================================
来源：http://see.aizwys.cn

统计汇总
来源：http://sye.cqqwz.cn

================================================================================
来源：http://qfw.9152youxi.cn

按语言统计（条）：
来源：http://jwd.zhijiandao.cn

Python ......... 252
来源：http://ljv.tian-w.cn

PHP ............ 252
来源：http://cru.cashguo.top

JavaScript ..... 252
来源：http://ycs.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://ocw.zhengqikj.top

Java ........... 212
来源：http://eaz.zhengqikj.top

Go ............. 212
来源：http://lmb.epnwcf.com

Ruby ........... 212
来源：http://mpl.guannengcc.top

C# ............. 212
来源：http://wgd.jianghu66.top

C .............. 30
来源：http://yfg.snrcjt.cn

C++ ............ 30
来源：http://cjd.wangshuangyany.cn

SQL ............ 90
来源：http://omz.shangyingyoupin.top

Bash ........... 80
来源：http://qba.meibo888.top

Kotlin ......... 15
来源：http://fvl.mhx1999.top

Swift .......... 15
来源：http://qjd.gaohongyu789.top

Lua ............ 10
来源：http://hhv.ppjwa.cn

Perl ........... 10
来源：http://ytf.ivvv.top

Scala .......... 10
来源：http://nip.dianchejie.cn

------------------------------------
来源：http://ubk.ybcxt.top

合计 ........... 2106 条
来源：http://nci.hesvh.cn

按章节统计：
来源：http://zow.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kbf.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dic.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rhb.xylfe.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://huv.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dvl.meibo888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sdy.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lob.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://olu.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vax.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nmp.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cfd.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uda.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uzj.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://juq.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vgv.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://afo.redwolf501.top

Q SQL 专题                              90
来源：http://qtl.snrcjt.cn

R Bash 专题                             80
来源：http://cgp.bjfxy.top

S C / C++ 专题                          60
来源：http://fbj.vqdsnc.cn

T 其他语言补充                          60
来源：http://khe.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://xnl.cdnleiting.top

------------------------------------
来源：http://aww.jiagoushi.top

合计                                  2106 条
来源：http://xec.sxryk.cn

--------------------------------------------------------------------------------
来源：http://dyn.haohaochexian.top

使用提醒
来源：http://gkx.tarul.cn

--------------------------------------------------------------------------------
来源：http://jnl.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jfc.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vxn.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gnv.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wfk.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://phn.shangyingyoupin.top

—— 文件结束 ——
来源：http://nub.yj20258.top

================================================================================
来源：http://gan.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://lld.fzhhl.top

Common Programming Examples Cheat Book
来源：http://jjh.gotoacloud.top

================================================================================
来源：http://mrf.nanxinkj.top

【收录内容】
来源：http://lzg.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nwt.nanxuanxn.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wje.redwolf501.top

SQL · Bash · C · C++
来源：http://jyx.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rqe.xylfe.cn

【使用说明】
来源：http://iok.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bqg.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xdg.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://veh.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fae.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cao.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uwu.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vmn.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rli.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wrr.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hlm.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xkp.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bit.jinyuanbaomall.cn

【文件统计】
来源：http://pou.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tjf.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://nrq.hysaishi.cn

目  录
来源：http://ifq.aizwys.cn

--------------------------------------------------------------------------------
来源：http://yle.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pyw.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gak.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://scr.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://osw.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dfi.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lpk.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qsi.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ryl.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aaz.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://trl.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rqp.sufxvd.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mgl.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jpc.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ejz.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ung.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bue.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cwi.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lmg.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gxk.pengpengdd.cyou

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yab.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fyw.ybcxt.top

================================================================================
来源：http://vmt.wangdashe.top

A. 基础语法与类型
来源：http://nnq.ydzc1.top

================================================================================
来源：http://sum.shuidangran.top

[A01] Hello World
来源：http://rdr.nanxinkj.top

Py:   print("Hello, World!")
来源：http://byr.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://mvz.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://ues.zhijiandao.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yth.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://ytv.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://ytb.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://dne.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nmw.gaohongyu789.top

[A02] 变量声明与赋值
来源：http://irk.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lyc.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qyv.yonumen.top

JS:   let name = "Alex"; const age = 20;
来源：http://ofa.gzhubu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jtl.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://kwz.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://scl.jiagoushi.top

Ruby: name = "Alex"; age = 20
来源：http://sol.snrcjt.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vja.iojbl.cn

[A03] 常量定义
来源：http://sdf.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://buy.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://iib.nwbrower.top

JS:   const PI = 3.14159;
来源：http://sbu.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://ttc.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://djm.redwolf501.top

Go:   const PI = 3.14159
来源：http://xtd.dashuyun.cn

Ruby: PI = 3.14159
来源：http://dan.tanke756.top

C#:   const double PI = 3.14159;
来源：http://ybp.bjfxy.top

[A04] 判断变量类型
来源：http://lsn.uphjek.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://lmj.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pyz.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vbj.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://cya.fengsongda.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ppw.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gzp.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://zvl.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://uqu.yueranfly.top

[A05] 整数除法与取模
来源：http://wuu.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bwo.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://paq.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xic.chenlongwang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vcx.ybcxt.top

Java: 7 / 2; 7 % 2
来源：http://tcv.tianlin.xyz

Go:   7 / 2; 7 % 2
来源：http://caj.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://oev.zhongyouzk.top

C#:   7 / 2; 7 % 2
来源：http://izb.havefunace.top

[A06] 字符串转数字
来源：http://tgk.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://kgt.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cig.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mlf.ppjwa.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ylh.ctjpmb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hbi.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ius.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://uil.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dzj.52xcode.cn

[A07] 数字转字符串
来源：http://zdx.jianghu66.top

Py:   str(42)
来源：http://rlw.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://gsb.tian-w.cn

JS:   String(42); (42).toString()
来源：http://rpb.snrcjt.cn

TS:   String(42)
来源：http://vxg.yangfankeji.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://duv.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://jnu.birdmap.top

Ruby: 42.to_s
来源：http://yhf.52xcode.cn

C#:   42.ToString()
来源：http://cye.vqdsnc.cn

[A08] 取整与四舍五入
来源：http://dqw.svipenyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qlc.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://slr.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://plp.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ngo.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://emy.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mxl.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ebh.fengsongda.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://muj.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://pou.jqgfzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ajx.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ing.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://klz.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ysq.sysykeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vys.yueranfly.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vyj.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jgs.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://olv.zdbjq.cn

[A10] 生成随机数
来源：http://paa.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://ghq.vqdsnc.cn

PHP:  random_int(1, 100);
来源：http://sfl.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yty.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rwr.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://peu.ivvv.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vjg.yuanzhike.top

Ruby: rand(1..100)
来源：http://irs.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://mpz.xylfe.cn

[A11] 条件表达式（三元）
来源：http://upi.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://ubt.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pwj.zhengqikj.top

JS:   x > 0 ? "yes" : "no"
来源：http://naq.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ytb.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://frs.yj20258888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lud.fktsv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hmm.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://qxo.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://dpq.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hft.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vzh.hnqzz.top

JS:   `Hello, ${name}!`
来源：http://rds.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://seu.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://oix.zdqjudy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tde.jinghuilouyu.cn

Ruby: "Hello, #{name}!"
来源：http://rmq.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://muf.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hun.hammf.cn

Py:   "第一行\n第二行"
来源：http://rzd.kuanghao11.cn

PHP:  "第一行\n第二行"
来源：http://nod.ybcxt.top

JS:   "第一行\n第二行"
来源：http://chp.sweek.top

TS:   "第一行\n第二行"
来源：http://zzp.tanke756.top

Java: "第一行\n第二行"
来源：http://lxk.andypj.xyz

Go:   "第一行\n第二行"
来源：http://smm.redwolf501.top

Ruby: "第一行\n第二行"
来源：http://aeu.vehdjk.com

C#:   "第一行\n第二行"
来源：http://rtx.sjlbkw.cn

[A14] 注释写法
来源：http://cdo.xuetiantiany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fed.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jsc.jinghuilouyu.cn

JS:   // 单行；/* 多行 */
来源：http://xev.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://jfr.hcnkem.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jky.jinghuilouyu.cn

Go:   // 单行；/* 多行 */
来源：http://orm.mhx1999.top

Ruby: # 单行；=begin 多行 =end
来源：http://cdq.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://ekb.cqqwz.cn

[A15] 空值判断与默认值
来源：http://ile.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://txa.cucudq.cn

PHP:  $value = $data ?? "默认值";
来源：http://lby.jinqigfzy.top

JS:   const value = data ?? "默认值";
来源：http://qec.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://irg.xingfuxueyuan.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://skw.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://cql.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://slb.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://uau.yvedp.cn

[A16] 真假值判断规则
来源：http://xlm.xingfuxueyuan.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qzd.mhx1999.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ctq.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gox.fzhhl.top

TS:   if (!x) {}
来源：http://yst.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hzs.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rzk.sysykeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://mqg.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lfg.haohaochexian.top

[A17] 位运算
来源：http://cih.shangyingyoupin.top


<!-- 参考信息 -->