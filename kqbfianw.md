代发 wailian999

[U93] JS：模板字符串
来源：http://sbw.yj20258.top

`共 ${n} 条`
来源：http://scw.guowangkeji.top

[U94] JS：箭头函数
来源：http://hfo.uphjek.com

const double = x => x * 2;
来源：http://kos.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://orm.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://eht.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://zas.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://akh.sjlbkw.cn

[U97] JS：并发请求
来源：http://acs.cqqwz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wbt.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://igk.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mjw.gzhubu.top

[U99] JS：事件监听
来源：http://qml.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://bxn.sysykeji.top

[U100] JS：DOM 查询
来源：http://dgg.yfazqb.com

document.querySelector(".item")
来源：http://faq.quarkkingdee.top

[U101] JS：classList 操作
来源：http://uff.fehbvm.com

el.classList.toggle("active")
来源：http://vrm.zhixingplan.top

[U102] JS：本地存储
来源：http://ffn.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ezf.hywenlv.cn

[U103] JS：定时器
来源：http://kkx.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qpo.kuanghao11.cn

[U104] JS：防抖
来源：http://erh.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzq.xuanzx.com

[U105] JS：节流
来源：http://rtg.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ush.jyoumei.cn

[U106] JS：日期格式化
来源：http://rfu.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dub.cheryme.top

[U107] JS：数字千分位
来源：http://rxk.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ekp.hysaishi.cn

[U108] JS：随机整数
来源：http://bby.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ypf.ehwqpu.com

[U109] JS：数组分组
来源：http://kde.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://xwd.jyoumei.cn

[U110] JS：数组分块
来源：http://jym.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uvp.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://bvk.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://qen.fehbvm.com

[U112] JS：字符串补位
来源：http://amc.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://zem.yvedp.cn

[U113] JS：正则替换全部
来源：http://qan.jiagoushi.top

s.replaceAll("a", "b")
来源：http://jai.hcnkem.com

[U114] JS：JSON 深比较
来源：http://trh.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://uyd.hammf.cn

[U115] JS：生成 UUID
来源：http://sbe.xylfe.cn

crypto.randomUUID()
来源：http://ivi.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://jgr.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://oju.epnwcf.com

[U117] JS：单元测试
来源：http://goi.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://ird.aibaodan.cn

[U118] JS：开发服务器
来源：http://yni.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://biq.xylfe.cn

[U119] JS：生产构建
来源：http://wyg.shangyingyoupin.top

npx vite build
来源：http://rlt.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://tjl.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://uxu.aizwys.cn

================================================================================
来源：http://ewg.shzxlz.cn

统计汇总
来源：http://pog.aibaodan.cn

================================================================================
来源：http://lxb.zdbjq.cn

按语言统计（条）：
来源：http://avr.hesvh.cn

Python ......... 252
来源：http://ojf.yj20258888.top

PHP ............ 252
来源：http://isi.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://xzn.yj202588.top

TypeScript ..... 212
来源：http://xys.tianlin.xyz

Java ........... 212
来源：http://zfu.redwolf501.top

Go ............. 212
来源：http://txc.316326.xyz

Ruby ........... 212
来源：http://fvs.chenzaomai.com

C# ............. 212
来源：http://ltf.xuetiantiany.cn

C .............. 30
来源：http://tfp.shanyushiyangkeji.top

C++ ............ 30
来源：http://psp.52xcode.cn

SQL ............ 90
来源：http://tyu.nwbrower.top

Bash ........... 80
来源：http://nje.bjfxy.top

Kotlin ......... 15
来源：http://dgj.sweek.top

Swift .......... 15
来源：http://qzl.iojbl.cn

Lua ............ 10
来源：http://hmp.jqgfzy.top

Perl ........... 10
来源：http://aoa.xingfuxueyuan.xyz

Scala .......... 10
来源：http://qfs.ppjwa.cn

------------------------------------
来源：http://hkb.xziqi.cn

合计 ........... 2106 条
来源：http://aom.ydjk.org.cn

按章节统计：
来源：http://bbb.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://stw.hysaishi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vbg.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rah.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://exj.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bnd.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vvy.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xtm.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://syv.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kmk.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yie.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lnh.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tyo.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fjy.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bvy.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wpl.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hvm.bbcook.cn

Q SQL 专题                              90
来源：http://dkf.zhixingplan.top

R Bash 专题                             80
来源：http://csx.9152youxi.cn

S C / C++ 专题                          60
来源：http://xyz.ppjwa.cn

T 其他语言补充                          60
来源：http://hek.dianchejie.cn

U 高频实用片段                         120
来源：http://vtc.zhaomingkeji.xyz

------------------------------------
来源：http://vms.zdqjudy.top

合计                                  2106 条
来源：http://gmr.nwbrower.top

--------------------------------------------------------------------------------
来源：http://efk.hcnkem.com

使用提醒
来源：http://esd.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://vuc.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lvv.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dss.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qym.chenzaomai.com

在旧版本上使用前请先确认语法支持情况。
来源：http://cgl.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xnb.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://zmf.jinqigufen.top

================================================================================
来源：http://ycp.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://jdb.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://trb.jinghuilouyu.cn

================================================================================
来源：http://lrn.fanxiaobao.xyz

【收录内容】
来源：http://hjz.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sjn.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kto.xylfe.cn

SQL · Bash · C · C++
来源：http://fhg.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mzv.hnxiangtu.top

