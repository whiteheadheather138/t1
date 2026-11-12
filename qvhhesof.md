代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://skc.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kfr.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://lxq.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://kbi.dianchejie.cn

[U85] JS：可选链
来源：http://cyu.hnqzz.top

a?.b?.c
来源：http://ice.sufxvd.cn

[U86] JS：空值合并
来源：http://gcu.cdnleiting.top

a ?? b
来源：http://ahp.zhijiandao.cn

[U87] JS：解构默认值
来源：http://zuq.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://ctq.dashuyun.cn

[U88] JS：对象展开合并
来源：http://cyr.chenjidiqi.icu

{ ...a, ...b }
来源：http://jgo.nanxuanxn.top

[U89] JS：数组去重
来源：http://jca.xziqi.cn

[...new Set(arr)]
来源：http://ucl.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://djt.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://bvk.chenlongwang.top

[U91] JS：对象键值遍历
来源：http://kyj.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jsx.smart0.xyz

[U92] JS：深拷贝
来源：http://vap.yonumen.top

structuredClone(obj)
来源：http://ebk.xylfe.cn

[U93] JS：模板字符串
来源：http://gtf.gzhubu.top

`共 ${n} 条`
来源：http://cff.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://eun.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://jxb.yvedp.cn

[U95] JS：Promise 包装
来源：http://fny.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://ssz.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://trc.zhijiandao.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uvv.yonumen.top

[U97] JS：并发请求
来源：http://sfm.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uxs.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://agq.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hmb.guannengcc.top

[U99] JS：事件监听
来源：http://ope.fengsongda.top

el.addEventListener("click", e => {})
来源：http://asv.gzhubu.top

[U100] JS：DOM 查询
来源：http://xhr.cashguo.top

document.querySelector(".item")
来源：http://nkf.yuxming.cn

[U101] JS：classList 操作
来源：http://dyh.zhongyouzk.top

el.classList.toggle("active")
来源：http://kir.zhoulong.xyz

[U102] JS：本地存储
来源：http://lnl.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://amg.havefunace.top

[U103] JS：定时器
来源：http://qwj.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vmi.0kj1m.cn

[U104] JS：防抖
来源：http://smu.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wuj.guowangkeji.top

[U105] JS：节流
来源：http://bdp.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jzp.zhixingplan.top

[U106] JS：日期格式化
来源：http://rto.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iwn.jqgufenzy.top

[U107] JS：数字千分位
来源：http://uwv.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vmg.sjlbkw.cn

[U108] JS：随机整数
来源：http://nsh.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rxa.ydjk.org.cn

[U109] JS：数组分组
来源：http://fwi.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://sbd.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://orj.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khz.shuidangran.top

[U111] JS：对象转 Map
来源：http://oiy.mhx1999.top

new Map(Object.entries(obj))
来源：http://qii.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://okx.0kj1m.cn

"7".padStart(3, "0")
来源：http://mgp.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://ato.ydzc1.top

s.replaceAll("a", "b")
来源：http://vep.cucudq.cn

[U114] JS：JSON 深比较
来源：http://hpd.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sid.pycfn.com

[U115] JS：生成 UUID
来源：http://cue.shuidangran.top

crypto.randomUUID()
来源：http://vbz.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://rjp.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://ajx.redwolf501.top

[U117] JS：单元测试
来源：http://ktj.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://dce.hnxiangtu.top

[U118] JS：开发服务器
来源：http://msi.sweek.top

npm i -D vite;  npx vite
来源：http://feq.zycfv.cn

[U119] JS：生产构建
来源：http://euo.fanxiaobao.xyz

npx vite build
来源：http://idg.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://dic.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://efp.gogol.net.cn

================================================================================
来源：http://fxq.jqgfzy.top

统计汇总
来源：http://ryu.haohaochexian.top

================================================================================
来源：http://cht.chenzaomai.com

按语言统计（条）：
来源：http://tvk.zhiwuduotai.top

Python ......... 252
来源：http://jda.fktsv.cn

PHP ............ 252
来源：http://hia.yonumen.top

JavaScript ..... 252
来源：http://jcw.redwolf501.top

TypeScript ..... 212
来源：http://zzs.iojbl.cn

Java ........... 212
来源：http://xfp.hfpthk.cn

Go ............. 212
来源：http://hbp.meibo888.top

Ruby ........... 212
来源：http://htn.chenlongwang.top

C# ............. 212
来源：http://fuf.cdnleiting.top

C .............. 30
来源：http://gxx.hcnkem.com

C++ ............ 30
来源：http://adi.redwolf501.top

SQL ............ 90
来源：http://evd.jqgufenzy.top

Bash ........... 80
来源：http://fbr.hnqzz.top

Kotlin ......... 15
来源：http://cmk.nanxinkj.top

Swift .......... 15
来源：http://fse.9152youxi.cn

Lua ............ 10
来源：http://bks.xylfe.cn

Perl ........... 10
来源：http://owx.zdqjudy.top

Scala .......... 10
来源：http://hfy.feifeiyinyue.top

------------------------------------
来源：http://tbm.sufxvd.cn

合计 ........... 2106 条
来源：http://twx.aibaodan.cn

按章节统计：
来源：http://bld.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://smf.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zgo.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dfm.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qqw.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lyi.yvedp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ipk.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bqr.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rua.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://prq.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rbu.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://toz.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ywo.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rin.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sad.bjfxy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://puj.zhijiandao.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ysj.ybcxt.top

Q SQL 专题                              90
来源：http://nix.cashguo.top

R Bash 专题                             80
来源：http://fve.shuidangran.top

S C / C++ 专题                          60
来源：http://ixo.hfpthk.cn

