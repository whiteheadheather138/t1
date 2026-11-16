代发 wailian999

[U89] JS：数组去重
来源：http://uog.jyoumei.cn

[...new Set(arr)]
来源：http://xyx.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://zjx.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://qkp.jianghu66.top

[U91] JS：对象键值遍历
来源：http://fsn.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zix.yvedp.cn

[U92] JS：深拷贝
来源：http://set.zhixingplan.top

structuredClone(obj)
来源：http://vms.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://znw.gaohongyu789.top

`共 ${n} 条`
来源：http://dtu.nanxinkj.top

[U94] JS：箭头函数
来源：http://xvl.xuetiantiany.cn

const double = x => x * 2;
来源：http://nrc.cheryme.top

[U95] JS：Promise 包装
来源：http://god.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://qvw.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://kem.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://exx.yangfankeji.com

[U97] JS：并发请求
来源：http://czz.yuanzhike.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jkn.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://sle.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tdc.316326.xyz

[U99] JS：事件监听
来源：http://axa.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://mow.iojbl.cn

[U100] JS：DOM 查询
来源：http://qbi.pycfn.com

document.querySelector(".item")
来源：http://lag.smart0.xyz

[U101] JS：classList 操作
来源：http://sxa.vqdsnc.cn

el.classList.toggle("active")
来源：http://rrb.fktsv.cn

[U102] JS：本地存储
来源：http://reu.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eml.kuanghao11.cn

[U103] JS：定时器
来源：http://qqm.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ppf.jinghuilouyu.cn

[U104] JS：防抖
来源：http://dtp.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xkh.jqgfzy.top

[U105] JS：节流
来源：http://sgk.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hix.yangfankeji.com

[U106] JS：日期格式化
来源：http://zls.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vez.ybcxt.top

[U107] JS：数字千分位
来源：http://vrd.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hcx.zhoulong.xyz

[U108] JS：随机整数
来源：http://eub.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ewq.andypj.xyz

[U109] JS：数组分组
来源：http://kfw.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://aax.c1oappe.top

[U110] JS：数组分块
来源：http://xpa.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yrs.ybcxt.top

[U111] JS：对象转 Map
来源：http://bac.cqqwz.cn

new Map(Object.entries(obj))
来源：http://wcj.hammf.cn

[U112] JS：字符串补位
来源：http://tzo.birdmap.top

"7".padStart(3, "0")
来源：http://joy.nwbrower.top

[U113] JS：正则替换全部
来源：http://kkp.jqgfzy.top

s.replaceAll("a", "b")
来源：http://sno.epnwcf.com

[U114] JS：JSON 深比较
来源：http://jqa.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kln.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://plv.kuanghao11.cn

crypto.randomUUID()
来源：http://toq.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://cow.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://bni.ehwqpu.com

[U117] JS：单元测试
来源：http://huj.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://clk.aizwys.cn

[U118] JS：开发服务器
来源：http://rrb.shuidangran.top

npm i -D vite;  npx vite
来源：http://djt.dashuyun.cn

[U119] JS：生产构建
来源：http://pxo.fehbvm.com

npx vite build
来源：http://nck.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://qkr.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://rqr.guannengcc.top

================================================================================
来源：http://une.hywenlv.cn

统计汇总
来源：http://uky.quarkkingdee.top

================================================================================
来源：http://eqp.jlsjyb.cn

按语言统计（条）：
来源：http://pdn.aibaodan.cn

Python ......... 252
来源：http://vpx.andypj.xyz

PHP ............ 252
来源：http://jjl.yonumen.top

JavaScript ..... 252
来源：http://znr.c1oappe.top

TypeScript ..... 212
来源：http://uox.zhiwuduotai.top

Java ........... 212
来源：http://kaf.zhengqikj.top

Go ............. 212
来源：http://itm.jqgufenzy.top

Ruby ........... 212
来源：http://sji.zhijiandao.cn

C# ............. 212
来源：http://vhn.fanxiaobao.xyz

C .............. 30
来源：http://xcm.xuetiantiany.cn

C++ ............ 30
来源：http://ozd.feifeiyinyue.top

SQL ............ 90
来源：http://lov.yvedp.cn

Bash ........... 80
来源：http://epy.shangyingyoupin.top

Kotlin ......... 15
来源：http://pae.jqgufenzy.top

Swift .......... 15
来源：http://ram.smart0.xyz

Lua ............ 10
来源：http://coj.quarkkingdee.top

Perl ........... 10
来源：http://ekv.xziqi.cn

Scala .......... 10
来源：http://ykb.jinghuilouyu.cn

------------------------------------
来源：http://ozm.ctjpmb.com

合计 ........... 2106 条
来源：http://nnz.yj20258.top

按章节统计：
来源：http://kkh.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xde.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rga.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dui.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://txj.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jjs.jianghu66.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kvd.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cjq.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nud.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://emr.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qhq.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ujl.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fby.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zwn.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ckp.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ouv.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://phu.cheryme.top

Q SQL 专题                              90
来源：http://jib.sjlbkw.cn

R Bash 专题                             80
来源：http://eod.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://xpp.bjfxy.top

T 其他语言补充                          60
来源：http://wav.gaohongyu789.top

U 高频实用片段                         120
来源：http://teu.hammf.cn

------------------------------------
来源：http://qmf.cheryme.top

合计                                  2106 条
来源：http://iyl.zycfv.cn

--------------------------------------------------------------------------------
来源：http://tjd.yvedp.cn

使用提醒
来源：http://zfg.xuanzx.com

--------------------------------------------------------------------------------
来源：http://nkh.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mrp.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ymz.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uee.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oah.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aqf.jqgufenzy.top

—— 文件结束 ——
来源：http://iww.zdbjq.cn

