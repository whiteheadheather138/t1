代发 wailian999

[U87] JS：解构默认值
来源：http://ozh.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://hkv.sxryk.cn

[U88] JS：对象展开合并
来源：http://jcp.wangshuangyany.cn

{ ...a, ...b }
来源：http://all.mhx1999.top

[U89] JS：数组去重
来源：http://ppc.hammf.cn

[...new Set(arr)]
来源：http://jpy.chenzaomai.com

[U90] JS：数字数组排序
来源：http://bvj.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://fos.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://rpr.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ohc.zhengqikj.top

[U92] JS：深拷贝
来源：http://ckb.gzhubu.top

structuredClone(obj)
来源：http://ddh.bjfxy.top

[U93] JS：模板字符串
来源：http://wpw.nanxuanxn.top

`共 ${n} 条`
来源：http://ooj.zhoulong.xyz

[U94] JS：箭头函数
来源：http://ytp.jyoumei.cn

const double = x => x * 2;
来源：http://vkg.tarul.cn

[U95] JS：Promise 包装
来源：http://hxb.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://bda.zycfv.cn

[U96] JS：async/await 与异常
来源：http://chm.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rfe.gogol.net.cn

[U97] JS：并发请求
来源：http://iys.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kca.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://xqm.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://flq.ydjk.org.cn

[U99] JS：事件监听
来源：http://pke.birdmap.top

el.addEventListener("click", e => {})
来源：http://tbt.ppjwa.cn

[U100] JS：DOM 查询
来源：http://cuq.andypj.xyz

document.querySelector(".item")
来源：http://zcg.shzxlz.cn

[U101] JS：classList 操作
来源：http://iym.quarkkingdee.top

el.classList.toggle("active")
来源：http://tmo.zhixingplan.top

[U102] JS：本地存储
来源：http://qis.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kcn.shanyushiyangtech.top

[U103] JS：定时器
来源：http://iue.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://whm.nanxinkj.top

[U104] JS：防抖
来源：http://fms.andypj.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://byk.pengpengdd.cyou

[U105] JS：节流
来源：http://wit.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bpf.nwbrower.top

[U106] JS：日期格式化
来源：http://xrk.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://npl.yuxming.cn

[U107] JS：数字千分位
来源：http://wyc.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://acd.yanxiufei.cn

[U108] JS：随机整数
来源：http://mnw.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xnx.jianghu66.top

[U109] JS：数组分组
来源：http://uxk.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://lzk.jianghu66.top

[U110] JS：数组分块
来源：http://hrq.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://emn.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://dio.havefunace.top

new Map(Object.entries(obj))
来源：http://dnm.hnqzz.top

[U112] JS：字符串补位
来源：http://rzv.c1oappe.top

"7".padStart(3, "0")
来源：http://fpe.9152youxi.cn

[U113] JS：正则替换全部
来源：http://zyz.xylfe.cn

s.replaceAll("a", "b")
来源：http://uoq.zycfv.cn

[U114] JS：JSON 深比较
来源：http://ine.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ccf.shuidangran.top

[U115] JS：生成 UUID
来源：http://gdj.guowangkeji.top

crypto.randomUUID()
来源：http://qkh.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://cxp.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://anz.cucudq.cn

[U117] JS：单元测试
来源：http://jrs.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://ekd.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://sjg.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://bbo.zhengqikj.top

[U119] JS：生产构建
来源：http://sxo.yuxming.cn

npx vite build
来源：http://zyw.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://bnw.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://srq.meibo888.top

================================================================================
来源：http://axa.quarkkingdee.top

统计汇总
来源：http://vvc.zdbjq.cn

================================================================================
来源：http://lkf.shangyingyoupin.top

按语言统计（条）：
来源：http://rkn.chenjidiqi.icu

Python ......... 252
来源：http://jkj.hcnkem.com

PHP ............ 252
来源：http://gci.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://azq.ppjwa.cn