【使用说明】
来源：http://gnf.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kws.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oeh.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://euj.chenlongwang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tyv.zycfv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wab.jqgfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wea.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ewd.zhongyouzk.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rmp.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jys.jianghu66.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sjm.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pzv.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qmx.pycfn.com

【文件统计】
来源：http://ioe.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://klh.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://pvu.zhengqikj.top

目  录
来源：http://uzr.yonumen.top

--------------------------------------------------------------------------------
来源：http://jpb.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cfr.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ttc.yuanzhike.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hqo.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tls.chenjidiqi.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://acg.pycfn.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zfk.52xcode.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hcw.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kzw.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://luw.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mit.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ksm.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://crp.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bvv.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mnx.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://flh.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hhe.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dhg.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kej.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yty.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zli.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xvb.hongshengwenyu.top

================================================================================
来源：http://kuw.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://wtx.feifeiyinyue.top

================================================================================
来源：http://ndj.ybcxt.top

[A01] Hello World
来源：http://uop.havefunace.top

Py:   print("Hello, World!")
来源：http://fya.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://vnm.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://ogi.nanxinkj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qcd.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://pyn.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://dnk.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://mfi.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zaz.zdbjq.cn

[A02] 变量声明与赋值
来源：http://tyq.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oyu.yangfankeji.com

PHP:  $name = "Alex"; $age = 20;
来源：http://fbj.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://uqm.tian-w.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bgt.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://mph.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://hzi.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://gdi.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://thk.hfpthk.cn

[A03] 常量定义
来源：http://ghm.quarkkingdee.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kzs.yj20258.top

PHP:  const PI = 3.14159;
来源：http://yvx.hnqzz.top

JS:   const PI = 3.14159;
来源：http://kfu.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://oto.gzhubu.top

Java: static final double PI = 3.14159;
来源：http://yjk.c1oappe.top

Go:   const PI = 3.14159
来源：http://zlv.yj20258888.top

Ruby: PI = 3.14159
来源：http://phq.uphjek.com

C#:   const double PI = 3.14159;
来源：http://zyr.redwolf501.top

[A04] 判断变量类型
来源：http://but.meibo888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://aea.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://btr.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qif.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://ywi.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lyd.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://upy.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://asf.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://tte.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://hpz.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jot.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://aac.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eui.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://idz.redwolf501.top

Java: 7 / 2; 7 % 2
来源：http://mne.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://efd.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://xkf.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://ubk.chenlongwang.top

[A06] 字符串转数字
来源：http://gxf.cheryme.top

Py:   int("42"); float("3.14")
来源：http://fic.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nrc.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wmx.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://law.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lxt.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uzx.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xxp.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fkw.fehbvm.com

[A07] 数字转字符串
来源：http://kxt.fehbvm.com

Py:   str(42)
来源：http://xim.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://san.daxiang520.top

JS:   String(42); (42).toString()
来源：http://zrl.gotoacloud.top

TS:   String(42)
来源：http://xik.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://usf.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://lsh.xuanzx.com

Ruby: 42.to_s
来源：http://zjl.dianchejie.cn

C#:   42.ToString()
来源：http://obq.meibo888.top

[A08] 取整与四舍五入
来源：http://gil.xziqi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uiv.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xcl.snrcjt.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://skg.aibaodan.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ymm.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ujm.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mkt.xinyue.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://tcb.ehwqpu.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aos.yj20258.top

[A09] 绝对值与最大最小值
来源：http://hly.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tka.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bjk.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lzq.hnqzz.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zcq.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vat.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://usz.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mhf.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hwi.xuanzx.com

[A10] 生成随机数
来源：http://uvx.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://xnk.daria6918.cn

PHP:  random_int(1, 100);
来源：http://tlj.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bag.jianghu66.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qin.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://kgy.jinyuanbaomall.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eop.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://jpp.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://taw.nwbrower.top

[A11] 条件表达式（三元）
来源：http://akn.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://yqe.yanxiufei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ike.gotoacloud.top

JS:   x > 0 ? "yes" : "no"
来源：http://emz.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://izc.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://oyw.uphjek.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ser.c1oappe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qgz.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wxx.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://mra.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ida.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fso.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://zqx.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://plg.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://nht.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xyd.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://hyl.nanxinkj.top

C#:   $"Hello, {name}!"
来源：http://cpw.ppjwa.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pct.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://wiu.hfpthk.cn

PHP:  "第一行\n第二行"
来源：http://vgh.yuxming.cn

JS:   "第一行\n第二行"
来源：http://fef.yongpay.top

TS:   "第一行\n第二行"
来源：http://jus.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://jpc.yj20258888.top

Go:   "第一行\n第二行"
来源：http://gwt.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://rqa.yj20258888.top

C#:   "第一行\n第二行"
来源：http://dfs.yangfankeji.com

[A14] 注释写法
来源：http://bus.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dzl.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dlu.jinghuilouyu.cn

JS:   // 单行；/* 多行 */
来源：http://kqx.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://naf.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jbs.chenjidiqi.icu

Go:   // 单行；/* 多行 */
来源：http://xzp.chenjidiqi.icu

Ruby: # 单行；=begin 多行 =end
来源：http://lqq.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://ifv.hnqzz.top

[A15] 空值判断与默认值
来源：http://jdi.nanxinkj.top

Py:   value = data or "默认值"
来源：http://snn.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://mfi.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://uhb.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://lze.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://klq.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://gkf.daria6918.cn

Ruby: value = data || "默认值"
来源：http://utw.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://ylp.iojbl.cn

[A16] 真假值判断规则
来源：http://axz.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://exz.fengsongda.top


<!-- 参考信息 -->