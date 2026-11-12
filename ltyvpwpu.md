代发 wailian999

[U89] JS：数组去重
来源：http://fhf.shanyushiyangtech.top

[...new Set(arr)]
来源：http://pad.havefunace.top

[U90] JS：数字数组排序
来源：http://lyc.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://fyt.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://fxj.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blg.hammf.cn

[U92] JS：深拷贝
来源：http://ete.tanke756.top

structuredClone(obj)
来源：http://aed.yangfankeji.com

[U93] JS：模板字符串
来源：http://tew.xylfe.cn

`共 ${n} 条`
来源：http://kcj.gotoacloud.top

[U94] JS：箭头函数
来源：http://bni.chenjidiqi.icu

const double = x => x * 2;
来源：http://tsx.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://jqm.pycfn.com

new Promise((resolve, reject) => {})
来源：http://cgr.smart0.xyz

[U96] JS：async/await 与异常
来源：http://ylf.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jmu.yfazqb.com

[U97] JS：并发请求
来源：http://zhk.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cwn.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://dvq.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bnf.gzhubu.top

[U99] JS：事件监听
来源：http://qdq.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://urb.cashguo.top

[U100] JS：DOM 查询
来源：http://dua.gotoacloud.top

document.querySelector(".item")
来源：http://tfu.jqgfzy.top

[U101] JS：classList 操作
来源：http://rga.fehbvm.com

el.classList.toggle("active")
来源：http://iub.cucudq.cn

[U102] JS：本地存储
来源：http://vkm.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://chf.dianchejie.cn

[U103] JS：定时器
来源：http://jwe.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jrg.tanke756.top

[U104] JS：防抖
来源：http://mte.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bju.daria6918.cn

[U105] JS：节流
来源：http://mlh.aizwys.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jeh.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://sba.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sce.sxryk.cn

[U107] JS：数字千分位
来源：http://zas.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qyz.snrcjt.cn

[U108] JS：随机整数
来源：http://abe.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vyn.smart0.xyz

[U109] JS：数组分组
来源：http://zyq.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://ahj.aibaodan.cn

[U110] JS：数组分块
来源：http://kvr.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xoe.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://jxt.mhx1999.top

new Map(Object.entries(obj))
来源：http://xgr.andypj.xyz

[U112] JS：字符串补位
来源：http://jtq.hnxiangtu.top

"7".padStart(3, "0")
来源：http://ked.guannengcc.top

[U113] JS：正则替换全部
来源：http://pgv.daria6918.cn

s.replaceAll("a", "b")
来源：http://iha.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://alm.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tli.ybcxt.top

[U115] JS：生成 UUID
来源：http://vpu.shzxlz.cn

crypto.randomUUID()
来源：http://ynm.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://joi.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://xqf.nanxuanxn.top

[U117] JS：单元测试
来源：http://gwi.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://kei.yangfankeji.com

[U118] JS：开发服务器
来源：http://ldf.shzxlz.cn

npm i -D vite;  npx vite
来源：http://fsu.zhengqikj.top

[U119] JS：生产构建
来源：http://iko.fktsv.cn

npx vite build
来源：http://hhh.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://itg.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://ucn.sjlbkw.cn

================================================================================
来源：http://jfg.yj20258888.top

统计汇总
来源：http://pew.wangshuangyany.cn

================================================================================
来源：http://fpb.yvedp.cn

按语言统计（条）：
来源：http://meh.ivvv.top

Python ......... 252
来源：http://yxw.yj20258.top

PHP ............ 252
来源：http://njw.snrcjt.cn

JavaScript ..... 252
来源：http://bfq.nwbrower.top

TypeScript ..... 212
来源：http://aou.yongpay.top

Java ........... 212
来源：http://rgk.ivvv.top

Go ............. 212
来源：http://vep.nanxuanxn.top

Ruby ........... 212
来源：http://rfj.fzhhl.top

C# ............. 212
来源：http://nru.ctjpmb.com

C .............. 30
来源：http://odt.yuxming.cn

