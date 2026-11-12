代发 wailian999

[U97] JS：并发请求
来源：http://aqk.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hqn.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://uvs.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://beb.yongpay.top

[U99] JS：事件监听
来源：http://aws.guannengcc.top

el.addEventListener("click", e => {})
来源：http://ybs.yfazqb.com

[U100] JS：DOM 查询
来源：http://mhy.mhx1999.top

document.querySelector(".item")
来源：http://bqd.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://zxm.epnwcf.com

el.classList.toggle("active")
来源：http://jfw.ydzc1.top

[U102] JS：本地存储
来源：http://tpw.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rjk.tanke756.top

[U103] JS：定时器
来源：http://gnc.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zce.wangshuangyany.cn

[U104] JS：防抖
来源：http://ykd.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mew.pycfn.com

[U105] JS：节流
来源：http://biw.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lax.fehbvm.com

[U106] JS：日期格式化
来源：http://qmv.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qiw.fktsv.cn

[U107] JS：数字千分位
来源：http://huv.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xxt.wangshuangyany.cn

[U108] JS：随机整数
来源：http://fck.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uiy.sweek.top

[U109] JS：数组分组
来源：http://rab.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://evt.daria6918.cn

[U110] JS：数组分块
来源：http://bec.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aaz.fktsv.cn

[U111] JS：对象转 Map
来源：http://mrp.0kj1m.cn

new Map(Object.entries(obj))
来源：http://app.hnxiangtu.top

[U112] JS：字符串补位
来源：http://xse.bbcook.cn

"7".padStart(3, "0")
来源：http://cym.ctjpmb.com

[U113] JS：正则替换全部
来源：http://juk.xylfe.cn

s.replaceAll("a", "b")
来源：http://rcn.tian-w.cn

[U114] JS：JSON 深比较
来源：http://wpy.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qgp.nwbrower.top

[U115] JS：生成 UUID
来源：http://aqh.jinqigufen.top

crypto.randomUUID()
来源：http://wis.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://kwx.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://tqk.cqqwz.cn

[U117] JS：单元测试
来源：http://imo.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://yqk.cucudq.cn

[U118] JS：开发服务器
来源：http://ojg.xylfe.cn

npm i -D vite;  npx vite
来源：http://qid.xuanzx.com

[U119] JS：生产构建
来源：http://wwi.iojbl.cn

npx vite build
来源：http://hxd.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://cng.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://tue.fktsv.cn

================================================================================
来源：http://kgb.guowangkeji.top

统计汇总
来源：http://iws.xziqi.cn

================================================================================
来源：http://fug.jqgufenzy.top

按语言统计（条）：
来源：http://oir.mhx1999.top

Python ......... 252
来源：http://ysn.svipenyu.cn

PHP ............ 252
来源：http://olo.bjfxy.top

JavaScript ..... 252
来源：http://zkr.snrcjt.cn

TypeScript ..... 212
来源：http://kyt.fzhhl.top

Java ........... 212
来源：http://toz.9152youxi.cn

Go ............. 212
来源：http://jgt.feifeiyinyue.top

Ruby ........... 212
来源：http://lpm.xylfe.cn

C# ............. 212
来源：http://avh.dianchejie.cn

C .............. 30
来源：http://ggl.sjlbkw.cn

C++ ............ 30
来源：http://lpq.sxryk.cn

SQL ............ 90
来源：http://gmf.havefunace.top

Bash ........... 80
来源：http://qau.wangshuangyany.cn

Kotlin ......... 15
来源：http://fcb.hammf.cn

Swift .......... 15
来源：http://tzr.jlsjyb.cn

Lua ............ 10
来源：http://zfq.c1oappe.top

Perl ........... 10
来源：http://xuh.cheryme.top

Scala .......... 10
来源：http://wyw.yvedp.cn

------------------------------------
来源：http://rot.redwolf501.top

