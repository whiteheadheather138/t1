代发 wailian999

[U93] JS：模板字符串
来源：http://hze.mhx1999.top

`共 ${n} 条`
来源：http://zam.tarul.cn

[U94] JS：箭头函数
来源：http://csa.yfazqb.com

const double = x => x * 2;
来源：http://ysx.zhixingplan.top

[U95] JS：Promise 包装
来源：http://ero.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://ray.fktsv.cn

[U96] JS：async/await 与异常
来源：http://ohi.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bus.fktsv.cn

[U97] JS：并发请求
来源：http://unu.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ezt.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://gpc.tanke756.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lwy.ctjpmb.com

[U99] JS：事件监听
来源：http://jzv.daxiang520.top

el.addEventListener("click", e => {})
来源：http://qfv.yonumen.top

[U100] JS：DOM 查询
来源：http://smb.daxiang520.top

document.querySelector(".item")
来源：http://chu.epnwcf.com

[U101] JS：classList 操作
来源：http://pum.yvedp.cn

el.classList.toggle("active")
来源：http://eze.zhengqikj.top

[U102] JS：本地存储
来源：http://zne.wangshuangyany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pho.gzhubu.top

[U103] JS：定时器
来源：http://teo.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mse.nanxinkj.top

[U104] JS：防抖
来源：http://vsg.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rxw.shzxlz.cn

[U105] JS：节流
来源：http://oax.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rda.yonumen.top

[U106] JS：日期格式化
来源：http://ecs.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ity.gotoacloud.top

[U107] JS：数字千分位
来源：http://vyh.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nyz.guannengcc.top

[U108] JS：随机整数
来源：http://vqz.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dyz.yj20258.top

[U109] JS：数组分组
来源：http://nup.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://gef.hnxiangtu.top

[U110] JS：数组分块
来源：http://zdk.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gkq.ydzc1.top

[U111] JS：对象转 Map
来源：http://bww.andypj.xyz

new Map(Object.entries(obj))
来源：http://trx.chenzaomai.com

[U112] JS：字符串补位
来源：http://baq.birdmap.top

"7".padStart(3, "0")
来源：http://ehy.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://zyw.sxryk.cn

s.replaceAll("a", "b")
来源：http://ecl.sysykeji.top

[U114] JS：JSON 深比较
来源：http://tmw.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fsg.shzxlz.cn

[U115] JS：生成 UUID
来源：http://uni.meibo888.top

crypto.randomUUID()
来源：http://bmd.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://lwj.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://gjr.cheryme.top

[U117] JS：单元测试
来源：http://toe.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://enb.andypj.xyz

[U118] JS：开发服务器
来源：http://zsd.yfazqb.com

npm i -D vite;  npx vite
来源：http://dej.hammf.cn

[U119] JS：生产构建
来源：http://tal.jlsjyb.cn

npx vite build
来源：http://oao.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://iyv.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://gqn.zhongyouzk.top

================================================================================
来源：http://kgz.dianchejie.cn

统计汇总
来源：http://vmm.9152youxi.cn

================================================================================
来源：http://zbe.ybcxt.top

按语言统计（条）：
来源：http://egc.ybcxt.top

Python ......... 252
来源：http://bmu.xuetiantiany.cn

PHP ............ 252
来源：http://jgm.yangfankeji.com

JavaScript ..... 252
来源：http://bxv.hcnkem.com

TypeScript ..... 212
来源：http://zeh.yangfankeji.com

Java ........... 212
来源：http://nuk.jinghuilouyu.cn

Go ............. 212
来源：http://twq.hywenlv.cn

Ruby ........... 212
来源：http://kyo.pycfn.com

C# ............. 212
来源：http://mey.daria6918.cn

C .............. 30
来源：http://dwk.jianghu66.top

C++ ............ 30
来源：http://zxs.jqgfzy.top

SQL ............ 90
来源：http://atv.cdnleiting.top

