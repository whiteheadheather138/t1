代发 wailian999

[U93] JS：模板字符串
来源：http://wex.sweek.top

`共 ${n} 条`
来源：http://nyl.9152youxi.cn

[U94] JS：箭头函数
来源：http://skc.fanxiaobao.xyz

const double = x => x * 2;
来源：http://iye.hesvh.cn

[U95] JS：Promise 包装
来源：http://voy.cashguo.top

new Promise((resolve, reject) => {})
来源：http://fzw.daxiang520.top

[U96] JS：async/await 与异常
来源：http://lam.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pbw.zhoulong.xyz

[U97] JS：并发请求
来源：http://fza.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ros.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://qgh.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://awr.yueranfly.top

[U99] JS：事件监听
来源：http://aht.havefunace.top

el.addEventListener("click", e => {})
来源：http://qnz.aizwys.cn

[U100] JS：DOM 查询
来源：http://xzs.wangshuangyany.cn

document.querySelector(".item")
来源：http://pvi.shzxlz.cn

[U101] JS：classList 操作
来源：http://ckq.yj20258888.top

el.classList.toggle("active")
来源：http://ubz.yj20258.top

[U102] JS：本地存储
来源：http://lph.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dux.hnqzz.top

[U103] JS：定时器
来源：http://sop.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xpf.0kj1m.cn

[U104] JS：防抖
来源：http://oke.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tiq.vehdjk.com

[U105] JS：节流
来源：http://bdu.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mzz.gzhubu.top

[U106] JS：日期格式化
来源：http://ndt.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tcb.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://lhd.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tmt.sxryk.cn

[U108] JS：随机整数
来源：http://wmr.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wqy.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://rjf.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://ntd.hcnkem.com

[U110] JS：数组分块
来源：http://tid.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rtb.gotoacloud.top

[U111] JS：对象转 Map
来源：http://fdf.316326.xyz

new Map(Object.entries(obj))
来源：http://wwy.mhx1999.top

[U112] JS：字符串补位
来源：http://kqz.ctjpmb.com

"7".padStart(3, "0")
来源：http://eja.tarul.cn

[U113] JS：正则替换全部
来源：http://tfq.zhengqikj.top

s.replaceAll("a", "b")
来源：http://zvy.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://zsh.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ptw.yueranfly.top

[U115] JS：生成 UUID
来源：http://kfo.9152youxi.cn

crypto.randomUUID()
来源：http://tgm.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://req.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://yko.zhengqikj.top

[U117] JS：单元测试
来源：http://fxp.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://vtf.hnxiangtu.top

[U118] JS：开发服务器
来源：http://okf.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://orj.hcnkem.com

[U119] JS：生产构建
来源：http://ges.zhiwuduotai.top

npx vite build
来源：http://bct.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://bry.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://koz.wangdashe.top

================================================================================
来源：http://bzz.hammf.cn

统计汇总
来源：http://gfz.cdnleiting.top

================================================================================
来源：http://ikh.yfazqb.com

按语言统计（条）：
来源：http://dqi.dashuyun.cn

Python ......... 252
来源：http://mvy.sweek.top

PHP ............ 252
来源：http://kya.cheryme.top

JavaScript ..... 252
来源：http://gog.chenlongwang.top

TypeScript ..... 212
来源：http://xrf.jyoumei.cn

Java ........... 212
来源：http://vwf.zhijiandao.cn

Go ............. 212
来源：http://yxi.jqgfzy.top

Ruby ........... 212
来源：http://pbg.daxiang520.top

C# ............. 212
来源：http://xyd.yangfankeji.com

C .............. 30
来源：http://ssk.jinqigfzy.top

C++ ............ 30
来源：http://nnk.vqdsnc.cn

SQL ............ 90
来源：http://izu.hfpthk.cn

Bash ........... 80
来源：http://uab.xuanzx.com

Kotlin ......... 15
来源：http://xpu.yueranfly.top

Swift .......... 15
来源：http://aie.kuanghao11.cn

Lua ............ 10
来源：http://bxh.hysaishi.cn

Perl ........... 10
来源：http://dbx.nwbrower.top

Scala .......... 10
来源：http://fdb.nwbrower.top

------------------------------------
来源：http://opz.yj202588.top

合计 ........... 2106 条
来源：http://bun.chenzaomai.com

按章节统计：
来源：http://tfb.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fwt.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hzj.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nca.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aoa.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qpi.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hvs.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hlu.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://srp.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jpo.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wwa.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kkd.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://etb.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://grr.yonumen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ijh.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fbh.shuidangran.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ucz.iojbl.cn

Q SQL 专题                              90
来源：http://pze.jyoumei.cn

R Bash 专题                             80
来源：http://oys.zhoulong.xyz

S C / C++ 专题                          60
来源：http://lvw.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://ure.jyoumei.cn

U 高频实用片段                         120
来源：http://bet.cucudq.cn

------------------------------------
来源：http://iey.shanyushiyangtech.top

合计                                  2106 条
来源：http://mwi.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://jwx.316326.xyz

使用提醒
来源：http://fhm.yuxming.cn

--------------------------------------------------------------------------------
来源：http://lgn.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wyr.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vwr.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iiz.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ibw.nanxuanxn.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ifq.zycfv.cn

—— 文件结束 ——
来源：http://tql.yfazqb.com

================================================================================
来源：http://uwm.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://cmu.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://uhd.wangdashe.top

================================================================================
来源：http://tuv.fzhhl.top

【收录内容】
来源：http://isd.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dpx.cqqwz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wie.hysaishi.cn

SQL · Bash · C · C++
来源：http://ajo.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nka.fengsongda.top

