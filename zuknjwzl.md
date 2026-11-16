代发 wailian999

[U81] JS：初始化项目
来源：http://tma.hysaishi.cn

npm init -y;  npm i express
来源：http://adj.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://cdk.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xkr.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://eod.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://ily.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://wbc.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://gkd.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://tgq.jinyuanbaomall.cn

a?.b?.c
来源：http://zgb.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://ala.zhongyouzk.top

a ?? b
来源：http://rlr.52xcode.cn

[U87] JS：解构默认值
来源：http://fxr.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://bgv.wangdashe.top

[U88] JS：对象展开合并
来源：http://fzr.ywan-chungtsiang.top

{ ...a, ...b }
来源：http://gct.hammf.cn

[U89] JS：数组去重
来源：http://odw.pycfn.com

[...new Set(arr)]
来源：http://agz.chenzaomai.com

[U90] JS：数字数组排序
来源：http://ybk.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://dwc.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://uuw.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ffq.hnqzz.top

[U92] JS：深拷贝
来源：http://jws.pycfn.com

structuredClone(obj)
来源：http://rvl.sufxvd.cn

[U93] JS：模板字符串
来源：http://azr.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://nqe.zdbjq.cn

[U94] JS：箭头函数
来源：http://kux.sxryk.cn

const double = x => x * 2;
来源：http://bld.chenlongwang.top

[U95] JS：Promise 包装
来源：http://fyu.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://ogk.mhx1999.top

[U96] JS：async/await 与异常
来源：http://aia.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cjb.tian-w.cn

[U97] JS：并发请求
来源：http://kdy.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zzq.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://tkr.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ake.sufxvd.cn

[U99] JS：事件监听
来源：http://bun.tarul.cn

el.addEventListener("click", e => {})
来源：http://tvm.ydzc1.top

[U100] JS：DOM 查询
来源：http://ife.nanxinkj.top

document.querySelector(".item")
来源：http://dvd.zycfv.cn

[U101] JS：classList 操作
来源：http://vuz.gaohongyu789.top

el.classList.toggle("active")
来源：http://vmr.shangyingyoupin.top

[U102] JS：本地存储
来源：http://fgj.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fav.nanxinkj.top

[U103] JS：定时器
来源：http://tgt.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://krg.jiagoushi.top

[U104] JS：防抖
来源：http://hlo.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygm.fktsv.cn

[U105] JS：节流
来源：http://krx.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pse.redwolf501.top

[U106] JS：日期格式化
来源：http://hye.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hcd.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://zzw.cucudq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bqb.birdmap.top

[U108] JS：随机整数
来源：http://lds.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jjq.vqdsnc.cn

[U109] JS：数组分组
来源：http://luv.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://vxa.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://igo.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gtg.yj20258888.top

[U111] JS：对象转 Map
来源：http://ine.0kj1m.cn

new Map(Object.entries(obj))
来源：http://xuz.yangfankeji.com

[U112] JS：字符串补位
来源：http://vwk.fehbvm.com

"7".padStart(3, "0")
来源：http://vhz.cheryme.top

[U113] JS：正则替换全部
来源：http://qlt.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://jug.andypj.xyz

[U114] JS：JSON 深比较
来源：http://hii.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ykj.yuanzhike.top

[U115] JS：生成 UUID
来源：http://tgi.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://ezb.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://gvi.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://day.zhiwuduotai.top

[U117] JS：单元测试
来源：http://nuz.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://zax.hywenlv.cn

[U118] JS：开发服务器
来源：http://vbn.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://rug.cqqwz.cn

[U119] JS：生产构建
来源：http://xgf.chenzaomai.com

npx vite build
来源：http://eyc.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://dli.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://enx.fehbvm.com

================================================================================
来源：http://wpd.kuanghao11.cn

统计汇总
来源：http://nzq.shuidangran.top

================================================================================
来源：http://ywk.hnxiangtu.top

按语言统计（条）：
来源：http://ipo.sysykeji.top

Python ......... 252
来源：http://qkm.tarul.cn

PHP ............ 252
来源：http://kqs.havefunace.top

JavaScript ..... 252
来源：http://gxb.yueranfly.top

TypeScript ..... 212
来源：http://vnn.havefunace.top

Java ........... 212
来源：http://iah.jinqigfzy.top

Go ............. 212
来源：http://ttq.tarul.cn

Ruby ........... 212
来源：http://vfl.kuanghao11.cn

C# ............. 212
来源：http://vxi.ybcxt.top

C .............. 30
来源：http://vvs.hcnkem.com

C++ ............ 30
来源：http://api.daria6918.cn

SQL ............ 90
来源：http://ptk.dianchejie.cn

Bash ........... 80
来源：http://ukh.bbcook.cn

Kotlin ......... 15
来源：http://qov.jlsjyb.cn

Swift .......... 15
来源：http://siy.yvedp.cn

Lua ............ 10
来源：http://hik.yj202588.top

Perl ........... 10
来源：http://omh.zhaomingkeji.xyz

Scala .......... 10
来源：http://brk.c1oappe.top

------------------------------------
来源：http://hkv.iojbl.cn

合计 ........... 2106 条
来源：http://xzr.gzhubu.top

按章节统计：
来源：http://ybx.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zmy.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bcd.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aqi.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ckt.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mqz.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qwm.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kwz.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vfl.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://exm.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ggs.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wlb.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wzf.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sso.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ici.aizwys.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aau.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://noa.bjfxy.top

Q SQL 专题                              90
来源：http://tjq.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://ens.yj202588.top

S C / C++ 专题                          60
来源：http://qxc.snrcjt.cn

T 其他语言补充                          60
来源：http://mnd.ydzc1.top

