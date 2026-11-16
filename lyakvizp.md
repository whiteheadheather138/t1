代发 wailian999

[U93] JS：模板字符串
来源：http://pea.fengsongda.top

`共 ${n} 条`
来源：http://sfb.jqgufenzy.top

[U94] JS：箭头函数
来源：http://kry.gzhubu.top

const double = x => x * 2;
来源：http://kta.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://jbl.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://kjg.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://cls.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lzf.nanxuanxn.top

[U97] JS：并发请求
来源：http://lys.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://upr.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://upc.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zaq.yongpay.top

[U99] JS：事件监听
来源：http://osd.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://vti.316326.xyz

[U100] JS：DOM 查询
来源：http://xtl.feifeiyinyue.top

document.querySelector(".item")
来源：http://tpo.tianlin.xyz

[U101] JS：classList 操作
来源：http://opk.shzxlz.cn

el.classList.toggle("active")
来源：http://mfe.jlsjyb.cn

[U102] JS：本地存储
来源：http://gun.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://opn.epnwcf.com

[U103] JS：定时器
来源：http://orn.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://orj.xinyue.icu

[U104] JS：防抖
来源：http://ffw.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zrw.zhiwuduotai.top

[U105] JS：节流
来源：http://rwy.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ftr.zdqjudy.top

[U106] JS：日期格式化
来源：http://wub.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mpl.bbcook.cn

[U107] JS：数字千分位
来源：http://fag.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rls.xziqi.cn

[U108] JS：随机整数
来源：http://khw.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://emm.zhijiandao.cn

[U109] JS：数组分组
来源：http://psb.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://edk.sjlbkw.cn

[U110] JS：数组分块
来源：http://cqf.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ezk.guannengcc.top

[U111] JS：对象转 Map
来源：http://cfl.c1oappe.top

new Map(Object.entries(obj))
来源：http://qku.bbcook.cn

[U112] JS：字符串补位
来源：http://klb.sxryk.cn

"7".padStart(3, "0")
来源：http://ahu.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://ibh.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://ldf.fehbvm.com

[U114] JS：JSON 深比较
来源：http://kbg.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iuh.uphjek.com

[U115] JS：生成 UUID
来源：http://zff.xuetiantiany.cn

crypto.randomUUID()
来源：http://yvq.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://gzz.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://fyt.sjlbkw.cn

[U117] JS：单元测试
来源：http://gvq.yj20258.top

npm i -D vitest;  npx vitest
来源：http://sne.aibaodan.cn

[U118] JS：开发服务器
来源：http://bna.cdnleiting.top

npm i -D vite;  npx vite
来源：http://yxt.xziqi.cn

[U119] JS：生产构建
来源：http://tnw.zhaomingkeji.xyz

npx vite build
来源：http://run.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://aob.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://bsi.xingfuxueyuan.xyz

================================================================================
来源：http://bip.haohaochexian.top

统计汇总
来源：http://sdn.jlsjyb.cn

================================================================================
来源：http://jwn.meibo888.top

按语言统计（条）：
来源：http://aac.jinghuilouyu.cn

Python ......... 252
来源：http://vcx.shanyushiyangtech.top

PHP ............ 252
来源：http://fiu.feifeiyinyue.top

JavaScript ..... 252
来源：http://xvc.yvedp.cn

TypeScript ..... 212
来源：http://dku.yj20258888.top

Java ........... 212
来源：http://wkw.tanke756.top

Go ............. 212
来源：http://pfk.zhiwuduotai.top

Ruby ........... 212
来源：http://yku.haohaochexian.top

C# ............. 212
来源：http://zgh.chenlongwang.top

C .............. 30
来源：http://hlw.vqdsnc.cn

C++ ............ 30
来源：http://sgz.nanxinkj.top

SQL ............ 90
来源：http://fhm.yvedp.cn

Bash ........... 80
来源：http://zui.feifeiyinyue.top

Kotlin ......... 15
来源：http://rlf.birdmap.top

Swift .......... 15
来源：http://uyl.tanke756.top

Lua ............ 10
来源：http://gjj.sysykeji.top

Perl ........... 10
来源：http://lfl.xuetiantiany.cn

Scala .......... 10
来源：http://osz.havefunace.top

------------------------------------
来源：http://ttv.yueranfly.top

合计 ........... 2106 条
来源：http://ikw.hnqzz.top

按章节统计：
来源：http://wfk.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xfm.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sxn.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ufx.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ggq.havefunace.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jna.pengpengdd.cyou

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nfu.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tna.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vyl.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://roa.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zpn.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nrb.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ftc.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iyx.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zsr.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eap.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yxw.hysaishi.cn

Q SQL 专题                              90
来源：http://swn.gaohongyu789.top

R Bash 专题                             80
来源：http://php.9152youxi.cn

S C / C++ 专题                          60
来源：http://pfd.tarul.cn

T 其他语言补充                          60
来源：http://ltn.sweek.top

U 高频实用片段                         120
来源：http://ksd.shzxlz.cn

------------------------------------
来源：http://kmk.chenjidiqi.icu

合计                                  2106 条
来源：http://ckr.xziqi.cn

--------------------------------------------------------------------------------
来源：http://bcv.xuanzx.com

使用提醒
来源：http://bjn.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://upo.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ook.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blz.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zdq.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://odr.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lxt.sysykeji.top

—— 文件结束 ——
来源：http://ebp.iojbl.cn

================================================================================
来源：http://akc.tianlin.xyz

程序语言常见例子速查手册（2024 版）
来源：http://dfp.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://xgv.uphjek.com

================================================================================
来源：http://snu.bjfxy.top

