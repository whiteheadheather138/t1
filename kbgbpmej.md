代发 wailian999

[U95] JS：Promise 包装
来源：http://ego.havefunace.top

new Promise((resolve, reject) => {})
来源：http://ifg.wangdashe.top

[U96] JS：async/await 与异常
来源：http://zai.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xiw.zhongyouzk.top

[U97] JS：并发请求
来源：http://tib.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kbw.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://gln.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mcy.tarul.cn

[U99] JS：事件监听
来源：http://fev.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://mjz.dashuyun.cn

[U100] JS：DOM 查询
来源：http://eqx.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://mbx.zhixingplan.top

[U101] JS：classList 操作
来源：http://iqd.guowangkeji.top

el.classList.toggle("active")
来源：http://vqj.vehdjk.com

[U102] JS：本地存储
来源：http://ssy.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bwy.wangdashe.top

[U103] JS：定时器
来源：http://oye.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qyv.chenzaomai.com

[U104] JS：防抖
来源：http://qkt.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yrm.feifeiyinyue.top

[U105] JS：节流
来源：http://wfh.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lxy.nanxinkj.top

[U106] JS：日期格式化
来源：http://azv.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rbq.cucudq.cn

[U107] JS：数字千分位
来源：http://isz.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://deo.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://lqm.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hey.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://tae.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://akz.hcnkem.com

[U110] JS：数组分块
来源：http://yvp.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lqp.fzhhl.top

[U111] JS：对象转 Map
来源：http://erc.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://ngt.yj20258.top

[U112] JS：字符串补位
来源：http://zyr.hammf.cn

"7".padStart(3, "0")
来源：http://kva.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://xse.hysaishi.cn

s.replaceAll("a", "b")
来源：http://vds.sxryk.cn

[U114] JS：JSON 深比较
来源：http://qde.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nlu.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://hmm.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://czh.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://edk.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://ned.fzhhl.top

[U117] JS：单元测试
来源：http://llw.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://ocw.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://vyb.ybcxt.top

npm i -D vite;  npx vite
来源：http://lfo.shangyingyoupin.top

[U119] JS：生产构建
来源：http://vmt.sufxvd.cn

npx vite build
来源：http://ryu.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://esw.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://vgq.daxiang520.top

================================================================================
来源：http://bhq.gotoacloud.top

统计汇总
来源：http://ahv.yueranfly.top

================================================================================
来源：http://rjg.redwolf501.top

按语言统计（条）：
来源：http://wei.dashuyun.cn

Python ......... 252
来源：http://num.yj20258888.top

PHP ............ 252
来源：http://bat.jlsjyb.cn

JavaScript ..... 252
来源：http://kpw.fengsongda.top

TypeScript ..... 212
来源：http://ydb.tanke756.top

Java ........... 212
来源：http://uqz.sysykeji.top

Go ............. 212
来源：http://lgt.daxiang520.top

Ruby ........... 212
来源：http://jgv.hnqzz.top

C# ............. 212
来源：http://odb.dianchejie.cn

C .............. 30
来源：http://xlr.wangshuangyany.cn

C++ ............ 30
来源：http://mez.mhx1999.top

SQL ............ 90
来源：http://xgf.fktsv.cn

Bash ........... 80
来源：http://rxh.uphjek.com

Kotlin ......... 15
来源：http://ulf.fehbvm.com

Swift .......... 15
来源：http://jur.ctjpmb.com

Lua ............ 10
来源：http://pra.cheryme.top

Perl ........... 10
来源：http://wfv.cdnleiting.top

Scala .......... 10
来源：http://epe.9152youxi.cn

------------------------------------
来源：http://hpl.jiagoushi.top

合计 ........... 2106 条
来源：http://tgf.zhaomingkeji.xyz

按章节统计：
来源：http://rcr.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qor.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zvz.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vlr.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bhh.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hck.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bgo.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fkj.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gxt.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fdi.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pbr.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ptp.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wip.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://crg.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xli.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rdc.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spk.meibo888.top

Q SQL 专题                              90
来源：http://qhb.hesvh.cn

R Bash 专题                             80
来源：http://yjt.zhengqikj.top

S C / C++ 专题                          60
来源：http://ast.shzxlz.cn

T 其他语言补充                          60
来源：http://eqy.nwbrower.top

U 高频实用片段                         120
来源：http://svl.andypj.xyz

------------------------------------
来源：http://jcf.9152youxi.cn

合计                                  2106 条
来源：http://xcr.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://nqx.jlsjyb.cn

使用提醒
来源：http://meh.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://keq.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dox.uphjek.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gdg.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://for.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://emd.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eai.meibo888.top

—— 文件结束 ——
来源：http://jhg.hnxiangtu.top

================================================================================
来源：http://mjb.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://whj.pycfn.com

Common Programming Examples Cheat Book
来源：http://wfj.chenjidiqi.icu

================================================================================
来源：http://kft.xylfe.cn

【收录内容】
来源：http://yaz.tian-w.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gvu.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rgg.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://vkz.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rkz.chenzaomai.com

【使用说明】
来源：http://sud.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://shl.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://apa.yvedp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wby.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fwe.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://fai.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kiu.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kpl.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hfo.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ize.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ajb.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mid.xuetiantiany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dlm.wangshuangyany.cn

【文件统计】
来源：http://sbk.shuidangran.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bbb.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://mdh.gzhubu.top

目  录
来源：http://qlh.daria6918.cn

