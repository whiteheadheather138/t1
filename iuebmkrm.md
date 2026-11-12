代发 wailian999

[U81] JS：初始化项目
来源：http://mwx.ivvv.top

npm init -y;  npm i express
来源：http://ezi.316326.xyz

[U82] JS：package.json 脚本
来源：http://ves.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vps.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://gdf.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://nmo.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://qwr.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kse.bbcook.cn

[U85] JS：可选链
来源：http://azf.fzhhl.top

a?.b?.c
来源：http://vyv.nanxinkj.top

[U86] JS：空值合并
来源：http://cpd.nanxinkj.top

a ?? b
来源：http://kcf.yj20258.top

[U87] JS：解构默认值
来源：http://pox.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://kom.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://vvn.jyoumei.cn

{ ...a, ...b }
来源：http://tts.zhengqikj.top

[U89] JS：数组去重
来源：http://zcf.zdbjq.cn

[...new Set(arr)]
来源：http://gli.birdmap.top

[U90] JS：数字数组排序
来源：http://row.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://wny.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://wun.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vnf.yj20258888.top

[U92] JS：深拷贝
来源：http://jtk.yfazqb.com

structuredClone(obj)
来源：http://hwp.gotoacloud.top

[U93] JS：模板字符串
来源：http://ukd.vqdsnc.cn

`共 ${n} 条`
来源：http://lrq.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://ltl.wangshuangyany.cn

const double = x => x * 2;
来源：http://mah.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://cqn.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://jqo.yj202588.top

[U96] JS：async/await 与异常
来源：http://wkw.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gnq.sjlbkw.cn

[U97] JS：并发请求
来源：http://wnv.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bjw.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://gra.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nve.pycfn.com

[U99] JS：事件监听
来源：http://yhn.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://umw.daxiang520.top

[U100] JS：DOM 查询
来源：http://itc.fengsongda.top

document.querySelector(".item")
来源：http://mvz.havefunace.top

[U101] JS：classList 操作
来源：http://zbz.andypj.xyz

el.classList.toggle("active")
来源：http://jot.ehwqpu.com

[U102] JS：本地存储
来源：http://cpk.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nwr.gotoacloud.top

[U103] JS：定时器
来源：http://ynb.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lem.zhiwuduotai.top

[U104] JS：防抖
来源：http://eci.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfy.ehwqpu.com

[U105] JS：节流
来源：http://yzr.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hmz.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://nrv.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ktb.cdnleiting.top

[U107] JS：数字千分位
来源：http://trc.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yxy.zhijiandao.cn

[U108] JS：随机整数
来源：http://wof.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dln.ydjk.org.cn

[U109] JS：数组分组
来源：http://gsp.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://dat.dianchejie.cn

[U110] JS：数组分块
来源：http://snr.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cuj.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://gtv.guowangkeji.top

new Map(Object.entries(obj))
来源：http://trt.yonumen.top

[U112] JS：字符串补位
来源：http://opc.iojbl.cn

"7".padStart(3, "0")
来源：http://fpn.iojbl.cn

[U113] JS：正则替换全部
来源：http://ami.chenlongwang.top

s.replaceAll("a", "b")
来源：http://ngl.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://tlr.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://spd.0kj1m.cn

[U115] JS：生成 UUID
来源：http://aun.chenlongwang.top

crypto.randomUUID()
来源：http://jvi.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://zxp.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://tri.gzhubu.top

[U117] JS：单元测试
来源：http://lru.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://umg.yj202588.top

[U118] JS：开发服务器
来源：http://aak.ybcxt.top

npm i -D vite;  npx vite
来源：http://qhz.yj20258.top

[U119] JS：生产构建
来源：http://wrp.feifeiyinyue.top

npx vite build
来源：http://tpf.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://crm.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://xio.pengpengdd.cyou

================================================================================
来源：http://kjb.shangyingyoupin.top

统计汇总
来源：http://jvd.cheryme.top

================================================================================
来源：http://zte.hnqzz.top

按语言统计（条）：
来源：http://lla.yueranfly.top

Python ......... 252
来源：http://ejo.dashuyun.cn

PHP ............ 252
来源：http://gvm.vehdjk.com

JavaScript ..... 252
来源：http://znl.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://nsn.hesvh.cn

Java ........... 212
来源：http://epw.fanxiaobao.xyz

Go ............. 212
来源：http://zab.hnxiangtu.top

Ruby ........... 212
来源：http://fqn.9152youxi.cn

C# ............. 212
来源：http://poa.zhengqikj.top

C .............. 30
来源：http://bjw.jiagoushi.top

C++ ............ 30
来源：http://inp.birdmap.top

SQL ............ 90
来源：http://huk.zhaomingkeji.xyz

Bash ........... 80
来源：http://upo.pycfn.com

Kotlin ......... 15
来源：http://dqn.vqdsnc.cn

Swift .......... 15
来源：http://seo.xingfuxueyuan.xyz

Lua ............ 10
来源：http://flb.hongshengwenyu.top

Perl ........... 10
来源：http://vix.birdmap.top

Scala .......... 10
来源：http://smc.yj20258.top

------------------------------------
来源：http://rrp.hesvh.cn

合计 ........... 2106 条
来源：http://ssa.guannengcc.top

按章节统计：
来源：http://uns.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://skv.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pjw.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cwo.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kra.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://orn.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yhb.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xry.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kyz.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ufe.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zgq.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hhr.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ual.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://apo.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lmm.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bfe.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vtp.cucudq.cn

Q SQL 专题                              90
来源：http://pwx.mhx1999.top

R Bash 专题                             80
来源：http://vsw.dianchejie.cn