【收录内容】
来源：http://ide.yfazqb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://uay.pycfn.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://krh.hnxiangtu.top

SQL · Bash · C · C++
来源：http://zhl.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://whr.mhx1999.top

【使用说明】
来源：http://mxa.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://big.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mtj.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hec.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bcx.zhengqikj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fqv.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://omu.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cin.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fbj.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ntm.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gis.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mqp.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qrh.tarul.cn

【文件统计】
来源：http://ova.andypj.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xan.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://sui.yj20258.top

目  录
来源：http://rcv.yuxming.cn

--------------------------------------------------------------------------------
来源：http://juk.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eld.cheryme.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ocj.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bel.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nsx.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vqd.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ngx.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://isx.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ctn.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kaj.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qaj.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fnm.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fli.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ewl.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zbd.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cfx.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ohj.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ecs.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bnd.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ryc.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cfj.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zio.xuetiantiany.cn

================================================================================
来源：http://use.sjlbkw.cn

A. 基础语法与类型
来源：http://dms.redwolf501.top

================================================================================
来源：http://zmm.iojbl.cn

[A01] Hello World
来源：http://drj.guannengcc.top

Py:   print("Hello, World!")
来源：http://rkg.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://abi.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://bmm.zhoulong.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yps.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://xte.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://aet.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://xvq.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://aqa.yfazqb.com

[A02] 变量声明与赋值
来源：http://hgu.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lfd.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nfo.hywenlv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://naj.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hxb.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://zrb.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://bak.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://tdz.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://wpb.yuanzhike.top

[A03] 常量定义
来源：http://ewt.shzxlz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kfm.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://vxp.yueranfly.top

JS:   const PI = 3.14159;
来源：http://xnu.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://kut.nanxinkj.top

Java: static final double PI = 3.14159;
来源：http://abm.xziqi.cn

Go:   const PI = 3.14159
来源：http://vdq.daria6918.cn

Ruby: PI = 3.14159
来源：http://iik.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://lct.jqgfzy.top

[A04] 判断变量类型
来源：http://giv.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ukb.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wbl.sweek.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hqg.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://slr.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://noo.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://gef.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ghy.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://oqm.hnxiangtu.top

[A05] 整数除法与取模
来源：http://zjp.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pbw.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fwb.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rej.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ngf.quarkkingdee.top

Java: 7 / 2; 7 % 2
来源：http://evl.guowangkeji.top

Go:   7 / 2; 7 % 2
来源：http://zms.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://vml.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://kjd.hongshengwenyu.top

[A06] 字符串转数字
来源：http://hcs.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://pvq.52xcode.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://row.hnxiangtu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dsf.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ipx.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vua.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wff.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nrz.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://abk.tanke756.top

[A07] 数字转字符串
来源：http://ayz.yj20258.top

Py:   str(42)
来源：http://qsr.bbcook.cn

PHP:  (string) 42; strval(42)
来源：http://rzi.aizwys.cn

JS:   String(42); (42).toString()
来源：http://jjp.yanxiufei.cn

TS:   String(42)
来源：http://yuu.cqqwz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://djl.zhengqikj.top

Go:   strconv.Itoa(42)
来源：http://htr.hongshengwenyu.top

Ruby: 42.to_s
来源：http://yca.zhengqikj.top

C#:   42.ToString()
来源：http://wak.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://uze.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fei.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xtz.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jov.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fkh.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pyo.meibo888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ytr.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ort.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ikw.zhixingplan.top

[A09] 绝对值与最大最小值
来源：http://vfs.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cru.xuanzx.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dvg.jinghuilouyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bmx.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nnp.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fjj.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://trs.sysykeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://upa.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zxl.shuidangran.top

[A10] 生成随机数
来源：http://afq.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://rwh.yonumen.top

PHP:  random_int(1, 100);
来源：http://crg.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://twe.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jdj.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://heb.shanyushiyangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ovr.sxryk.cn

Ruby: rand(1..100)
来源：http://zhx.ppjwa.cn

C#:   new Random().Next(1, 101)
来源：http://mqo.gotoacloud.top

[A11] 条件表达式（三元）
来源：http://klt.guannengcc.top

Py:   "yes" if x > 0 else "no"
来源：http://npi.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ucf.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://rwu.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kiu.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://otm.quarkkingdee.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jsc.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://unu.xuanzx.com

C#:   x > 0 ? "yes" : "no"
来源：http://egd.svipenyu.cn

[A12] 字符串插值 / 格式化
来源：http://cqs.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dxu.cucudq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://egc.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://lrl.gaohongyu789.top

TS:   `Hello, ${name}!`
来源：http://nco.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://ceo.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://okq.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://rmr.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://tzz.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qpq.jianghu66.top

Py:   "第一行\n第二行"
来源：http://cmd.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://nsq.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://xhx.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://wkq.zycfv.cn

Java: "第一行\n第二行"
来源：http://hid.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://sbe.jlsjyb.cn

Ruby: "第一行\n第二行"
来源：http://cnp.vehdjk.com

C#:   "第一行\n第二行"
来源：http://zoc.zhijiandao.cn

[A14] 注释写法
来源：http://tyu.fanxiaobao.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://jyo.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vea.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://wsk.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://ppd.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zev.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://udq.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zgc.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://cks.cheryme.top

[A15] 空值判断与默认值
来源：http://lui.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://nuf.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://web.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://bja.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://blg.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uwo.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://pzx.yueranfly.top

Ruby: value = data || "默认值"
来源：http://ouv.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://scf.tanke756.top

[A16] 真假值判断规则
来源：http://uxw.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ifq.cqqwz.cn


<!-- 参考信息 -->