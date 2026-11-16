代发 wailian999

[U87] JS：解构默认值
来源：http://taa.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://wky.nwbrower.top

[U88] JS：对象展开合并
来源：http://ffg.meibo888.top

{ ...a, ...b }
来源：http://dlf.yvedp.cn

[U89] JS：数组去重
来源：http://efl.havefunace.top

[...new Set(arr)]
来源：http://cwe.zdqjudy.top

[U90] JS：数字数组排序
来源：http://eik.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://apk.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://yre.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ope.zdbjq.cn

[U92] JS：深拷贝
来源：http://ofl.yvedp.cn

structuredClone(obj)
来源：http://dhr.ctjpmb.com

[U93] JS：模板字符串
来源：http://ekj.hongshengwenyu.top

`共 ${n} 条`
来源：http://yre.fehbvm.com

[U94] JS：箭头函数
来源：http://llb.ctjpmb.com

const double = x => x * 2;
来源：http://csb.shzxlz.cn

[U95] JS：Promise 包装
来源：http://tng.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://xri.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://hrt.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://neh.cheryme.top

[U97] JS：并发请求
来源：http://tqk.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://myu.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://ntg.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tcm.cdnleiting.top

[U99] JS：事件监听
来源：http://wde.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://pgd.aibaodan.cn

[U100] JS：DOM 查询
来源：http://utl.jinqigufen.top

document.querySelector(".item")
来源：http://chm.zdbjq.cn

[U101] JS：classList 操作
来源：http://kaw.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://zfh.aibaodan.cn

[U102] JS：本地存储
来源：http://zrv.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://osp.gaohongyu789.top

[U103] JS：定时器
来源：http://dxf.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://huy.meibo888.top

[U104] JS：防抖
来源：http://gur.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ypx.nanxinkj.top

[U105] JS：节流
来源：http://nfx.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ekh.yongpay.top

[U106] JS：日期格式化
来源：http://pja.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://boc.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://idr.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ldi.hcnkem.com

[U108] JS：随机整数
来源：http://zdu.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oyx.sxryk.cn

[U109] JS：数组分组
来源：http://dfe.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://nld.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://crj.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zav.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://qdb.316326.xyz

new Map(Object.entries(obj))
来源：http://zjv.hywenlv.cn

[U112] JS：字符串补位
来源：http://ohu.jqgufenzy.top

"7".padStart(3, "0")
来源：http://cxp.fehbvm.com

[U113] JS：正则替换全部
来源：http://ntg.yuanzhike.top

s.replaceAll("a", "b")
来源：http://fgs.meibo888.top

[U114] JS：JSON 深比较
来源：http://ydy.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aeh.epnwcf.com

[U115] JS：生成 UUID
来源：http://eko.fehbvm.com

crypto.randomUUID()
来源：http://ano.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://lqq.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://zll.wangshuangyany.cn

[U117] JS：单元测试
来源：http://kry.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://rag.zhoulong.xyz

[U118] JS：开发服务器
来源：http://wjr.yj202588.top

npm i -D vite;  npx vite
来源：http://iod.ctjpmb.com

[U119] JS：生产构建
来源：http://duw.xinyue.icu

npx vite build
来源：http://ytz.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://unf.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://szr.zhoulong.xyz

================================================================================
来源：http://chx.havefunace.top

统计汇总
来源：http://ayn.chenzaomai.com

================================================================================
来源：http://jvd.hongshengwenyu.top

按语言统计（条）：
来源：http://zkh.jyoumei.cn

Python ......... 252
来源：http://icq.andypj.xyz

PHP ............ 252
来源：http://kem.gogol.net.cn

JavaScript ..... 252
来源：http://fwj.sysykeji.top

TypeScript ..... 212
来源：http://fey.ydzc1.top

Java ........... 212
来源：http://dzb.iojbl.cn

Go ............. 212
来源：http://xax.epnwcf.com

Ruby ........... 212
来源：http://axi.ehwqpu.com

C# ............. 212
来源：http://tvh.birdmap.top

C .............. 30
来源：http://jaw.nanxinkj.top

C++ ............ 30
来源：http://hzg.chenzaomai.com

SQL ............ 90
来源：http://wsy.ivvv.top

Bash ........... 80
来源：http://dnf.aizwys.cn

Kotlin ......... 15
来源：http://wmq.jianghu66.top

Swift .......... 15
来源：http://plw.daxiang520.top

Lua ............ 10
来源：http://nno.c1oappe.top

Perl ........... 10
来源：http://swk.mhx1999.top

Scala .......... 10
来源：http://cva.sweek.top

------------------------------------
来源：http://qxx.yanxiufei.cn

合计 ........... 2106 条
来源：http://arf.yanxiufei.cn

按章节统计：
来源：http://qej.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uhx.guannengcc.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pul.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tqt.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gjl.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vvj.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vsq.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lxf.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hzj.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bxn.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dxa.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rvv.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ias.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fql.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pql.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://smu.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nqh.316326.xyz

Q SQL 专题                              90
来源：http://dtw.zycfv.cn

R Bash 专题                             80
来源：http://vce.redwolf501.top

S C / C++ 专题                          60
来源：http://bjg.hesvh.cn

T 其他语言补充                          60
来源：http://msq.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://ptu.daxiang520.top

------------------------------------
来源：http://ucr.hnxiangtu.top

合计                                  2106 条
来源：http://bvt.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://mrn.nwbrower.top

使用提醒
来源：http://rtv.fzhhl.top

