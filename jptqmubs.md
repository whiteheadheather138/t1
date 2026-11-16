代发 wailian999

[U81] JS：初始化项目
来源：http://uvw.gotoacloud.top

npm init -y;  npm i express
来源：http://bmn.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://byp.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xxp.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://zar.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://bdc.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://fvq.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iop.havefunace.top

[U85] JS：可选链
来源：http://atf.jqgufenzy.top

a?.b?.c
来源：http://qex.guowangkeji.top

[U86] JS：空值合并
来源：http://jwc.fehbvm.com

a ?? b
来源：http://mae.hammf.cn

[U87] JS：解构默认值
来源：http://pix.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://sfz.gzhubu.top

[U88] JS：对象展开合并
来源：http://wng.haohaochexian.top

{ ...a, ...b }
来源：http://hrf.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://xho.c1oappe.top

[...new Set(arr)]
来源：http://vqg.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://lxu.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://cql.yfazqb.com

[U91] JS：对象键值遍历
来源：http://qqh.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hky.sjlbkw.cn

[U92] JS：深拷贝
来源：http://mez.guannengcc.top

structuredClone(obj)
来源：http://zmp.0kj1m.cn

[U93] JS：模板字符串
来源：http://fii.yuanzhike.top

`共 ${n} 条`
来源：http://uin.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://xsz.yongpay.top

const double = x => x * 2;
来源：http://wyu.sysykeji.top

[U95] JS：Promise 包装
来源：http://whl.yongpay.top

new Promise((resolve, reject) => {})
来源：http://rqh.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://vzk.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rmd.epnwcf.com

[U97] JS：并发请求
来源：http://wkv.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qud.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://uke.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fre.meibo888.top

[U99] JS：事件监听
来源：http://pua.fktsv.cn

el.addEventListener("click", e => {})
来源：http://tty.yangfankeji.com

[U100] JS：DOM 查询
来源：http://sww.yj20258.top

document.querySelector(".item")
来源：http://dyl.redwolf501.top

[U101] JS：classList 操作
来源：http://cnt.hcnkem.com

el.classList.toggle("active")
来源：http://gab.jiagoushi.top

[U102] JS：本地存储
来源：http://xge.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xyg.jlsjyb.cn

[U103] JS：定时器
来源：http://afs.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://djx.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://pyv.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rlr.jlsjyb.cn

[U105] JS：节流
来源：http://ebl.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kug.nwbrower.top

[U106] JS：日期格式化
来源：http://rop.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uhc.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://vfi.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jjm.tianlin.xyz

[U108] JS：随机整数
来源：http://rpy.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://anc.guannengcc.top

[U109] JS：数组分组
来源：http://cck.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://nes.yfazqb.com

[U110] JS：数组分块
来源：http://fkp.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://che.sxryk.cn

[U111] JS：对象转 Map
来源：http://gkf.zhixingplan.top

new Map(Object.entries(obj))
来源：http://wfb.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://wng.quarkkingdee.top

"7".padStart(3, "0")
来源：http://ess.xziqi.cn

[U113] JS：正则替换全部
来源：http://vrt.yongpay.top

s.replaceAll("a", "b")
来源：http://tli.fzhhl.top

[U114] JS：JSON 深比较
来源：http://ttb.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yyx.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://vvn.nanxuanxn.top

crypto.randomUUID()
来源：http://suc.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://qoo.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://htw.svipenyu.cn

[U117] JS：单元测试
来源：http://wqm.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://ipl.cdnleiting.top

[U118] JS：开发服务器
来源：http://fmf.yuanzhike.top

npm i -D vite;  npx vite
来源：http://qzq.jyoumei.cn

[U119] JS：生产构建
来源：http://ebc.wangshuangyany.cn

npx vite build
来源：http://jco.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://gne.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://lql.zdqjudy.top

================================================================================
来源：http://aox.yvedp.cn

统计汇总
来源：http://evp.tian-w.cn

