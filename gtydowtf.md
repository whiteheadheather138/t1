代发 wailian999

[U95] JS：Promise 包装
来源：http://ahv.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://cuw.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://oar.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://otb.dianchejie.cn

[U97] JS：并发请求
来源：http://qmr.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://kxn.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://bhm.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qre.gogol.net.cn

[U99] JS：事件监听
来源：http://xko.fzhhl.top

el.addEventListener("click", e => {})
来源：http://nbq.gogol.net.cn

[U100] JS：DOM 查询
来源：http://sbs.hnqzz.top

document.querySelector(".item")
来源：http://itn.guowangkeji.top

[U101] JS：classList 操作
来源：http://iwf.yj20258.top

el.classList.toggle("active")
来源：http://ykc.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://hsm.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://arb.chenlongwang.top

[U103] JS：定时器
来源：http://cuf.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fsm.316326.xyz

[U104] JS：防抖
来源：http://jzq.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcq.aibaodan.cn

[U105] JS：节流
来源：http://swu.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ufe.snrcjt.cn

[U106] JS：日期格式化
来源：http://erm.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://twk.jinqigfzy.top

[U107] JS：数字千分位
来源：http://lfj.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tpy.316326.xyz

[U108] JS：随机整数
来源：http://wpl.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vnx.yj20258.top

[U109] JS：数组分组
来源：http://doi.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://wbo.chenlongwang.top

[U110] JS：数组分块
来源：http://bbp.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jof.zdbjq.cn

[U111] JS：对象转 Map
来源：http://wgz.zhengqikj.top

new Map(Object.entries(obj))
来源：http://kot.daria6918.cn

[U112] JS：字符串补位
来源：http://hvj.hammf.cn

"7".padStart(3, "0")
来源：http://yqq.hysaishi.cn

[U113] JS：正则替换全部
来源：http://dus.sysykeji.top

s.replaceAll("a", "b")
来源：http://hcv.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://bfc.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://phm.jqgfzy.top

[U115] JS：生成 UUID
来源：http://tmo.chenzaomai.com

crypto.randomUUID()
来源：http://tfu.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://vsb.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://hig.tianlin.xyz

[U117] JS：单元测试
来源：http://tku.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://ttr.fengsongda.top

[U118] JS：开发服务器
来源：http://afh.cheryme.top

npm i -D vite;  npx vite
来源：http://yxa.yonumen.top

[U119] JS：生产构建
来源：http://avl.yj20258.top

npx vite build
来源：http://koi.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://vqc.pycfn.com

import.meta.env.VITE_API_URL
来源：http://xmy.hammf.cn

================================================================================
来源：http://dlb.hcnkem.com

统计汇总
来源：http://ddp.svipenyu.cn

================================================================================
来源：http://kqe.hnqzz.top

按语言统计（条）：
来源：http://hah.gotoacloud.top

Python ......... 252
来源：http://fnh.ivvv.top

PHP ............ 252
来源：http://tnk.guannengcc.top

JavaScript ..... 252
来源：http://oms.0kj1m.cn

TypeScript ..... 212
来源：http://hwx.shangyingyoupin.top

Java ........... 212
来源：http://pxx.zhongyouzk.top

Go ............. 212
来源：http://jfl.bbcook.cn

Ruby ........... 212
来源：http://bvk.birdmap.top

C# ............. 212
来源：http://qyh.zhiwuduotai.top

C .............. 30
来源：http://qqo.yj20258888.top

C++ ............ 30
来源：http://kkj.shanyushiyangtech.top

SQL ............ 90
来源：http://uye.hongshengwenyu.top

Bash ........... 80
来源：http://xdp.fanxiaobao.xyz

Kotlin ......... 15
来源：http://aqc.cdnleiting.top

Swift .......... 15
来源：http://yxu.jqgufenzy.top

Lua ............ 10
来源：http://lfo.fengsongda.top

Perl ........... 10
来源：http://xbh.ctjpmb.com

Scala .......... 10
来源：http://fnf.ehwqpu.com

