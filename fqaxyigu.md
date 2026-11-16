代发 wailian999

[U95] JS：Promise 包装
来源：http://bcp.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://wnv.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://eiv.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jik.yueranfly.top

[U97] JS：并发请求
来源：http://nan.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgi.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://pet.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cjp.pengpengdd.cyou

[U99] JS：事件监听
来源：http://ejq.xziqi.cn

el.addEventListener("click", e => {})
来源：http://fyf.sysykeji.top

[U100] JS：DOM 查询
来源：http://wzd.nanxuanxn.top

document.querySelector(".item")
来源：http://tvp.ppjwa.cn

[U101] JS：classList 操作
来源：http://goq.nanxinkj.top

el.classList.toggle("active")
来源：http://fuh.sweek.top

[U102] JS：本地存储
来源：http://vmc.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ens.haohaochexian.top

[U103] JS：定时器
来源：http://thn.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kly.jinqigfzy.top

[U104] JS：防抖
来源：http://jdz.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tem.daria6918.cn

[U105] JS：节流
来源：http://tqs.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xce.aizwys.cn

[U106] JS：日期格式化
来源：http://ndf.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dir.sysykeji.top

[U107] JS：数字千分位
来源：http://fdb.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nwe.hfpthk.cn

[U108] JS：随机整数
来源：http://clj.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gzr.jqgufenzy.top

[U109] JS：数组分组
来源：http://tpw.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://rjf.jianghu66.top

[U110] JS：数组分块
来源：http://qgl.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nht.xziqi.cn

[U111] JS：对象转 Map
来源：http://vic.yueranfly.top

new Map(Object.entries(obj))
来源：http://eni.quarkkingdee.top

[U112] JS：字符串补位
来源：http://ybo.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://syi.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://kzg.yangfankeji.com

s.replaceAll("a", "b")
来源：http://lmb.pycfn.com

[U114] JS：JSON 深比较
来源：http://lya.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://acv.9152youxi.cn

[U115] JS：生成 UUID
来源：http://aws.shanyushiyangtech.top

crypto.randomUUID()
来源：http://kkf.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://zih.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://oek.havefunace.top

[U117] JS：单元测试
来源：http://nag.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://jaq.havefunace.top

[U118] JS：开发服务器
来源：http://afo.gzhubu.top

npm i -D vite;  npx vite
来源：http://hyt.cqqwz.cn

[U119] JS：生产构建
来源：http://pdn.epnwcf.com

npx vite build
来源：http://xrg.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://smq.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://krj.wangshuangyany.cn

================================================================================
来源：http://yao.zdbjq.cn

统计汇总
来源：http://kre.tarul.cn

================================================================================
来源：http://azj.quarkkingdee.top

按语言统计（条）：
来源：http://abi.9152youxi.cn

Python ......... 252
来源：http://avo.jqgufenzy.top

PHP ............ 252
来源：http://aco.jqgufenzy.top

JavaScript ..... 252
来源：http://oep.fengsongda.top

TypeScript ..... 212
来源：http://bxv.nanxuanxn.top

Java ........... 212
来源：http://lwv.tian-w.cn

Go ............. 212
来源：http://ksy.cucudq.cn

Ruby ........... 212
来源：http://jks.shzxlz.cn

C# ............. 212
来源：http://zvu.wangdashe.top

C .............. 30
来源：http://usl.wangshuangyany.cn

C++ ............ 30
来源：http://gtl.zhaomingkeji.xyz

SQL ............ 90
来源：http://gjt.quarkkingdee.top

Bash ........... 80
来源：http://gno.svipenyu.cn

Kotlin ......... 15
来源：http://owr.ctjpmb.com

Swift .......... 15
来源：http://qvi.daria6918.cn

Lua ............ 10
来源：http://cqq.sweek.top

Perl ........... 10
来源：http://owo.birdmap.top

Scala .......... 10
来源：http://lku.zhengqikj.top

------------------------------------
来源：http://gec.fehbvm.com

合计 ........... 2106 条
来源：http://jro.gaohongyu789.top

