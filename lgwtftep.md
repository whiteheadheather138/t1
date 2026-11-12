代发 wailian999

[U87] JS：解构默认值
来源：http://ejh.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://cja.fehbvm.com

[U88] JS：对象展开合并
来源：http://ozq.daxiang520.top

{ ...a, ...b }
来源：http://yvh.quarkkingdee.top

[U89] JS：数组去重
来源：http://nbu.cqqwz.cn

[...new Set(arr)]
来源：http://euu.cheryme.top

[U90] JS：数字数组排序
来源：http://iwn.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://kss.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://nej.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nej.ehwqpu.com

[U92] JS：深拷贝
来源：http://vtv.yfazqb.com

structuredClone(obj)
来源：http://zoj.daxiang520.top

[U93] JS：模板字符串
来源：http://edc.shangyingyoupin.top

`共 ${n} 条`
来源：http://gsd.jlsjyb.cn

[U94] JS：箭头函数
来源：http://ttb.316326.xyz

const double = x => x * 2;
来源：http://smm.hcnkem.com

[U95] JS：Promise 包装
来源：http://xvo.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://fwn.nwbrower.top

[U96] JS：async/await 与异常
来源：http://xzz.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pcj.vehdjk.com

[U97] JS：并发请求
来源：http://hpy.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tuv.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://ynv.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vex.pengpengdd.cyou

[U99] JS：事件监听
来源：http://pqv.hnqzz.top

el.addEventListener("click", e => {})
来源：http://stk.tanke756.top

[U100] JS：DOM 查询
来源：http://jsz.iojbl.cn

document.querySelector(".item")
来源：http://kah.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://mkp.vqdsnc.cn

el.classList.toggle("active")
来源：http://lfq.epnwcf.com

[U102] JS：本地存储
来源：http://otk.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lid.jinqigufen.top

[U103] JS：定时器
来源：http://fvv.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hbm.zhongyouzk.top

[U104] JS：防抖
来源：http://zhu.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zba.daria6918.cn

[U105] JS：节流
来源：http://rok.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kyx.zhijiandao.cn

[U106] JS：日期格式化
来源：http://itb.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rid.yongpay.top

[U107] JS：数字千分位
来源：http://hhh.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dsa.kuanghao11.cn

[U108] JS：随机整数
来源：http://ctm.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://owj.chenlongwang.top

[U109] JS：数组分组
来源：http://isv.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://kmf.xylfe.cn

[U110] JS：数组分块
来源：http://wyd.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vjb.snrcjt.cn

[U111] JS：对象转 Map
来源：http://gcs.0kj1m.cn

new Map(Object.entries(obj))
来源：http://spg.gzhubu.top

[U112] JS：字符串补位
来源：http://tiy.sweek.top

"7".padStart(3, "0")
来源：http://vve.guannengcc.top

[U113] JS：正则替换全部
来源：http://htw.yvedp.cn

s.replaceAll("a", "b")
来源：http://kwv.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://ots.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vbu.yj20258.top

[U115] JS：生成 UUID
来源：http://isd.tianlin.xyz

crypto.randomUUID()
来源：http://oqi.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://dqb.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://owj.zhengqikj.top

[U117] JS：单元测试
来源：http://ltr.jqgufenzy.top

npm i -D vitest;  npx vitest
来源：http://eak.tianlin.xyz

[U118] JS：开发服务器
来源：http://vyj.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://wor.sweek.top

[U119] JS：生产构建
来源：http://phb.vqdsnc.cn

npx vite build
来源：http://uyp.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vhr.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://ukh.meibo888.top

================================================================================
来源：http://knh.nwbrower.top

统计汇总
来源：http://quw.iojbl.cn

================================================================================
来源：http://kph.fehbvm.com

按语言统计（条）：
来源：http://zuq.uphjek.com

Python ......... 252
来源：http://jvv.fanxiaobao.xyz

PHP ............ 252
来源：http://oyz.tian-w.cn

JavaScript ..... 252
来源：http://lno.cdnleiting.top

TypeScript ..... 212
来源：http://jda.meibo888.top

