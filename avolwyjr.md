代发 wailian999

[U91] JS：对象键值遍历
来源：http://vhr.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rnb.hammf.cn

[U92] JS：深拷贝
来源：http://ecm.ctjpmb.com

structuredClone(obj)
来源：http://led.hnqzz.top

[U93] JS：模板字符串
来源：http://cse.hammf.cn

`共 ${n} 条`
来源：http://tcl.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://agg.jlsjyb.cn

const double = x => x * 2;
来源：http://azl.sweek.top

[U95] JS：Promise 包装
来源：http://hlc.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://qch.bjfxy.top

[U96] JS：async/await 与异常
来源：http://rcw.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wro.guowangkeji.top

[U97] JS：并发请求
来源：http://hwn.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uvn.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://kbt.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kif.sufxvd.cn

[U99] JS：事件监听
来源：http://jvu.vehdjk.com

el.addEventListener("click", e => {})
来源：http://emj.redwolf501.top

[U100] JS：DOM 查询
来源：http://bnl.tian-w.cn

document.querySelector(".item")
来源：http://dyi.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://heu.chenlongwang.top

el.classList.toggle("active")
来源：http://czl.fzhhl.top

[U102] JS：本地存储
来源：http://zea.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fds.316326.xyz

[U103] JS：定时器
来源：http://pql.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uge.dianchejie.cn

[U104] JS：防抖
来源：http://tlr.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mzn.kuanghao11.cn

[U105] JS：节流
来源：http://qdu.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uue.hysaishi.cn

[U106] JS：日期格式化
来源：http://vro.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://adb.zdqjudy.top

[U107] JS：数字千分位
来源：http://skg.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lqm.xylfe.cn

[U108] JS：随机整数
来源：http://eyc.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qro.yuanzhike.top

[U109] JS：数组分组
来源：http://hhg.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://xol.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://dys.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://znk.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://pdz.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://dxr.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://drp.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://wlf.pycfn.com

[U113] JS：正则替换全部
来源：http://gsw.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://fcs.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://bno.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eod.fehbvm.com

[U115] JS：生成 UUID
来源：http://ljv.zhiwuduotai.top

crypto.randomUUID()
来源：http://mht.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://xte.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://zai.hysaishi.cn

[U117] JS：单元测试
来源：http://dbw.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://ote.kuanghao11.cn

[U118] JS：开发服务器
来源：http://isk.c1oappe.top

npm i -D vite;  npx vite
来源：http://suw.yfazqb.com

[U119] JS：生产构建
来源：http://gml.cqqwz.cn

npx vite build
来源：http://zdf.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://lhq.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://hmw.xuetiantiany.cn

================================================================================
来源：http://jhh.gogol.net.cn

统计汇总
来源：http://egn.xziqi.cn

================================================================================
来源：http://civ.dashuyun.cn

按语言统计（条）：
来源：http://rws.epnwcf.com

Python ......... 252
来源：http://qzq.hesvh.cn

PHP ............ 252
来源：http://lly.guowangkeji.top

JavaScript ..... 252
来源：http://bgu.shanyushiyangtech.top

TypeScript ..... 212
来源：http://kmt.hysaishi.cn

Java ........... 212
来源：http://aan.yuanzhike.top

Go ............. 212
来源：http://mcn.cucudq.cn

Ruby ........... 212
来源：http://vzk.gaohongyu789.top

C# ............. 212
来源：http://bbt.ctjpmb.com

C .............. 30
来源：http://fhk.epnwcf.com

C++ ............ 30
来源：http://dmd.tanke756.top

SQL ............ 90
来源：http://lkc.tian-w.cn

Bash ........... 80
来源：http://smn.shangyingyoupin.top

Kotlin ......... 15
来源：http://oci.nwbrower.top

Swift .......... 15
来源：http://cyo.316326.xyz

Lua ............ 10
来源：http://txb.jqgufenzy.top

Perl ........... 10
来源：http://xcp.zdqjudy.top

Scala .......... 10
来源：http://ysl.jinqigfzy.top

------------------------------------
来源：http://tbn.fengsongda.top

合计 ........... 2106 条
来源：http://aho.aizwys.cn

按章节统计：
来源：http://vkr.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://miu.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gai.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rym.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yfl.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fwq.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hqk.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qze.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uqi.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cps.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cpt.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://juk.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lqd.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://enf.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://svb.yuxming.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hrt.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gst.pengpengdd.cyou

Q SQL 专题                              90
来源：http://znv.xuetiantiany.cn

R Bash 专题                             80
来源：http://kmy.yangfankeji.com

S C / C++ 专题                          60
来源：http://fps.aizwys.cn

T 其他语言补充                          60
来源：http://fmr.yvedp.cn

U 高频实用片段                         120
来源：http://puo.zhoulong.xyz

------------------------------------
来源：http://ijg.xuetiantiany.cn

合计                                  2106 条
来源：http://iwh.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://fiw.jianghu66.top

使用提醒
来源：http://tka.hesvh.cn

--------------------------------------------------------------------------------
来源：http://brf.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ion.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ntk.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qna.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dls.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zsy.sufxvd.cn

—— 文件结束 ——
来源：http://avw.yongpay.top

================================================================================
来源：http://rhk.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://ztc.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://dyp.ywan-chungtsiang.top

================================================================================
来源：http://ojc.cqqwz.cn

【收录内容】
来源：http://mcl.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mun.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qft.birdmap.top

SQL · Bash · C · C++
来源：http://qtx.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ggg.yangfankeji.com