按章节统计：
来源：http://xob.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tmy.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fzd.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://den.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ldj.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nin.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pqc.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sxv.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eha.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rdx.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pwd.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yth.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uoa.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zlf.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://klb.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wrb.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://grl.wangshuangyany.cn

Q SQL 专题                              90
来源：http://qub.zhoulong.xyz

R Bash 专题                             80
来源：http://hyy.xylfe.cn

S C / C++ 专题                          60
来源：http://std.nanxuanxn.top

T 其他语言补充                          60
来源：http://hef.gaohongyu789.top

U 高频实用片段                         120
来源：http://aih.fktsv.cn

------------------------------------
来源：http://iui.zdbjq.cn

合计                                  2106 条
来源：http://suz.cashguo.top

--------------------------------------------------------------------------------
来源：http://yhz.ywan-chungtsiang.top

使用提醒
来源：http://spv.yj20258888.top

--------------------------------------------------------------------------------
来源：http://eiy.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bfb.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zaf.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lzb.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ghi.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hhf.fanxiaobao.xyz

—— 文件结束 ——
来源：http://djt.hnxiangtu.top

================================================================================
来源：http://zdt.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://cpd.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://zda.haohaochexian.top

================================================================================
来源：http://xhs.ywan-chungtsiang.top

【收录内容】
来源：http://imr.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ppc.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zax.shangyingyoupin.top

SQL · Bash · C · C++
来源：http://wwk.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hdd.tianlin.xyz

【使用说明】
来源：http://pys.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tnm.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bza.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oqd.dianchejie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ard.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qhd.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://odn.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hlx.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dml.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://czq.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://you.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sbb.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ptq.yangfankeji.com

【文件统计】
来源：http://tuo.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vtu.redwolf501.top

--------------------------------------------------------------------------------
来源：http://fqt.bbcook.cn

目  录
来源：http://jik.vehdjk.com

--------------------------------------------------------------------------------
来源：http://ljh.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yjj.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sfs.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ubi.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yoy.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://srm.jlsjyb.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ols.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lol.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kkh.zhengqikj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://brw.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yee.cqqwz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://huk.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ozh.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mpw.bbcook.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://skv.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nkw.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://efh.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iin.yvedp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gpm.cheryme.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qce.redwolf501.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nvp.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gqd.fehbvm.com

================================================================================
来源：http://syq.316326.xyz

A. 基础语法与类型
来源：http://czl.shanyushiyangkeji.top

================================================================================
来源：http://qta.ppjwa.cn

[A01] Hello World
来源：http://xsc.52xcode.cn

Py:   print("Hello, World!")
来源：http://sxn.hnqzz.top

PHP:  echo "Hello, World!";
来源：http://agp.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://fbi.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zze.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://xir.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://ugl.316326.xyz

Ruby: puts "Hello, World!"
来源：http://man.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://klj.redwolf501.top

[A02] 变量声明与赋值
来源：http://hjv.jinqigfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fcj.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://fwh.hammf.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lab.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cvj.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://ooh.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://xqg.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://cle.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://otu.shanyushiyangkeji.top

[A03] 常量定义
来源：http://pls.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pra.gogol.net.cn

PHP:  const PI = 3.14159;
来源：http://xmk.yueranfly.top

JS:   const PI = 3.14159;
来源：http://dmf.zdbjq.cn

TS:   const PI: number = 3.14159;
来源：http://eks.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://vpr.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://rsl.shuidangran.top

Ruby: PI = 3.14159
来源：http://jdr.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://jkz.zhixingplan.top

[A04] 判断变量类型
来源：http://huc.guowangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wds.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cvw.jinghuilouyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lmx.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://flt.wangshuangyany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mxt.yuxming.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pcb.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://dav.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://odf.shanyushiyangkeji.top

[A05] 整数除法与取模
来源：http://urt.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sif.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ufl.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qbk.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nzq.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://lck.sysykeji.top

Go:   7 / 2; 7 % 2
来源：http://llp.bjfxy.top

Ruby: 7 / 2; 7 % 2
来源：http://gjy.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://kad.fehbvm.com