--------------------------------------------------------------------------------
来源：http://yzx.hnqzz.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xrp.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wff.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rma.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zet.nwbrower.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nxr.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ucf.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ebn.gogol.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ykp.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fcj.zhixingplan.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://efl.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uow.nanxinkj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pft.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rim.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aiv.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://feo.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ams.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dkw.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kgc.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ryu.pengpengdd.cyou

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://amk.uphjek.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ewt.pycfn.com

================================================================================
来源：http://zdx.zycfv.cn

A. 基础语法与类型
来源：http://heo.316326.xyz

================================================================================
来源：http://noh.chenlongwang.top

[A01] Hello World
来源：http://opt.yangfankeji.com

Py:   print("Hello, World!")
来源：http://ckz.tarul.cn

PHP:  echo "Hello, World!";
来源：http://cvr.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://hmv.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iwf.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://cey.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://pds.tianlin.xyz

Ruby: puts "Hello, World!"
来源：http://ixc.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wgc.0kj1m.cn

[A02] 变量声明与赋值
来源：http://fqp.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vkn.ydjk.org.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dpp.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sbg.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xbg.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://hdm.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://aul.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://eki.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://rvm.jianghu66.top

[A03] 常量定义
来源：http://bsx.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://npm.uphjek.com

PHP:  const PI = 3.14159;
来源：http://apa.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://aog.xinyue.icu

TS:   const PI: number = 3.14159;
来源：http://tcx.meibo888.top

Java: static final double PI = 3.14159;
来源：http://mmh.hcnkem.com

Go:   const PI = 3.14159
来源：http://xjv.jyoumei.cn

Ruby: PI = 3.14159
来源：http://nxz.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://jld.gotoacloud.top

[A04] 判断变量类型
来源：http://luw.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dob.havefunace.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mza.xuanzx.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qyj.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://jdh.cdnleiting.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mhx.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xid.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rdc.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://kuf.sysykeji.top

[A05] 整数除法与取模
来源：http://iai.fktsv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nkq.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dor.pengpengdd.cyou

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://myx.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cza.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://lsg.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://ega.xinyue.icu

Ruby: 7 / 2; 7 % 2
来源：http://eec.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://keh.sxryk.cn

[A06] 字符串转数字
来源：http://mpa.yvedp.cn

Py:   int("42"); float("3.14")
来源：http://itb.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xha.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uuo.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://nac.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iak.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fzm.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pau.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nno.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://ldx.jinyuanbaomall.cn

Py:   str(42)
来源：http://egr.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://wna.guannengcc.top

JS:   String(42); (42).toString()
来源：http://fhh.c1oappe.top

TS:   String(42)
来源：http://goc.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://pqx.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://zcz.wangdashe.top

Ruby: 42.to_s
来源：http://xit.nwbrower.top

C#:   42.ToString()
来源：http://abz.yuxming.cn

[A08] 取整与四舍五入
来源：http://ack.jyoumei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fkq.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rxz.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vvt.smart0.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ziq.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://buj.gzhubu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rth.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mpp.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://onc.fanxiaobao.xyz

[A09] 绝对值与最大最小值
来源：http://cii.ehwqpu.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kqn.zdbjq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jab.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lic.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://osz.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yhm.shangyingyoupin.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://htw.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bau.gaohongyu789.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wye.dianchejie.cn

[A10] 生成随机数
来源：http://mzy.yongpay.top

Py:   import random; random.randint(1, 100)
来源：http://umr.yueranfly.top

PHP:  random_int(1, 100);
来源：http://jgk.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pnk.hywenlv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://onv.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://djc.zhiwuduotai.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qtp.fktsv.cn

Ruby: rand(1..100)
来源：http://mec.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://vlg.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://jrw.zhoulong.xyz

Py:   "yes" if x > 0 else "no"
来源：http://bhb.nanxinkj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://epk.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://jkh.c1oappe.top

TS:   x > 0 ? "yes" : "no"
来源：http://qbv.zdbjq.cn

Java: x > 0 ? "yes" : "no"
来源：http://vgw.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://psv.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://oqg.hfpthk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ykx.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://xfq.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pet.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gad.yj202588.top

JS:   `Hello, ${name}!`
来源：http://hzp.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://ppf.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://oiz.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ybp.tian-w.cn

Ruby: "Hello, #{name}!"
来源：http://zun.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://yxd.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vzb.jlsjyb.cn

Py:   "第一行\n第二行"
来源：http://qgt.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://eer.hcnkem.com

JS:   "第一行\n第二行"
来源：http://vcg.c1oappe.top

TS:   "第一行\n第二行"
来源：http://rds.redwolf501.top

Java: "第一行\n第二行"
来源：http://pry.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://gjx.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://xge.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://qlx.chenjidiqi.icu

[A14] 注释写法
来源：http://ayx.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nxf.ctjpmb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://xsf.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://jva.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://ptp.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qdu.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://obw.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zcq.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://bcu.nwbrower.top

[A15] 空值判断与默认值
来源：http://lli.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://upo.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://lzd.xylfe.cn

JS:   const value = data ?? "默认值";
来源：http://czf.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://tiu.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hot.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://yny.jyoumei.cn

Ruby: value = data || "默认值"
来源：http://fno.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://qfa.uphjek.com

[A16] 真假值判断规则
来源：http://daf.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://clq.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lbh.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kdi.mhx1999.top

TS:   if (!x) {}
来源：http://jtq.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sfu.zhengqikj.top


<!-- 参考信息 -->