代发 wailian999

[U81] JS：初始化项目
来源：http://fxq.cdnleiting.top

npm init -y;  npm i express
来源：http://ncw.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://ect.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bbb.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://lhg.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qhx.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://jig.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oyw.yueranfly.top

[U85] JS：可选链
来源：http://ptq.bjfxy.top

a?.b?.c
来源：http://xxi.yuanzhike.top

[U86] JS：空值合并
来源：http://kdr.jlsjyb.cn

a ?? b
来源：http://apu.ehwqpu.com

[U87] JS：解构默认值
来源：http://upg.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://rvx.bbcook.cn

[U88] JS：对象展开合并
来源：http://dkw.ybcxt.top

{ ...a, ...b }
来源：http://apl.zhijiandao.cn

[U89] JS：数组去重
来源：http://vcu.zhixingplan.top

[...new Set(arr)]
来源：http://dev.yangfankeji.com

[U90] JS：数字数组排序
来源：http://bhu.sweek.top

[...arr].sort((a, b) => a - b)
来源：http://fjv.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://cuh.redwolf501.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wax.guowangkeji.top

[U92] JS：深拷贝
来源：http://rgf.aibaodan.cn

structuredClone(obj)
来源：http://fwi.zhoulong.xyz

[U93] JS：模板字符串
来源：http://bdu.ehwqpu.com

`共 ${n} 条`
来源：http://sko.nanxuanxn.top

[U94] JS：箭头函数
来源：http://lda.jinqigfzy.top

const double = x => x * 2;
来源：http://esf.jiagoushi.top

[U95] JS：Promise 包装
来源：http://ykg.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://aee.xinyue.icu

[U96] JS：async/await 与异常
来源：http://kts.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qvc.0kj1m.cn

[U97] JS：并发请求
来源：http://qil.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://fxy.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://yhf.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pgl.uphjek.com

[U99] JS：事件监听
来源：http://yfv.wangdashe.top

el.addEventListener("click", e => {})
来源：http://exc.ctjpmb.com

[U100] JS：DOM 查询
来源：http://ago.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://aim.uphjek.com

[U101] JS：classList 操作
来源：http://omr.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://cnv.zycfv.cn

[U102] JS：本地存储
来源：http://hls.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vyw.quarkkingdee.top

[U103] JS：定时器
来源：http://ibj.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qer.hnxiangtu.top

[U104] JS：防抖
来源：http://crc.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgp.xylfe.cn

[U105] JS：节流
来源：http://wue.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dju.nanxuanxn.top

[U106] JS：日期格式化
来源：http://dvy.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fhg.cdnleiting.top

[U107] JS：数字千分位
来源：http://lom.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jyx.yangfankeji.com

[U108] JS：随机整数
来源：http://lxm.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gcm.yvedp.cn

[U109] JS：数组分组
来源：http://mqn.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://rai.ybcxt.top

[U110] JS：数组分块
来源：http://pws.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xez.jqgfzy.top

[U111] JS：对象转 Map
来源：http://ztz.fengsongda.top

new Map(Object.entries(obj))
来源：http://nvz.ppjwa.cn

[U112] JS：字符串补位
来源：http://bzh.redwolf501.top

"7".padStart(3, "0")
来源：http://kve.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://jwt.9152youxi.cn

s.replaceAll("a", "b")
来源：http://tpw.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://bdr.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://aos.tian-w.cn

[U115] JS：生成 UUID
来源：http://nrd.yj20258.top

crypto.randomUUID()
来源：http://nwj.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://ogs.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://jcy.sysykeji.top

[U117] JS：单元测试
来源：http://mbq.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://aqn.zdbjq.cn

[U118] JS：开发服务器
来源：http://vow.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://pck.feifeiyinyue.top

[U119] JS：生产构建
来源：http://dtl.nwbrower.top

npx vite build
来源：http://shu.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://opq.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://omj.hnxiangtu.top

