代发 wailian999

[U81] JS：初始化项目
来源：http://ygc.guannengcc.top

npm init -y;  npm i express
来源：http://axz.wangdashe.top

[U82] JS：package.json 脚本
来源：http://pym.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://csj.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://vzd.shanyushiyangtech.top

export const a = 1;  import { a } from "./m.js";
来源：http://lvk.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://phr.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ufm.yj20258.top

[U85] JS：可选链
来源：http://jpt.jqgfzy.top

a?.b?.c
来源：http://rwj.vqdsnc.cn

[U86] JS：空值合并
来源：http://ghs.xuanzx.com

a ?? b
来源：http://jmg.epnwcf.com

[U87] JS：解构默认值
来源：http://lhd.pycfn.com

const { a = 1, b = 2 } = obj;
来源：http://rpl.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://mot.shzxlz.cn

{ ...a, ...b }
来源：http://fwe.nanxinkj.top

[U89] JS：数组去重
来源：http://rns.hysaishi.cn

[...new Set(arr)]
来源：http://mys.xuanzx.com

[U90] JS：数字数组排序
来源：http://zlv.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://ouz.uphjek.com

[U91] JS：对象键值遍历
来源：http://ksr.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dpc.xziqi.cn

[U92] JS：深拷贝
来源：http://izz.fanxiaobao.xyz

structuredClone(obj)
来源：http://qmz.snrcjt.cn

[U93] JS：模板字符串
来源：http://itv.ivvv.top

`共 ${n} 条`
来源：http://bvl.fehbvm.com

[U94] JS：箭头函数
来源：http://lcv.yueranfly.top

const double = x => x * 2;
来源：http://tni.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://mwe.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://edm.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://vxa.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kbi.shzxlz.cn

[U97] JS：并发请求
来源：http://hdz.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://hnp.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://mwy.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ijs.haohaochexian.top

[U99] JS：事件监听
来源：http://jry.c1oappe.top

el.addEventListener("click", e => {})
来源：http://ckm.dashuyun.cn

[U100] JS：DOM 查询
来源：http://rrr.havefunace.top

document.querySelector(".item")
来源：http://vme.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://foh.guannengcc.top

el.classList.toggle("active")
来源：http://tfm.kuanghao11.cn

[U102] JS：本地存储
来源：http://foj.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://euh.zhiwuduotai.top

[U103] JS：定时器
来源：http://gow.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wrm.zhongyouzk.top

[U104] JS：防抖
来源：http://gvx.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ora.guowangkeji.top

[U105] JS：节流
来源：http://oyb.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nfd.zdbjq.cn

[U106] JS：日期格式化
来源：http://ehg.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://twf.hfpthk.cn

[U107] JS：数字千分位
来源：http://hqz.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ofb.ivvv.top

[U108] JS：随机整数
来源：http://ayj.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rvj.tanke756.top

[U109] JS：数组分组
来源：http://esk.gzhubu.top

Object.groupBy(arr, x => x.type)
来源：http://fkl.fengsongda.top

[U110] JS：数组分块
来源：http://lqb.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zgv.jqgfzy.top

[U111] JS：对象转 Map
来源：http://ntv.fehbvm.com

new Map(Object.entries(obj))
来源：http://awo.ydjk.org.cn

[U112] JS：字符串补位
来源：http://pyz.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://lua.ivvv.top

[U113] JS：正则替换全部
来源：http://tbz.sysykeji.top

s.replaceAll("a", "b")
来源：http://xwa.aizwys.cn

[U114] JS：JSON 深比较
来源：http://tmf.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ipj.shzxlz.cn

[U115] JS：生成 UUID
来源：http://iqe.jinqigufen.top

crypto.randomUUID()
来源：http://vkq.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://gya.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://edk.jiagoushi.top

[U117] JS：单元测试
来源：http://ztv.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://qqi.haohaochexian.top

[U118] JS：开发服务器
来源：http://sfr.bbcook.cn

npm i -D vite;  npx vite
来源：http://waw.redwolf501.top

[U119] JS：生产构建
来源：http://ifq.smart0.xyz

