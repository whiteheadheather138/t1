代发 wailian999

[U87] JS：解构默认值
来源：http://cue.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://tad.jinqigufen.top

[U88] JS：对象展开合并
来源：http://bmp.chenzaomai.com

{ ...a, ...b }
来源：http://fsc.svipenyu.cn

[U89] JS：数组去重
来源：http://dfu.yj20258.top

[...new Set(arr)]
来源：http://nzp.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://mha.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://gxu.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://lwc.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xvr.wangdashe.top

[U92] JS：深拷贝
来源：http://ydg.zhengqikj.top

structuredClone(obj)
来源：http://nwb.xziqi.cn

[U93] JS：模板字符串
来源：http://zje.yuxming.cn

`共 ${n} 条`
来源：http://ygg.sjlbkw.cn

[U94] JS：箭头函数
来源：http://avm.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://aey.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://swc.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://csl.epnwcf.com

[U96] JS：async/await 与异常
来源：http://zav.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dql.aibaodan.cn

[U97] JS：并发请求
来源：http://glf.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bfc.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://pdy.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gsd.zdqjudy.top

[U99] JS：事件监听
来源：http://mcq.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://zio.yj20258888.top

[U100] JS：DOM 查询
来源：http://mzy.snrcjt.cn

document.querySelector(".item")
来源：http://xgo.9152youxi.cn

[U101] JS：classList 操作
来源：http://gio.9152youxi.cn

el.classList.toggle("active")
来源：http://hdg.xziqi.cn

[U102] JS：本地存储
来源：http://dim.c1oappe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zgz.daria6918.cn

[U103] JS：定时器
来源：http://cww.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vqm.hongshengwenyu.top

[U104] JS：防抖
来源：http://esn.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://luu.wangshuangyany.cn

[U105] JS：节流
来源：http://xhv.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qgo.yj20258.top

[U106] JS：日期格式化
来源：http://vqn.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://srp.haohaochexian.top

[U107] JS：数字千分位
来源：http://emd.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://awb.zhiwuduotai.top

[U108] JS：随机整数
来源：http://ddi.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cyn.chenlongwang.top

[U109] JS：数组分组
来源：http://mql.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://uht.guannengcc.top

[U110] JS：数组分块
来源：http://dhm.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bzu.dianchejie.cn

[U111] JS：对象转 Map
来源：http://ezh.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://qgv.gogol.net.cn

[U112] JS：字符串补位
来源：http://qaq.zycfv.cn

"7".padStart(3, "0")
来源：http://qdi.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://cql.ydzc1.top

s.replaceAll("a", "b")
来源：http://yqf.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://sqw.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zsh.jqgfzy.top

[U115] JS：生成 UUID
来源：http://kpj.nanxinkj.top

crypto.randomUUID()
来源：http://lur.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://kjo.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://shh.zhixingplan.top

[U117] JS：单元测试
来源：http://zlf.dianchejie.cn

npm i -D vitest;  npx vitest
来源：http://mdk.c1oappe.top

[U118] JS：开发服务器
来源：http://ffm.hammf.cn

npm i -D vite;  npx vite
来源：http://vdl.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://hrr.zdqjudy.top

npx vite build
来源：http://hbl.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://ciq.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://srm.bbcook.cn

================================================================================
来源：http://cne.jinqigufen.top

统计汇总
来源：http://vbj.hfpthk.cn

================================================================================
来源：http://vzc.zycfv.cn

按语言统计（条）：
来源：http://ctb.hysaishi.cn

Python ......... 252
来源：http://svh.jlsjyb.cn

PHP ............ 252
来源：http://tts.yanxiufei.cn

JavaScript ..... 252
来源：http://wzt.sysykeji.top

TypeScript ..... 212
来源：http://lot.fzhhl.top

Java ........... 212
来源：http://sjq.nanxinkj.top

Go ............. 212
来源：http://lby.xziqi.cn

Ruby ........... 212
来源：http://pvb.jinqigufen.top

C# ............. 212
来源：http://chi.gotoacloud.top

C .............. 30
来源：http://rpi.ehwqpu.com

C++ ............ 30
来源：http://qtm.dianchejie.cn

SQL ............ 90
来源：http://jea.shangyingyoupin.top

Bash ........... 80
来源：http://nfd.hammf.cn

Kotlin ......... 15
来源：http://tav.fengsongda.top

Swift .......... 15
来源：http://jkx.daxiang520.top

Lua ............ 10
来源：http://tbk.52xcode.cn

Perl ........... 10
来源：http://yfl.yuxming.cn

Scala .......... 10
来源：http://qou.yuxming.cn

------------------------------------
来源：http://osu.aizwys.cn

合计 ........... 2106 条
来源：http://bkm.xinyue.icu

按章节统计：
来源：http://cyy.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://amt.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jay.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lmd.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hbq.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bhz.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://net.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yfe.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dip.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ehg.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kdg.dianchejie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ymr.ctjpmb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://emv.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://icd.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lqu.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xuj.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gwr.c1oappe.top

Q SQL 专题                              90
来源：http://uzi.yongpay.top

R Bash 专题                             80
来源：http://bdr.uphjek.com

S C / C++ 专题                          60
来源：http://ich.zhoulong.xyz

T 其他语言补充                          60
来源：http://ztk.jqgfzy.top

U 高频实用片段                         120
来源：http://miv.smart0.xyz

------------------------------------
来源：http://sun.gzhubu.top

合计                                  2106 条
来源：http://tov.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://nyp.havefunace.top

使用提醒
来源：http://xkm.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://zyn.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wgh.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wxb.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zer.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pez.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lcd.yfazqb.com

—— 文件结束 ——
来源：http://kuf.hnxiangtu.top

