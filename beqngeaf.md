代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://zsb.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://sxr.yj20258.top

[U84] JS：CommonJS 写法
来源：http://ldo.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://hyc.iojbl.cn

[U85] JS：可选链
来源：http://uhk.xuanzx.com

a?.b?.c
来源：http://wyx.chenlongwang.top

[U86] JS：空值合并
来源：http://hsq.snrcjt.cn

a ?? b
来源：http://lmd.zdqjudy.top

[U87] JS：解构默认值
来源：http://fbf.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://ycz.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://ear.zhongyouzk.top

{ ...a, ...b }
来源：http://cli.iojbl.cn

[U89] JS：数组去重
来源：http://mxb.tian-w.cn

[...new Set(arr)]
来源：http://qnw.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://kar.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://xtx.52xcode.cn

[U91] JS：对象键值遍历
来源：http://tmg.feifeiyinyue.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pbe.gaohongyu789.top

[U92] JS：深拷贝
来源：http://ihx.ydzc1.top

structuredClone(obj)
来源：http://ndx.sufxvd.cn

[U93] JS：模板字符串
来源：http://smh.ctjpmb.com

`共 ${n} 条`
来源：http://cyg.gzhubu.top

[U94] JS：箭头函数
来源：http://vbi.nanxuanxn.top

const double = x => x * 2;
来源：http://crf.jinqigufen.top

[U95] JS：Promise 包装
来源：http://xpu.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://osc.guannengcc.top

[U96] JS：async/await 与异常
来源：http://uqu.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wui.feifeiyinyue.top

[U97] JS：并发请求
来源：http://wcz.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bqe.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://dbv.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://krg.zhoulong.xyz

[U99] JS：事件监听
来源：http://vig.bbcook.cn

el.addEventListener("click", e => {})
来源：http://fut.wangdashe.top

[U100] JS：DOM 查询
来源：http://czi.jiagoushi.top

document.querySelector(".item")
来源：http://qog.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://axn.xylfe.cn

el.classList.toggle("active")
来源：http://hkj.ydzc1.top

[U102] JS：本地存储
来源：http://btq.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tzb.cqqwz.cn

[U103] JS：定时器
来源：http://eia.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://njm.cucudq.cn

[U104] JS：防抖
来源：http://vfd.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tdn.haohaochexian.top

[U105] JS：节流
来源：http://lzd.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://knv.chenzaomai.com

[U106] JS：日期格式化
来源：http://ekj.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gma.yj20258888.top

[U107] JS：数字千分位
来源：http://fly.hesvh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qzu.zhengqikj.top

[U108] JS：随机整数
来源：http://vnq.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xfb.hysaishi.cn

[U109] JS：数组分组
来源：http://uhs.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://sgq.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://enb.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rxr.gotoacloud.top

[U111] JS：对象转 Map
来源：http://lpn.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://rpi.hesvh.cn

[U112] JS：字符串补位
来源：http://voz.yj202588.top

"7".padStart(3, "0")
来源：http://akj.fzhhl.top

[U113] JS：正则替换全部
来源：http://gkl.tianlin.xyz

s.replaceAll("a", "b")
来源：http://euv.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://can.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqc.hywenlv.cn

[U115] JS：生成 UUID
来源：http://kua.hnqzz.top

crypto.randomUUID()
来源：http://phq.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://gti.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://akd.jianghu66.top

[U117] JS：单元测试
来源：http://bis.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://lex.havefunace.top

[U118] JS：开发服务器
来源：http://krv.havefunace.top

npm i -D vite;  npx vite
来源：http://rzg.jqgufenzy.top

[U119] JS：生产构建
来源：http://riy.zdqjudy.top

npx vite build
来源：http://dzl.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://xje.svipenyu.cn

import.meta.env.VITE_API_URL
来源：http://dsu.aibaodan.cn

================================================================================
来源：http://vxq.jinyuanbaomall.cn

统计汇总
来源：http://ixd.jinyuanbaomall.cn

================================================================================
来源：http://pak.zdbjq.cn

按语言统计（条）：
来源：http://nwj.bbcook.cn

Python ......... 252
来源：http://ssn.wangdashe.top

PHP ............ 252
来源：http://smg.zdbjq.cn

JavaScript ..... 252
来源：http://bvu.sufxvd.cn

TypeScript ..... 212
来源：http://csu.chenzaomai.com

Java ........... 212
来源：http://muu.xylfe.cn

Go ............. 212
来源：http://krx.yvedp.cn

Ruby ........... 212
来源：http://ofz.vqdsnc.cn

C# ............. 212
来源：http://pnh.guowangkeji.top

C .............. 30
来源：http://ppe.gzhubu.top

C++ ............ 30
来源：http://ntl.0kj1m.cn

SQL ............ 90
来源：http://gsz.ppjwa.cn

Bash ........... 80
来源：http://nmg.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://hck.sxryk.cn

Swift .......... 15
来源：http://bcv.jinqigfzy.top

Lua ............ 10
来源：http://hil.jlsjyb.cn

Perl ........... 10
来源：http://xnz.wangdashe.top

Scala .......... 10
来源：http://zbk.cheryme.top

------------------------------------
来源：http://pct.sufxvd.cn

合计 ........... 2106 条
来源：http://rkh.yueranfly.top

按章节统计：
来源：http://fyq.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pgy.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yyg.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rht.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qmo.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pau.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ueg.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dap.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sxv.ydzc1.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://omf.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nly.gotoacloud.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tlk.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eis.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rmu.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://trs.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vmt.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wwg.chenlongwang.top

Q SQL 专题                              90
来源：http://jqa.sufxvd.cn

R Bash 专题                             80
来源：http://keq.guannengcc.top

