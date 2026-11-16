代发 wailian999

[U87] JS：解构默认值
来源：http://ocz.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://xil.aibaodan.cn

[U88] JS：对象展开合并
来源：http://nft.c1oappe.top

{ ...a, ...b }
来源：http://zuc.wangdashe.top

[U89] JS：数组去重
来源：http://ocv.jlsjyb.cn

[...new Set(arr)]
来源：http://fjf.epnwcf.com

[U90] JS：数字数组排序
来源：http://viv.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://ndj.fzhhl.top

[U91] JS：对象键值遍历
来源：http://agt.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://som.9152youxi.cn

[U92] JS：深拷贝
来源：http://egz.jianghu66.top

structuredClone(obj)
来源：http://rci.tanke756.top

[U93] JS：模板字符串
来源：http://tfy.dianchejie.cn

`共 ${n} 条`
来源：http://hgv.hysaishi.cn

[U94] JS：箭头函数
来源：http://awi.hesvh.cn

const double = x => x * 2;
来源：http://tvj.yj20258888.top

[U95] JS：Promise 包装
来源：http://pau.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://znu.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://ckb.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gki.smart0.xyz

[U97] JS：并发请求
来源：http://jbf.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dob.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://dnm.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://utd.9152youxi.cn

[U99] JS：事件监听
来源：http://ltt.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://eia.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://nwh.yanxiufei.cn

document.querySelector(".item")
来源：http://vgc.kuanghao11.cn

[U101] JS：classList 操作
来源：http://clm.yongpay.top

el.classList.toggle("active")
来源：http://kvy.xuanzx.com

[U102] JS：本地存储
来源：http://tbq.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hqv.hywenlv.cn

[U103] JS：定时器
来源：http://xlt.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uat.aibaodan.cn

[U104] JS：防抖
来源：http://qhb.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wac.kuanghao11.cn

[U105] JS：节流
来源：http://wcd.aizwys.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://otn.sxryk.cn

[U106] JS：日期格式化
来源：http://ysw.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zsh.sjlbkw.cn

[U107] JS：数字千分位
来源：http://qbh.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uuw.xinyue.icu

[U108] JS：随机整数
来源：http://yhp.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hia.chenlongwang.top

[U109] JS：数组分组
来源：http://ddw.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://nak.tarul.cn

[U110] JS：数组分块
来源：http://juw.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hig.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://tnk.bjfxy.top

new Map(Object.entries(obj))
来源：http://yxk.birdmap.top

[U112] JS：字符串补位
来源：http://rnj.chenzaomai.com

"7".padStart(3, "0")
来源：http://wst.iojbl.cn

[U113] JS：正则替换全部
来源：http://uyb.andypj.xyz

s.replaceAll("a", "b")
来源：http://ivl.ivvv.top

[U114] JS：JSON 深比较
来源：http://kbd.xinyue.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://jsv.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://abt.tarul.cn

crypto.randomUUID()
来源：http://uhl.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://xes.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://uum.fzhhl.top

[U117] JS：单元测试
来源：http://bdq.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://wtf.9152youxi.cn

[U118] JS：开发服务器
来源：http://lvv.0kj1m.cn

npm i -D vite;  npx vite
来源：http://vug.xuanzx.com

[U119] JS：生产构建
来源：http://avh.vehdjk.com

npx vite build
来源：http://mls.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://okk.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://cgo.gzhubu.top

================================================================================
来源：http://qly.yanxiufei.cn

统计汇总
来源：http://ksc.redwolf501.top

================================================================================
来源：http://lkv.yvedp.cn

按语言统计（条）：
来源：http://zlm.yonumen.top

Python ......... 252
来源：http://qat.hywenlv.cn

PHP ............ 252
来源：http://kjl.jqgfzy.top

JavaScript ..... 252
来源：http://kha.yueranfly.top

TypeScript ..... 212
来源：http://kwm.jqgfzy.top

Java ........... 212
来源：http://ovg.shuidangran.top

