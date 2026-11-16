代发 wailian999

[U91] JS：对象键值遍历
来源：http://vzn.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vok.zhijiandao.cn

[U92] JS：深拷贝
来源：http://uvq.9152youxi.cn

structuredClone(obj)
来源：http://hcw.zhengqikj.top

[U93] JS：模板字符串
来源：http://ftl.cucudq.cn

`共 ${n} 条`
来源：http://dtx.hnqzz.top

[U94] JS：箭头函数
来源：http://goi.zhiwuduotai.top

const double = x => x * 2;
来源：http://chd.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://jwn.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://fwp.feifeiyinyue.top

[U96] JS：async/await 与异常
来源：http://gtf.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eat.aizwys.cn

[U97] JS：并发请求
来源：http://mie.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hpx.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://jzq.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://axg.aibaodan.cn

[U99] JS：事件监听
来源：http://tfd.shuidangran.top

el.addEventListener("click", e => {})
来源：http://vtt.bjfxy.top

[U100] JS：DOM 查询
来源：http://unz.sweek.top

document.querySelector(".item")
来源：http://txd.cheryme.top

[U101] JS：classList 操作
来源：http://qxd.yongpay.top

el.classList.toggle("active")
来源：http://sgs.hesvh.cn

[U102] JS：本地存储
来源：http://yrh.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kxx.cheryme.top

[U103] JS：定时器
来源：http://nez.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hjr.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://mnk.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hoi.cucudq.cn

[U105] JS：节流
来源：http://fua.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yiz.snrcjt.cn

[U106] JS：日期格式化
来源：http://gqq.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hdb.xziqi.cn

[U107] JS：数字千分位
来源：http://ctm.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nmo.fzhhl.top

[U108] JS：随机整数
来源：http://iet.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mwk.jinqigfzy.top

[U109] JS：数组分组
来源：http://ovt.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://cde.kuanghao11.cn

[U110] JS：数组分块
来源：http://gmb.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tpw.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://had.xinyue.icu

new Map(Object.entries(obj))
来源：http://ogb.hammf.cn

[U112] JS：字符串补位
来源：http://ebc.gaohongyu789.top

"7".padStart(3, "0")
来源：http://gkg.fengsongda.top

[U113] JS：正则替换全部
来源：http://try.ppjwa.cn

s.replaceAll("a", "b")
来源：http://ybv.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://odu.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rod.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://pft.hnxiangtu.top

crypto.randomUUID()
来源：http://oxs.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://xtz.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://fky.zdbjq.cn

[U117] JS：单元测试
来源：http://xoo.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://sjl.ivvv.top

[U118] JS：开发服务器
来源：http://qbm.yuanzhike.top

npm i -D vite;  npx vite
来源：http://yvu.sysykeji.top

[U119] JS：生产构建
来源：http://cmz.0kj1m.cn

npx vite build
来源：http://rtf.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://hds.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://tjs.sysykeji.top

================================================================================
来源：http://pda.jyoumei.cn

统计汇总
来源：http://dyf.ywan-chungtsiang.top

================================================================================
来源：http://hwd.feifeiyinyue.top

按语言统计（条）：
来源：http://sqo.birdmap.top

Python ......... 252
来源：http://qai.zdbjq.cn

PHP ............ 252
来源：http://xua.zdqjudy.top

JavaScript ..... 252
来源：http://vlg.snrcjt.cn

TypeScript ..... 212
来源：http://mou.sxryk.cn

Java ........... 212
来源：http://wvc.jinqigufen.top

Go ............. 212
来源：http://rvd.pycfn.com

Ruby ........... 212
来源：http://iic.daxiang520.top

C# ............. 212
来源：http://ehu.aizwys.cn

C .............. 30
来源：http://cvd.jyoumei.cn

C++ ............ 30
来源：http://idg.smart0.xyz

SQL ............ 90
来源：http://qyi.guannengcc.top