Java ........... 212
来源：http://jkd.cheryme.top

Go ............. 212
来源：http://mml.quarkkingdee.top

Ruby ........... 212
来源：http://gog.smart0.xyz

C# ............. 212
来源：http://bmm.ppjwa.cn

C .............. 30
来源：http://lkc.chenlongwang.top

C++ ............ 30
来源：http://yus.hammf.cn

SQL ............ 90
来源：http://wve.xuanzx.com

Bash ........... 80
来源：http://dji.meibo888.top

Kotlin ......... 15
来源：http://wot.shanyushiyangtech.top

Swift .......... 15
来源：http://npw.sxryk.cn

Lua ............ 10
来源：http://jqu.chenlongwang.top

Perl ........... 10
来源：http://zpi.yfazqb.com

Scala .......... 10
来源：http://lwn.shanyushiyangkeji.top

------------------------------------
来源：http://ycf.nanxuanxn.top

合计 ........... 2106 条
来源：http://cos.chenlongwang.top

按章节统计：
来源：http://xhc.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dek.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uvl.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://edc.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lno.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ecn.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ula.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kqn.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xxi.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lnl.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bnl.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ebi.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dkp.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ucr.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tzq.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ygr.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ooz.cucudq.cn

Q SQL 专题                              90
来源：http://lxu.aizwys.cn

R Bash 专题                             80
来源：http://ahu.dianchejie.cn

S C / C++ 专题                          60
来源：http://rck.ehwqpu.com

T 其他语言补充                          60
来源：http://cad.zhoulong.xyz

U 高频实用片段                         120
来源：http://hty.hnqzz.top

------------------------------------
来源：http://orx.sysykeji.top

合计                                  2106 条
来源：http://jjo.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://lpj.mhx1999.top

使用提醒
来源：http://hlu.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://cio.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uhv.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vhg.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sny.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://jdr.xuanzx.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mxs.shzxlz.cn

—— 文件结束 ——
来源：http://ipz.zhiwuduotai.top

================================================================================
来源：http://ppx.yanxiufei.cn

程序语言常见例子速查手册（2024 版）
来源：http://qca.aizwys.cn

Common Programming Examples Cheat Book
来源：http://pjz.zhixingplan.top

================================================================================
来源：http://vis.chenjidiqi.icu

【收录内容】
来源：http://bmx.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xlv.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ldl.cdnleiting.top

SQL · Bash · C · C++
来源：http://fwi.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://drj.tarul.cn

【使用说明】
来源：http://aqm.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eiy.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hdm.zhaomingkeji.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jlc.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sgp.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aan.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zmd.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pcd.shangyingyoupin.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rqp.jinghuilouyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jtm.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uxt.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mky.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fss.tianlin.xyz

【文件统计】
来源：http://jwk.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lay.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://nno.c1oappe.top

目  录
来源：http://ruw.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://rcm.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tih.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kki.zhengqikj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zdh.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fel.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gly.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aym.vehdjk.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jhi.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://izp.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jfk.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gmf.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hmj.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ccp.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xzy.zhixingplan.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://stn.hesvh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rlm.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gfa.andypj.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dve.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jya.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://foe.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pqj.sysykeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nuj.yj20258.top

================================================================================
来源：http://hnz.snrcjt.cn

A. 基础语法与类型
来源：http://eqt.pengpengdd.cyou

================================================================================
来源：http://jmu.smart0.xyz

[A01] Hello World
来源：http://oei.sweek.top

Py:   print("Hello, World!")
来源：http://uat.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://dbh.pycfn.com

JS:   console.log("Hello, World!");
来源：http://nvr.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cqm.zhongyouzk.top

Java: System.out.println("Hello, World!");
来源：http://gju.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://gmb.yongpay.top

Ruby: puts "Hello, World!"
来源：http://elm.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kda.zycfv.cn

[A02] 变量声明与赋值
来源：http://yyk.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iba.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iae.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ray.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ylj.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://wav.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://wwn.jinqigfzy.top

Ruby: name = "Alex"; age = 20
来源：http://fbt.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://ovz.gaohongyu789.top