================================================================================
来源：http://nut.bjfxy.top

统计汇总
来源：http://kji.haohaochexian.top

================================================================================
来源：http://veh.quarkkingdee.top

按语言统计（条）：
来源：http://whf.bjfxy.top

Python ......... 252
来源：http://itq.gotoacloud.top

PHP ............ 252
来源：http://epb.ppjwa.cn

JavaScript ..... 252
来源：http://nlj.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://nkm.cheryme.top

Java ........... 212
来源：http://tqh.zhaomingkeji.xyz

Go ............. 212
来源：http://rez.gotoacloud.top

Ruby ........... 212
来源：http://rzf.uphjek.com

C# ............. 212
来源：http://pkq.jqgfzy.top

C .............. 30
来源：http://omg.fzhhl.top

C++ ............ 30
来源：http://hli.yj202588.top

SQL ............ 90
来源：http://vkp.zhongyouzk.top

Bash ........... 80
来源：http://ufp.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://tln.fktsv.cn

Swift .......... 15
来源：http://izz.52xcode.cn

Lua ............ 10
来源：http://nlc.yuanzhike.top

Perl ........... 10
来源：http://yyp.tian-w.cn

Scala .......... 10
来源：http://ewg.9152youxi.cn

------------------------------------
来源：http://xzt.jqgfzy.top

合计 ........... 2106 条
来源：http://ezs.fzhhl.top

按章节统计：
来源：http://tsy.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zqi.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tva.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ymr.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pgl.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hck.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nmk.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cqx.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rwq.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iyv.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xhj.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bmd.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ujz.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iuq.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nnx.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yzq.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bsd.aizwys.cn

Q SQL 专题                              90
来源：http://kxq.tanke756.top

R Bash 专题                             80
来源：http://mnk.hesvh.cn

S C / C++ 专题                          60
来源：http://wag.ivvv.top

T 其他语言补充                          60
来源：http://myh.xziqi.cn

U 高频实用片段                         120
来源：http://nmw.meibo888.top

------------------------------------
来源：http://mje.gzhubu.top

合计                                  2106 条
来源：http://lnb.smart0.xyz

--------------------------------------------------------------------------------
来源：http://ycw.cucudq.cn

使用提醒
来源：http://bcb.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://nvl.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dzb.epnwcf.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://okd.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://siw.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://czg.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blw.jqgfzy.top

—— 文件结束 ——
来源：http://hpt.jyoumei.cn

================================================================================
来源：http://aze.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://uiw.xuanzx.com

Common Programming Examples Cheat Book
来源：http://cyt.cqqwz.cn

================================================================================
来源：http://lpx.xuanzx.com

【收录内容】
来源：http://kog.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://qtt.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://etv.yuxming.cn

SQL · Bash · C · C++
来源：http://yix.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dof.c1oappe.top

【使用说明】
来源：http://gnb.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://goo.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mex.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zxe.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xdn.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wwf.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vni.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rln.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ydm.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jjv.feifeiyinyue.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hzp.xylfe.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://myq.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://svd.dashuyun.cn

【文件统计】
来源：http://zkm.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://apm.fzhhl.top

--------------------------------------------------------------------------------
来源：http://bmr.sysykeji.top

目  录
来源：http://fbh.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://ibr.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tzx.redwolf501.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wqj.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fkk.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://igb.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://meb.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jjn.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pog.zhoulong.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yoc.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zyp.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ruo.ydzc1.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vlt.ehwqpu.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ads.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://inq.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hzi.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://edh.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hii.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://abg.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://jna.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wqq.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://beu.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rok.kuanghao11.cn

================================================================================
来源：http://aca.quarkkingdee.top

A. 基础语法与类型
来源：http://dpa.chenlongwang.top

================================================================================
来源：http://ded.ydjk.org.cn

[A01] Hello World
来源：http://doh.daxiang520.top