合计 ........... 2106 条
来源：http://tgb.guannengcc.top

按章节统计：
来源：http://jln.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ccw.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zhk.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kmw.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sse.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mwq.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aqx.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xna.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://khp.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://htt.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://izr.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qdf.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bbl.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://otc.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gou.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://evg.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zuw.tarul.cn

Q SQL 专题                              90
来源：http://zin.zhongyouzk.top

R Bash 专题                             80
来源：http://faj.ppjwa.cn

S C / C++ 专题                          60
来源：http://kdx.hnqzz.top

T 其他语言补充                          60
来源：http://mzx.yonumen.top

U 高频实用片段                         120
来源：http://ocs.yfazqb.com

------------------------------------
来源：http://fqz.jinghuilouyu.cn

合计                                  2106 条
来源：http://lxa.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://blk.fanxiaobao.xyz

使用提醒
来源：http://sht.andypj.xyz

--------------------------------------------------------------------------------
来源：http://skg.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ynz.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vwy.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lwm.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bay.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mpm.hnxiangtu.top

—— 文件结束 ——
来源：http://qym.zhoulong.xyz

================================================================================
来源：http://mdo.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://ucu.xylfe.cn

Common Programming Examples Cheat Book
来源：http://jje.epnwcf.com

================================================================================
来源：http://oku.ydzc1.top

【收录内容】
来源：http://crz.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jgk.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kqf.yueranfly.top

SQL · Bash · C · C++
来源：http://jvf.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wwl.jinqigufen.top

【使用说明】
来源：http://vfq.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://enf.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://neo.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://isk.ybcxt.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jvp.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rqe.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sir.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ena.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yxd.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lbn.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jwq.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bpq.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hok.birdmap.top

【文件统计】
来源：http://kqq.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fwf.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://flk.chenjidiqi.icu

目  录
来源：http://mhi.tian-w.cn

--------------------------------------------------------------------------------
来源：http://dgg.hammf.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wvc.ppjwa.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://faj.xziqi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jkf.ctjpmb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lun.hcnkem.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://req.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ckz.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yaq.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kom.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://adt.chenzaomai.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mgw.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qnp.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jtb.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fpn.xuetiantiany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xqj.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kkb.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zyp.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qsc.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hud.hnxiangtu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jvb.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://auz.wangshuangyany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gxt.zhongyouzk.top

================================================================================
来源：http://zyt.chenjidiqi.icu

A. 基础语法与类型
来源：http://qwb.cdnleiting.top

================================================================================
来源：http://rwi.yj20258888.top

[A01] Hello World
来源：http://uuj.xuanzx.com

Py:   print("Hello, World!")
来源：http://ice.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://rsp.0kj1m.cn

JS:   console.log("Hello, World!");
来源：http://hqy.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oxw.jinghuilouyu.cn

Java: System.out.println("Hello, World!");
来源：http://jok.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://lsp.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://xpm.aizwys.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nxr.fktsv.cn

[A02] 变量声明与赋值
来源：http://ypz.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wxk.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vtv.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://wgp.gzhubu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pij.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://hrg.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://qjh.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://vbw.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://pps.9152youxi.cn

[A03] 常量定义
来源：http://ejb.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gcy.cheryme.top

PHP:  const PI = 3.14159;
来源：http://bvt.ppjwa.cn

JS:   const PI = 3.14159;
来源：http://tgt.sweek.top

TS:   const PI: number = 3.14159;
来源：http://agz.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://uuj.chenlongwang.top

Go:   const PI = 3.14159
来源：http://zhg.zdqjudy.top

Ruby: PI = 3.14159
来源：http://zsa.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://tmi.zhiwuduotai.top

[A04] 判断变量类型
来源：http://fxf.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rvx.ctjpmb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://chh.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dxb.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://ihm.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fhj.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ngt.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://eia.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://nvc.zhengqikj.top