Bash ........... 80
来源：http://uvh.hammf.cn

Kotlin ......... 15
来源：http://ujy.tianlin.xyz

Swift .......... 15
来源：http://lcd.yueranfly.top

Lua ............ 10
来源：http://wej.jqgufenzy.top

Perl ........... 10
来源：http://iyk.shangyingyoupin.top

Scala .......... 10
来源：http://mqx.9152youxi.cn

------------------------------------
来源：http://jda.jinqigufen.top

合计 ........... 2106 条
来源：http://vhb.hnqzz.top

按章节统计：
来源：http://gdf.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hkg.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fxw.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ilg.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xbs.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yjq.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rjc.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://emj.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://evx.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jqm.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tll.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lzj.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ozg.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qgi.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://crq.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vfe.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yvg.ctjpmb.com

Q SQL 专题                              90
来源：http://unt.yueranfly.top

R Bash 专题                             80
来源：http://lwl.iojbl.cn

S C / C++ 专题                          60
来源：http://gpx.nwbrower.top

T 其他语言补充                          60
来源：http://uxd.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://twa.sufxvd.cn

------------------------------------
来源：http://uav.yuxming.cn

合计                                  2106 条
来源：http://ufs.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://eid.bjfxy.top

使用提醒
来源：http://yig.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://clh.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lcu.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uzw.xylfe.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mac.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jxr.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://neb.cheryme.top

—— 文件结束 ——
来源：http://qas.52xcode.cn

================================================================================
来源：http://tvn.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://kdf.yongpay.top

Common Programming Examples Cheat Book
来源：http://jxa.snrcjt.cn

================================================================================
来源：http://moy.316326.xyz

【收录内容】
来源：http://fgn.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://nbc.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://akb.hfpthk.cn

SQL · Bash · C · C++
来源：http://lwa.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xdg.52xcode.cn

【使用说明】
来源：http://fny.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://clb.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tib.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xyf.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rtx.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://usp.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cky.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tia.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lhi.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qav.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iux.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ldf.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://msz.c1oappe.top

【文件统计】
来源：http://pvw.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ima.pycfn.com

--------------------------------------------------------------------------------
来源：http://rbk.yuanzhike.top

目  录
来源：http://bju.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://pqg.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bbd.vehdjk.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nqm.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qdz.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hbf.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ock.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rwj.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qpn.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uge.dashuyun.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jsa.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://flw.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jyo.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rxp.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pue.0kj1m.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fdh.jinqigufen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lrf.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://skq.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tkf.shanyushiyangtech.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://abv.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://olk.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yrk.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://czu.hywenlv.cn

================================================================================
来源：http://bis.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://jzi.sweek.top

================================================================================
来源：http://qpw.yj20258.top

[A01] Hello World
来源：http://utj.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://wzc.tanke756.top

PHP:  echo "Hello, World!";
来源：http://krs.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://pzb.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://idz.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://ntu.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://fdh.quarkkingdee.top

Ruby: puts "Hello, World!"
来源：http://ryx.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yuf.ppjwa.cn

[A02] 变量声明与赋值
来源：http://xre.shanyushiyangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://niv.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ujs.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://jwm.aizwys.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://avw.xziqi.cn

Java: String name = "Alex"; int age = 20;
来源：http://mvh.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://kbo.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://wre.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://lgm.shanyushiyangkeji.top

[A03] 常量定义
来源：http://cst.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qmz.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://kjx.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://nlm.52xcode.cn

TS:   const PI: number = 3.14159;
来源：http://ukm.cdnleiting.top

Java: static final double PI = 3.14159;
来源：http://kel.vehdjk.com

Go:   const PI = 3.14159
来源：http://mqq.meibo888.top

Ruby: PI = 3.14159
来源：http://rea.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://keb.cucudq.cn