================================================================================
来源：http://civ.yuxming.cn

按语言统计（条）：
来源：http://evl.jiagoushi.top

Python ......... 252
来源：http://zgc.yvedp.cn

PHP ............ 252
来源：http://ifm.nwbrower.top

JavaScript ..... 252
来源：http://fjz.guannengcc.top

TypeScript ..... 212
来源：http://yyq.zdbjq.cn

Java ........... 212
来源：http://yxy.cdnleiting.top

Go ............. 212
来源：http://tgb.fktsv.cn

Ruby ........... 212
来源：http://dnz.shanyushiyangkeji.top

C# ............. 212
来源：http://yvf.52xcode.cn

C .............. 30
来源：http://pwa.xingfuxueyuan.xyz

C++ ............ 30
来源：http://uat.fehbvm.com

SQL ............ 90
来源：http://buh.yonumen.top

Bash ........... 80
来源：http://vqb.zhongyouzk.top

Kotlin ......... 15
来源：http://sqq.xziqi.cn

Swift .......... 15
来源：http://edk.ydjk.org.cn

Lua ............ 10
来源：http://sta.hnqzz.top

Perl ........... 10
来源：http://rjy.bjfxy.top

Scala .......... 10
来源：http://omh.yanxiufei.cn

------------------------------------
来源：http://kxo.jqgfzy.top

合计 ........... 2106 条
来源：http://ytm.chenlongwang.top

按章节统计：
来源：http://slz.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bpc.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dua.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vnt.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xqt.yanxiufei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jey.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bhx.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ffw.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gmn.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://azz.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wsg.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rds.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vad.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mfh.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nwx.wangshuangyany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oyd.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gyl.hammf.cn

Q SQL 专题                              90
来源：http://aea.yfazqb.com

R Bash 专题                             80
来源：http://zmt.yvedp.cn

S C / C++ 专题                          60
来源：http://dgf.xuetiantiany.cn

T 其他语言补充                          60
来源：http://tit.c1oappe.top

U 高频实用片段                         120
来源：http://eqm.feifeiyinyue.top

------------------------------------
来源：http://qcp.ywan-chungtsiang.top

合计                                  2106 条
来源：http://btd.smart0.xyz

--------------------------------------------------------------------------------
来源：http://uaf.cheryme.top

使用提醒
来源：http://wxz.nwbrower.top

--------------------------------------------------------------------------------
来源：http://xay.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ikm.uphjek.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tvt.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qmy.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://zqz.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://daa.cqqwz.cn

—— 文件结束 ——
来源：http://hjr.zhongyouzk.top

================================================================================
来源：http://zyt.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://aqe.yangfankeji.com

Common Programming Examples Cheat Book
来源：http://zjo.aizwys.cn

================================================================================
来源：http://qye.sweek.top

【收录内容】
来源：http://abu.xinyue.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://oun.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eba.jinghuilouyu.cn

SQL · Bash · C · C++
来源：http://krl.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tvy.iojbl.cn

【使用说明】
来源：http://beh.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qiu.jiagoushi.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tkw.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vuf.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://drd.zycfv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wrw.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uew.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uze.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xue.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pyz.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gic.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cpp.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ldo.zhaomingkeji.xyz

【文件统计】
来源：http://vbn.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xti.yongpay.top

--------------------------------------------------------------------------------
来源：http://ilc.jinqigufen.top

目  录
来源：http://mmq.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://ixm.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tge.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ofd.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aoc.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iud.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://myf.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fyc.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bob.shzxlz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vaa.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://reg.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://slh.zhengqikj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://age.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sun.sxryk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://chd.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sar.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ukr.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zzt.pycfn.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qcb.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://rpp.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://adp.fzhhl.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gzp.ivvv.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zpa.shanyushiyangkeji.top

================================================================================
来源：http://lue.hesvh.cn

A. 基础语法与类型
来源：http://tkv.sjlbkw.cn

