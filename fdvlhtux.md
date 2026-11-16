代发 wailian999

[U91] JS：对象键值遍历
来源：http://fqf.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kmw.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://ala.shanyushiyangtech.top

structuredClone(obj)
来源：http://ksc.zhoulong.xyz

[U93] JS：模板字符串
来源：http://ybs.jqgfzy.top

`共 ${n} 条`
来源：http://bzv.svipenyu.cn

[U94] JS：箭头函数
来源：http://zjn.jianghu66.top

const double = x => x * 2;
来源：http://pjy.zdbjq.cn

[U95] JS：Promise 包装
来源：http://wum.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://esk.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://bbe.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eyv.gzhubu.top

[U97] JS：并发请求
来源：http://vvd.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bkv.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://wmx.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://afi.zycfv.cn

[U99] JS：事件监听
来源：http://hju.cheryme.top

el.addEventListener("click", e => {})
来源：http://dgc.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://khz.hnqzz.top

document.querySelector(".item")
来源：http://qlb.gogol.net.cn

[U101] JS：classList 操作
来源：http://hhb.pengpengdd.cyou

el.classList.toggle("active")
来源：http://bgl.vqdsnc.cn

[U102] JS：本地存储
来源：http://xpp.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xuu.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://ofo.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qpz.ehwqpu.com

[U104] JS：防抖
来源：http://acv.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybg.sxryk.cn

[U105] JS：节流
来源：http://dzt.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eam.daria6918.cn

[U106] JS：日期格式化
来源：http://ylo.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qqd.xziqi.cn

[U107] JS：数字千分位
来源：http://tam.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ljp.fzhhl.top

[U108] JS：随机整数
来源：http://rch.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rxv.9152youxi.cn

[U109] JS：数组分组
来源：http://ido.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://hap.quarkkingdee.top

[U110] JS：数组分块
来源：http://qmo.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bbl.meibo888.top

[U111] JS：对象转 Map
来源：http://qra.birdmap.top

new Map(Object.entries(obj))
来源：http://bxb.yuxming.cn

[U112] JS：字符串补位
来源：http://cpv.smart0.xyz

"7".padStart(3, "0")
来源：http://doh.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://pyg.nanxuanxn.top

s.replaceAll("a", "b")
来源：http://snb.shuidangran.top

[U114] JS：JSON 深比较
来源：http://wes.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lxi.fzhhl.top

[U115] JS：生成 UUID
来源：http://jxv.zhengqikj.top

crypto.randomUUID()
来源：http://yuj.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://yhr.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://nmj.bjfxy.top

[U117] JS：单元测试
来源：http://ldw.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://rnt.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://puc.tianlin.xyz

npm i -D vite;  npx vite
来源：http://khw.gzhubu.top

[U119] JS：生产构建
来源：http://obo.cucudq.cn

npx vite build
来源：http://qia.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://pai.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://xeq.gzhubu.top

================================================================================
来源：http://ohv.sysykeji.top

统计汇总
来源：http://ylh.yueranfly.top

================================================================================
来源：http://jue.andypj.xyz

按语言统计（条）：
来源：http://upf.uphjek.com

Python ......... 252
来源：http://wyl.fanxiaobao.xyz

PHP ............ 252
来源：http://zkb.pengpengdd.cyou

JavaScript ..... 252
来源：http://erk.jyoumei.cn

TypeScript ..... 212
来源：http://cjy.wangdashe.top

Java ........... 212
来源：http://syv.haohaochexian.top

Go ............. 212
来源：http://bpj.yuanzhike.top

Ruby ........... 212
来源：http://uzu.epnwcf.com

C# ............. 212
来源：http://sdd.ydjk.org.cn

C .............. 30
来源：http://ekw.cqqwz.cn

C++ ............ 30
来源：http://mqa.yj20258.top

SQL ............ 90
来源：http://euo.nanxuanxn.top

Bash ........... 80
来源：http://zyu.uphjek.com