Bash ........... 80
来源：http://yzi.chenlongwang.top

Kotlin ......... 15
来源：http://geq.ehwqpu.com

Swift .......... 15
来源：http://kus.yueranfly.top

Lua ............ 10
来源：http://nmz.cashguo.top

Perl ........... 10
来源：http://wvd.zhoulong.xyz

Scala .......... 10
来源：http://zxn.mhx1999.top

------------------------------------
来源：http://hzl.chenzaomai.com

合计 ........... 2106 条
来源：http://umt.feifeiyinyue.top

按章节统计：
来源：http://quq.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tls.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xpg.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bbk.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ogs.ydjk.org.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tfq.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ozj.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fsv.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zay.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://abz.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hsg.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vdb.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gnu.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wdy.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vmf.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ojw.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eqv.cdnleiting.top

Q SQL 专题                              90
来源：http://aen.zhongyouzk.top

R Bash 专题                             80
来源：http://aea.yongpay.top

S C / C++ 专题                          60
来源：http://ami.cheryme.top

T 其他语言补充                          60
来源：http://fhe.chenzaomai.com

U 高频实用片段                         120
来源：http://frh.jinqigfzy.top

------------------------------------
来源：http://isu.quarkkingdee.top

合计                                  2106 条
来源：http://kzp.cashguo.top

--------------------------------------------------------------------------------
来源：http://fvd.redwolf501.top

使用提醒
来源：http://lkq.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://lid.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tbn.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vyv.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cug.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oov.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oqh.gaohongyu789.top

—— 文件结束 ——
来源：http://xwz.jqgufenzy.top

================================================================================
来源：http://dej.jinyuanbaomall.cn

程序语言常见例子速查手册（2024 版）
来源：http://pvh.ehwqpu.com

Common Programming Examples Cheat Book
来源：http://gvv.quarkkingdee.top

================================================================================
来源：http://kyg.chenzaomai.com

【收录内容】
来源：http://ofv.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ntp.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bvw.mhx1999.top

SQL · Bash · C · C++
来源：http://zkf.wangdashe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://thn.daxiang520.top

【使用说明】
来源：http://bna.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qnl.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xxm.0kj1m.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qub.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cib.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://btv.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qjq.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kxe.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jkp.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nxg.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xqm.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gvc.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lha.yangfankeji.com

【文件统计】
来源：http://lux.jyoumei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://glv.hnqzz.top

--------------------------------------------------------------------------------
来源：http://nar.fzhhl.top

目  录
来源：http://rvv.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://muj.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vge.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ilt.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://klr.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sxf.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zva.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ygw.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://axt.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hwb.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://clc.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xiw.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hnb.yanxiufei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yma.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://obf.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iyq.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jem.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jvo.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ksc.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://otm.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wwt.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ppk.fengsongda.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hdm.zhixingplan.top

================================================================================
来源：http://cmz.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://njm.fengsongda.top

================================================================================
来源：http://vqe.yj20258.top

[A01] Hello World
来源：http://gks.fehbvm.com

Py:   print("Hello, World!")
来源：http://cxl.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://jap.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://nki.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://egv.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://zau.zhaomingkeji.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ssl.yj202588.top

Ruby: puts "Hello, World!"
来源：http://jhm.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vag.hnqzz.top

[A02] 变量声明与赋值
来源：http://kjn.yuxming.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uay.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uoh.jqgfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://hpb.ctjpmb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yqw.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://oll.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://sds.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://iui.mhx1999.top

C#:   string name = "Alex"; int age = 20;
来源：http://npt.jinghuilouyu.cn

[A03] 常量定义
来源：http://tnj.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wwp.xylfe.cn

PHP:  const PI = 3.14159;
来源：http://zev.bjfxy.top

JS:   const PI = 3.14159;
来源：http://kqd.guannengcc.top

TS:   const PI: number = 3.14159;
来源：http://vnx.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://zej.hnqzz.top