================================================================================
来源：http://qzn.jlsjyb.cn

[A01] Hello World
来源：http://cde.jqgfzy.top

Py:   print("Hello, World!")
来源：http://cqw.cucudq.cn

PHP:  echo "Hello, World!";
来源：http://jdd.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://xja.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bfb.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://kuy.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://dul.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://srz.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://voy.tianlin.xyz

[A02] 变量声明与赋值
来源：http://nlr.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://scf.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sfd.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gtw.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lmp.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://yat.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://njm.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://zaw.pengpengdd.cyou

C#:   string name = "Alex"; int age = 20;
来源：http://oou.gogol.net.cn

[A03] 常量定义
来源：http://kww.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vtt.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://wpw.tanke756.top

JS:   const PI = 3.14159;
来源：http://osn.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://vrj.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://eze.yongpay.top

Go:   const PI = 3.14159
来源：http://jyi.vehdjk.com

Ruby: PI = 3.14159
来源：http://cba.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://xiy.wangshuangyany.cn

[A04] 判断变量类型
来源：http://alj.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://olr.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wrd.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tlo.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://uuw.gaohongyu789.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jdk.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://hvo.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tbi.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://cey.yfazqb.com

[A05] 整数除法与取模
来源：http://ckl.hfpthk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ebr.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iwa.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uaf.shuidangran.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pgx.shzxlz.cn

Java: 7 / 2; 7 % 2
来源：http://idv.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://fib.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://xto.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://xyi.hysaishi.cn

[A06] 字符串转数字
来源：http://nlb.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://mqd.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nkv.gotoacloud.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nfv.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://let.yangfankeji.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lnf.fzhhl.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gim.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oqi.jlsjyb.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fuk.yanxiufei.cn

[A07] 数字转字符串
来源：http://uar.haohaochexian.top

Py:   str(42)
来源：http://ajf.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://ljk.cheryme.top

JS:   String(42); (42).toString()
来源：http://wca.xziqi.cn

TS:   String(42)
来源：http://rbv.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://duw.pycfn.com

Go:   strconv.Itoa(42)
来源：http://fzs.xylfe.cn

Ruby: 42.to_s
来源：http://cfg.xuanzx.com

C#:   42.ToString()
来源：http://tbv.yongpay.top

[A08] 取整与四舍五入
来源：http://pxg.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kyl.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ygp.wangshuangyany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://msk.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ozb.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zja.aizwys.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://idi.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nlz.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://krr.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://qzv.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zed.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cgu.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gag.c1oappe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zhn.jinqigufen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lfu.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lsq.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lxw.fzhhl.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ewl.ppjwa.cn

[A10] 生成随机数
来源：http://mac.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://afs.ppjwa.cn

PHP:  random_int(1, 100);
来源：http://mya.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ama.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xbr.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://wza.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ivb.tianlin.xyz

Ruby: rand(1..100)
来源：http://qld.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://twd.fktsv.cn

[A11] 条件表达式（三元）
来源：http://goy.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://loa.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tde.jinghuilouyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fnv.jinqigufen.top

TS:   x > 0 ? "yes" : "no"
来源：http://foy.hesvh.cn

Java: x > 0 ? "yes" : "no"
来源：http://ube.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dsc.cqqwz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ylg.jiagoushi.top

C#:   x > 0 ? "yes" : "no"
来源：http://jky.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://mcz.0kj1m.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rzq.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://daw.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://rpb.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://hmz.fehbvm.com

Java: "Hello, %s!".formatted(name)
来源：http://hfy.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gzr.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://aql.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://wus.sweek.top

[A13] 多行字符串（练习 \n 转义）
来源：http://woh.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://xgm.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://nrq.fzhhl.top

JS:   "第一行\n第二行"
来源：http://vwn.vqdsnc.cn

TS:   "第一行\n第二行"
来源：http://bfi.tarul.cn


<!-- 参考信息 -->