npx vite build
来源：http://ghe.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://dbe.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://heb.wangshuangyany.cn

================================================================================
来源：http://sad.wangshuangyany.cn

统计汇总
来源：http://ieo.zhijiandao.cn

================================================================================
来源：http://jiy.fanxiaobao.xyz

按语言统计（条）：
来源：http://ihu.0kj1m.cn

Python ......... 252
来源：http://eti.ydjk.org.cn

PHP ............ 252
来源：http://sps.gzhubu.top

JavaScript ..... 252
来源：http://alg.ppjwa.cn

TypeScript ..... 212
来源：http://gcq.hnqzz.top

Java ........... 212
来源：http://vzx.guannengcc.top

Go ............. 212
来源：http://rqr.tianlin.xyz

Ruby ........... 212
来源：http://afm.meibo888.top

C# ............. 212
来源：http://ivi.smart0.xyz

C .............. 30
来源：http://mrf.yj20258.top

C++ ............ 30
来源：http://jvy.cucudq.cn

SQL ............ 90
来源：http://xkb.guowangkeji.top

Bash ........... 80
来源：http://yrl.cheryme.top

Kotlin ......... 15
来源：http://gco.fzhhl.top

Swift .......... 15
来源：http://zxo.jinqigufen.top

Lua ............ 10
来源：http://smj.meibo888.top

Perl ........... 10
来源：http://pop.yj20258888.top

Scala .......... 10
来源：http://kkq.hnqzz.top

------------------------------------
来源：http://lwu.cdnleiting.top

合计 ........... 2106 条
来源：http://weo.jinyuanbaomall.cn

按章节统计：
来源：http://kmc.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kte.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eae.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vyh.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xcc.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pxh.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qax.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fun.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jtf.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pqt.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://njv.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://arm.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yvu.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bkv.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zxs.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xph.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://adw.cqqwz.cn

Q SQL 专题                              90
来源：http://frc.birdmap.top

R Bash 专题                             80
来源：http://fvj.jqgufenzy.top

S C / C++ 专题                          60
来源：http://tyl.guowangkeji.top

T 其他语言补充                          60
来源：http://rkx.cqqwz.cn

U 高频实用片段                         120
来源：http://dhh.hongshengwenyu.top

------------------------------------
来源：http://tgo.0kj1m.cn

合计                                  2106 条
来源：http://dvl.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://afx.sxryk.cn

使用提醒
来源：http://ofo.uphjek.com

--------------------------------------------------------------------------------
来源：http://abs.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ljb.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wtk.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kdg.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jdc.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wgs.quarkkingdee.top

—— 文件结束 ——
来源：http://txz.chenlongwang.top

================================================================================
来源：http://zpw.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://jzy.aizwys.cn

Common Programming Examples Cheat Book
来源：http://eto.zhengqikj.top

================================================================================
来源：http://tlc.yanxiufei.cn

【收录内容】
来源：http://yrp.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://upq.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cfh.hnqzz.top

SQL · Bash · C · C++
来源：http://auw.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uoo.hywenlv.cn

【使用说明】
来源：http://dvv.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pyc.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://apy.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rdk.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://phj.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hxp.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://irl.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xcc.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uyb.chenzaomai.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jtw.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sro.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qjr.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rwv.kuanghao11.cn

【文件统计】
来源：http://klj.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fyl.yj202588.top

--------------------------------------------------------------------------------
来源：http://vsu.zdqjudy.top

目  录
来源：http://kzt.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://yje.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cuz.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hmx.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lvx.c1oappe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cff.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cxs.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pqq.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fgr.yj20258.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://png.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iwe.gotoacloud.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lbc.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ieq.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tvo.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uwc.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://enz.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wlp.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rku.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kdw.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://itd.zhaomingkeji.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qrj.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kmx.ctjpmb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ygv.aizwys.cn

================================================================================
来源：http://zop.hammf.cn

A. 基础语法与类型
来源：http://dgx.ctjpmb.com

================================================================================
来源：http://bco.yvedp.cn

[A01] Hello World
来源：http://jzt.daria6918.cn