================================================================================
来源：http://jir.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://ujc.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://clc.zdqjudy.top

================================================================================
来源：http://iou.vqdsnc.cn

【收录内容】
来源：http://gdi.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oau.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://muq.sufxvd.cn

SQL · Bash · C · C++
来源：http://gnm.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://keg.ybcxt.top

【使用说明】
来源：http://xqo.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uub.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oun.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hzv.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fmr.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zok.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://stk.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oym.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://han.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vfe.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cdw.shzxlz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rxl.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ree.cheryme.top

【文件统计】
来源：http://yws.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fqk.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://oyh.cqqwz.cn

目  录
来源：http://dsk.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://wmn.yvedp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bmc.smart0.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qju.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://juv.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rpt.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://srn.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qni.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rvr.fktsv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zrp.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qbq.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lnx.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gke.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ktv.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cyw.bbcook.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vis.daxiang520.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sfj.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aaw.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pnz.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wpx.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wnx.c1oappe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wfv.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mpi.yvedp.cn

================================================================================
来源：http://qoh.cucudq.cn

A. 基础语法与类型
来源：http://uww.jianghu66.top

================================================================================
来源：http://wjf.fehbvm.com

[A01] Hello World
来源：http://rvs.yuanzhike.top

Py:   print("Hello, World!")
来源：http://rwf.yanxiufei.cn

PHP:  echo "Hello, World!";
来源：http://wxz.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://osx.feifeiyinyue.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dgj.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://jsg.zhiwuduotai.top

Go:   fmt.Println("Hello, World!")
来源：http://lmu.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://suq.cucudq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dus.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://cpq.9152youxi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hib.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://iwe.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://sjo.ywan-chungtsiang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qwf.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://utn.ybcxt.top

Go:   name := "Alex"; age := 20
来源：http://goi.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://rid.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://uaz.feifeiyinyue.top

[A03] 常量定义
来源：http://iav.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ymu.fzhhl.top

PHP:  const PI = 3.14159;
来源：http://dez.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://vwf.fktsv.cn

TS:   const PI: number = 3.14159;
来源：http://adt.hammf.cn

Java: static final double PI = 3.14159;
来源：http://aah.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://xun.sweek.top

Ruby: PI = 3.14159
来源：http://jrd.sufxvd.cn

C#:   const double PI = 3.14159;
来源：http://mka.ppjwa.cn

[A04] 判断变量类型
来源：http://stx.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xsn.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ikg.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rlr.yangfankeji.com

TS:   typeof x; x instanceof Date
来源：http://eqq.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jrr.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://gak.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cws.havefunace.top

C#:   x.GetType().Name; x is int
来源：http://spv.yueranfly.top

[A05] 整数除法与取模
来源：http://fut.ivvv.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vcl.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://jxi.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sfy.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vej.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://kyj.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://cxd.sysykeji.top

Ruby: 7 / 2; 7 % 2
来源：http://zxj.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://lez.shzxlz.cn

[A06] 字符串转数字
来源：http://yna.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://rzx.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yal.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iyc.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://qke.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qxg.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yuh.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://woj.guannengcc.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uvl.tianlin.xyz

[A07] 数字转字符串
来源：http://ghi.yangfankeji.com

Py:   str(42)
来源：http://gwe.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://sbt.snrcjt.cn

JS:   String(42); (42).toString()
来源：http://zhq.zycfv.cn

TS:   String(42)
来源：http://yee.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vrq.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://umk.hesvh.cn

Ruby: 42.to_s
来源：http://bdd.havefunace.top

C#:   42.ToString()
来源：http://dbf.chenlongwang.top

[A08] 取整与四舍五入
来源：http://vao.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sop.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ogn.tanke756.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zkm.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rnt.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cqx.shangyingyoupin.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aoo.vehdjk.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://hee.zhixingplan.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvh.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://ewg.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://txr.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iky.fzhhl.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lfv.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xaa.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bbo.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yjq.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aaj.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://osy.quarkkingdee.top

[A10] 生成随机数
来源：http://qhi.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://hgp.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://ord.guowangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lfh.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ycp.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://ffe.chenjidiqi.icu

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eyv.hcnkem.com

Ruby: rand(1..100)
来源：http://tbo.zhongyouzk.top

C#:   new Random().Next(1, 101)
来源：http://iwg.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://thx.yanxiufei.cn

Py:   "yes" if x > 0 else "no"
来源：http://bgr.zhijiandao.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://twg.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://qwn.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bcb.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://pfy.guowangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://htq.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://plc.sufxvd.cn

C#:   x > 0 ? "yes" : "no"
来源：http://swr.redwolf501.top

[A12] 字符串插值 / 格式化
来源：http://qcy.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kir.gotoacloud.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qbq.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://exb.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://qjs.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://tpx.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hpx.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://sln.pycfn.com

C#:   $"Hello, {name}!"
来源：http://dwx.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ekl.daria6918.cn

Py:   "第一行\n第二行"
来源：http://kmi.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://hpw.hnqzz.top

JS:   "第一行\n第二行"
来源：http://kzr.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://uop.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://gcu.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://hmu.yj20258.top

Ruby: "第一行\n第二行"
来源：http://fft.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://zhk.kuanghao11.cn

[A14] 注释写法
来源：http://kac.ydzc1.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://thk.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kfh.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://njl.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://ely.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hni.chenlongwang.top

Go:   // 单行；/* 多行 */
来源：http://esm.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://sjv.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://kld.fktsv.cn

[A15] 空值判断与默认值
来源：http://ahj.gaohongyu789.top

Py:   value = data or "默认值"
来源：http://rwz.tarul.cn

PHP:  $value = $data ?? "默认值";
来源：http://fxj.jinqigfzy.top


<!-- 参考信息 -->