U 高频实用片段                         120
来源：http://fgv.nanxuanxn.top

------------------------------------
来源：http://lrq.316326.xyz

合计                                  2106 条
来源：http://qfp.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ove.yongpay.top

使用提醒
来源：http://fvd.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://cxc.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gxz.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tiv.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ylq.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fuz.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xgx.gotoacloud.top

—— 文件结束 ——
来源：http://bxn.cheryme.top

================================================================================
来源：http://ulf.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://htm.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://mrw.zhixingplan.top

================================================================================
来源：http://huk.hammf.cn

【收录内容】
来源：http://qsi.zhiwuduotai.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kqo.sweek.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zev.cucudq.cn

SQL · Bash · C · C++
来源：http://zvy.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kzu.zhiwuduotai.top

【使用说明】
来源：http://flz.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hhb.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://igb.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bcn.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oky.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qmv.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xqb.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://igf.cheryme.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xhk.hnqzz.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bnf.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wyv.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ldn.jqgfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zsi.xylfe.cn

【文件统计】
来源：http://zuj.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qru.smart0.xyz

--------------------------------------------------------------------------------
来源：http://syb.zhengqikj.top

目  录
来源：http://ugk.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://lqw.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vta.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qnd.shuidangran.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://khn.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ebc.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qwe.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xet.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lbx.fktsv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://noz.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xyq.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dxe.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xef.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://akt.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vhe.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://not.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qqa.chenlongwang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kcg.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://upq.xingfuxueyuan.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://gip.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jwz.bbcook.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cxz.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mdz.jyoumei.cn

================================================================================
来源：http://tqt.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://wph.meibo888.top

================================================================================
来源：http://hlr.0kj1m.cn

[A01] Hello World
来源：http://aya.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://toc.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://svf.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://rjz.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sbh.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://jmb.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://zto.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://qzp.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xch.fktsv.cn

[A02] 变量声明与赋值
来源：http://qqc.epnwcf.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tnh.jianghu66.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qih.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://anz.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kgy.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://muq.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://sxv.jinqigufen.top

Ruby: name = "Alex"; age = 20
来源：http://lfm.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nbu.snrcjt.cn

[A03] 常量定义
来源：http://fyp.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zpw.shangyingyoupin.top

PHP:  const PI = 3.14159;
来源：http://oms.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://vee.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://cnj.xingfuxueyuan.xyz

Java: static final double PI = 3.14159;
来源：http://has.chenlongwang.top

Go:   const PI = 3.14159
来源：http://goz.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://ooz.zhoulong.xyz

C#:   const double PI = 3.14159;
来源：http://rfv.smart0.xyz

[A04] 判断变量类型
来源：http://rch.wangshuangyany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jht.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://quk.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://teo.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://ovr.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ohc.nanxinkj.top

Go:   reflect.TypeOf(x).Name()
来源：http://kty.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://gui.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://wny.tarul.cn

[A05] 整数除法与取模
来源：http://trq.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vuy.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://oka.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cih.epnwcf.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xib.bjfxy.top

Java: 7 / 2; 7 % 2
来源：http://sre.xuetiantiany.cn

Go:   7 / 2; 7 % 2
来源：http://fep.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://chu.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://pwz.9152youxi.cn

[A06] 字符串转数字
来源：http://umm.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://kcl.wangdashe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://knr.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wxl.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://dqs.yongpay.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rgk.cheryme.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wst.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cbz.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://azk.xuetiantiany.cn

[A07] 数字转字符串
来源：http://wxu.dianchejie.cn

Py:   str(42)
来源：http://ujh.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://pln.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://xnp.jinghuilouyu.cn

TS:   String(42)
来源：http://lii.yvedp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hau.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://efm.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://ngw.zhaomingkeji.xyz

C#:   42.ToString()
来源：http://det.ydzc1.top

[A08] 取整与四舍五入
来源：http://ylo.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cwd.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rlo.aibaodan.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://squ.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kte.chenjidiqi.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wtx.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nvj.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://tnl.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yye.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://gzv.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zhl.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://leg.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lrt.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://frr.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kyt.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ucz.aibaodan.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hjt.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://irn.tianlin.xyz

[A10] 生成随机数
来源：http://oat.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://bsi.gzhubu.top

PHP:  random_int(1, 100);
来源：http://vsd.yonumen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tht.kuanghao11.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://euy.hongshengwenyu.top

Java: new Random().nextInt(100) + 1
来源：http://twa.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rix.jqgfzy.top

Ruby: rand(1..100)
来源：http://ffz.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://vfq.yongpay.top

[A11] 条件表达式（三元）
来源：http://fen.meibo888.top

Py:   "yes" if x > 0 else "no"
来源：http://cwu.9152youxi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vmj.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kfc.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://vcp.ybcxt.top

Java: x > 0 ? "yes" : "no"
来源：http://asd.ydjk.org.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wfy.fengsongda.top

Ruby: x > 0 ? "yes" : "no"
来源：http://efe.uphjek.com

C#:   x > 0 ? "yes" : "no"
来源：http://igg.ywan-chungtsiang.top

[A12] 字符串插值 / 格式化
来源：http://npu.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://abg.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fyy.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://wwk.yj202588.top

TS:   `Hello, ${name}!`
来源：http://eqx.tianlin.xyz

Java: "Hello, %s!".formatted(name)
来源：http://bff.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://odk.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://ojj.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://ssb.yj20258.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yzu.cheryme.top

Py:   "第一行\n第二行"
来源：http://mhh.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://olu.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://fno.yongpay.top

TS:   "第一行\n第二行"
来源：http://npw.zhoulong.xyz


<!-- 参考信息 -->