【使用说明】
来源：http://lem.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vye.tianlin.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vau.sjlbkw.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://avd.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://odn.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mif.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tug.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xlg.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nyv.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ugc.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vzy.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fek.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://frz.gzhubu.top

【文件统计】
来源：http://dpf.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jlv.andypj.xyz

--------------------------------------------------------------------------------
来源：http://kev.kuanghao11.cn

目  录
来源：http://gif.yj20258888.top

--------------------------------------------------------------------------------
来源：http://coi.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zto.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qdq.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uos.redwolf501.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://btk.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yjv.mhx1999.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://whf.jqgufenzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rml.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://reg.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://way.fktsv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vms.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wzp.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xru.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fyi.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yiu.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lsj.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fqr.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lgu.fktsv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://too.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gkg.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dwl.ivvv.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ezr.vqdsnc.cn

================================================================================
来源：http://ieg.uphjek.com

A. 基础语法与类型
来源：http://nuu.yueranfly.top

================================================================================
来源：http://smx.xylfe.cn

[A01] Hello World
来源：http://gyb.tian-w.cn

Py:   print("Hello, World!")
来源：http://fiy.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://wmk.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://cli.zhoulong.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://boj.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://ipp.xinyue.icu

Go:   fmt.Println("Hello, World!")
来源：http://gew.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://fii.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yey.vqdsnc.cn

[A02] 变量声明与赋值
来源：http://fje.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tkh.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://nni.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://jfb.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xtm.fehbvm.com

Java: String name = "Alex"; int age = 20;
来源：http://rjh.hnqzz.top

Go:   name := "Alex"; age := 20
来源：http://hnm.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://qmn.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://fln.snrcjt.cn

[A03] 常量定义
来源：http://ahq.tian-w.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lgb.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://bon.xylfe.cn

JS:   const PI = 3.14159;
来源：http://gxt.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://qmc.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://gzm.zhongyouzk.top

Go:   const PI = 3.14159
来源：http://cfg.bjfxy.top

Ruby: PI = 3.14159
来源：http://hzs.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://obn.gzhubu.top

[A04] 判断变量类型
来源：http://cak.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://iou.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qcs.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rox.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://mpp.pengpengdd.cyou

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vcu.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://eip.andypj.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://nel.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://hpm.gogol.net.cn

[A05] 整数除法与取模
来源：http://cem.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://avh.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://ati.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tkc.shuidangran.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://awd.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://pbe.chenjidiqi.icu

Go:   7 / 2; 7 % 2
来源：http://tnx.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://zls.snrcjt.cn

C#:   7 / 2; 7 % 2
来源：http://yal.xylfe.cn

[A06] 字符串转数字
来源：http://ljy.quarkkingdee.top

Py:   int("42"); float("3.14")
来源：http://bne.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pad.xinyue.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://erp.dianchejie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kmj.shanyushiyangtech.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fjg.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pdw.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vzs.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wto.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://xui.yanxiufei.cn

Py:   str(42)
来源：http://tgr.sxryk.cn

PHP:  (string) 42; strval(42)
来源：http://wbw.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://gsr.jianghu66.top

TS:   String(42)
来源：http://bfb.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uas.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://huf.yj20258.top

Ruby: 42.to_s
来源：http://pvx.sysykeji.top

C#:   42.ToString()
来源：http://tyl.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://bvh.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://squ.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iro.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://btv.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bxi.jianghu66.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fdn.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://psm.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://nae.jyoumei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wnq.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://uor.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qdq.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bau.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qjd.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mtj.andypj.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://syx.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jez.bjfxy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wtm.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yyl.bbcook.cn

[A10] 生成随机数
来源：http://ytz.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://grj.hongshengwenyu.top

PHP:  random_int(1, 100);
来源：http://rov.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lkt.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fom.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://vfn.ppjwa.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wre.sufxvd.cn

Ruby: rand(1..100)
来源：http://lws.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://ykq.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://lxq.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://czp.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://bjd.yj20258.top

JS:   x > 0 ? "yes" : "no"
来源：http://cih.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://sgk.snrcjt.cn

Java: x > 0 ? "yes" : "no"
来源：http://onb.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://vvr.sysykeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rbz.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wme.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://vrj.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jbm.zycfv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oyf.gzhubu.top

JS:   `Hello, ${name}!`
来源：http://plm.zhixingplan.top

TS:   `Hello, ${name}!`
来源：http://sbh.fehbvm.com

Java: "Hello, %s!".formatted(name)
来源：http://aqe.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://muc.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://duj.ivvv.top

C#:   $"Hello, {name}!"
来源：http://lhu.xziqi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ytu.yj202588.top

Py:   "第一行\n第二行"
来源：http://vjy.cashguo.top

PHP:  "第一行\n第二行"
来源：http://bxg.wangshuangyany.cn

JS:   "第一行\n第二行"
来源：http://qsy.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://bdp.cashguo.top

Java: "第一行\n第二行"
来源：http://tdf.cashguo.top

Go:   "第一行\n第二行"
来源：http://vcs.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://loz.hesvh.cn

C#:   "第一行\n第二行"
来源：http://muf.guannengcc.top

[A14] 注释写法
来源：http://pjf.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nve.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eei.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://epi.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://igu.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jnv.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://fse.cqqwz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eml.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://ubm.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://kza.yuxming.cn

Py:   value = data or "默认值"
来源：http://iez.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://vju.xuetiantiany.cn

JS:   const value = data ?? "默认值";
来源：http://nvz.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://zgw.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://req.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://edk.dianchejie.cn


<!-- 参考信息 -->