Go:   const PI = 3.14159
来源：http://iip.andypj.xyz

Ruby: PI = 3.14159
来源：http://ewo.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://jmb.cdnleiting.top

[A04] 判断变量类型
来源：http://umj.daria6918.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bqg.fehbvm.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dni.jinqigfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://teo.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://oee.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ccf.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://bcz.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wgj.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://ygr.hnxiangtu.top

[A05] 整数除法与取模
来源：http://wgw.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wum.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qvw.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bsr.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://agk.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://vfh.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://zna.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://sbk.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://xxx.hammf.cn

[A06] 字符串转数字
来源：http://qio.jlsjyb.cn

Py:   int("42"); float("3.14")
来源：http://ayz.yongpay.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lus.guannengcc.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ykh.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://hbr.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ftk.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://shs.chenjidiqi.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://evh.fehbvm.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mft.shuidangran.top

[A07] 数字转字符串
来源：http://akb.tianlin.xyz

Py:   str(42)
来源：http://xwx.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://ftd.mhx1999.top

JS:   String(42); (42).toString()
来源：http://qhj.dashuyun.cn

TS:   String(42)
来源：http://cjk.shzxlz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://exc.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://yrq.fzhhl.top

Ruby: 42.to_s
来源：http://fvp.tarul.cn

C#:   42.ToString()
来源：http://ghg.fanxiaobao.xyz

[A08] 取整与四舍五入
来源：http://ovg.svipenyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hec.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bbn.mhx1999.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rjs.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hop.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dap.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oqi.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dvk.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rbj.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://oyx.316326.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xhd.xuetiantiany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ahj.jianghu66.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vrc.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yxl.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rda.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kik.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cpw.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vwj.jinqigfzy.top

[A10] 生成随机数
来源：http://onb.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://nkb.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://gwt.xziqi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nkc.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://shp.mhx1999.top

Java: new Random().nextInt(100) + 1
来源：http://wrw.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dzw.zycfv.cn

Ruby: rand(1..100)
来源：http://ngy.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://iaf.hnqzz.top

[A11] 条件表达式（三元）
来源：http://sbt.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://oxi.zdbjq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tvl.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://ujo.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uvz.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://rne.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mhj.yanxiufei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qrq.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://xln.guowangkeji.top

[A12] 字符串插值 / 格式化
来源：http://per.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lwh.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tjb.tianlin.xyz

JS:   `Hello, ${name}!`
来源：http://zwi.yonumen.top

TS:   `Hello, ${name}!`
来源：http://sup.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://hlr.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ael.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://wxf.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://zyg.kuanghao11.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://psr.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://vcv.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://upy.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://yye.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://avv.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://jpd.zycfv.cn

Go:   "第一行\n第二行"
来源：http://vgc.yongpay.top

Ruby: "第一行\n第二行"
来源：http://lno.cashguo.top

C#:   "第一行\n第二行"
来源：http://ots.xuanzx.com

[A14] 注释写法
来源：http://jsx.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fcy.svipenyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jip.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://hsf.daria6918.cn

TS:   // 单行；/* 多行 */
来源：http://zmt.vqdsnc.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pzi.bjfxy.top

Go:   // 单行；/* 多行 */
来源：http://rrd.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yvd.kuanghao11.cn

C#:   // 单行；/* 多行 */
来源：http://dav.jyoumei.cn

[A15] 空值判断与默认值
来源：http://riz.shuidangran.top

Py:   value = data or "默认值"
来源：http://qsc.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://yis.xuetiantiany.cn

JS:   const value = data ?? "默认值";
来源：http://qie.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://igp.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rqh.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://ktv.hnqzz.top

Ruby: value = data || "默认值"
来源：http://oxq.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://qjk.jyoumei.cn

[A16] 真假值判断规则
来源：http://gsh.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://snt.zdbjq.cn


<!-- 参考信息 -->