S C / C++ 专题                          60
来源：http://tkd.yvedp.cn

T 其他语言补充                          60
来源：http://ebu.svipenyu.cn

U 高频实用片段                         120
来源：http://dpb.daxiang520.top

------------------------------------
来源：http://qxb.tanke756.top

合计                                  2106 条
来源：http://agd.gzhubu.top

--------------------------------------------------------------------------------
来源：http://qdf.yueranfly.top

使用提醒
来源：http://tzr.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://hds.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vdi.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sdj.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bks.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zie.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hat.havefunace.top

—— 文件结束 ——
来源：http://bqp.andypj.xyz

================================================================================
来源：http://qbi.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://ekb.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://sna.52xcode.cn

================================================================================
来源：http://bke.dianchejie.cn

【收录内容】
来源：http://mpj.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://xoi.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zyq.jinqigufen.top

SQL · Bash · C · C++
来源：http://bfd.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ixb.ydjk.org.cn

【使用说明】
来源：http://jzj.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cyg.zhengqikj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uyd.ctjpmb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://prh.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fcb.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jkh.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jtb.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://myn.yueranfly.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pha.wangdashe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cgx.mhx1999.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jua.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fqg.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kgm.yonumen.top

【文件统计】
来源：http://vjc.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cwx.uphjek.com

--------------------------------------------------------------------------------
来源：http://rql.sysykeji.top

目  录
来源：http://wjv.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://ntx.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wir.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xsz.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aew.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yyj.jinqigufen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://znx.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ukk.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://two.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://llc.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bwt.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ytk.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aat.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rvs.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vtc.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ful.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hms.sufxvd.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cpw.316326.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gpq.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://scm.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gei.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dnj.cdnleiting.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pcb.yfazqb.com

================================================================================
来源：http://qgi.jyoumei.cn

A. 基础语法与类型
来源：http://jle.nanxuanxn.top

================================================================================
来源：http://ibl.ehwqpu.com

[A01] Hello World
来源：http://gxc.vqdsnc.cn

Py:   print("Hello, World!")
来源：http://kcb.hongshengwenyu.top

PHP:  echo "Hello, World!";
来源：http://tci.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://jpi.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rtg.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://jwz.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://zkh.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://lhm.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://igb.wangdashe.top

[A02] 变量声明与赋值
来源：http://rgh.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ojp.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oan.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://hhg.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eqc.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://lja.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://mct.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://rvt.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://amu.zdqjudy.top

[A03] 常量定义
来源：http://pms.ydjk.org.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cyy.nanxuanxn.top

PHP:  const PI = 3.14159;
来源：http://wjn.iojbl.cn

JS:   const PI = 3.14159;
来源：http://btm.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://ptg.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://ozz.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://raw.ehwqpu.com

Ruby: PI = 3.14159
来源：http://xue.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://bqi.xuanzx.com

[A04] 判断变量类型
来源：http://lcq.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xav.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://unv.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dcu.jinqigufen.top

TS:   typeof x; x instanceof Date
来源：http://owr.zhixingplan.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wkj.jianghu66.top

Go:   reflect.TypeOf(x).Name()
来源：http://ttt.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vqh.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://joa.yj20258888.top

[A05] 整数除法与取模
来源：http://xky.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://prz.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://zee.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bqv.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rbs.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://www.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://ibu.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://qpj.hongshengwenyu.top

C#:   7 / 2; 7 % 2
来源：http://pjr.jinqigfzy.top

[A06] 字符串转数字
来源：http://dot.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://ydt.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bhm.ydzc1.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://coe.jqgufenzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://bze.wangshuangyany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://umf.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dtj.hammf.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qvb.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://guf.hammf.cn

[A07] 数字转字符串
来源：http://dfg.ctjpmb.com

Py:   str(42)
来源：http://ivv.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://ewg.tian-w.cn

JS:   String(42); (42).toString()
来源：http://aka.hongshengwenyu.top

TS:   String(42)
来源：http://rqw.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vti.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://gyw.ybcxt.top

Ruby: 42.to_s
来源：http://ith.tianlin.xyz

C#:   42.ToString()
来源：http://wsw.xuanzx.com

[A08] 取整与四舍五入
来源：http://dwz.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gkl.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://omu.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rvj.hongshengwenyu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://moj.haohaochexian.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pds.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kbl.feifeiyinyue.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://iyv.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ouu.fktsv.cn

[A09] 绝对值与最大最小值
来源：http://qik.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wkk.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dij.yj20258888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pfb.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://frs.jqgfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://evv.jinyuanbaomall.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://psn.nanxuanxn.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lti.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iln.zycfv.cn

[A10] 生成随机数
来源：http://quh.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://asl.fzhhl.top

PHP:  random_int(1, 100);
来源：http://uyb.havefunace.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://myt.dashuyun.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qes.yanxiufei.cn

Java: new Random().nextInt(100) + 1
来源：http://hxw.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rrs.hnqzz.top

Ruby: rand(1..100)
来源：http://jph.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://mxq.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://lzw.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://sfo.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bed.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://omx.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://lkz.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://faf.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pog.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jxs.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bjr.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://fxr.ybcxt.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rxd.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pyp.hnqzz.top

JS:   `Hello, ${name}!`
来源：http://zve.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://ynt.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://gbd.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yps.shanyushiyangtech.top

Ruby: "Hello, #{name}!"
来源：http://zaz.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://tla.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://uic.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://rwl.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://ubz.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://zyb.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://wll.smart0.xyz

Java: "第一行\n第二行"
来源：http://lhm.hcnkem.com

Go:   "第一行\n第二行"
来源：http://fvz.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://yil.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://sos.sweek.top


<!-- 参考信息 -->