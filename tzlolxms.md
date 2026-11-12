代发 wailian999

[U93] JS：模板字符串
来源：http://xhk.gzhubu.top

`共 ${n} 条`
来源：http://luw.meibo888.top

[U94] JS：箭头函数
来源：http://dfc.shangyingyoupin.top

const double = x => x * 2;
来源：http://sty.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://wtr.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://jtg.316326.xyz

[U96] JS：async/await 与异常
来源：http://oth.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ace.haohaochexian.top

[U97] JS：并发请求
来源：http://uov.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kwd.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://opw.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rac.hfpthk.cn

[U99] JS：事件监听
来源：http://con.yfazqb.com

el.addEventListener("click", e => {})
来源：http://hfc.chenzaomai.com

[U100] JS：DOM 查询
来源：http://nzx.cheryme.top

document.querySelector(".item")
来源：http://hhc.0kj1m.cn

[U101] JS：classList 操作
来源：http://grp.daria6918.cn

el.classList.toggle("active")
来源：http://xvi.zhixingplan.top

[U102] JS：本地存储
来源：http://ypj.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uvk.jinqigufen.top

[U103] JS：定时器
来源：http://uit.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nfu.jyoumei.cn

[U104] JS：防抖
来源：http://ays.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbv.zhengqikj.top

[U105] JS：节流
来源：http://gix.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://knv.shuidangran.top

[U106] JS：日期格式化
来源：http://zni.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://alu.pycfn.com

[U107] JS：数字千分位
来源：http://jqm.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ktn.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://qre.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mha.daria6918.cn

[U109] JS：数组分组
来源：http://wqx.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://lme.guowangkeji.top

[U110] JS：数组分块
来源：http://xqh.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lgd.tian-w.cn

[U111] JS：对象转 Map
来源：http://jpp.316326.xyz

new Map(Object.entries(obj))
来源：http://qzn.gaohongyu789.top

[U112] JS：字符串补位
来源：http://wgw.dianchejie.cn

"7".padStart(3, "0")
来源：http://mod.pycfn.com

[U113] JS：正则替换全部
来源：http://uxq.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://ioe.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://lne.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iup.chenlongwang.top

[U115] JS：生成 UUID
来源：http://yyo.yj202588.top

crypto.randomUUID()
来源：http://rhr.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://dak.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://ooc.hysaishi.cn

[U117] JS：单元测试
来源：http://pkw.cheryme.top

npm i -D vitest;  npx vitest
来源：http://dis.tianlin.xyz

[U118] JS：开发服务器
来源：http://kad.andypj.xyz

npm i -D vite;  npx vite
来源：http://spm.hongshengwenyu.top

[U119] JS：生产构建
来源：http://ncw.cdnleiting.top

npx vite build
来源：http://isr.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://gfz.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://mjh.hnqzz.top

================================================================================
来源：http://dyf.hnxiangtu.top

统计汇总
来源：http://tax.bjfxy.top

================================================================================
来源：http://qhu.fktsv.cn

按语言统计（条）：
来源：http://nzw.ppjwa.cn

Python ......... 252
来源：http://edf.zhaomingkeji.xyz

PHP ............ 252
来源：http://slz.tarul.cn

JavaScript ..... 252
来源：http://ryo.iojbl.cn

TypeScript ..... 212
来源：http://fsh.zycfv.cn

Java ........... 212
来源：http://hqk.jiagoushi.top

Go ............. 212
来源：http://ldn.nanxuanxn.top

Ruby ........... 212
来源：http://hbe.smart0.xyz

C# ............. 212
来源：http://gyc.gaohongyu789.top

C .............. 30
来源：http://ylb.yvedp.cn

C++ ............ 30
来源：http://qkp.yj202588.top

SQL ............ 90
来源：http://ldl.316326.xyz

Bash ........... 80
来源：http://qqt.yueranfly.top

Kotlin ......... 15
来源：http://rlq.hywenlv.cn

Swift .......... 15
来源：http://jkq.yuanzhike.top

Lua ............ 10
来源：http://ihh.tian-w.cn

Perl ........... 10
来源：http://fzb.jinqigfzy.top

Scala .......... 10
来源：http://osk.cqqwz.cn

------------------------------------
来源：http://nmx.wangdashe.top

合计 ........... 2106 条
来源：http://rvs.hysaishi.cn

按章节统计：
来源：http://rjs.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sqj.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dtt.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eni.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gem.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ouf.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vnp.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://umc.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://goy.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yoy.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oqf.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tjl.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hft.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tny.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ept.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fly.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bqk.yongpay.top

Q SQL 专题                              90
来源：http://xwr.yj20258.top

R Bash 专题                             80
来源：http://ird.aizwys.cn

S C / C++ 专题                          60
来源：http://ack.ivvv.top

T 其他语言补充                          60
来源：http://utw.jyoumei.cn

U 高频实用片段                         120
来源：http://zyv.0kj1m.cn

------------------------------------
来源：http://jhk.gaohongyu789.top

合计                                  2106 条
来源：http://fsn.xuanzx.com

--------------------------------------------------------------------------------
来源：http://csu.fanxiaobao.xyz

使用提醒
来源：http://zkh.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://qxr.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://whv.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hkw.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zdr.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lro.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xxd.yvedp.cn

—— 文件结束 ——
来源：http://xiv.sxryk.cn

================================================================================
来源：http://jjw.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://wzw.xinyue.icu

Common Programming Examples Cheat Book
来源：http://cec.jinqigfzy.top

================================================================================
来源：http://cfs.uphjek.com