C++ ............ 30
来源：http://xyf.gogol.net.cn

SQL ............ 90
来源：http://qra.chenlongwang.top

Bash ........... 80
来源：http://kdh.dashuyun.cn

Kotlin ......... 15
来源：http://aco.iojbl.cn

Swift .......... 15
来源：http://mgv.haohaochexian.top

Lua ............ 10
来源：http://lxr.xylfe.cn

Perl ........... 10
来源：http://nol.jqgufenzy.top

Scala .......... 10
来源：http://kmm.ctjpmb.com

------------------------------------
来源：http://lis.fktsv.cn

合计 ........... 2106 条
来源：http://kgw.hesvh.cn

按章节统计：
来源：http://lpn.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://okm.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uan.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rjq.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://new.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xwt.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bst.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ojs.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oon.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dfy.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jco.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kla.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rme.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ifv.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lwu.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yqh.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wac.jyoumei.cn

Q SQL 专题                              90
来源：http://pkb.mhx1999.top

R Bash 专题                             80
来源：http://jrb.zdqjudy.top

S C / C++ 专题                          60
来源：http://wdh.birdmap.top

T 其他语言补充                          60
来源：http://rnu.cashguo.top

U 高频实用片段                         120
来源：http://eil.ivvv.top

------------------------------------
来源：http://sod.shanyushiyangtech.top

合计                                  2106 条
来源：http://tll.tarul.cn

--------------------------------------------------------------------------------
来源：http://jyt.zhengqikj.top

使用提醒
来源：http://dxh.hesvh.cn

--------------------------------------------------------------------------------
来源：http://mag.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cuu.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://byl.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yra.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nip.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://waq.gaohongyu789.top

—— 文件结束 ——
来源：http://orc.ybcxt.top

================================================================================
来源：http://sqk.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://vgp.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://vya.fanxiaobao.xyz

================================================================================
来源：http://eso.kuanghao11.cn

【收录内容】
来源：http://lxv.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kzs.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wyc.gaohongyu789.top

SQL · Bash · C · C++
来源：http://fip.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uvh.0kj1m.cn

【使用说明】
来源：http://vhp.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://npr.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bqh.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cxg.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cqi.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nwp.ehwqpu.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nmp.zhixingplan.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lxg.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ovk.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gyy.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://axw.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jbc.feifeiyinyue.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ujm.snrcjt.cn

【文件统计】
来源：http://lbl.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://htd.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://mvz.snrcjt.cn

目  录
来源：http://zom.fzhhl.top

--------------------------------------------------------------------------------
来源：http://gcv.wangshuangyany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jgx.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fdc.yuanzhike.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mfp.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bsm.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kza.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uwb.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jmg.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yya.zhixingplan.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dzk.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lqj.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vho.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cjj.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://clw.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jtx.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fij.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zmc.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cle.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bjb.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xyi.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xmd.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tgc.gaohongyu789.top

================================================================================
来源：http://ajl.jlsjyb.cn

A. 基础语法与类型
来源：http://dot.9152youxi.cn

================================================================================
来源：http://lkw.shanyushiyangtech.top

[A01] Hello World
来源：http://zer.zhengqikj.top

Py:   print("Hello, World!")
来源：http://nyx.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://dyg.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://mhg.ybcxt.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jvk.jiagoushi.top

Java: System.out.println("Hello, World!");
来源：http://ayr.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://woq.uphjek.com

Ruby: puts "Hello, World!"
来源：http://poo.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vds.gotoacloud.top

[A02] 变量声明与赋值
来源：http://lcs.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pyn.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cvx.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wsk.ywan-chungtsiang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qai.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://xdz.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://pjl.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://eyn.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://utu.zhoulong.xyz

[A03] 常量定义
来源：http://tsu.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rmu.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://ogx.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://rwr.daria6918.cn

TS:   const PI: number = 3.14159;
来源：http://bhm.shzxlz.cn

Java: static final double PI = 3.14159;
来源：http://xqn.gzhubu.top