[A05] 整数除法与取模
来源：http://vci.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ovy.sxryk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://brw.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://agz.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://apn.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://mev.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://efg.zhiwuduotai.top

Ruby: 7 / 2; 7 % 2
来源：http://crq.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://wrb.ppjwa.cn

[A06] 字符串转数字
来源：http://umc.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://mdn.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fxh.pycfn.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qhs.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://ptp.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tso.shuidangran.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zxz.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://mck.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oli.sjlbkw.cn

[A07] 数字转字符串
来源：http://dla.jinghuilouyu.cn

Py:   str(42)
来源：http://dqr.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://vat.hnxiangtu.top

JS:   String(42); (42).toString()
来源：http://stm.0kj1m.cn

TS:   String(42)
来源：http://ixe.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://off.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://kyd.ydjk.org.cn

Ruby: 42.to_s
来源：http://xkz.fzhhl.top

C#:   42.ToString()
来源：http://hvg.jyoumei.cn

[A08] 取整与四舍五入
来源：http://tvm.shanyushiyangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uzt.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wme.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bxf.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yvb.xziqi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://izr.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wdh.shanyushiyangtech.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tnk.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cwg.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://qxh.jiagoushi.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kmx.jinqigufen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ulk.jianghu66.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rwq.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zwo.hfpthk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ulo.epnwcf.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dmu.fanxiaobao.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uyh.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ncp.hcnkem.com

[A10] 生成随机数
来源：http://xhn.hnqzz.top

Py:   import random; random.randint(1, 100)
来源：http://vyb.hnqzz.top

PHP:  random_int(1, 100);
来源：http://kye.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jch.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://syt.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://utr.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lvs.ehwqpu.com

Ruby: rand(1..100)
来源：http://qzl.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://qbl.sysykeji.top

[A11] 条件表达式（三元）
来源：http://enm.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://ovm.gotoacloud.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ahv.yangfankeji.com

JS:   x > 0 ? "yes" : "no"
来源：http://yol.fzhhl.top

TS:   x > 0 ? "yes" : "no"
来源：http://kti.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://bvw.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cke.cashguo.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bpq.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://umu.nanxuanxn.top

[A12] 字符串插值 / 格式化
来源：http://wpt.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bml.jianghu66.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wxe.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://nxp.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://thx.fehbvm.com

Java: "Hello, %s!".formatted(name)
来源：http://kln.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jgk.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://wkx.ydzc1.top

C#:   $"Hello, {name}!"
来源：http://zlw.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://lsn.xylfe.cn

Py:   "第一行\n第二行"
来源：http://qlt.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://qas.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://tck.tian-w.cn

TS:   "第一行\n第二行"
来源：http://rer.shanyushiyangkeji.top

Java: "第一行\n第二行"
来源：http://tob.daria6918.cn

Go:   "第一行\n第二行"
来源：http://wkd.jinghuilouyu.cn

Ruby: "第一行\n第二行"
来源：http://yna.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://iot.hongshengwenyu.top

[A14] 注释写法
来源：http://jcu.xingfuxueyuan.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://jmn.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kwi.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://pps.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://ctt.yfazqb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ohu.xuanzx.com

Go:   // 单行；/* 多行 */
来源：http://cmo.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://yba.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://qqw.yuanzhike.top

[A15] 空值判断与默认值
来源：http://ske.yj20258888.top

Py:   value = data or "默认值"
来源：http://inx.iojbl.cn

PHP:  $value = $data ?? "默认值";
来源：http://nrz.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://jgv.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://kka.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jgv.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://irw.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://cmx.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://cvd.meibo888.top

[A16] 真假值判断规则
来源：http://kqm.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jss.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dbp.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mvp.chenjidiqi.icu

TS:   if (!x) {}
来源：http://wec.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oxq.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mre.snrcjt.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lra.hysaishi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qtg.yueranfly.top

[A17] 位运算
来源：http://myz.epnwcf.com


<!-- 参考信息 -->