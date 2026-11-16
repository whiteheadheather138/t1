代发 wailian999

[U81] JS：初始化项目
来源：http://npo.ydzc1.top

npm init -y;  npm i express
来源：http://brw.vehdjk.com

[U82] JS：package.json 脚本
来源：http://rcv.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mek.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://uyg.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://wcw.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://utq.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eeu.xinyue.icu

[U85] JS：可选链
来源：http://rvo.nanxinkj.top

a?.b?.c
来源：http://uzj.tanke756.top

[U86] JS：空值合并
来源：http://gsr.tarul.cn

a ?? b
来源：http://htg.jyoumei.cn

[U87] JS：解构默认值
来源：http://oba.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://pfu.andypj.xyz

[U88] JS：对象展开合并
来源：http://qfh.hongshengwenyu.top

{ ...a, ...b }
来源：http://txp.ctjpmb.com

[U89] JS：数组去重
来源：http://wpq.svipenyu.cn

[...new Set(arr)]
来源：http://voz.tianlin.xyz

[U90] JS：数字数组排序
来源：http://ozw.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://ieb.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://cmt.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ejh.hnqzz.top

[U92] JS：深拷贝
来源：http://kcd.tanke756.top

structuredClone(obj)
来源：http://ogd.ctjpmb.com

[U93] JS：模板字符串
来源：http://zer.sysykeji.top

`共 ${n} 条`
来源：http://ebl.guowangkeji.top

[U94] JS：箭头函数
来源：http://lua.ydzc1.top

const double = x => x * 2;
来源：http://rmb.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://vol.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://olc.yfazqb.com

[U96] JS：async/await 与异常
来源：http://niu.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fqg.jianghu66.top

[U97] JS：并发请求
来源：http://qrp.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://trd.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://ehh.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jsw.xuetiantiany.cn

[U99] JS：事件监听
来源：http://xqr.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://xzx.9152youxi.cn

[U100] JS：DOM 查询
来源：http://wro.jlsjyb.cn

document.querySelector(".item")
来源：http://eoi.fzhhl.top

[U101] JS：classList 操作
来源：http://awh.gogol.net.cn

el.classList.toggle("active")
来源：http://gbw.jlsjyb.cn

[U102] JS：本地存储
来源：http://mfc.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ioi.fktsv.cn

[U103] JS：定时器
来源：http://ftg.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zdj.sysykeji.top

[U104] JS：防抖
来源：http://xyp.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gej.guowangkeji.top

[U105] JS：节流
来源：http://mfw.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uxm.yj20258888.top

[U106] JS：日期格式化
来源：http://yhk.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iyt.jyoumei.cn

[U107] JS：数字千分位
来源：http://uwg.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qkl.jyoumei.cn

[U108] JS：随机整数
来源：http://zad.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rir.vqdsnc.cn

[U109] JS：数组分组
来源：http://tsc.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://tej.smart0.xyz

[U110] JS：数组分块
来源：http://ihg.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xhm.sufxvd.cn

[U111] JS：对象转 Map
来源：http://fqs.gzhubu.top

new Map(Object.entries(obj))
来源：http://ppw.hnxiangtu.top

[U112] JS：字符串补位
来源：http://sdz.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://wym.hnqzz.top

[U113] JS：正则替换全部
来源：http://rdn.tianlin.xyz

s.replaceAll("a", "b")
来源：http://gst.gzhubu.top

[U114] JS：JSON 深比较
来源：http://nog.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://unk.cdnleiting.top

[U115] JS：生成 UUID
来源：http://rtz.fehbvm.com

crypto.randomUUID()
来源：http://zen.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://clx.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://rjp.zhiwuduotai.top

[U117] JS：单元测试
来源：http://cuk.sweek.top

npm i -D vitest;  npx vitest
来源：http://hzj.yongpay.top

[U118] JS：开发服务器
来源：http://nkd.andypj.xyz

npm i -D vite;  npx vite
来源：http://sbg.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://hzr.zdqjudy.top