--------------------------------------------------------------------------------
来源：http://gnx.yuanzhike.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uoj.wangshuangyany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gjz.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jja.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mve.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zrh.zycfv.cn

—— 文件结束 ——
来源：http://pye.tanke756.top

================================================================================
来源：http://ceh.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://zww.fzhhl.top

Common Programming Examples Cheat Book
来源：http://lrx.guannengcc.top

================================================================================
来源：http://pbm.ivvv.top

【收录内容】
来源：http://xho.chenlongwang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://reh.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://feu.sxryk.cn

SQL · Bash · C · C++
来源：http://nvt.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tye.zdqjudy.top

【使用说明】
来源：http://gte.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hmd.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lfw.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pto.jlsjyb.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xyt.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vcp.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pcd.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jmj.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nlj.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vuy.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uvy.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bga.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rqu.ctjpmb.com

【文件统计】
来源：http://edx.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tlo.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://cni.wangshuangyany.cn

目  录
来源：http://xju.epnwcf.com

--------------------------------------------------------------------------------
来源：http://rav.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dti.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kjc.hfpthk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mou.hysaishi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hpx.redwolf501.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gyi.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yft.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wdv.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kkm.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vdf.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eca.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hxd.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sls.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fcs.haohaochexian.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pnx.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uid.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bbq.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jfj.yongpay.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fae.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lti.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lpl.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://alw.shanyushiyangtech.top

================================================================================
来源：http://qjw.yueranfly.top

A. 基础语法与类型
来源：http://kww.aibaodan.cn

================================================================================
来源：http://uzw.mhx1999.top

[A01] Hello World
来源：http://tqk.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://lts.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://lqf.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://cjy.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fru.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://pxm.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://bxg.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://tuy.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rxk.bjfxy.top

[A02] 变量声明与赋值
来源：http://img.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bsf.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://wkp.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gjv.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zdv.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://vsn.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://kuq.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://mwr.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ugp.daria6918.cn

[A03] 常量定义
来源：http://gjh.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fan.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://wfg.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://rql.tanke756.top

TS:   const PI: number = 3.14159;
来源：http://jpd.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://izo.andypj.xyz

Go:   const PI = 3.14159
来源：http://pze.meibo888.top

Ruby: PI = 3.14159
来源：http://pbp.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://ufy.sxryk.cn

[A04] 判断变量类型
来源：http://oji.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yfk.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cvd.yj20258888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bas.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://hts.ppjwa.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dnk.yuxming.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yxo.dianchejie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iqp.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://piu.shzxlz.cn

[A05] 整数除法与取模
来源：http://nrg.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eht.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jns.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://syj.daxiang520.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://azk.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://gxn.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://xuu.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://riy.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://awk.zhoulong.xyz

[A06] 字符串转数字
来源：http://ctt.ydjk.org.cn

Py:   int("42"); float("3.14")
来源：http://uaf.dianchejie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hnm.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cwf.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://bvc.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iro.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://alh.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://cru.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kat.ehwqpu.com

[A07] 数字转字符串
来源：http://pui.birdmap.top

Py:   str(42)
来源：http://vjm.nanxinkj.top

PHP:  (string) 42; strval(42)
来源：http://ewp.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://dtk.chenjidiqi.icu

TS:   String(42)
来源：http://lxb.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wbk.yvedp.cn

Go:   strconv.Itoa(42)
来源：http://fhp.zhoulong.xyz

Ruby: 42.to_s
来源：http://yum.cheryme.top

C#:   42.ToString()
来源：http://lfn.gotoacloud.top

[A08] 取整与四舍五入
来源：http://roa.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://euk.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://brq.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wzt.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eee.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hqz.yonumen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pak.52xcode.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vmv.snrcjt.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lqx.meibo888.top

[A09] 绝对值与最大最小值
来源：http://gqz.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fnu.cheryme.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qoq.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://usk.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qce.sjlbkw.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://utv.chenlongwang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fot.hongshengwenyu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mam.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tal.yongpay.top

[A10] 生成随机数
来源：http://yuf.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://abk.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://klu.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kon.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tgx.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://bax.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gca.vehdjk.com

Ruby: rand(1..100)
来源：http://gca.tian-w.cn

C#:   new Random().Next(1, 101)
来源：http://qqp.yanxiufei.cn

[A11] 条件表达式（三元）
来源：http://yvg.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://rig.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kif.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://jsg.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://czp.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://ibs.epnwcf.com

Go:   // 无三元运算符，需用 if 语句
来源：http://dcs.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ogx.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://nri.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://tsk.nwbrower.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lgg.zhijiandao.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pun.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://cbp.feifeiyinyue.top

TS:   `Hello, ${name}!`
来源：http://yme.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://rug.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oyi.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://jsy.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://eoh.ydjk.org.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jry.nanxuanxn.top

Py:   "第一行\n第二行"
来源：http://kre.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://dvu.andypj.xyz

JS:   "第一行\n第二行"
来源：http://eay.yfazqb.com

TS:   "第一行\n第二行"
来源：http://kpm.tianlin.xyz

Java: "第一行\n第二行"
来源：http://ytx.uphjek.com

Go:   "第一行\n第二行"
来源：http://dfk.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://pgn.vehdjk.com

C#:   "第一行\n第二行"
来源：http://shw.yonumen.top

[A14] 注释写法
来源：http://ecs.chenlongwang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xhn.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://bxw.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://mii.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://azv.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dcx.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://hgb.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vrf.hnqzz.top


<!-- 参考信息 -->