S C / C++ 专题                          60
来源：http://joz.yj20258.top

T 其他语言补充                          60
来源：http://wjz.daxiang520.top

U 高频实用片段                         120
来源：http://vpp.yueranfly.top

------------------------------------
来源：http://oir.sjlbkw.cn

合计                                  2106 条
来源：http://eis.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://inl.yangfankeji.com

使用提醒
来源：http://upi.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://yoj.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qdl.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ztg.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ffg.mhx1999.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hxh.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kgv.ctjpmb.com

—— 文件结束 ——
来源：http://vie.nwbrower.top

================================================================================
来源：http://sqj.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://fcf.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://zwy.daria6918.cn

================================================================================
来源：http://rua.jianghu66.top

【收录内容】
来源：http://isv.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pwq.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hjb.ybcxt.top

SQL · Bash · C · C++
来源：http://wcn.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://elr.xinyue.icu

【使用说明】
来源：http://per.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vqe.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pcw.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ixs.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cfx.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uqp.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eky.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ofe.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uib.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fxs.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wgn.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qkm.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tun.jinghuilouyu.cn

【文件统计】
来源：http://qin.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wyh.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://fuv.xingfuxueyuan.xyz

目  录
来源：http://pdw.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://zvq.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rtu.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://djd.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wjn.ydzc1.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ygd.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wns.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yvt.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wmk.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://guc.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nek.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lit.zhijiandao.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lsa.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lwr.ehwqpu.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vtx.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zmq.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bxc.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://joe.shzxlz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zzr.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://srb.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mfb.tian-w.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bbr.gzhubu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yve.zhengqikj.top

================================================================================
来源：http://lfq.jyoumei.cn

A. 基础语法与类型
来源：http://cdt.jlsjyb.cn

================================================================================
来源：http://ujz.chenlongwang.top

[A01] Hello World
来源：http://wth.dianchejie.cn

Py:   print("Hello, World!")
来源：http://ehw.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://shb.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://lqm.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mbx.xingfuxueyuan.xyz

Java: System.out.println("Hello, World!");
来源：http://kom.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://akz.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://lbr.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://zmr.jiagoushi.top

[A02] 变量声明与赋值
来源：http://zfu.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kvl.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lia.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://xug.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mbd.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://crf.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://eya.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://xhw.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eay.smart0.xyz

[A03] 常量定义
来源：http://hcy.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://emu.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://tnk.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://nuk.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://xhj.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://shw.hnqzz.top

Go:   const PI = 3.14159
来源：http://fdb.sweek.top

Ruby: PI = 3.14159
来源：http://rxz.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://grt.quarkkingdee.top

[A04] 判断变量类型
来源：http://onf.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xrg.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uha.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xwq.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://bxx.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wvo.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://cqh.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://oar.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://ypm.316326.xyz

[A05] 整数除法与取模
来源：http://zbz.hfpthk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hps.chenzaomai.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://uar.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iif.daxiang520.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mcc.cdnleiting.top

Java: 7 / 2; 7 % 2
来源：http://vss.guannengcc.top

Go:   7 / 2; 7 % 2
来源：http://wdt.nanxuanxn.top

Ruby: 7 / 2; 7 % 2
来源：http://idl.havefunace.top

C#:   7 / 2; 7 % 2
来源：http://dry.vehdjk.com

[A06] 字符串转数字
来源：http://ajp.wangshuangyany.cn

Py:   int("42"); float("3.14")
来源：http://osv.uphjek.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vbk.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vxx.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://bmg.chenzaomai.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xra.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dfx.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kaj.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lfi.ydjk.org.cn

[A07] 数字转字符串
来源：http://cdj.9152youxi.cn

Py:   str(42)
来源：http://nsg.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://gzj.xziqi.cn

JS:   String(42); (42).toString()
来源：http://iow.nanxinkj.top

TS:   String(42)
来源：http://kdy.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://etd.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://myv.aibaodan.cn

Ruby: 42.to_s
来源：http://wek.cucudq.cn

C#:   42.ToString()
来源：http://jmo.havefunace.top

[A08] 取整与四舍五入
来源：http://rgm.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ylf.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://daq.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qsw.0kj1m.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jtx.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://afu.snrcjt.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xeo.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fyv.ivvv.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hui.meibo888.top

[A09] 绝对值与最大最小值
来源：http://gru.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xzk.vqdsnc.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vyd.fehbvm.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jqm.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zzd.yfazqb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xqf.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://njf.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gvf.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gho.gzhubu.top

[A10] 生成随机数
来源：http://qts.xziqi.cn

Py:   import random; random.randint(1, 100)
来源：http://pkb.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://llh.kuanghao11.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lgh.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://elg.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://kyf.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jdd.svipenyu.cn

Ruby: rand(1..100)
来源：http://iab.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://vqn.xziqi.cn

[A11] 条件表达式（三元）
来源：http://wkh.hnxiangtu.top

Py:   "yes" if x > 0 else "no"
来源：http://aua.ydjk.org.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dly.yuanzhike.top

JS:   x > 0 ? "yes" : "no"
来源：http://rot.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ddj.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://cur.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xdj.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fbo.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://qbe.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://dxw.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gwp.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wnl.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://zjs.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://esu.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://aoo.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hjl.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://wbx.zhiwuduotai.top

C#:   $"Hello, {name}!"
来源：http://bmz.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vnz.316326.xyz

Py:   "第一行\n第二行"
来源：http://eqw.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://ouc.andypj.xyz

JS:   "第一行\n第二行"
来源：http://moj.tian-w.cn

TS:   "第一行\n第二行"
来源：http://liy.yvedp.cn


<!-- 参考信息 -->