Py:   print("Hello, World!")
来源：http://bqp.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://lmu.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://wgl.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://khy.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://iso.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://jbk.zhengqikj.top

Ruby: puts "Hello, World!"
来源：http://cjs.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://vrq.316326.xyz

[A02] 变量声明与赋值
来源：http://att.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xba.nanxuanxn.top

PHP:  $name = "Alex"; $age = 20;
来源：http://aer.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://one.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xry.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://hgk.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://zvi.uphjek.com

Ruby: name = "Alex"; age = 20
来源：http://vtz.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://nwe.shanyushiyangtech.top

[A03] 常量定义
来源：http://bba.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zqe.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://cxi.meibo888.top

JS:   const PI = 3.14159;
来源：http://mcn.sweek.top

TS:   const PI: number = 3.14159;
来源：http://rio.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://wjn.52xcode.cn

Go:   const PI = 3.14159
来源：http://bjc.havefunace.top

Ruby: PI = 3.14159
来源：http://nkg.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://lqq.xinyue.icu

[A04] 判断变量类型
来源：http://dfv.epnwcf.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hjl.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xsy.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ajg.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://guu.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tdi.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://xum.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://fvt.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://cah.zhongyouzk.top

[A05] 整数除法与取模
来源：http://eot.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xvg.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://yan.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nqw.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lbm.tianlin.xyz

Java: 7 / 2; 7 % 2
来源：http://zwi.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://grb.mhx1999.top

Ruby: 7 / 2; 7 % 2
来源：http://jhl.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://ljd.zhoulong.xyz

[A06] 字符串转数字
来源：http://ock.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://bmd.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qmd.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kyy.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://mwg.sxryk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tjh.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ugy.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jbr.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gim.fzhhl.top

[A07] 数字转字符串
来源：http://lhs.jqgufenzy.top

Py:   str(42)
来源：http://kvg.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://pkg.shzxlz.cn

JS:   String(42); (42).toString()
来源：http://hzo.gotoacloud.top

TS:   String(42)
来源：http://mdd.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oed.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://wri.zhijiandao.cn

Ruby: 42.to_s
来源：http://rdo.xziqi.cn

C#:   42.ToString()
来源：http://lqj.jyoumei.cn

[A08] 取整与四舍五入
来源：http://gft.feifeiyinyue.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://enj.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kdj.gzhubu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://crz.aibaodan.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bbt.zhixingplan.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zlg.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qkk.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wpl.daria6918.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ica.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://mgb.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jqn.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xey.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kit.haohaochexian.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oki.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://omx.ctjpmb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iuw.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://znd.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://chw.jinqigfzy.top

[A10] 生成随机数
来源：http://wux.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://nkc.chenzaomai.com

PHP:  random_int(1, 100);
来源：http://rrp.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fvc.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jrh.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://fsw.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tsq.zhixingplan.top

Ruby: rand(1..100)
来源：http://qgm.yj202588.top

C#:   new Random().Next(1, 101)
来源：http://bmv.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://xtw.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://cxv.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tnq.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://hgq.fehbvm.com

TS:   x > 0 ? "yes" : "no"
来源：http://bvw.hywenlv.cn

Java: x > 0 ? "yes" : "no"
来源：http://ubu.jinghuilouyu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dio.ctjpmb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://wvq.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://peq.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://vfb.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lvo.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yfj.zycfv.cn

JS:   `Hello, ${name}!`
来源：http://tgw.zhixingplan.top

TS:   `Hello, ${name}!`
来源：http://igk.hywenlv.cn

Java: "Hello, %s!".formatted(name)
来源：http://flt.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dbp.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://giu.zdqjudy.top

C#:   $"Hello, {name}!"
来源：http://jdi.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://jez.sjlbkw.cn

Py:   "第一行\n第二行"
来源：http://cfw.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://kmj.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://nel.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://lwh.daria6918.cn


<!-- 参考信息 -->