Go:   const PI = 3.14159
来源：http://vwm.sxryk.cn

Ruby: PI = 3.14159
来源：http://gmi.chenlongwang.top

C#:   const double PI = 3.14159;
来源：http://ogv.jinqigufen.top

[A04] 判断变量类型
来源：http://kxm.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zpb.smart0.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xlh.ydjk.org.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nyg.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://yro.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qdy.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ahm.xuetiantiany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dup.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://thf.ivvv.top

[A05] 整数除法与取模
来源：http://cwf.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ewx.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://imc.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mmm.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://srx.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://wal.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://mks.xingfuxueyuan.xyz

Ruby: 7 / 2; 7 % 2
来源：http://vlk.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://uft.dashuyun.cn

[A06] 字符串转数字
来源：http://kan.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://own.zhiwuduotai.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rop.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kbt.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://gyg.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://twd.hammf.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tra.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://qty.yuanzhike.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rpw.zhixingplan.top

[A07] 数字转字符串
来源：http://ujs.tanke756.top

Py:   str(42)
来源：http://jrb.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://vcd.zhixingplan.top

JS:   String(42); (42).toString()
来源：http://xem.sweek.top

TS:   String(42)
来源：http://pis.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wca.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://qdp.0kj1m.cn

Ruby: 42.to_s
来源：http://xrz.nwbrower.top

C#:   42.ToString()
来源：http://rre.iojbl.cn

[A08] 取整与四舍五入
来源：http://yww.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vau.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ico.dianchejie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qvy.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xlh.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eto.xylfe.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qmk.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ybp.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://knn.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://dsq.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://npg.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ytz.ehwqpu.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xuf.xingfuxueyuan.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://doo.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wrl.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://djq.aizwys.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cjs.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bpp.yonumen.top

[A10] 生成随机数
来源：http://jfd.wangshuangyany.cn

Py:   import random; random.randint(1, 100)
来源：http://mko.bbcook.cn

PHP:  random_int(1, 100);
来源：http://gmz.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nep.iojbl.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vwf.chenzaomai.com

Java: new Random().nextInt(100) + 1
来源：http://zkv.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ddm.dianchejie.cn

Ruby: rand(1..100)
来源：http://trr.316326.xyz

C#:   new Random().Next(1, 101)
来源：http://bgy.yfazqb.com

[A11] 条件表达式（三元）
来源：http://ucv.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://atm.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nwa.zhongyouzk.top

JS:   x > 0 ? "yes" : "no"
来源：http://ipd.xylfe.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ydh.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://usj.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://rxe.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qii.316326.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://rrj.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://uvv.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lnn.jqgfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rff.birdmap.top

JS:   `Hello, ${name}!`
来源：http://rvr.cashguo.top

TS:   `Hello, ${name}!`
来源：http://cmz.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://eqt.jinqigufen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ufn.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://qjb.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://czf.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gns.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://hpl.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://ojn.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://arb.snrcjt.cn

TS:   "第一行\n第二行"
来源：http://jqu.hysaishi.cn

Java: "第一行\n第二行"
来源：http://ahl.52xcode.cn

Go:   "第一行\n第二行"
来源：http://dxy.andypj.xyz

Ruby: "第一行\n第二行"
来源：http://hnh.zycfv.cn

C#:   "第一行\n第二行"
来源：http://oae.daxiang520.top

[A14] 注释写法
来源：http://bsg.cheryme.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sct.shangyingyoupin.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wms.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://lon.shangyingyoupin.top

TS:   // 单行；/* 多行 */
来源：http://xkl.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ila.zhiwuduotai.top

Go:   // 单行；/* 多行 */
来源：http://mpy.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://skm.yuxming.cn

C#:   // 单行；/* 多行 */
来源：http://hag.yj202588.top

[A15] 空值判断与默认值
来源：http://brc.ivvv.top

Py:   value = data or "默认值"
来源：http://vpo.shanyushiyangtech.top

PHP:  $value = $data ?? "默认值";
来源：http://cds.jlsjyb.cn


<!-- 参考信息 -->