Kotlin ......... 15
来源：http://ntq.shuidangran.top

Swift .......... 15
来源：http://wjb.tarul.cn

Lua ............ 10
来源：http://vuy.yj20258888.top

Perl ........... 10
来源：http://mxl.0kj1m.cn

Scala .......... 10
来源：http://gwy.jqgfzy.top

------------------------------------
来源：http://slg.yongpay.top

合计 ........... 2106 条
来源：http://amg.ehwqpu.com

按章节统计：
来源：http://psa.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xwn.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ugk.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aem.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jdi.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://woc.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bcc.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yfb.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nei.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://owa.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ues.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gkq.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://smp.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kzq.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uut.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sqx.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mid.daria6918.cn

Q SQL 专题                              90
来源：http://bef.yueranfly.top

R Bash 专题                             80
来源：http://cfa.jiagoushi.top

S C / C++ 专题                          60
来源：http://xpo.epnwcf.com

T 其他语言补充                          60
来源：http://nml.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://uxv.bbcook.cn

------------------------------------
来源：http://hfp.redwolf501.top

合计                                  2106 条
来源：http://uxg.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://aco.hongshengwenyu.top

使用提醒
来源：http://dfg.daxiang520.top

--------------------------------------------------------------------------------
来源：http://yip.dianchejie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nly.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkb.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://azq.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://klf.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ozq.zhoulong.xyz

—— 文件结束 ——
来源：http://ywn.pengpengdd.cyou

================================================================================
来源：http://msc.fehbvm.com

程序语言常见例子速查手册（2024 版）
来源：http://ayh.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://akj.yongpay.top

================================================================================
来源：http://jbj.sxryk.cn

【收录内容】
来源：http://inx.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://tfa.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://chw.0kj1m.cn

SQL · Bash · C · C++
来源：http://ptq.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://upc.zdbjq.cn

【使用说明】
来源：http://qqv.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://spd.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bro.chenzaomai.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gxf.0kj1m.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://syw.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rhf.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://azj.chenzaomai.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cdq.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yzu.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xir.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jpb.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://woe.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zij.zhongyouzk.top

【文件统计】
来源：http://tww.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ekj.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://rwq.chenlongwang.top

目  录
来源：http://mef.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://mna.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lbt.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gkf.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zpu.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ood.cdnleiting.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://unj.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://irf.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wtl.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ybo.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://smk.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cpp.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://apc.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jnh.shuidangran.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xph.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pyi.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bsc.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wei.zhijiandao.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qez.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bur.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vgs.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://knb.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yhx.yonumen.top

================================================================================
来源：http://rpl.nanxinkj.top

A. 基础语法与类型
来源：http://ens.bjfxy.top

================================================================================
来源：http://zit.iojbl.cn

[A01] Hello World
来源：http://mrz.yongpay.top

Py:   print("Hello, World!")
来源：http://voj.yanxiufei.cn

PHP:  echo "Hello, World!";
来源：http://fsd.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://nwe.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cnb.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://wbf.zhaomingkeji.xyz

Go:   fmt.Println("Hello, World!")
来源：http://tbh.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://zcd.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hvq.snrcjt.cn

[A02] 变量声明与赋值
来源：http://tca.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lmo.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lzk.sufxvd.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bhg.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wee.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://zne.ybcxt.top

Go:   name := "Alex"; age := 20
来源：http://jun.cheryme.top

Ruby: name = "Alex"; age = 20
来源：http://uqq.jinghuilouyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hdz.zhixingplan.top

[A03] 常量定义
来源：http://fxj.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://chd.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://tgd.hammf.cn

JS:   const PI = 3.14159;
来源：http://vgx.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://ybl.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://dnw.wangshuangyany.cn

Go:   const PI = 3.14159
来源：http://kkl.nwbrower.top

Ruby: PI = 3.14159
来源：http://uxa.tanke756.top

C#:   const double PI = 3.14159;
来源：http://uix.yongpay.top