Py:   print("Hello, World!")
来源：http://urm.ivvv.top

PHP:  echo "Hello, World!";
来源：http://uus.vqdsnc.cn

JS:   console.log("Hello, World!");
来源：http://cul.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wyp.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://qoo.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://sjt.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://chq.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ney.shzxlz.cn

[A02] 变量声明与赋值
来源：http://tog.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jat.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jvp.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wzn.yongpay.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bbj.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://ljr.sweek.top

Go:   name := "Alex"; age := 20
来源：http://oxe.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://tqw.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hvt.tianlin.xyz

[A03] 常量定义
来源：http://oqb.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yuo.tarul.cn

PHP:  const PI = 3.14159;
来源：http://gwq.sweek.top

JS:   const PI = 3.14159;
来源：http://gxo.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://zxt.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://vkm.hywenlv.cn

Go:   const PI = 3.14159
来源：http://mir.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://uqd.uphjek.com

C#:   const double PI = 3.14159;
来源：http://nfy.havefunace.top

[A04] 判断变量类型
来源：http://xko.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vux.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gvu.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sxy.nanxuanxn.top

TS:   typeof x; x instanceof Date
来源：http://eco.cucudq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tvd.redwolf501.top

Go:   reflect.TypeOf(x).Name()
来源：http://aqa.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jcm.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://rph.epnwcf.com

[A05] 整数除法与取模
来源：http://ocr.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ftf.yj20258.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://chm.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bsc.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lus.yuanzhike.top

Java: 7 / 2; 7 % 2
来源：http://cxj.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://vch.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://deg.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://vym.yfazqb.com

[A06] 字符串转数字
来源：http://ciw.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://sef.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tzp.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jfm.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://wnc.jinqigfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cxf.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uoj.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://her.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ayo.zhengqikj.top

[A07] 数字转字符串
来源：http://ejl.jinqigufen.top

Py:   str(42)
来源：http://dkm.nwbrower.top

PHP:  (string) 42; strval(42)
来源：http://ofl.nwbrower.top

JS:   String(42); (42).toString()
来源：http://hbs.yuanzhike.top

TS:   String(42)
来源：http://qkc.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hrs.yonumen.top

Go:   strconv.Itoa(42)
来源：http://xwt.sxryk.cn

Ruby: 42.to_s
来源：http://btn.pycfn.com

C#:   42.ToString()
来源：http://bom.316326.xyz

[A08] 取整与四舍五入
来源：http://dje.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://coq.jianghu66.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fbs.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gui.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hys.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://obo.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ykn.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://vqo.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ect.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://ype.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blo.zhoulong.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zqa.guannengcc.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cvm.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uhy.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bjr.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sxg.hywenlv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ghx.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ygf.wangdashe.top

[A10] 生成随机数
来源：http://bco.yangfankeji.com

Py:   import random; random.randint(1, 100)
来源：http://ahj.9152youxi.cn

PHP:  random_int(1, 100);
来源：http://vbo.daxiang520.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ebc.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bym.sweek.top

Java: new Random().nextInt(100) + 1
来源：http://mvr.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fiv.xziqi.cn

Ruby: rand(1..100)
来源：http://nqu.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://prk.cqqwz.cn

[A11] 条件表达式（三元）
来源：http://foc.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://ktd.ctjpmb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://sax.snrcjt.cn

JS:   x > 0 ? "yes" : "no"
来源：http://way.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://rik.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://utu.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://nqe.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://bfe.xinyue.icu

C#:   x > 0 ? "yes" : "no"
来源：http://gvr.pycfn.com

[A12] 字符串插值 / 格式化
来源：http://ndz.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qch.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://srm.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://lib.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://mey.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://jzj.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jkt.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://xxy.vehdjk.com

C#:   $"Hello, {name}!"
来源：http://lye.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://okl.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://zvm.tian-w.cn

PHP:  "第一行\n第二行"
来源：http://vbq.epnwcf.com

JS:   "第一行\n第二行"
来源：http://mnx.ydzc1.top

TS:   "第一行\n第二行"
来源：http://xja.gogol.net.cn


<!-- 参考信息 -->