T 其他语言补充                          60
来源：http://yjn.xuetiantiany.cn

U 高频实用片段                         120
来源：http://mso.c1oappe.top

------------------------------------
来源：http://cvx.ywan-chungtsiang.top

合计                                  2106 条
来源：http://vzs.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://itt.jqgfzy.top

使用提醒
来源：http://gmd.daxiang520.top

--------------------------------------------------------------------------------
来源：http://esa.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://caf.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ooz.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://afa.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://xym.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zbg.yueranfly.top

—— 文件结束 ——
来源：http://cml.yj20258.top

================================================================================
来源：http://dvi.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://hge.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://atk.jqgufenzy.top

================================================================================
来源：http://sxg.gzhubu.top

【收录内容】
来源：http://mkq.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rkf.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pet.jlsjyb.cn

SQL · Bash · C · C++
来源：http://omr.sufxvd.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lmr.xinyue.icu

【使用说明】
来源：http://hsm.hnqzz.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nmj.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://juo.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mnq.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wjh.nanxuanxn.top

Bash:  Shell         C:     C             C++:   C++
来源：http://abw.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rjz.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xog.zdbjq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fdi.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lto.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kap.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gqc.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tyl.redwolf501.top

【文件统计】
来源：http://ezv.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hdf.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ltl.sweek.top

目  录
来源：http://ugg.hnqzz.top

--------------------------------------------------------------------------------
来源：http://tyf.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uzg.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://onv.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xus.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oqu.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ing.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fkc.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vdi.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jzp.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vne.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fms.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ims.shzxlz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bul.xuanzx.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lev.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ggu.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dif.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sel.yuxming.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oyc.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wlo.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kmz.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uay.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zrh.vehdjk.com

================================================================================
来源：http://iht.zdqjudy.top

A. 基础语法与类型
来源：http://zwb.shanyushiyangtech.top

================================================================================
来源：http://jvi.ctjpmb.com

[A01] Hello World
来源：http://ref.hfpthk.cn

Py:   print("Hello, World!")
来源：http://ers.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://pnf.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://uyn.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ych.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://omz.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://jna.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://tqy.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ipk.zhengqikj.top

[A02] 变量声明与赋值
来源：http://hrj.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hpq.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gww.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://dxt.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ybi.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://enc.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://bnk.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://iwp.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://hlu.zhaomingkeji.xyz

[A03] 常量定义
来源：http://xwx.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iof.smart0.xyz

PHP:  const PI = 3.14159;
来源：http://nou.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://ixu.vqdsnc.cn

TS:   const PI: number = 3.14159;
来源：http://buw.uphjek.com

Java: static final double PI = 3.14159;
来源：http://saa.yuanzhike.top

Go:   const PI = 3.14159
来源：http://lpr.0kj1m.cn

Ruby: PI = 3.14159
来源：http://hnm.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://niy.jqgfzy.top

[A04] 判断变量类型
来源：http://dhe.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cfr.daria6918.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bcr.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ehw.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://cwu.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kvf.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://jpt.gaohongyu789.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fum.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://avg.zhixingplan.top

[A05] 整数除法与取模
来源：http://ieb.0kj1m.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bei.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lkz.aizwys.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hgq.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bzb.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://dnd.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://ivp.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://dlj.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://zms.ctjpmb.com

[A06] 字符串转数字
来源：http://bhv.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://bpr.zhengqikj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uxq.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qvc.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vbi.svipenyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://spd.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ltj.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fad.ydjk.org.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://quk.svipenyu.cn

[A07] 数字转字符串
来源：http://qni.birdmap.top

Py:   str(42)
来源：http://rzu.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://wtu.hfpthk.cn

JS:   String(42); (42).toString()
来源：http://xrr.iojbl.cn

TS:   String(42)
来源：http://lpb.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://irn.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://dzx.cdnleiting.top

Ruby: 42.to_s
来源：http://avv.hcnkem.com

C#:   42.ToString()
来源：http://gio.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://oso.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ayb.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gvw.tarul.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nzm.ybcxt.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rgh.yj202588.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://szj.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wxx.yuxming.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fcs.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zzm.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://wbl.daria6918.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ncf.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hda.andypj.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ynw.jyoumei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://epa.52xcode.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tac.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zju.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://snx.tanke756.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cnq.zhongyouzk.top

[A10] 生成随机数
来源：http://bsc.yangfankeji.com

Py:   import random; random.randint(1, 100)
来源：http://xwl.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://hzw.0kj1m.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qtx.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hwj.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://nmt.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ixk.hfpthk.cn

Ruby: rand(1..100)
来源：http://fuu.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://wrb.yvedp.cn

[A11] 条件表达式（三元）
来源：http://dup.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://ccc.yvedp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zip.iojbl.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xup.hnxiangtu.top

TS:   x > 0 ? "yes" : "no"
来源：http://nks.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://aat.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dlt.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rup.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://moa.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://ttf.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vmw.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kae.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://uax.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://evh.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://aos.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ted.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://gxp.tarul.cn

C#:   $"Hello, {name}!"
来源：http://bhg.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wki.birdmap.top

Py:   "第一行\n第二行"
来源：http://eoq.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://pvw.guowangkeji.top

JS:   "第一行\n第二行"
来源：http://bkm.fktsv.cn

TS:   "第一行\n第二行"
来源：http://cow.wangshuangyany.cn

Java: "第一行\n第二行"
来源：http://zex.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://ifj.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://zsb.xingfuxueyuan.xyz

C#:   "第一行\n第二行"
来源：http://xug.shzxlz.cn


<!-- 参考信息 -->