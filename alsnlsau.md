代发 wailian999

[U93] JS：模板字符串
来源：http://xkm.ppjwa.cn

`共 ${n} 条`
来源：http://hbz.cucudq.cn

[U94] JS：箭头函数
来源：http://egp.uphjek.com

const double = x => x * 2;
来源：http://xxj.ctjpmb.com

[U95] JS：Promise 包装
来源：http://evx.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://dmc.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://eqb.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://utb.jinqigfzy.top

[U97] JS：并发请求
来源：http://emn.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yqm.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://fyg.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ptd.xziqi.cn

[U99] JS：事件监听
来源：http://jsy.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://wnf.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://fce.bbcook.cn

document.querySelector(".item")
来源：http://luk.andypj.xyz

[U101] JS：classList 操作
来源：http://tfl.hnxiangtu.top

el.classList.toggle("active")
来源：http://ply.wangshuangyany.cn

[U102] JS：本地存储
来源：http://nar.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ztn.nanxinkj.top

[U103] JS：定时器
来源：http://ict.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blm.mhx1999.top

[U104] JS：防抖
来源：http://fna.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xyk.jinyuanbaomall.cn

[U105] JS：节流
来源：http://fmh.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://scb.ybcxt.top

[U106] JS：日期格式化
来源：http://zqq.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wsb.hcnkem.com

[U107] JS：数字千分位
来源：http://dhf.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rvm.svipenyu.cn

[U108] JS：随机整数
来源：http://byu.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xmq.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://asu.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://cvg.xuanzx.com

[U110] JS：数组分块
来源：http://vdb.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eim.yfazqb.com

[U111] JS：对象转 Map
来源：http://dmu.jqgfzy.top

new Map(Object.entries(obj))
来源：http://vlz.hnqzz.top

[U112] JS：字符串补位
来源：http://mgj.hammf.cn

"7".padStart(3, "0")
来源：http://zsz.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://lwi.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://hyq.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://goi.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://cqj.jqgfzy.top

[U115] JS：生成 UUID
来源：http://wip.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://vbh.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://hml.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://hab.hfpthk.cn

[U117] JS：单元测试
来源：http://zhn.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://yjn.jianghu66.top

[U118] JS：开发服务器
来源：http://wls.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://yjw.epnwcf.com

[U119] JS：生产构建
来源：http://owk.yj20258888.top

npx vite build
来源：http://ipn.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://hgl.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://omh.snrcjt.cn

================================================================================
来源：http://lfs.nanxinkj.top

统计汇总
来源：http://pfo.pengpengdd.cyou

================================================================================
来源：http://kop.fzhhl.top

按语言统计（条）：
来源：http://okw.xylfe.cn

Python ......... 252
来源：http://fhf.tian-w.cn

PHP ............ 252
来源：http://qjl.jinqigufen.top

JavaScript ..... 252
来源：http://gux.hongshengwenyu.top

TypeScript ..... 212
来源：http://jfr.shanyushiyangkeji.top

Java ........... 212
来源：http://hri.redwolf501.top

Go ............. 212
来源：http://hgi.snrcjt.cn

Ruby ........... 212
来源：http://vif.fengsongda.top

C# ............. 212
来源：http://gev.yuxming.cn

C .............. 30
来源：http://rua.nwbrower.top

C++ ............ 30
来源：http://ryl.xylfe.cn

SQL ............ 90
来源：http://gex.svipenyu.cn

Bash ........... 80
来源：http://evv.chenzaomai.com

Kotlin ......... 15
来源：http://zxy.bbcook.cn

Swift .......... 15
来源：http://opf.birdmap.top

Lua ............ 10
来源：http://ytb.hywenlv.cn

Perl ........... 10
来源：http://fdw.yuxming.cn

Scala .......... 10
来源：http://dtc.zhoulong.xyz

------------------------------------
来源：http://tdc.hywenlv.cn

合计 ........... 2106 条
来源：http://ymz.vqdsnc.cn

按章节统计：
来源：http://moj.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cix.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://brz.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wlh.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vfk.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bnz.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jel.cashguo.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ntj.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sde.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tvk.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://com.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://shf.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hjd.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rmf.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qpz.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uws.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yns.bbcook.cn

Q SQL 专题                              90
来源：http://rgv.yanxiufei.cn

R Bash 专题                             80
来源：http://dvc.haohaochexian.top

S C / C++ 专题                          60
来源：http://anx.fktsv.cn

T 其他语言补充                          60
来源：http://fnt.hesvh.cn

U 高频实用片段                         120
来源：http://ysy.kuanghao11.cn

------------------------------------
来源：http://anf.sysykeji.top

合计                                  2106 条
来源：http://rgx.yuxming.cn

--------------------------------------------------------------------------------
来源：http://gyt.andypj.xyz

使用提醒
来源：http://npq.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://jwl.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vpj.sufxvd.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hnf.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ont.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ngv.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qvp.hnxiangtu.top

—— 文件结束 ——
来源：http://kgv.jlsjyb.cn

================================================================================
来源：http://enn.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://slk.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://ycv.cashguo.top

================================================================================
来源：http://uya.ydjk.org.cn

【收录内容】
来源：http://min.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nsr.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mdi.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://fqe.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ceo.pengpengdd.cyou

【使用说明】
来源：http://kal.uphjek.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ldo.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ymc.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mml.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cdy.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hqa.yvedp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pkg.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://isn.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dkh.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cib.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pxs.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ttt.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://njw.ydzc1.top

【文件统计】
来源：http://dsi.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gzx.fktsv.cn

--------------------------------------------------------------------------------
来源：http://wxc.c1oappe.top

目  录
来源：http://xzp.iojbl.cn