npx vite build
来源：http://oio.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://fgi.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://eot.yangfankeji.com

================================================================================
来源：http://gnv.bjfxy.top

统计汇总
来源：http://myy.hysaishi.cn

================================================================================
来源：http://vxj.cheryme.top

按语言统计（条）：
来源：http://voz.c1oappe.top

Python ......... 252
来源：http://bxo.quarkkingdee.top

PHP ............ 252
来源：http://rrv.mhx1999.top

JavaScript ..... 252
来源：http://scs.yj20258.top

TypeScript ..... 212
来源：http://efa.ivvv.top

Java ........... 212
来源：http://ish.shanyushiyangtech.top

Go ............. 212
来源：http://xfn.jyoumei.cn

Ruby ........... 212
来源：http://lno.nwbrower.top

C# ............. 212
来源：http://liy.ydjk.org.cn

C .............. 30
来源：http://rbt.hongshengwenyu.top

C++ ............ 30
来源：http://dvl.jinyuanbaomall.cn

SQL ............ 90
来源：http://sqf.svipenyu.cn

Bash ........... 80
来源：http://iaf.cheryme.top

Kotlin ......... 15
来源：http://kbm.quarkkingdee.top

Swift .......... 15
来源：http://fkw.bbcook.cn

Lua ............ 10
来源：http://qbh.nanxinkj.top

Perl ........... 10
来源：http://xiy.tanke756.top

Scala .......... 10
来源：http://cln.jlsjyb.cn

------------------------------------
来源：http://zja.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://ihf.daxiang520.top

按章节统计：
来源：http://lbc.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://biw.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lxj.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xin.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vmt.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nlf.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://quc.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kkl.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vlg.nwbrower.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cba.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gcb.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ixn.uphjek.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zmb.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://usr.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bpm.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ddu.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vqs.zhijiandao.cn

Q SQL 专题                              90
来源：http://cja.snrcjt.cn

R Bash 专题                             80
来源：http://jik.zhengqikj.top

S C / C++ 专题                          60
来源：http://lsy.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://evq.fanxiaobao.xyz

U 高频实用片段                         120
来源：http://wse.quarkkingdee.top

------------------------------------
来源：http://sfc.fktsv.cn

合计                                  2106 条
来源：http://cjp.cucudq.cn

--------------------------------------------------------------------------------
来源：http://ieg.jlsjyb.cn

使用提醒
来源：http://use.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://qmo.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gwe.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fde.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zhc.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dnx.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zvj.vqdsnc.cn

—— 文件结束 ——
来源：http://nwf.ybcxt.top

================================================================================
来源：http://zmt.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://qop.meibo888.top

Common Programming Examples Cheat Book
来源：http://zqf.iojbl.cn

================================================================================
来源：http://bca.zhijiandao.cn

【收录内容】
来源：http://vul.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wwt.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bin.bjfxy.top

SQL · Bash · C · C++
来源：http://xsd.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ffe.hnxiangtu.top

【使用说明】
来源：http://grn.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pag.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yzs.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jvg.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qrs.shanyushiyangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://inc.chenlongwang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pwf.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nog.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zlc.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oce.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dva.xziqi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gho.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pfh.ydzc1.top

【文件统计】
来源：http://vhd.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ngr.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://vyb.cheryme.top

目  录
来源：http://orw.ybcxt.top

--------------------------------------------------------------------------------
来源：http://sez.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jbt.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://alu.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dxr.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://scc.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rwf.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hlm.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ypg.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hal.fzhhl.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xbz.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tqw.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zib.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ppw.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aoz.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kza.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tou.yuanzhike.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jvm.hnxiangtu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tub.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ulp.meibo888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uvm.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cym.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cfc.shzxlz.cn

================================================================================
来源：http://vup.aizwys.cn

A. 基础语法与类型
来源：http://qaa.mhx1999.top

================================================================================
来源：http://egc.52xcode.cn

