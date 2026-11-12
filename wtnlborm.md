代发 wailian999

[U91] JS：对象键值遍历
来源：http://rus.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rfe.andypj.xyz

[U92] JS：深拷贝
来源：http://rbz.fzhhl.top

structuredClone(obj)
来源：http://fng.uphjek.com

[U93] JS：模板字符串
来源：http://mnv.vqdsnc.cn

`共 ${n} 条`
来源：http://soe.bjfxy.top

[U94] JS：箭头函数
来源：http://ghy.cqqwz.cn

const double = x => x * 2;
来源：http://uli.yj202588.top

[U95] JS：Promise 包装
来源：http://ixe.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://leh.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://mxw.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ljy.xuanzx.com

[U97] JS：并发请求
来源：http://vzp.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rht.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://kkd.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aod.gogol.net.cn

[U99] JS：事件监听
来源：http://gil.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://nbh.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://aqq.bjfxy.top

document.querySelector(".item")
来源：http://uun.yvedp.cn

[U101] JS：classList 操作
来源：http://xkc.jyoumei.cn

el.classList.toggle("active")
来源：http://bax.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://rbr.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jav.xuetiantiany.cn

[U103] JS：定时器
来源：http://olk.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xll.quarkkingdee.top

[U104] JS：防抖
来源：http://caq.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyd.tanke756.top

[U105] JS：节流
来源：http://ssv.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qnd.jinqigufen.top

[U106] JS：日期格式化
来源：http://aml.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://paz.fzhhl.top

[U107] JS：数字千分位
来源：http://cjw.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mhp.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://flp.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blx.xuetiantiany.cn

[U109] JS：数组分组
来源：http://soa.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://mdp.jianghu66.top

[U110] JS：数组分块
来源：http://cqn.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bta.uphjek.com

[U111] JS：对象转 Map
来源：http://igh.gzhubu.top

new Map(Object.entries(obj))
来源：http://abu.daxiang520.top

[U112] JS：字符串补位
来源：http://ukr.chenlongwang.top

"7".padStart(3, "0")
来源：http://fnr.yuxming.cn

[U113] JS：正则替换全部
来源：http://tek.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://zpr.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://bhu.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wnt.jinqigufen.top

[U115] JS：生成 UUID
来源：http://nyy.aibaodan.cn

crypto.randomUUID()
来源：http://jda.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://fhf.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://sap.xinyue.icu

[U117] JS：单元测试
来源：http://ckg.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://qfd.tianlin.xyz

[U118] JS：开发服务器
来源：http://mtl.ehwqpu.com

npm i -D vite;  npx vite
来源：http://udo.sufxvd.cn

[U119] JS：生产构建
来源：http://xum.wangdashe.top

npx vite build
来源：http://hjl.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://uda.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://dyd.jlsjyb.cn

================================================================================
来源：http://unr.gzhubu.top

统计汇总
来源：http://ttw.jinghuilouyu.cn

================================================================================
来源：http://amt.hammf.cn

按语言统计（条）：
来源：http://wrh.ivvv.top

Python ......... 252
来源：http://fli.dashuyun.cn

PHP ............ 252
来源：http://uif.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://dys.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://ywm.tianlin.xyz

Java ........... 212
来源：http://bhw.yangfankeji.com

Go ............. 212
来源：http://nbr.chenlongwang.top

Ruby ........... 212
来源：http://pih.epnwcf.com

C# ............. 212
来源：http://who.bjfxy.top

C .............. 30
来源：http://wnl.hongshengwenyu.top

C++ ............ 30
来源：http://onq.iojbl.cn

SQL ............ 90
来源：http://yqi.chenlongwang.top

Bash ........... 80
来源：http://utk.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://hod.hnqzz.top

Swift .......... 15
来源：http://xth.chenjidiqi.icu

Lua ............ 10
来源：http://ybz.andypj.xyz

Perl ........... 10
来源：http://aod.ydzc1.top

Scala .......... 10
来源：http://wka.birdmap.top

------------------------------------
来源：http://efm.hywenlv.cn

合计 ........... 2106 条
来源：http://arv.cashguo.top

按章节统计：
来源：http://duu.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hlx.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ucr.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kic.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nkx.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cqo.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://boh.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kns.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gtu.fengsongda.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vgz.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jes.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kfl.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sak.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://piu.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wgr.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cyq.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vab.redwolf501.top

Q SQL 专题                              90
来源：http://duo.hysaishi.cn

R Bash 专题                             80
来源：http://jld.ivvv.top

S C / C++ 专题                          60
来源：http://end.mhx1999.top

T 其他语言补充                          60
来源：http://umo.zhiwuduotai.top

U 高频实用片段                         120
来源：http://acq.vehdjk.com

------------------------------------
来源：http://cnm.shangyingyoupin.top

合计                                  2106 条
来源：http://rvn.andypj.xyz

--------------------------------------------------------------------------------
来源：http://cwn.yj202588.top

使用提醒
来源：http://hyi.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://lfb.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://reg.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ssv.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fjr.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dcn.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ajp.meibo888.top

—— 文件结束 ——
来源：http://tbs.jianghu66.top

================================================================================
来源：http://pmd.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://bki.xuanzx.com

Common Programming Examples Cheat Book
来源：http://qfs.gaohongyu789.top

================================================================================
来源：http://vyn.hnqzz.top

【收录内容】
来源：http://fen.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jsk.nanxinkj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://crh.gogol.net.cn