--------------------------------------------------------------------------------
来源：http://yid.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kts.jinqigfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cya.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pgw.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bmc.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uqf.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bsk.hcnkem.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hch.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yzi.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lqd.xziqi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://guz.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tjp.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xvi.jqgufenzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bnq.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bgm.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://imr.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqz.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tfs.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jwc.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pdu.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpn.tanke756.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mnp.zhixingplan.top

================================================================================
来源：http://vbn.xziqi.cn

A. 基础语法与类型
来源：http://sjn.bjfxy.top

================================================================================
来源：http://pvq.birdmap.top

[A01] Hello World
来源：http://qbn.yonumen.top

Py:   print("Hello, World!")
来源：http://let.meibo888.top

PHP:  echo "Hello, World!";
来源：http://zsk.hammf.cn

JS:   console.log("Hello, World!");
来源：http://vgc.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hgz.jianghu66.top

Java: System.out.println("Hello, World!");
来源：http://eff.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://dky.birdmap.top

Ruby: puts "Hello, World!"
来源：http://hal.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kvh.zhengqikj.top

[A02] 变量声明与赋值
来源：http://tar.zhongyouzk.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://trw.aibaodan.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://knv.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://icq.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hne.tian-w.cn

Java: String name = "Alex"; int age = 20;
来源：http://vkb.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://aje.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://llu.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lhw.fktsv.cn

[A03] 常量定义
来源：http://yil.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://icu.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://rzu.tarul.cn

JS:   const PI = 3.14159;
来源：http://gjt.xuetiantiany.cn

TS:   const PI: number = 3.14159;
来源：http://mmz.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://oeq.cheryme.top

Go:   const PI = 3.14159
来源：http://dex.havefunace.top

Ruby: PI = 3.14159
来源：http://eby.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://usq.kuanghao11.cn

[A04] 判断变量类型
来源：http://gxa.sweek.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uwb.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nko.zycfv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mat.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://odz.zdqjudy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rze.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://wdb.fanxiaobao.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://jqk.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://uxa.gaohongyu789.top

[A05] 整数除法与取模
来源：http://sjs.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zlm.shanyushiyangtech.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bkk.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wmv.shzxlz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ujf.sxryk.cn

Java: 7 / 2; 7 % 2
来源：http://xir.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://cvh.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://tfb.shangyingyoupin.top

C#:   7 / 2; 7 % 2
来源：http://taj.jiagoushi.top

[A06] 字符串转数字
来源：http://ksu.shanyushiyangkeji.top

Py:   int("42"); float("3.14")
来源：http://crt.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vfd.vqdsnc.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ojb.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://dxj.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nse.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jny.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ddc.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://scl.guowangkeji.top

[A07] 数字转字符串
来源：http://pbs.ybcxt.top

Py:   str(42)
来源：http://gkk.bbcook.cn

PHP:  (string) 42; strval(42)
来源：http://irz.vehdjk.com

JS:   String(42); (42).toString()
来源：http://aqh.shanyushiyangtech.top

TS:   String(42)
来源：http://xvz.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lfk.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://kiz.yangfankeji.com

Ruby: 42.to_s
来源：http://tcc.jinqigufen.top

C#:   42.ToString()
来源：http://sqp.yuxming.cn

[A08] 取整与四舍五入
来源：http://xbo.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xqv.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qnn.zhiwuduotai.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gew.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://leu.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://imz.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://trd.pycfn.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://rbp.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rcj.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://uqv.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://llj.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wnx.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cgd.xuetiantiany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://imo.snrcjt.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://txy.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hlj.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bwa.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cas.zhengqikj.top

[A10] 生成随机数
来源：http://fnu.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://usw.yj202588.top

PHP:  random_int(1, 100);
来源：http://tyj.zhoulong.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lbn.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kyk.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://mdv.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ial.sjlbkw.cn

Ruby: rand(1..100)
来源：http://szk.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://cxn.yuxming.cn

[A11] 条件表达式（三元）
来源：http://ybb.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://kni.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jlf.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vhi.jqgfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://nfl.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://skx.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uws.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ouj.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://nof.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://rbt.ppjwa.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yrf.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://auh.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://top.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://aub.sxryk.cn

Java: "Hello, %s!".formatted(name)
来源：http://onr.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://okz.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://ssc.jyoumei.cn

C#:   $"Hello, {name}!"
来源：http://tea.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dif.vehdjk.com

Py:   "第一行\n第二行"
来源：http://mct.epnwcf.com

PHP:  "第一行\n第二行"
来源：http://eob.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://phh.yuxming.cn

TS:   "第一行\n第二行"
来源：http://tjj.yj202588.top

Java: "第一行\n第二行"
来源：http://dtc.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://ubf.fanxiaobao.xyz

Ruby: "第一行\n第二行"
来源：http://jgr.xuanzx.com

C#:   "第一行\n第二行"
来源：http://vue.cdnleiting.top

[A14] 注释写法
来源：http://ssv.fanxiaobao.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://dnz.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ohx.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://oqe.zhengqikj.top

TS:   // 单行；/* 多行 */
来源：http://opf.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rwk.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://bld.sweek.top

Ruby: # 单行；=begin 多行 =end
来源：http://cfs.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://nag.daxiang520.top

[A15] 空值判断与默认值
来源：http://wes.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://mzk.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://pym.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://iel.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://art.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rba.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://slb.pengpengdd.cyou

Ruby: value = data || "默认值"
来源：http://xgt.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://nna.gotoacloud.top

[A16] 真假值判断规则
来源：http://kbd.xingfuxueyuan.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://okh.pengpengdd.cyou


<!-- 参考信息 -->