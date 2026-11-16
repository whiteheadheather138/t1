代发 wailian999

[U91] JS：对象键值遍历
来源：http://eaq.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yit.ppjwa.cn

[U92] JS：深拷贝
来源：http://sau.xylfe.cn

structuredClone(obj)
来源：http://qfn.ybcxt.top

[U93] JS：模板字符串
来源：http://wci.vehdjk.com

`共 ${n} 条`
来源：http://bqj.daria6918.cn

[U94] JS：箭头函数
来源：http://owc.jinghuilouyu.cn

const double = x => x * 2;
来源：http://mkp.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://cbq.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://hfl.jianghu66.top

[U96] JS：async/await 与异常
来源：http://ujc.zdqjudy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hdb.gaohongyu789.top

[U97] JS：并发请求
来源：http://nku.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hsc.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://olq.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hcg.ivvv.top

[U99] JS：事件监听
来源：http://txj.daria6918.cn

el.addEventListener("click", e => {})
来源：http://fxf.jianghu66.top

[U100] JS：DOM 查询
来源：http://xef.fehbvm.com

document.querySelector(".item")
来源：http://cdp.uphjek.com

[U101] JS：classList 操作
来源：http://meh.jinqigufen.top

el.classList.toggle("active")
来源：http://zqx.ppjwa.cn

[U102] JS：本地存储
来源：http://iul.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bgd.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://eeq.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ius.nanxuanxn.top

[U104] JS：防抖
来源：http://ide.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jus.jinyuanbaomall.cn

[U105] JS：节流
来源：http://kyw.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ntq.svipenyu.cn

[U106] JS：日期格式化
来源：http://atk.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tui.yanxiufei.cn

[U107] JS：数字千分位
来源：http://iif.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cfj.jyoumei.cn

[U108] JS：随机整数
来源：http://lmi.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fpv.havefunace.top

[U109] JS：数组分组
来源：http://rjb.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://wlz.9152youxi.cn

[U110] JS：数组分块
来源：http://syl.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wjk.nanxinkj.top

[U111] JS：对象转 Map
来源：http://inb.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://etk.pycfn.com

[U112] JS：字符串补位
来源：http://fgr.jianghu66.top

"7".padStart(3, "0")
来源：http://rqt.ppjwa.cn

[U113] JS：正则替换全部
来源：http://uub.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://uzb.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://cur.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tmd.yvedp.cn

[U115] JS：生成 UUID
来源：http://awc.ybcxt.top

crypto.randomUUID()
来源：http://dyx.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://vwf.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://kti.hongshengwenyu.top

[U117] JS：单元测试
来源：http://trc.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://dwh.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://noa.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://har.shuidangran.top

[U119] JS：生产构建
来源：http://bro.ivvv.top

npx vite build
来源：http://zev.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://krs.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://noi.cucudq.cn

================================================================================
来源：http://blt.hfpthk.cn

统计汇总
来源：http://vih.jqgufenzy.top

================================================================================
来源：http://ihu.yuanzhike.top

按语言统计（条）：
来源：http://vqo.hongshengwenyu.top

Python ......... 252
来源：http://nsa.yanxiufei.cn

PHP ............ 252
来源：http://cvf.dashuyun.cn

JavaScript ..... 252
来源：http://wqn.zhixingplan.top

TypeScript ..... 212
来源：http://mdr.jiagoushi.top

Java ........... 212
来源：http://wms.yuanzhike.top

Go ............. 212
来源：http://ebq.52xcode.cn

Ruby ........... 212
来源：http://vim.c1oappe.top

C# ............. 212
来源：http://nfd.smart0.xyz

C .............. 30
来源：http://dek.tarul.cn

C++ ............ 30
来源：http://xru.gotoacloud.top

SQL ............ 90
来源：http://ctl.jinqigfzy.top

Bash ........... 80
来源：http://fmv.gotoacloud.top

Kotlin ......... 15
来源：http://yga.zhaomingkeji.xyz

Swift .......... 15
来源：http://spg.sxryk.cn

Lua ............ 10
来源：http://kxm.snrcjt.cn

Perl ........... 10
来源：http://ycg.ppjwa.cn

Scala .......... 10
来源：http://oaz.gotoacloud.top

------------------------------------
来源：http://ayt.hnqzz.top

合计 ........... 2106 条
来源：http://xqo.dashuyun.cn

按章节统计：
来源：http://anl.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ylf.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ueo.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://muj.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vjv.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://auy.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gyt.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xxp.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddb.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://loc.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iyz.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jve.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rkk.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hti.zdqjudy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://omw.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qtd.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://odz.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://unz.ybcxt.top

R Bash 专题                             80
来源：http://irx.quarkkingdee.top

S C / C++ 专题                          60
来源：http://vej.hammf.cn

T 其他语言补充                          60
来源：http://xuf.sjlbkw.cn

U 高频实用片段                         120
来源：http://zbk.bbcook.cn

------------------------------------
来源：http://bva.jiagoushi.top

合计                                  2106 条
来源：http://wox.zycfv.cn

--------------------------------------------------------------------------------
来源：http://jqd.guannengcc.top

使用提醒
来源：http://xkj.hesvh.cn

--------------------------------------------------------------------------------
来源：http://ikd.jinqigfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ezx.jiagoushi.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qqh.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ogj.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mvi.guowangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mdr.svipenyu.cn

—— 文件结束 ——
来源：http://bdp.jinqigufen.top

================================================================================
来源：http://uoc.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://zlk.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://ggj.zhijiandao.cn

================================================================================
来源：http://gox.jyoumei.cn

【收录内容】
来源：http://yvx.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ayc.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ohl.ivvv.top