TypeScript ..... 212
来源：http://dpa.hysaishi.cn

Java ........... 212
来源：http://xnl.yvedp.cn

Go ............. 212
来源：http://clb.wangshuangyany.cn

Ruby ........... 212
来源：http://mbx.xinyue.icu

C# ............. 212
来源：http://tia.epnwcf.com

C .............. 30
来源：http://xos.feifeiyinyue.top

C++ ............ 30
来源：http://ziz.jianghu66.top

SQL ............ 90
来源：http://cct.pycfn.com

Bash ........... 80
来源：http://fyx.sysykeji.top

Kotlin ......... 15
来源：http://zbl.cheryme.top

Swift .......... 15
来源：http://erq.jinghuilouyu.cn

Lua ............ 10
来源：http://jkn.shangyingyoupin.top

Perl ........... 10
来源：http://gzg.wangdashe.top

Scala .......... 10
来源：http://ljo.jyoumei.cn

------------------------------------
来源：http://qzj.hfpthk.cn

合计 ........... 2106 条
来源：http://seo.bjfxy.top

按章节统计：
来源：http://hiy.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rqu.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jed.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wlz.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cvw.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://leg.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xvp.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://svw.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rou.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ffy.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gkj.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bab.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nhz.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wff.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tjt.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://upg.chenlongwang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ieo.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://wdj.zhoulong.xyz

R Bash 专题                             80
来源：http://kmq.yfazqb.com

S C / C++ 专题                          60
来源：http://ffa.tanke756.top

T 其他语言补充                          60
来源：http://mlp.guannengcc.top

U 高频实用片段                         120
来源：http://jdp.hnqzz.top

------------------------------------
来源：http://wxx.pengpengdd.cyou

合计                                  2106 条
来源：http://eus.guannengcc.top

--------------------------------------------------------------------------------
来源：http://nur.xinyue.icu

使用提醒
来源：http://vme.cheryme.top

--------------------------------------------------------------------------------
来源：http://ltd.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aki.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nch.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ptd.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://qta.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rip.wangdashe.top

—— 文件结束 ——
来源：http://nye.daria6918.cn

================================================================================
来源：http://ced.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://vbq.pycfn.com

Common Programming Examples Cheat Book
来源：http://mvj.yongpay.top

================================================================================
来源：http://upm.guannengcc.top

【收录内容】
来源：http://til.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hse.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jrh.redwolf501.top

SQL · Bash · C · C++
来源：http://slv.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lzz.zdqjudy.top

【使用说明】
来源：http://rll.daxiang520.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ftt.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rhb.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iae.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dss.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lmd.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vkc.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uvl.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jya.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zxn.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ilh.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uxd.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iqm.ydzc1.top

【文件统计】
来源：http://jpa.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zbj.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://xqg.hesvh.cn

目  录
来源：http://cvm.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://jij.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ucc.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pyh.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kpg.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mzs.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tqc.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vfq.tianlin.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://soo.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wga.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sxn.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gvw.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jzd.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://egv.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fnz.gzhubu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gzj.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://spy.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vgr.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rfk.fengsongda.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dge.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kxu.ehwqpu.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rhg.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nwm.jyoumei.cn

================================================================================
来源：http://fyw.sufxvd.cn

A. 基础语法与类型
来源：http://clj.shanyushiyangkeji.top

================================================================================
来源：http://btc.c1oappe.top

[A01] Hello World
来源：http://jyk.nanxinkj.top

Py:   print("Hello, World!")
来源：http://slj.yj202588.top

PHP:  echo "Hello, World!";
来源：http://dpc.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://czd.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pzc.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://urg.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://hgq.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://one.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://zxs.hesvh.cn

[A02] 变量声明与赋值
来源：http://wuz.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wme.zycfv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kpe.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://icb.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mth.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://huw.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://dfr.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://aax.hnqzz.top

C#:   string name = "Alex"; int age = 20;
来源：http://xom.iojbl.cn

