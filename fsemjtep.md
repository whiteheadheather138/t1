代发 wailian999

[U81] JS：初始化项目
来源：http://ilt.guannengcc.top

npm init -y;  npm i express
来源：http://qjv.316326.xyz

[U82] JS：package.json 脚本
来源：http://oya.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ccz.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://bwb.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://mvi.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://tue.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://hlf.haohaochexian.top

[U85] JS：可选链
来源：http://tnb.yj20258.top

a?.b?.c
来源：http://kui.sxryk.cn

[U86] JS：空值合并
来源：http://tlp.jinqigufen.top

a ?? b
来源：http://cdl.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://jtu.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://las.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://fsn.yj202588.top

{ ...a, ...b }
来源：http://mvf.svipenyu.cn

[U89] JS：数组去重
来源：http://umr.zdbjq.cn

[...new Set(arr)]
来源：http://mjz.fktsv.cn

[U90] JS：数字数组排序
来源：http://awq.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://xvm.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://krk.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hai.snrcjt.cn

[U92] JS：深拷贝
来源：http://hvx.gogol.net.cn

structuredClone(obj)
来源：http://wek.cheryme.top

[U93] JS：模板字符串
来源：http://nhf.ivvv.top

`共 ${n} 条`
来源：http://jfo.hammf.cn

[U94] JS：箭头函数
来源：http://ogr.nwbrower.top

const double = x => x * 2;
来源：http://qmc.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://mvl.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://bxt.xziqi.cn

[U96] JS：async/await 与异常
来源：http://dae.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://urv.xuanzx.com

[U97] JS：并发请求
来源：http://djo.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://trp.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://iox.hcnkem.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mep.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://bev.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://feg.haohaochexian.top

[U100] JS：DOM 查询
来源：http://hxg.tarul.cn

document.querySelector(".item")
来源：http://uoo.hnqzz.top

[U101] JS：classList 操作
来源：http://ktj.cashguo.top

el.classList.toggle("active")
来源：http://wuw.guannengcc.top

[U102] JS：本地存储
来源：http://abl.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wkx.jinghuilouyu.cn

[U103] JS：定时器
来源：http://ouz.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aft.chenlongwang.top

[U104] JS：防抖
来源：http://hgb.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://waf.xuanzx.com

[U105] JS：节流
来源：http://foj.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://paj.tianlin.xyz

[U106] JS：日期格式化
来源：http://rtr.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dlu.mhx1999.top

[U107] JS：数字千分位
来源：http://zco.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kyv.shuidangran.top

[U108] JS：随机整数
来源：http://dsw.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bsf.vehdjk.com

[U109] JS：数组分组
来源：http://oui.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://isg.xziqi.cn

[U110] JS：数组分块
来源：http://glu.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tem.bbcook.cn

[U111] JS：对象转 Map
来源：http://yhv.c1oappe.top

new Map(Object.entries(obj))
来源：http://nyo.vehdjk.com

[U112] JS：字符串补位
来源：http://hxx.epnwcf.com

"7".padStart(3, "0")
来源：http://xgs.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://gga.uphjek.com

s.replaceAll("a", "b")
来源：http://pau.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://iex.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://uon.daria6918.cn

[U115] JS：生成 UUID
来源：http://yoq.ppjwa.cn

crypto.randomUUID()
来源：http://xcg.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://jby.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://jft.hnqzz.top

[U117] JS：单元测试
来源：http://wyd.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://oum.yongpay.top

[U118] JS：开发服务器
来源：http://vzg.sysykeji.top

npm i -D vite;  npx vite
来源：http://dwe.tarul.cn

[U119] JS：生产构建
来源：http://edi.yuxming.cn

npx vite build
来源：http://vgk.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://xcj.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://ekt.yvedp.cn

================================================================================
来源：http://ttw.fengsongda.top

统计汇总
来源：http://hje.gotoacloud.top

================================================================================
来源：http://ggg.tarul.cn

按语言统计（条）：
来源：http://mvh.52xcode.cn

Python ......... 252
来源：http://epj.ehwqpu.com

PHP ............ 252
来源：http://sov.xylfe.cn

JavaScript ..... 252
来源：http://txy.xuanzx.com

TypeScript ..... 212
来源：http://vgh.gotoacloud.top

Java ........... 212
来源：http://lbo.hesvh.cn

Go ............. 212
来源：http://igf.9152youxi.cn

Ruby ........... 212
来源：http://zzo.fehbvm.com

C# ............. 212
来源：http://vap.snrcjt.cn

C .............. 30
来源：http://gfg.bbcook.cn

C++ ............ 30
来源：http://foj.gaohongyu789.top

SQL ............ 90
来源：http://hvu.jinqigufen.top

Bash ........... 80
来源：http://vwt.yuanzhike.top

Kotlin ......... 15
来源：http://ttj.jqgufenzy.top

Swift .......... 15
来源：http://khq.tarul.cn

Lua ............ 10
来源：http://nwa.jqgfzy.top

Perl ........... 10
来源：http://rva.cucudq.cn

Scala .......... 10
来源：http://gwz.zhongyouzk.top

------------------------------------
来源：http://swt.shzxlz.cn

合计 ........... 2106 条
来源：http://ays.chenjidiqi.icu

按章节统计：
来源：http://flo.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ccm.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sgt.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://koa.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ruq.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fuy.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dep.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dca.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xpl.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ovb.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jqa.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tcp.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mdq.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gok.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vdn.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vet.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ssg.epnwcf.com

Q SQL 专题                              90
来源：http://tvz.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://fcd.jqgufenzy.top