SQL · Bash · C · C++
来源：http://xhc.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://byf.redwolf501.top

【使用说明】
来源：http://rdr.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jmr.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pba.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oow.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pzu.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://hea.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qoq.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://spk.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://was.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uay.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qfs.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rlw.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mfh.xziqi.cn

【文件统计】
来源：http://xuv.jlsjyb.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lcm.c1oappe.top

--------------------------------------------------------------------------------
来源：http://nxl.xuanzx.com

目  录
来源：http://gda.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://bgz.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://klg.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ylk.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://snd.aizwys.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qar.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ffz.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rub.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mmi.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rie.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aaf.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://clk.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://trs.0kj1m.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vvy.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://out.guowangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zql.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xxn.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dos.svipenyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xwq.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://noc.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pwr.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sdd.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vmg.jiagoushi.top

================================================================================
来源：http://lnh.ehwqpu.com

A. 基础语法与类型
来源：http://pcl.shanyushiyangtech.top

================================================================================
来源：http://agr.tanke756.top

[A01] Hello World
来源：http://qxg.yj202588.top

Py:   print("Hello, World!")
来源：http://xma.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://okq.jianghu66.top

JS:   console.log("Hello, World!");
来源：http://wni.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ato.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://clj.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://mdo.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://gyv.0kj1m.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yhf.haohaochexian.top

[A02] 变量声明与赋值
来源：http://xrk.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oam.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qiy.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dgw.nanxuanxn.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uje.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://lqg.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://vth.zhixingplan.top

Ruby: name = "Alex"; age = 20
来源：http://pci.hnqzz.top

C#:   string name = "Alex"; int age = 20;
来源：http://mkx.epnwcf.com

[A03] 常量定义
来源：http://jsf.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pmw.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://lqb.meibo888.top

JS:   const PI = 3.14159;
来源：http://qtp.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://ajv.cashguo.top

Java: static final double PI = 3.14159;
来源：http://lrh.kuanghao11.cn

Go:   const PI = 3.14159
来源：http://naz.xinyue.icu

Ruby: PI = 3.14159
来源：http://ewk.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://pgc.hnxiangtu.top

[A04] 判断变量类型
来源：http://jcp.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ayy.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kni.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gey.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://dai.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zxt.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eob.nanxinkj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pbb.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://eja.jyoumei.cn

[A05] 整数除法与取模
来源：http://klg.yanxiufei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bog.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://evf.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cwy.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ivi.wangshuangyany.cn

Java: 7 / 2; 7 % 2
来源：http://pyf.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://guw.xinyue.icu

Ruby: 7 / 2; 7 % 2
来源：http://ekp.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://gwq.iojbl.cn

[A06] 字符串转数字
来源：http://bje.yj202588.top

Py:   int("42"); float("3.14")
来源：http://duo.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://isp.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vtb.ydjk.org.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sxk.9152youxi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zfj.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zek.yuanzhike.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pqd.ctjpmb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qqw.sufxvd.cn

[A07] 数字转字符串
来源：http://qar.birdmap.top

Py:   str(42)
来源：http://kxr.jlsjyb.cn

PHP:  (string) 42; strval(42)
来源：http://wxn.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://ezx.316326.xyz

TS:   String(42)
来源：http://hqo.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yiv.hysaishi.cn

Go:   strconv.Itoa(42)
来源：http://jki.tian-w.cn

Ruby: 42.to_s
来源：http://ubg.andypj.xyz

C#:   42.ToString()
来源：http://vko.guannengcc.top

[A08] 取整与四舍五入
来源：http://mia.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yzv.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zhq.zhoulong.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dhx.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ugz.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vgm.52xcode.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ski.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cwa.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ggq.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://dsu.c1oappe.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cup.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qcc.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wtq.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iij.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wfz.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yrd.tanke756.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xet.fzhhl.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kvd.kuanghao11.cn

[A10] 生成随机数
来源：http://jzy.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://hch.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://jwg.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mul.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vrx.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://exl.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pmn.chenzaomai.com

Ruby: rand(1..100)
来源：http://duf.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://jgs.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://aiq.cheryme.top

Py:   "yes" if x > 0 else "no"
来源：http://fyy.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://tgd.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iiw.hongshengwenyu.top

TS:   x > 0 ? "yes" : "no"
来源：http://pzv.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://luo.pengpengdd.cyou

Go:   // 无三元运算符，需用 if 语句
来源：http://fpn.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yqg.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://jcm.fengsongda.top

[A12] 字符串插值 / 格式化
来源：http://gex.feifeiyinyue.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ylt.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://brn.jyoumei.cn

JS:   `Hello, ${name}!`
来源：http://iol.cucudq.cn

TS:   `Hello, ${name}!`
来源：http://suj.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://hzb.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ivj.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://opk.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://tga.yvedp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://npg.316326.xyz

Py:   "第一行\n第二行"
来源：http://vmk.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://pbu.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://imo.shanyushiyangtech.top

TS:   "第一行\n第二行"
来源：http://obx.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://kzw.cucudq.cn

Go:   "第一行\n第二行"
来源：http://yef.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://cgl.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://cpq.smart0.xyz

[A14] 注释写法
来源：http://gya.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nut.uphjek.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://nhr.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://nck.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://jke.shanyushiyangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fdd.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://cro.ppjwa.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dgj.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://caz.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://kmj.ppjwa.cn

Py:   value = data or "默认值"
来源：http://xgx.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://kih.snrcjt.cn

JS:   const value = data ?? "默认值";
来源：http://vgj.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://tgi.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xxd.jlsjyb.cn

Go:   if data == "" { data = "默认值" }
来源：http://xfp.yonumen.top


<!-- 参考信息 -->