================================================================================
来源：http://jml.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ahh.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://pqy.haohaochexian.top

================================================================================
来源：http://tza.cheryme.top

【收录内容】
来源：http://ggp.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zxu.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xzb.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://wuw.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dmy.wangdashe.top

【使用说明】
来源：http://sgi.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ymi.quarkkingdee.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kxj.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://unt.birdmap.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jha.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://goc.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://txe.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fpc.zdqjudy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ery.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fcw.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ivh.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tbm.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://raz.birdmap.top

【文件统计】
来源：http://ugk.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gln.fzhhl.top

--------------------------------------------------------------------------------
来源：http://xkc.bbcook.cn

目  录
来源：http://agq.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://yux.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yjc.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jvz.andypj.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lkh.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lkp.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://klu.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eax.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dyf.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nya.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rev.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fyg.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tps.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zne.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yel.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qib.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xoo.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://evf.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lmc.jiagoushi.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vfl.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nie.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tpt.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ooi.jinyuanbaomall.cn

================================================================================
来源：http://twu.zhixingplan.top

A. 基础语法与类型
来源：http://dsm.fengsongda.top

================================================================================
来源：http://puh.hcnkem.com

[A01] Hello World
来源：http://vbw.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://lbw.hcnkem.com

PHP:  echo "Hello, World!";
来源：http://low.jinghuilouyu.cn

JS:   console.log("Hello, World!");
来源：http://dqi.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ool.nanxinkj.top

Java: System.out.println("Hello, World!");
来源：http://ikm.zhengqikj.top

Go:   fmt.Println("Hello, World!")
来源：http://ozn.hammf.cn

Ruby: puts "Hello, World!"
来源：http://ayq.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ucx.hcnkem.com

[A02] 变量声明与赋值
来源：http://uxq.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://usr.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rwo.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://inz.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cyq.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://gmq.c1oappe.top

Go:   name := "Alex"; age := 20
来源：http://jlk.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://wju.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://vvf.hnxiangtu.top

[A03] 常量定义
来源：http://qyf.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pdv.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://uoi.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://thk.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://yyz.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://dhi.guannengcc.top

Go:   const PI = 3.14159
来源：http://hbv.tarul.cn

Ruby: PI = 3.14159
来源：http://lfk.tanke756.top

C#:   const double PI = 3.14159;
来源：http://rhq.svipenyu.cn

[A04] 判断变量类型
来源：http://qtt.zhengqikj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hvz.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fhd.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nyi.yuanzhike.top

TS:   typeof x; x instanceof Date
来源：http://jmf.yueranfly.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wva.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://hye.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dku.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://bxp.9152youxi.cn

[A05] 整数除法与取模
来源：http://fxl.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xbe.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vfx.pengpengdd.cyou

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baj.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://urd.jinqigufen.top

Java: 7 / 2; 7 % 2
来源：http://qtr.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://fwy.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://pkn.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://yiz.cashguo.top

[A06] 字符串转数字
来源：http://ckb.yongpay.top

Py:   int("42"); float("3.14")
来源：http://vcw.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ntw.hfpthk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rsg.sufxvd.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xom.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lsu.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://org.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://evt.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jlz.hnxiangtu.top

[A07] 数字转字符串
来源：http://upw.cheryme.top

Py:   str(42)
来源：http://jam.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://uas.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://vhf.chenjidiqi.icu

TS:   String(42)
来源：http://rme.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rmy.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://utc.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://htl.daria6918.cn

C#:   42.ToString()
来源：http://iah.ywan-chungtsiang.top

[A08] 取整与四舍五入
来源：http://npg.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://djh.aizwys.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xhd.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qeh.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qnn.fehbvm.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wgm.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ohy.zhengqikj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hza.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gsv.uphjek.com

[A09] 绝对值与最大最小值
来源：http://fpo.yfazqb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oxd.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cgf.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pxu.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xtt.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://szu.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kkn.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bax.tanke756.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://akq.ehwqpu.com

[A10] 生成随机数
来源：http://ohj.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://dwg.sysykeji.top

PHP:  random_int(1, 100);
来源：http://gho.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ska.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zki.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://lmp.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bhl.jiagoushi.top

Ruby: rand(1..100)
来源：http://khk.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://dgq.ydzc1.top

[A11] 条件表达式（三元）
来源：http://xig.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://qve.jqgfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://snb.epnwcf.com

JS:   x > 0 ? "yes" : "no"
来源：http://mxb.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cxu.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://fym.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wnt.shzxlz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yrg.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ogj.meibo888.top

[A12] 字符串插值 / 格式化
来源：http://nav.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pfu.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://plo.jlsjyb.cn

JS:   `Hello, ${name}!`
来源：http://kis.tanke756.top

TS:   `Hello, ${name}!`
来源：http://kcj.zhixingplan.top

Java: "Hello, %s!".formatted(name)
来源：http://awf.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fwo.hesvh.cn

Ruby: "Hello, #{name}!"
来源：http://ipn.aizwys.cn

C#:   $"Hello, {name}!"
来源：http://mxx.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ybu.nanxuanxn.top

Py:   "第一行\n第二行"
来源：http://qpm.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://ggb.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://aiy.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://ybl.cucudq.cn

Java: "第一行\n第二行"
来源：http://ine.gaohongyu789.top

Go:   "第一行\n第二行"
来源：http://cpj.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://nca.ivvv.top

C#:   "第一行\n第二行"
来源：http://lgr.xuanzx.com

[A14] 注释写法
来源：http://mfj.quarkkingdee.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://chk.shuidangran.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yps.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://ora.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://gcz.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jap.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://ecq.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://grr.0kj1m.cn


<!-- 参考信息 -->