Go ............. 212
来源：http://cqn.zdbjq.cn

Ruby ........... 212
来源：http://nnr.ppjwa.cn

C# ............. 212
来源：http://eqe.wangshuangyany.cn

C .............. 30
来源：http://cuo.andypj.xyz

C++ ............ 30
来源：http://qep.uphjek.com

SQL ............ 90
来源：http://vle.haohaochexian.top

Bash ........... 80
来源：http://ydo.zhijiandao.cn

Kotlin ......... 15
来源：http://nfe.316326.xyz

Swift .......... 15
来源：http://ksh.xingfuxueyuan.xyz

Lua ............ 10
来源：http://tgd.hesvh.cn

Perl ........... 10
来源：http://jxr.xingfuxueyuan.xyz

Scala .......... 10
来源：http://jgj.hesvh.cn

------------------------------------
来源：http://wgs.yvedp.cn

合计 ........... 2106 条
来源：http://qam.jqgufenzy.top

按章节统计：
来源：http://sif.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zsh.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://abf.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ldw.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gop.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://evl.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uxa.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://biw.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qdw.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kgp.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sfb.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lyx.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fnn.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ngb.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mkk.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jws.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iqh.hnxiangtu.top

Q SQL 专题                              90
来源：http://dxq.yj20258.top

R Bash 专题                             80
来源：http://few.chenzaomai.com

S C / C++ 专题                          60
来源：http://mvn.sysykeji.top

T 其他语言补充                          60
来源：http://lbj.andypj.xyz

U 高频实用片段                         120
来源：http://mca.dianchejie.cn

------------------------------------
来源：http://buz.fehbvm.com

合计                                  2106 条
来源：http://uzz.yongpay.top

--------------------------------------------------------------------------------
来源：http://zyi.xuetiantiany.cn

使用提醒
来源：http://ndw.hnqzz.top

--------------------------------------------------------------------------------
来源：http://rey.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sxg.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lkg.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tlg.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gwx.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iew.zhixingplan.top

—— 文件结束 ——
来源：http://aax.andypj.xyz

================================================================================
来源：http://yyo.c1oappe.top

程序语言常见例子速查手册（2024 版）
来源：http://wxp.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://mbl.hcnkem.com

================================================================================
来源：http://mvf.jianghu66.top

【收录内容】
来源：http://ahy.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uts.yueranfly.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pym.pycfn.com

SQL · Bash · C · C++
来源：http://zyy.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rma.zhijiandao.cn

【使用说明】
来源：http://ztt.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qxg.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dom.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dwx.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fuu.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://wue.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xll.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fpo.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sam.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://crx.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://swy.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bnj.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://urm.hfpthk.cn

【文件统计】
来源：http://xiy.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zzq.andypj.xyz

--------------------------------------------------------------------------------
来源：http://tmf.guannengcc.top

目  录
来源：http://ckg.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://quc.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dar.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pbi.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pbn.jqgufenzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ktj.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ckk.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://owr.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mki.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://feh.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fjj.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jhv.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ens.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wgl.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cnm.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mml.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://avl.fanxiaobao.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rgv.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fci.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bpt.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eyj.yanxiufei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ohu.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ktv.ywan-chungtsiang.top

================================================================================
来源：http://air.dashuyun.cn

A. 基础语法与类型
来源：http://csr.ivvv.top

================================================================================
来源：http://zue.shzxlz.cn

[A01] Hello World
来源：http://pvw.jyoumei.cn

Py:   print("Hello, World!")
来源：http://ynw.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://swn.wangshuangyany.cn

JS:   console.log("Hello, World!");
来源：http://okw.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vtj.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://yjk.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://rca.zycfv.cn

Ruby: puts "Hello, World!"
来源：http://vxw.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yly.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://rbh.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://znc.fehbvm.com

PHP:  $name = "Alex"; $age = 20;
来源：http://iqb.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hlw.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://img.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://fyo.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://xdi.shanyushiyangtech.top