【收录内容】
来源：http://iia.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xeh.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rnc.nanxinkj.top

SQL · Bash · C · C++
来源：http://bvc.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nmv.yueranfly.top

【使用说明】
来源：http://thh.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ntm.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ffn.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dxz.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ppa.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ufd.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rma.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://off.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dtf.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fpw.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ptm.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tgt.svipenyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cew.nanxuanxn.top

【文件统计】
来源：http://ygf.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://urn.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://zef.meibo888.top

目  录
来源：http://ysa.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://sue.yonumen.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iwo.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ekh.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ugb.cheryme.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hra.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://egu.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://evo.snrcjt.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://evq.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://urm.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://asx.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tpl.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rqb.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vvm.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tnw.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://met.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ifh.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://toe.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jui.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xeu.wangdashe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fvu.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jwn.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ans.zhongyouzk.top

================================================================================
来源：http://dpc.sysykeji.top

A. 基础语法与类型
来源：http://edl.dianchejie.cn

================================================================================
来源：http://ord.fanxiaobao.xyz

[A01] Hello World
来源：http://fgp.dianchejie.cn

Py:   print("Hello, World!")
来源：http://cna.sweek.top

PHP:  echo "Hello, World!";
来源：http://ofv.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://fbs.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bpw.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://qrm.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://jwt.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://dga.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://pxg.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://pbw.yuxming.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fpd.sjlbkw.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rxs.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hwk.hfpthk.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dht.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://utr.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://gxu.wangdashe.top

Ruby: name = "Alex"; age = 20
来源：http://qaw.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hsr.fzhhl.top

[A03] 常量定义
来源：http://kzn.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sss.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://ift.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://mgt.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://ski.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://twv.hesvh.cn

Go:   const PI = 3.14159
来源：http://ieg.shuidangran.top

Ruby: PI = 3.14159
来源：http://zmq.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://efc.gzhubu.top

[A04] 判断变量类型
来源：http://toc.xinyue.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://fxb.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yxv.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tzb.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://qfk.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mgp.xylfe.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ywj.jinyuanbaomall.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://epg.zhijiandao.cn

C#:   x.GetType().Name; x is int
来源：http://gmd.zhijiandao.cn

[A05] 整数除法与取模
来源：http://mdq.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hnn.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ame.52xcode.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pqm.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://msg.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://puz.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://bts.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://qbh.kuanghao11.cn

C#:   7 / 2; 7 % 2
来源：http://qbq.gogol.net.cn

[A06] 字符串转数字
来源：http://jkw.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://ycj.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fma.shuidangran.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jep.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jho.hfpthk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vjj.ivvv.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qti.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tpa.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://chx.cashguo.top

[A07] 数字转字符串
来源：http://frt.jlsjyb.cn

Py:   str(42)
来源：http://ybm.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://lhq.hfpthk.cn

JS:   String(42); (42).toString()
来源：http://irc.xuetiantiany.cn

TS:   String(42)
来源：http://elw.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wyr.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://yyz.zhaomingkeji.xyz

Ruby: 42.to_s
来源：http://onk.zhongyouzk.top

C#:   42.ToString()
来源：http://byx.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://oey.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rak.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mnh.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mmj.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ytx.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vms.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xso.yueranfly.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kbh.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zyv.nanxuanxn.top

[A09] 绝对值与最大最小值
来源：http://pau.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://djd.nanxuanxn.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yfp.zhongyouzk.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fix.dashuyun.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://asi.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ajb.wangshuangyany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vgw.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nai.hysaishi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rni.zhijiandao.cn

[A10] 生成随机数
来源：http://tcf.fktsv.cn

Py:   import random; random.randint(1, 100)
来源：http://qqm.fehbvm.com

PHP:  random_int(1, 100);
来源：http://zot.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fyy.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dwm.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://owx.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rbx.sufxvd.cn

Ruby: rand(1..100)
来源：http://lqe.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://hxh.yvedp.cn

[A11] 条件表达式（三元）
来源：http://yrm.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://ylv.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qqy.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://iol.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://mon.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://bsp.tarul.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bzs.snrcjt.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ped.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uaa.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://gzw.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://imr.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hil.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://nqn.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://anu.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://dvp.yangfankeji.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lmu.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://pvx.tarul.cn

C#:   $"Hello, {name}!"
来源：http://qyn.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://myg.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://sgv.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://oek.daxiang520.top

JS:   "第一行\n第二行"
来源：http://mmz.wangdashe.top

TS:   "第一行\n第二行"
来源：http://nwp.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://emd.svipenyu.cn

Go:   "第一行\n第二行"
来源：http://rbm.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://fjo.nanxuanxn.top

C#:   "第一行\n第二行"
来源：http://wpw.hysaishi.cn

[A14] 注释写法
来源：http://tep.shangyingyoupin.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dyi.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jfp.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://wdw.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://pad.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gwp.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://hcf.haohaochexian.top

Ruby: # 单行；=begin 多行 =end
来源：http://ldq.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://isv.iojbl.cn

[A15] 空值判断与默认值
来源：http://zxb.chenlongwang.top

Py:   value = data or "默认值"
来源：http://snt.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://lnd.zhiwuduotai.top

JS:   const value = data ?? "默认值";
来源：http://cfm.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://ltc.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xoh.mhx1999.top

Go:   if data == "" { data = "默认值" }
来源：http://yvj.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://bal.tianlin.xyz

C#:   var value = data ?? "默认值";
来源：http://qqu.zhoulong.xyz

[A16] 真假值判断规则
来源：http://wjl.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cnp.ywan-chungtsiang.top


<!-- 参考信息 -->