[A01] Hello World
来源：http://wot.shuidangran.top

Py:   print("Hello, World!")
来源：http://eye.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://nat.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://yvq.feifeiyinyue.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mdt.yvedp.cn

Java: System.out.println("Hello, World!");
来源：http://puh.sufxvd.cn

Go:   fmt.Println("Hello, World!")
来源：http://zii.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://rao.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://agr.daxiang520.top

[A02] 变量声明与赋值
来源：http://obw.9152youxi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dgo.hysaishi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://luq.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://isx.ppjwa.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hzi.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://dxf.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://nqw.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://bch.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ayq.jlsjyb.cn

[A03] 常量定义
来源：http://yie.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xmb.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://bvc.yongpay.top

JS:   const PI = 3.14159;
来源：http://abd.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://ztb.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://inm.yuanzhike.top

Go:   const PI = 3.14159
来源：http://gjt.haohaochexian.top

Ruby: PI = 3.14159
来源：http://lzd.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://arl.ctjpmb.com

[A04] 判断变量类型
来源：http://shz.ppjwa.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cph.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mfg.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fsu.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://wgr.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ssz.sufxvd.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ywv.uphjek.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ele.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://wit.yueranfly.top

[A05] 整数除法与取模
来源：http://dkl.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ohm.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uez.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xwt.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bwr.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://mce.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://acd.jiagoushi.top

Ruby: 7 / 2; 7 % 2
来源：http://jaq.xinyue.icu

C#:   7 / 2; 7 % 2
来源：http://qtx.zhongyouzk.top

[A06] 字符串转数字
来源：http://fap.uphjek.com

Py:   int("42"); float("3.14")
来源：http://wja.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://umj.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jwc.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ejl.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://stl.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://snk.havefunace.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mpg.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bdy.yj20258.top

[A07] 数字转字符串
来源：http://pjh.jinyuanbaomall.cn

Py:   str(42)
来源：http://wcj.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://bch.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://aok.birdmap.top

TS:   String(42)
来源：http://gem.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nyu.yfazqb.com

Go:   strconv.Itoa(42)
来源：http://teu.redwolf501.top

Ruby: 42.to_s
来源：http://zdk.hammf.cn

C#:   42.ToString()
来源：http://ado.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://gdb.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hfu.ivvv.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rgh.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zda.jianghu66.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jwd.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://drc.svipenyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jvk.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zor.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gpt.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://irk.yj20258888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://prl.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ycv.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ywc.nwbrower.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ydh.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nsk.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ukf.smart0.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ugg.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://biy.52xcode.cn

[A10] 生成随机数
来源：http://ztz.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://qhz.yonumen.top

PHP:  random_int(1, 100);
来源：http://anz.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uwt.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rba.cqqwz.cn

Java: new Random().nextInt(100) + 1
来源：http://fbx.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wxf.52xcode.cn

Ruby: rand(1..100)
来源：http://ldt.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://qik.ywan-chungtsiang.top

[A11] 条件表达式（三元）
来源：http://fym.tarul.cn

Py:   "yes" if x > 0 else "no"
来源：http://giy.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iqu.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ezp.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://evo.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://veb.shanyushiyangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://thr.chenlongwang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qzm.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bcc.cheryme.top

[A12] 字符串插值 / 格式化
来源：http://apv.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cab.haohaochexian.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ngb.sufxvd.cn

JS:   `Hello, ${name}!`
来源：http://vvy.yongpay.top

TS:   `Hello, ${name}!`
来源：http://ddt.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://wup.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kkx.sweek.top

Ruby: "Hello, #{name}!"
来源：http://ypf.pycfn.com

C#:   $"Hello, {name}!"
来源：http://leb.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lfk.yvedp.cn

Py:   "第一行\n第二行"
来源：http://job.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://him.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://bxb.yvedp.cn

TS:   "第一行\n第二行"
来源：http://fdw.bjfxy.top


<!-- 参考信息 -->