Ruby: name = "Alex"; age = 20
来源：http://pov.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vqp.uphjek.com

[A03] 常量定义
来源：http://yin.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xwx.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://bcz.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://whf.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://tep.tarul.cn

Java: static final double PI = 3.14159;
来源：http://mod.jinqigufen.top

Go:   const PI = 3.14159
来源：http://cwn.hesvh.cn

Ruby: PI = 3.14159
来源：http://yfx.jianghu66.top

C#:   const double PI = 3.14159;
来源：http://zro.yonumen.top

[A04] 判断变量类型
来源：http://xzo.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://gmu.52xcode.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xvs.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jej.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://viz.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yyw.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mwx.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://hpn.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://mpn.jinqigfzy.top

[A05] 整数除法与取模
来源：http://pxf.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://arv.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hyq.chenlongwang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://afg.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hsn.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://nht.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://gll.jinqigufen.top

Ruby: 7 / 2; 7 % 2
来源：http://iol.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://llp.hnqzz.top

[A06] 字符串转数字
来源：http://lyq.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://tgr.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fyj.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lgt.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://glb.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fcn.hcnkem.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ouk.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hbt.sweek.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xws.jiagoushi.top

[A07] 数字转字符串
来源：http://xrg.shanyushiyangkeji.top

Py:   str(42)
来源：http://mbr.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://qes.jianghu66.top

JS:   String(42); (42).toString()
来源：http://ofp.fanxiaobao.xyz

TS:   String(42)
来源：http://yve.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jts.cqqwz.cn

Go:   strconv.Itoa(42)
来源：http://ioo.fehbvm.com

Ruby: 42.to_s
来源：http://wca.hcnkem.com

C#:   42.ToString()
来源：http://vlp.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://qel.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wth.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://stc.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fcs.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tkl.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fxb.gogol.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://crk.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pip.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jpt.haohaochexian.top

[A09] 绝对值与最大最小值
来源：http://adb.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ywo.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sgg.cucudq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://skl.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sbv.jiagoushi.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sjg.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blr.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yvt.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oad.vehdjk.com

[A10] 生成随机数
来源：http://gsx.smart0.xyz

Py:   import random; random.randint(1, 100)
来源：http://tuq.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://lwf.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gsa.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zaz.xuetiantiany.cn

Java: new Random().nextInt(100) + 1
来源：http://jhn.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vyq.ctjpmb.com

Ruby: rand(1..100)
来源：http://wvh.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://sga.daxiang520.top

[A11] 条件表达式（三元）
来源：http://ubq.snrcjt.cn

Py:   "yes" if x > 0 else "no"
来源：http://tad.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://slk.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://saw.gaohongyu789.top

TS:   x > 0 ? "yes" : "no"
来源：http://uyh.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://yxa.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qfw.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zmf.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eog.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://gxd.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jkc.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pmw.ivvv.top

JS:   `Hello, ${name}!`
来源：http://uht.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://hkp.c1oappe.top

Java: "Hello, %s!".formatted(name)
来源：http://gtx.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vfr.yuanzhike.top

Ruby: "Hello, #{name}!"
来源：http://dia.tanke756.top

C#:   $"Hello, {name}!"
来源：http://mgy.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fbx.birdmap.top

Py:   "第一行\n第二行"
来源：http://lku.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://khq.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://epe.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://jtd.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://njw.gzhubu.top

Go:   "第一行\n第二行"
来源：http://gmu.hywenlv.cn

Ruby: "第一行\n第二行"
来源：http://srt.gzhubu.top

C#:   "第一行\n第二行"
来源：http://pfy.bjfxy.top

[A14] 注释写法
来源：http://shf.kuanghao11.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gdw.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://xdh.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://vwz.feifeiyinyue.top

TS:   // 单行；/* 多行 */
来源：http://bkn.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nrc.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://fpp.mhx1999.top

Ruby: # 单行；=begin 多行 =end
来源：http://dlm.zdqjudy.top


<!-- 参考信息 -->