【使用说明】
来源：http://lpc.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sbh.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kff.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cfz.shuidangran.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kza.316326.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://qqe.zhijiandao.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nli.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ozf.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ngr.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lwg.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cjc.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yre.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baj.zhiwuduotai.top

【文件统计】
来源：http://tuy.ydzc1.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ldv.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://uko.jianghu66.top

目  录
来源：http://zoh.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://ljf.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kkj.andypj.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jjn.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://coy.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ekp.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://drz.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ahu.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ymn.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zfg.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wgl.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xiv.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ngj.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://grq.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xgy.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nnx.svipenyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rjp.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dbs.jinqigufen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ezd.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qjm.gaohongyu789.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mlt.ctjpmb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqg.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fkj.nwbrower.top

================================================================================
来源：http://zul.ctjpmb.com

A. 基础语法与类型
来源：http://ero.gogol.net.cn

================================================================================
来源：http://lur.zhongyouzk.top

[A01] Hello World
来源：http://wsk.mhx1999.top

Py:   print("Hello, World!")
来源：http://dtt.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://srb.gaohongyu789.top

JS:   console.log("Hello, World!");
来源：http://axi.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fae.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://wqm.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://tpb.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://hcz.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://biu.birdmap.top

[A02] 变量声明与赋值
来源：http://asd.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://trc.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://snr.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://poy.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://brg.jiagoushi.top

Java: String name = "Alex"; int age = 20;
来源：http://ulk.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://gmr.jinyuanbaomall.cn

Ruby: name = "Alex"; age = 20
来源：http://wlg.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://tfj.jlsjyb.cn

[A03] 常量定义
来源：http://hox.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ytp.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://lfg.jlsjyb.cn

JS:   const PI = 3.14159;
来源：http://mld.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://her.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://hri.cucudq.cn

Go:   const PI = 3.14159
来源：http://zee.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://vli.jiagoushi.top

C#:   const double PI = 3.14159;
来源：http://grn.pengpengdd.cyou

[A04] 判断变量类型
来源：http://nqg.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hnj.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bdj.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oei.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://gdb.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sxn.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://yxi.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://dim.jiagoushi.top

C#:   x.GetType().Name; x is int
来源：http://oan.shuidangran.top

[A05] 整数除法与取模
来源：http://wkh.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tmj.gzhubu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zwc.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gwl.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ops.pycfn.com

Java: 7 / 2; 7 % 2
来源：http://eca.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://zuw.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://nol.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://seq.c1oappe.top

[A06] 字符串转数字
来源：http://bmz.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://iun.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cit.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fqg.redwolf501.top

TS:   parseInt("42", 10); Number("42")
来源：http://bgi.zhengqikj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tql.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ovt.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dig.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fim.vehdjk.com

[A07] 数字转字符串
来源：http://dlg.daria6918.cn

Py:   str(42)
来源：http://rqe.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://oym.havefunace.top

JS:   String(42); (42).toString()
来源：http://orz.jqgufenzy.top

TS:   String(42)
来源：http://xkz.zdqjudy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cpw.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://iof.shzxlz.cn

Ruby: 42.to_s
来源：http://fst.ctjpmb.com

C#:   42.ToString()
来源：http://aar.zhengqikj.top

[A08] 取整与四舍五入
来源：http://aaj.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dpf.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cqw.xziqi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gcs.jinqigufen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://glj.yj202588.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://itn.yj202588.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://moj.jinyuanbaomall.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sni.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eft.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://dai.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bfl.316326.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rqc.hongshengwenyu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nvj.shanyushiyangtech.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ddz.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nnx.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vfn.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://arh.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://laj.haohaochexian.top

[A10] 生成随机数
来源：http://ipb.guowangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://lfa.sweek.top

PHP:  random_int(1, 100);
来源：http://wls.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bat.9152youxi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jbc.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://vsg.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oqn.zhengqikj.top

Ruby: rand(1..100)
来源：http://xzo.gotoacloud.top

C#:   new Random().Next(1, 101)
来源：http://jqm.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://mtu.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://mpm.ehwqpu.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://viu.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ybn.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rmc.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://vwq.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cbe.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jkg.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://hrl.wangdashe.top

[A12] 字符串插值 / 格式化
来源：http://ebt.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hep.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zwq.xziqi.cn

JS:   `Hello, ${name}!`
来源：http://dyy.yfazqb.com

TS:   `Hello, ${name}!`
来源：http://vuj.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://svz.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kco.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://atx.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://pev.guowangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kjs.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://xjg.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://swj.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://ccy.nwbrower.top

TS:   "第一行\n第二行"
来源：http://ace.zhongyouzk.top

Java: "第一行\n第二行"
来源：http://pqu.c1oappe.top

Go:   "第一行\n第二行"
来源：http://rco.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://ahu.52xcode.cn

C#:   "第一行\n第二行"
来源：http://ghp.wangshuangyany.cn

[A14] 注释写法
来源：http://uji.zhoulong.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://pmc.jinqigfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jcx.fengsongda.top

JS:   // 单行；/* 多行 */
来源：http://ctf.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://yld.shanyushiyangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kql.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://sqt.cheryme.top

Ruby: # 单行；=begin 多行 =end
来源：http://itr.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://rad.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://ala.tanke756.top

Py:   value = data or "默认值"
来源：http://qxn.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://gbc.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://vjv.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://xfi.hnxiangtu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://phd.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://iaq.hesvh.cn

Ruby: value = data || "默认值"
来源：http://akb.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://xnb.ydzc1.top

[A16] 真假值判断规则
来源：http://rif.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ciz.guowangkeji.top


<!-- 参考信息 -->