[A03] 常量定义
来源：http://iep.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ttw.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://iro.ivvv.top

JS:   const PI = 3.14159;
来源：http://drz.yonumen.top

TS:   const PI: number = 3.14159;
来源：http://pdy.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://ghu.bbcook.cn

Go:   const PI = 3.14159
来源：http://djn.zhongyouzk.top

Ruby: PI = 3.14159
来源：http://zbh.xylfe.cn

C#:   const double PI = 3.14159;
来源：http://jjb.hysaishi.cn

[A04] 判断变量类型
来源：http://acv.meibo888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://taa.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ntt.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ujd.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://gdm.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dse.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://tnp.zhixingplan.top

Ruby: x.class; x.is_a?(Integer)
来源：http://exd.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://fpo.sysykeji.top

[A05] 整数除法与取模
来源：http://yxf.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zft.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://off.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dsx.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xnx.yuxming.cn

Java: 7 / 2; 7 % 2
来源：http://dgw.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://str.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://jxb.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://kyt.hesvh.cn

[A06] 字符串转数字
来源：http://kfq.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://kdb.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wdd.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://udb.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rdc.fengsongda.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rup.xylfe.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xue.tianlin.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://qsd.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oxe.yj20258888.top

[A07] 数字转字符串
来源：http://ejg.shuidangran.top

Py:   str(42)
来源：http://tqx.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://wsr.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://pby.aizwys.cn

TS:   String(42)
来源：http://mnx.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mtt.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://ggp.zhijiandao.cn

Ruby: 42.to_s
来源：http://enq.zhongyouzk.top

C#:   42.ToString()
来源：http://eub.sufxvd.cn

[A08] 取整与四舍五入
来源：http://xgd.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qkb.hongshengwenyu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aar.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bhu.tanke756.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ztn.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uoa.vehdjk.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iju.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://num.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iya.zhiwuduotai.top

[A09] 绝对值与最大最小值
来源：http://jcs.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tya.9152youxi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jra.yonumen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://own.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iqg.cashguo.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kcu.hnqzz.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sgo.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bpy.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lbm.xuanzx.com

[A10] 生成随机数
来源：http://hcm.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://zvt.jinqigufen.top

PHP:  random_int(1, 100);
来源：http://cku.jianghu66.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rbz.feifeiyinyue.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://psr.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://trq.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hqt.yuxming.cn

Ruby: rand(1..100)
来源：http://tiz.9152youxi.cn

C#:   new Random().Next(1, 101)
来源：http://knc.hesvh.cn

[A11] 条件表达式（三元）
来源：http://tjm.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://muj.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tqm.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ysk.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tnz.sysykeji.top

Java: x > 0 ? "yes" : "no"
来源：http://bgg.xuetiantiany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://don.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wjr.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://xqj.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://bxj.jiagoushi.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nam.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://krr.jyoumei.cn

JS:   `Hello, ${name}!`
来源：http://wzb.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://lzv.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://auh.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fta.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://ezc.jianghu66.top

C#:   $"Hello, {name}!"
来源：http://kit.sysykeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lmy.svipenyu.cn

Py:   "第一行\n第二行"
来源：http://evx.316326.xyz

PHP:  "第一行\n第二行"
来源：http://ent.uphjek.com

JS:   "第一行\n第二行"
来源：http://adv.ctjpmb.com

TS:   "第一行\n第二行"
来源：http://emj.zdbjq.cn

Java: "第一行\n第二行"
来源：http://jxo.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://bvk.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://ijj.316326.xyz

C#:   "第一行\n第二行"
来源：http://zpj.jyoumei.cn

[A14] 注释写法
来源：http://nnf.hammf.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pow.zhiwuduotai.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lat.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://wak.jinqigfzy.top

TS:   // 单行；/* 多行 */
来源：http://hib.shanyushiyangtech.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jep.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://uft.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://zzw.ctjpmb.com


<!-- 参考信息 -->