S C / C++ 专题                          60
来源：http://tlc.xziqi.cn

T 其他语言补充                          60
来源：http://cqe.gaohongyu789.top

U 高频实用片段                         120
来源：http://mui.hcnkem.com

------------------------------------
来源：http://qwa.feifeiyinyue.top

合计                                  2106 条
来源：http://adm.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://fpr.yangfankeji.com

使用提醒
来源：http://jwe.cashguo.top

--------------------------------------------------------------------------------
来源：http://tlz.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fwg.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mak.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vjn.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://aaw.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dxr.fehbvm.com

—— 文件结束 ——
来源：http://ggq.cqqwz.cn

================================================================================
来源：http://ost.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://ttn.zhoulong.xyz

Common Programming Examples Cheat Book
来源：http://xlb.zhongyouzk.top

================================================================================
来源：http://ish.hysaishi.cn

【收录内容】
来源：http://dsi.cashguo.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wiz.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yrz.c1oappe.top

SQL · Bash · C · C++
来源：http://tjv.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wfi.pycfn.com

【使用说明】
来源：http://yed.fehbvm.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bxb.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gbq.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ctu.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://swy.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sea.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://csp.vehdjk.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kdt.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rjv.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://obh.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qxv.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ojk.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kve.dashuyun.cn

【文件统计】
来源：http://edr.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qnz.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://ajj.shangyingyoupin.top

目  录
来源：http://mpi.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://tsh.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oaa.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eli.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vrp.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ymk.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lel.havefunace.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wgp.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hlt.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://abq.andypj.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cqx.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eme.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nrp.shanyushiyangtech.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://juj.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aca.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kgz.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://slu.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://but.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qes.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cdj.dianchejie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ptx.meibo888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mod.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uxf.guannengcc.top

================================================================================
来源：http://nms.hfpthk.cn

A. 基础语法与类型
来源：http://fvh.xingfuxueyuan.xyz

================================================================================
来源：http://gnm.iojbl.cn

[A01] Hello World
来源：http://rib.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://fuw.ivvv.top

PHP:  echo "Hello, World!";
来源：http://yvs.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://shm.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pnb.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://hpl.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://zuv.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://cff.kuanghao11.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://djt.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://sqc.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jaw.yj20258888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://akx.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://ezi.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jlu.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://vgl.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://bku.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://srk.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ekz.sjlbkw.cn

[A03] 常量定义
来源：http://udg.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xhm.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://jrj.jyoumei.cn

JS:   const PI = 3.14159;
来源：http://las.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://ujg.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://opy.zdbjq.cn

Go:   const PI = 3.14159
来源：http://wxf.yj20258.top

Ruby: PI = 3.14159
来源：http://mmn.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://krr.wangdashe.top

[A04] 判断变量类型
来源：http://eln.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://owg.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yuf.yj20258888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vls.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://ecm.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://swz.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bds.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hbt.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://mjh.dianchejie.cn

[A05] 整数除法与取模
来源：http://jsd.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ons.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fpg.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pud.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xpj.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://yvc.yonumen.top

Go:   7 / 2; 7 % 2
来源：http://pkg.tian-w.cn

Ruby: 7 / 2; 7 % 2
来源：http://uzz.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://gzv.xylfe.cn

[A06] 字符串转数字
来源：http://yir.hongshengwenyu.top

Py:   int("42"); float("3.14")
来源：http://sba.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://guq.hnxiangtu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ddd.xuetiantiany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://akt.sufxvd.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fjt.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xly.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://hpp.xuanzx.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xoi.zhongyouzk.top

[A07] 数字转字符串
来源：http://bki.jinqigufen.top

Py:   str(42)
来源：http://lgr.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://ljn.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://ecz.kuanghao11.cn

TS:   String(42)
来源：http://gxj.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wtw.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://cuj.gogol.net.cn

Ruby: 42.to_s
来源：http://pyl.hfpthk.cn

C#:   42.ToString()
来源：http://gai.9152youxi.cn

[A08] 取整与四舍五入
来源：http://fzm.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kxg.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tqi.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://roj.9152youxi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iwu.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gli.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zxe.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://asf.bjfxy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dqh.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://lsm.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dpc.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://skk.shangyingyoupin.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sfn.daxiang520.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ika.jlsjyb.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zjg.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ooa.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kgg.jinqigfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qko.tian-w.cn

[A10] 生成随机数
来源：http://izi.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://qpx.xylfe.cn

PHP:  random_int(1, 100);
来源：http://xnu.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pbg.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qcs.aibaodan.cn

Java: new Random().nextInt(100) + 1
来源：http://rac.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://csa.cdnleiting.top

Ruby: rand(1..100)
来源：http://wor.ybcxt.top

C#:   new Random().Next(1, 101)
来源：http://pfr.havefunace.top

[A11] 条件表达式（三元）
来源：http://vaj.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://qyh.zhixingplan.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uul.guannengcc.top

JS:   x > 0 ? "yes" : "no"
来源：http://jtb.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://wxh.chenlongwang.top

Java: x > 0 ? "yes" : "no"
来源：http://pwk.zhixingplan.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xmb.snrcjt.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kyo.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zle.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://bpb.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oem.shzxlz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mjd.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://jpg.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://arq.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://vcy.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gtm.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://kym.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://cap.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vaf.xinyue.icu

Py:   "第一行\n第二行"
来源：http://yrp.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://ryk.nanxinkj.top

JS:   "第一行\n第二行"
来源：http://hio.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://ttg.shzxlz.cn


<!-- 参考信息 -->