[A03] 常量定义
来源：http://rqo.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qqn.cdnleiting.top

PHP:  const PI = 3.14159;
来源：http://ezo.fzhhl.top

JS:   const PI = 3.14159;
来源：http://vrg.haohaochexian.top

TS:   const PI: number = 3.14159;
来源：http://zor.ppjwa.cn

Java: static final double PI = 3.14159;
来源：http://arq.hnqzz.top

Go:   const PI = 3.14159
来源：http://gzk.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://spd.fehbvm.com

C#:   const double PI = 3.14159;
来源：http://ize.guowangkeji.top

[A04] 判断变量类型
来源：http://voe.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fen.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rbr.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mww.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://puh.tianlin.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ehz.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://azu.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://nts.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://lti.yuxming.cn

[A05] 整数除法与取模
来源：http://wvn.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://krp.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xdw.zdqjudy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://svi.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pwn.chenjidiqi.icu

Java: 7 / 2; 7 % 2
来源：http://xbx.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://zwa.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://nih.zycfv.cn

C#:   7 / 2; 7 % 2
来源：http://xfd.cucudq.cn

[A06] 字符串转数字
来源：http://xpw.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://zwj.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dds.9152youxi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://smj.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://kuj.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dqd.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wlv.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://yfx.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rpe.yuxming.cn

[A07] 数字转字符串
来源：http://lpe.andypj.xyz

Py:   str(42)
来源：http://uig.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://nox.ybcxt.top

JS:   String(42); (42).toString()
来源：http://kib.shanyushiyangkeji.top

TS:   String(42)
来源：http://gfd.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iif.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://shy.cashguo.top

Ruby: 42.to_s
来源：http://tbn.cheryme.top

C#:   42.ToString()
来源：http://chd.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://azb.9152youxi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ily.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vdw.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uhm.daxiang520.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qir.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://toy.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://axs.pycfn.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://oil.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zju.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://uym.jiagoushi.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jhj.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zhk.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yxd.wangdashe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://erw.haohaochexian.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://edj.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://paj.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://acu.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iou.yj20258888.top

[A10] 生成随机数
来源：http://sov.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://qhf.yj20258888.top

PHP:  random_int(1, 100);
来源：http://fzq.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jng.daxiang520.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qpv.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://pmj.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bkd.sufxvd.cn

Ruby: rand(1..100)
来源：http://yrc.yueranfly.top

C#:   new Random().Next(1, 101)
来源：http://sfo.wangdashe.top

[A11] 条件表达式（三元）
来源：http://fzw.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://eza.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mar.ybcxt.top

JS:   x > 0 ? "yes" : "no"
来源：http://tld.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://lqp.cdnleiting.top

Java: x > 0 ? "yes" : "no"
来源：http://zjr.316326.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://hvg.svipenyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lfy.yfazqb.com

C#:   x > 0 ? "yes" : "no"
来源：http://udd.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://gyp.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lxo.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zfy.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://kzt.zdqjudy.top

TS:   `Hello, ${name}!`
来源：http://unm.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://frv.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mex.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://pcm.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://qqp.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://edl.zhixingplan.top

Py:   "第一行\n第二行"
来源：http://fme.zhongyouzk.top

PHP:  "第一行\n第二行"
来源：http://bcm.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://rzn.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://jfv.yongpay.top

Java: "第一行\n第二行"
来源：http://gfc.vehdjk.com

Go:   "第一行\n第二行"
来源：http://jql.ctjpmb.com

Ruby: "第一行\n第二行"
来源：http://hvj.316326.xyz

C#:   "第一行\n第二行"
来源：http://hoa.hongshengwenyu.top

[A14] 注释写法
来源：http://snj.redwolf501.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tun.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rak.yongpay.top

JS:   // 单行；/* 多行 */
来源：http://htq.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://ezl.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gti.redwolf501.top

Go:   // 单行；/* 多行 */
来源：http://fig.gotoacloud.top

Ruby: # 单行；=begin 多行 =end
来源：http://kdo.hfpthk.cn


<!-- 参考信息 -->