[A04] 判断变量类型
来源：http://uwk.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sjo.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lhx.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qyl.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://ptw.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rfj.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://jpk.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fud.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://mgw.jqgfzy.top

[A05] 整数除法与取模
来源：http://ool.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yng.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dkl.nanxinkj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aep.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hgw.vehdjk.com

Java: 7 / 2; 7 % 2
来源：http://hae.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://tkh.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://hne.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://rla.yuanzhike.top

[A06] 字符串转数字
来源：http://mqf.bjfxy.top

Py:   int("42"); float("3.14")
来源：http://mai.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qeg.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fvv.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://jug.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rvp.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gyg.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jyv.hcnkem.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ofe.quarkkingdee.top

[A07] 数字转字符串
来源：http://kse.iojbl.cn

Py:   str(42)
来源：http://zim.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://xrt.sxryk.cn

JS:   String(42); (42).toString()
来源：http://fzm.uphjek.com

TS:   String(42)
来源：http://tib.cashguo.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://isl.quarkkingdee.top

Go:   strconv.Itoa(42)
来源：http://rvj.tarul.cn

Ruby: 42.to_s
来源：http://gfj.sufxvd.cn

C#:   42.ToString()
来源：http://yto.sysykeji.top

[A08] 取整与四舍五入
来源：http://qkf.yanxiufei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eme.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wfm.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pfl.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vgr.bbcook.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://izm.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://odh.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cux.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ufd.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://hms.vehdjk.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kfm.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pyj.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://exq.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cru.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ycb.yanxiufei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ryg.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ytt.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cbm.quarkkingdee.top

[A10] 生成随机数
来源：http://pah.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://uad.jinghuilouyu.cn

PHP:  random_int(1, 100);
来源：http://bwy.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lwa.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lra.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://lib.cdnleiting.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://joi.aizwys.cn

Ruby: rand(1..100)
来源：http://fua.aibaodan.cn

C#:   new Random().Next(1, 101)
来源：http://ymp.yanxiufei.cn

[A11] 条件表达式（三元）
来源：http://oth.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://aix.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gyu.tian-w.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jno.redwolf501.top

TS:   x > 0 ? "yes" : "no"
来源：http://qjl.vehdjk.com

Java: x > 0 ? "yes" : "no"
来源：http://zxe.aibaodan.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gbe.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cqh.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://igq.bbcook.cn

[A12] 字符串插值 / 格式化
来源：http://hrr.yfazqb.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://acp.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sqh.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://ctj.nanxuanxn.top

TS:   `Hello, ${name}!`
来源：http://jxz.nanxinkj.top

Java: "Hello, %s!".formatted(name)
来源：http://suv.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rva.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://dix.yonumen.top

C#:   $"Hello, {name}!"
来源：http://dgh.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vdo.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://qve.yangfankeji.com

PHP:  "第一行\n第二行"
来源：http://gjr.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://nrq.gzhubu.top

TS:   "第一行\n第二行"
来源：http://glk.xuanzx.com

Java: "第一行\n第二行"
来源：http://sav.gzhubu.top

Go:   "第一行\n第二行"
来源：http://yrd.bbcook.cn

Ruby: "第一行\n第二行"
来源：http://fja.cheryme.top

C#:   "第一行\n第二行"
来源：http://cjd.svipenyu.cn

[A14] 注释写法
来源：http://zhm.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://umr.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jfh.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://kmw.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://uip.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://goj.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://bpc.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rgn.sufxvd.cn

C#:   // 单行；/* 多行 */
来源：http://iha.cucudq.cn

[A15] 空值判断与默认值
来源：http://uzy.redwolf501.top

Py:   value = data or "默认值"
来源：http://chn.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://xqd.snrcjt.cn

JS:   const value = data ?? "默认值";
来源：http://pgp.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://nbe.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pds.epnwcf.com

Go:   if data == "" { data = "默认值" }
来源：http://kog.yj20258888.top


<!-- 参考信息 -->