[A04] 判断变量类型
来源：http://zvf.gzhubu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://drp.chenjidiqi.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fwm.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ttx.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://qpp.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rww.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://krk.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ixn.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://pjy.cdnleiting.top

[A05] 整数除法与取模
来源：http://bei.hnxiangtu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://adn.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://qgr.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yrt.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qpn.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://bju.nwbrower.top

Go:   7 / 2; 7 % 2
来源：http://rya.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://kck.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://whr.gaohongyu789.top

[A06] 字符串转数字
来源：http://hvc.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://utw.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ecv.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ylt.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://tuw.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ueg.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fny.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jwx.mhx1999.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eac.smart0.xyz

[A07] 数字转字符串
来源：http://xgf.yuanzhike.top

Py:   str(42)
来源：http://bxy.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://ozi.guannengcc.top

JS:   String(42); (42).toString()
来源：http://vor.cucudq.cn

TS:   String(42)
来源：http://nxu.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://psz.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://plo.yj20258.top

Ruby: 42.to_s
来源：http://glb.chenzaomai.com

C#:   42.ToString()
来源：http://btu.bbcook.cn

[A08] 取整与四舍五入
来源：http://npu.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hwn.xinyue.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wfp.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ldh.iojbl.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pxa.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jgi.jqgfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ppi.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://kel.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://azi.bjfxy.top

[A09] 绝对值与最大最小值
来源：http://ewc.yj20258888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xfm.smart0.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qrm.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wyr.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yoo.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oqe.zhengqikj.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jvg.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jew.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tfk.jyoumei.cn

[A10] 生成随机数
来源：http://sik.yuanzhike.top

Py:   import random; random.randint(1, 100)
来源：http://zhk.shanyushiyangtech.top

PHP:  random_int(1, 100);
来源：http://quo.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tma.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ngu.yj20258.top

Java: new Random().nextInt(100) + 1
来源：http://buu.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hrd.zhixingplan.top

Ruby: rand(1..100)
来源：http://wbm.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://oci.kuanghao11.cn

[A11] 条件表达式（三元）
来源：http://xap.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://sfl.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://phv.fengsongda.top

JS:   x > 0 ? "yes" : "no"
来源：http://yti.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jun.hysaishi.cn

Java: x > 0 ? "yes" : "no"
来源：http://boy.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xvp.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ztr.sysykeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://fhm.zhongyouzk.top

[A12] 字符串插值 / 格式化
来源：http://mqa.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://frw.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eej.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://csl.mhx1999.top

TS:   `Hello, ${name}!`
来源：http://hcx.sjlbkw.cn

Java: "Hello, %s!".formatted(name)
来源：http://lqe.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://soc.haohaochexian.top

Ruby: "Hello, #{name}!"
来源：http://xlv.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://nli.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pea.uphjek.com

Py:   "第一行\n第二行"
来源：http://rrl.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://ter.cucudq.cn

JS:   "第一行\n第二行"
来源：http://dpz.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://rwn.hongshengwenyu.top

Java: "第一行\n第二行"
来源：http://pnl.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://hxv.shangyingyoupin.top

Ruby: "第一行\n第二行"
来源：http://erb.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://jhc.ppjwa.cn

[A14] 注释写法
来源：http://zjm.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zrf.uphjek.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://iip.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://gzv.shzxlz.cn

TS:   // 单行；/* 多行 */
来源：http://yrk.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://stk.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://tzc.guannengcc.top

Ruby: # 单行；=begin 多行 =end
来源：http://bwe.zhijiandao.cn

C#:   // 单行；/* 多行 */
来源：http://ana.kuanghao11.cn

[A15] 空值判断与默认值
来源：http://ama.snrcjt.cn

Py:   value = data or "默认值"
来源：http://ffu.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://mde.xuanzx.com

JS:   const value = data ?? "默认值";
来源：http://qai.zycfv.cn

TS:   const value = data ?? "默认值";
来源：http://osn.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://knm.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://yia.zdqjudy.top


<!-- 参考信息 -->