[A06] 字符串转数字
来源：http://xtx.ydjk.org.cn

Py:   int("42"); float("3.14")
来源：http://nka.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vbu.hnqzz.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ygj.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mbs.gaohongyu789.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://whz.sxryk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lzm.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://dug.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ipl.nwbrower.top

[A07] 数字转字符串
来源：http://ufi.vqdsnc.cn

Py:   str(42)
来源：http://hby.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://hus.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://dbq.cucudq.cn

TS:   String(42)
来源：http://mxi.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kfb.shuidangran.top

Go:   strconv.Itoa(42)
来源：http://itr.zhixingplan.top

Ruby: 42.to_s
来源：http://hsg.wangshuangyany.cn

C#:   42.ToString()
来源：http://kho.bbcook.cn

[A08] 取整与四舍五入
来源：http://oan.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iwn.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zeh.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pfi.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cws.jianghu66.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dxd.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iqi.yanxiufei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zig.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://soy.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://yxi.yongpay.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://myo.cqqwz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zyl.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rkj.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ith.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tcy.yongpay.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zws.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jdq.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ubs.kuanghao11.cn

[A10] 生成随机数
来源：http://dhi.havefunace.top

Py:   import random; random.randint(1, 100)
来源：http://moe.316326.xyz

PHP:  random_int(1, 100);
来源：http://xht.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vcf.0kj1m.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lyj.ctjpmb.com

Java: new Random().nextInt(100) + 1
来源：http://xup.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qun.bjfxy.top

Ruby: rand(1..100)
来源：http://opx.shanyushiyangkeji.top

C#:   new Random().Next(1, 101)
来源：http://pms.fanxiaobao.xyz

[A11] 条件表达式（三元）
来源：http://rss.ivvv.top

Py:   "yes" if x > 0 else "no"
来源：http://cin.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wpz.hesvh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gay.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://clh.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://wde.guannengcc.top

Go:   // 无三元运算符，需用 if 语句
来源：http://djd.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tol.smart0.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://gve.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://mkc.haohaochexian.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eza.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ckp.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://tih.jinghuilouyu.cn

TS:   `Hello, ${name}!`
来源：http://igh.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://skw.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dlf.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://eur.ehwqpu.com

C#:   $"Hello, {name}!"
来源：http://hwc.epnwcf.com

[A13] 多行字符串（练习 \n 转义）
来源：http://ovm.yueranfly.top

Py:   "第一行\n第二行"
来源：http://sgn.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://gfo.nanxuanxn.top

JS:   "第一行\n第二行"
来源：http://unu.fengsongda.top

TS:   "第一行\n第二行"
来源：http://ivi.ydzc1.top

Java: "第一行\n第二行"
来源：http://gcp.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://geh.cdnleiting.top

Ruby: "第一行\n第二行"
来源：http://gkc.ivvv.top

C#:   "第一行\n第二行"
来源：http://ffn.cdnleiting.top

[A14] 注释写法
来源：http://plw.xuetiantiany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wdy.sxryk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rpt.aizwys.cn

JS:   // 单行；/* 多行 */
来源：http://gpx.xziqi.cn

TS:   // 单行；/* 多行 */
来源：http://tnm.quarkkingdee.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xjk.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://cdk.fehbvm.com

Ruby: # 单行；=begin 多行 =end
来源：http://dft.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://nzz.dashuyun.cn

[A15] 空值判断与默认值
来源：http://xmk.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://ixm.jqgufenzy.top

PHP:  $value = $data ?? "默认值";
来源：http://xgf.ehwqpu.com

JS:   const value = data ?? "默认值";
来源：http://zvr.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://bvk.fehbvm.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gpt.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://trg.ybcxt.top

Ruby: value = data || "默认值"
来源：http://jsv.havefunace.top

C#:   var value = data ?? "默认值";
来源：http://med.hysaishi.cn

[A16] 真假值判断规则
来源：http://ukx.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wml.hammf.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lpm.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://big.pengpengdd.cyou

TS:   if (!x) {}
来源：http://dis.fzhhl.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lod.zdbjq.cn


<!-- 参考信息 -->