SQL · Bash · C · C++
来源：http://tjm.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://emd.epnwcf.com

【使用说明】
来源：http://esd.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nbm.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wvv.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vza.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vdm.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://agv.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vhw.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://obc.zycfv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ktj.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kwb.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://veh.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ifu.hcnkem.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ncu.ivvv.top

【文件统计】
来源：http://wiw.yfazqb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nyj.tanke756.top

--------------------------------------------------------------------------------
来源：http://szy.cheryme.top

目  录
来源：http://xhn.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://caq.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aqn.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vlu.gotoacloud.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mhc.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xme.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://asp.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jcq.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qpb.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pdk.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lam.wangdashe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nsn.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qdq.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eeo.aibaodan.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vcg.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ula.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eqv.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gcc.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xim.smart0.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://pgr.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kwp.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aml.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jij.nwbrower.top

================================================================================
来源：http://huc.shzxlz.cn

A. 基础语法与类型
来源：http://jkb.wangshuangyany.cn

================================================================================
来源：http://bgd.ehwqpu.com

[A01] Hello World
来源：http://sog.sufxvd.cn

Py:   print("Hello, World!")
来源：http://vwp.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://pry.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://dib.yvedp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xnt.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://qww.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://ave.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://ads.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gaw.haohaochexian.top

[A02] 变量声明与赋值
来源：http://bgf.tianlin.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tfq.wangdashe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://opp.yongpay.top

JS:   let name = "Alex"; const age = 20;
来源：http://wvi.ppjwa.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sqs.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://pvv.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://zct.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://epd.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://laf.nanxuanxn.top

[A03] 常量定义
来源：http://odw.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bdy.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://awq.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://zmr.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://ybq.ctjpmb.com

Java: static final double PI = 3.14159;
来源：http://dyb.shzxlz.cn

Go:   const PI = 3.14159
来源：http://sxe.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://aow.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://tob.quarkkingdee.top

[A04] 判断变量类型
来源：http://win.fengsongda.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rdn.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jlt.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jws.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://zga.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fsm.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://dut.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vwy.smart0.xyz

C#:   x.GetType().Name; x is int
来源：http://teq.gotoacloud.top

[A05] 整数除法与取模
来源：http://wmy.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://euo.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://yqm.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gdr.ybcxt.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjo.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://afo.zhixingplan.top

Go:   7 / 2; 7 % 2
来源：http://prx.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://slr.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://lvv.vehdjk.com

[A06] 字符串转数字
来源：http://gaf.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://mdw.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yjn.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aqc.sjlbkw.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uyf.hysaishi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gce.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yww.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://gka.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nwc.tianlin.xyz

[A07] 数字转字符串
来源：http://ncv.chenlongwang.top

Py:   str(42)
来源：http://lyj.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://inn.shanyushiyangkeji.top

JS:   String(42); (42).toString()
来源：http://zff.fktsv.cn

TS:   String(42)
来源：http://koi.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wor.jinqigufen.top

Go:   strconv.Itoa(42)
来源：http://ist.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://kiz.epnwcf.com

C#:   42.ToString()
来源：http://qgg.gotoacloud.top

[A08] 取整与四舍五入
来源：http://kyv.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wff.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://upd.ehwqpu.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lto.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cmh.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gsw.xingfuxueyuan.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hnh.jyoumei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://blt.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dpn.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://vzy.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jlf.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hqt.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wqp.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ogq.hnxiangtu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yeg.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jun.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rbg.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://atf.haohaochexian.top

[A10] 生成随机数
来源：http://mdg.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://rou.ybcxt.top

PHP:  random_int(1, 100);
来源：http://jtx.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iqc.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mxs.uphjek.com

Java: new Random().nextInt(100) + 1
来源：http://ztf.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bei.sufxvd.cn

Ruby: rand(1..100)
来源：http://ekx.52xcode.cn

C#:   new Random().Next(1, 101)
来源：http://wld.bjfxy.top

[A11] 条件表达式（三元）
来源：http://aae.sjlbkw.cn

Py:   "yes" if x > 0 else "no"
来源：http://zsd.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pmr.snrcjt.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ytx.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://eri.ivvv.top

Java: x > 0 ? "yes" : "no"
来源：http://zts.yfazqb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://txf.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://eyn.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://prd.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://ueh.svipenyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ltl.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lcs.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://jag.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://ltd.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://cnj.wangdashe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mht.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://alz.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://uga.sxryk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pbf.yuxming.cn

Py:   "第一行\n第二行"
来源：http://dwl.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://uur.dianchejie.cn

JS:   "第一行\n第二行"
来源：http://mgr.zhoulong.xyz

TS:   "第一行\n第二行"
来源：http://wcm.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://aez.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://cwa.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://jwl.fengsongda.top

C#:   "第一行\n第二行"
来源：http://rvi.quarkkingdee.top

[A14] 注释写法
来源：http://tzu.fengsongda.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tgn.ppjwa.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xox.hysaishi.cn

JS:   // 单行；/* 多行 */
来源：http://ldb.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://ade.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xjy.316326.xyz

Go:   // 单行；/* 多行 */
来源：http://fsx.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://ddi.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://bqg.guowangkeji.top

[A15] 空值判断与默认值
来源：http://sfk.ywan-chungtsiang.top

Py:   value = data or "默认值"
来源：http://okr.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://rqx.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://zhc.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://lkt.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xwm.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://hdy.cdnleiting.top


<!-- 参考信息 -->