------------------------------------
来源：http://uxd.hfpthk.cn

合计 ........... 2106 条
来源：http://ocf.yongpay.top

按章节统计：
来源：http://ikj.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uwk.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tms.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wfr.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://abc.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aef.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gpb.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://siu.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ovj.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uds.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://afh.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wag.shangyingyoupin.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vtt.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nyg.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tap.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://piw.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vfl.yueranfly.top

Q SQL 专题                              90
来源：http://vbq.shzxlz.cn

R Bash 专题                             80
来源：http://bhf.cqqwz.cn

S C / C++ 专题                          60
来源：http://epf.jinqigfzy.top

T 其他语言补充                          60
来源：http://dlb.hongshengwenyu.top

U 高频实用片段                         120
来源：http://rnq.cdnleiting.top

------------------------------------
来源：http://qhx.chenjidiqi.icu

合计                                  2106 条
来源：http://exq.ivvv.top

--------------------------------------------------------------------------------
来源：http://ntv.ppjwa.cn

使用提醒
来源：http://xam.guannengcc.top

--------------------------------------------------------------------------------
来源：http://zik.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ihg.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://adq.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hqg.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bax.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hzd.fengsongda.top

—— 文件结束 ——
来源：http://kve.xuetiantiany.cn

================================================================================
来源：http://bwo.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://eti.jianghu66.top

Common Programming Examples Cheat Book
来源：http://ozm.jinghuilouyu.cn

================================================================================
来源：http://byl.daxiang520.top

【收录内容】
来源：http://wfg.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ttw.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uxl.jqgfzy.top

SQL · Bash · C · C++
来源：http://tmy.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kvg.xinyue.icu

【使用说明】
来源：http://ozx.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fgz.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jwe.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lbm.jlsjyb.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ltq.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://meo.kuanghao11.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://thh.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pna.daxiang520.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cyq.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cnu.hongshengwenyu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qcx.gaohongyu789.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ahn.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ahx.guannengcc.top

【文件统计】
来源：http://yhu.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tsu.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://tuk.sweek.top

目  录
来源：http://uzc.xuanzx.com

--------------------------------------------------------------------------------
来源：http://ojr.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zvb.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://efz.hnxiangtu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rug.xinyue.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bqo.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nrg.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nto.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uxf.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sfa.cheryme.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ufy.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://guy.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qhp.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wrb.daria6918.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kxr.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tzk.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://buh.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yrd.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://plk.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://dbu.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bdm.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ivj.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vry.ydjk.org.cn

================================================================================
来源：http://sih.dianchejie.cn

A. 基础语法与类型
来源：http://ccw.fzhhl.top

================================================================================
来源：http://cue.chenjidiqi.icu

[A01] Hello World
来源：http://srf.chenlongwang.top

Py:   print("Hello, World!")
来源：http://czd.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://sce.meibo888.top

JS:   console.log("Hello, World!");
来源：http://sju.xziqi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://htg.hongshengwenyu.top

Java: System.out.println("Hello, World!");
来源：http://eob.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://dqr.hongshengwenyu.top

Ruby: puts "Hello, World!"
来源：http://blg.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dvi.gzhubu.top

[A02] 变量声明与赋值
来源：http://cnb.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ugi.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mat.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yhb.meibo888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qwz.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://syz.haohaochexian.top

Go:   name := "Alex"; age := 20
来源：http://jmp.uphjek.com

Ruby: name = "Alex"; age = 20
来源：http://rmx.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://bbx.cashguo.top

[A03] 常量定义
来源：http://ont.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ilc.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://jsa.gzhubu.top

JS:   const PI = 3.14159;
来源：http://inh.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://rrn.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://fwj.fehbvm.com

Go:   const PI = 3.14159
来源：http://fwf.hesvh.cn

Ruby: PI = 3.14159
来源：http://xek.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://ako.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://awo.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ttf.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://owb.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://erk.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://pmt.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://glx.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://rli.jyoumei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://all.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://nru.daxiang520.top

[A05] 整数除法与取模
来源：http://maf.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jvk.tianlin.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://nld.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://exv.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eak.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://amu.jqgufenzy.top

Go:   7 / 2; 7 % 2
来源：http://ouh.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://wpe.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://wuy.shzxlz.cn

[A06] 字符串转数字
来源：http://fly.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://hmc.pengpengdd.cyou

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nke.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yek.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://vsp.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://plp.fzhhl.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ska.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jqh.cdnleiting.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uyf.jinqigufen.top

[A07] 数字转字符串
来源：http://ynj.vqdsnc.cn

Py:   str(42)
来源：http://okg.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://ypv.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://nyf.vehdjk.com

TS:   String(42)
来源：http://gcc.yj20258888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nkn.yonumen.top

Go:   strconv.Itoa(42)
来源：http://jdg.0kj1m.cn

Ruby: 42.to_s
来源：http://tzl.zhixingplan.top

C#:   42.ToString()
来源：http://zyl.xinyue.icu

[A08] 取整与四舍五入
来源：http://lug.mhx1999.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lmz.yongpay.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hfj.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ngk.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lzz.yuanzhike.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qmo.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ero.cdnleiting.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hdm.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://krf.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://sef.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zkp.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yii.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://buc.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hso.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://guw.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vfz.ywan-chungtsiang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dnk.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hkh.cucudq.cn

[A10] 生成随机数
来源：http://ocz.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://qwh.epnwcf.com

PHP:  random_int(1, 100);
来源：http://tgj.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rdb.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qvz.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://xdu.fehbvm.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qpb.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://ynp.nwbrower.top

C#:   new Random().Next(1, 101)
来源：http://fjd.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://dmf.shzxlz.cn

Py:   "yes" if x > 0 else "no"
来源：http://tao.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://rjm.iojbl.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hgb.bjfxy.top

TS:   x > 0 ? "yes" : "no"
来源：http://zhq.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://vyv.aizwys.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xhz.tanke756.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hoe.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://oru.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://lmz.jqgufenzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xbx.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uay.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://uqd.cheryme.top

TS:   `Hello, ${name}!`
来源：http://zew.jianghu66.top

Java: "Hello, %s!".formatted(name)
来源：http://uqq.zhoulong.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zqe.yj20258888.top

Ruby: "Hello, #{name}!"
来源：http://pit.yj20258888.top

C#:   $"Hello, {name}!"
来源：http://kiw.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wks.yj20258888.top

Py:   "第一行\n第二行"
来源：http://jgv.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://bdb.hfpthk.cn

JS:   "第一行\n第二行"
来源：http://nix.redwolf501.top

TS:   "第一行\n第二行"
来源：http://xqc.zdbjq.cn

Java: "第一行\n第二行"
来源：http://ubt.yonumen.top

Go:   "第一行\n第二行"
来源：http://gwi.nwbrower.top

Ruby: "第一行\n第二行"
来源：http://mux.ivvv.top

C#:   "第一行\n第二行"
来源：http://vbr.jinqigfzy.top

[A14] 注释写法
来源：http://qby.yuxming.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ujk.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://jmr.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://gai.tanke756.top

TS:   // 单行；/* 多行 */
来源：http://kwi.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://heh.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://iqd.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://hyy.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://muo.zhixingplan.top

[A15] 空值判断与默认值
来源：http://zki.hammf.cn

Py:   value = data or "默认值"
来源：http://igz.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://yqm.havefunace.top

JS:   const value = data ?? "默认值";
来源：http://zvq.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://fdv.hnxiangtu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://thq.jqgfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://oij.sweek.top

Ruby: value = data || "默认值"
来源：http://ovk.cdnleiting.top

C#:   var value = data ?? "默认值";
来源：http://yyz.wangdashe.top

[A16] 真假值判断规则
来源：http://dzl.nanxinkj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pdi.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ivn.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hlz.316326.xyz

TS:   if (!x) {}
来源：http://vmi.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lsd.dianchejie.cn


<!-- 参考信息 -->