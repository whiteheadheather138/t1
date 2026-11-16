代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://mqf.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wrg.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://eut.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://tmu.quarkkingdee.top

[U85] JS：可选链
来源：http://zfq.yongpay.top

a?.b?.c
来源：http://gtk.gzhubu.top

[U86] JS：空值合并
来源：http://ccj.zhijiandao.cn

a ?? b
来源：http://jrm.nwbrower.top

[U87] JS：解构默认值
来源：http://ibu.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://mqi.fehbvm.com

[U88] JS：对象展开合并
来源：http://mfa.yuxming.cn

{ ...a, ...b }
来源：http://myy.sxryk.cn

[U89] JS：数组去重
来源：http://wqo.yueranfly.top

[...new Set(arr)]
来源：http://mkm.yj20258888.top

[U90] JS：数字数组排序
来源：http://rui.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://wiv.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://sga.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yfe.vehdjk.com

[U92] JS：深拷贝
来源：http://rdk.chenjidiqi.icu

structuredClone(obj)
来源：http://rhl.yonumen.top

[U93] JS：模板字符串
来源：http://juz.yfazqb.com

`共 ${n} 条`
来源：http://rlw.yuxming.cn

[U94] JS：箭头函数
来源：http://llr.iojbl.cn

const double = x => x * 2;
来源：http://cnz.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://vch.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://zqp.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://zrf.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wad.smart0.xyz

[U97] JS：并发请求
来源：http://bzu.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tbs.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://zsb.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hnk.shuidangran.top

[U99] JS：事件监听
来源：http://sym.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://pjh.xziqi.cn

[U100] JS：DOM 查询
来源：http://hjm.tian-w.cn

document.querySelector(".item")
来源：http://kov.xziqi.cn

[U101] JS：classList 操作
来源：http://kmi.cashguo.top

el.classList.toggle("active")
来源：http://zvl.shangyingyoupin.top

[U102] JS：本地存储
来源：http://ctb.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://aee.meibo888.top

[U103] JS：定时器
来源：http://jsk.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xtn.shzxlz.cn

[U104] JS：防抖
来源：http://dqu.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aas.jqgfzy.top

[U105] JS：节流
来源：http://iqk.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ycu.jiagoushi.top

[U106] JS：日期格式化
来源：http://idq.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cxt.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://mif.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iug.tianlin.xyz

[U108] JS：随机整数
来源：http://qdo.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rmi.tian-w.cn

[U109] JS：数组分组
来源：http://mxn.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://emn.sxryk.cn

[U110] JS：数组分块
来源：http://lyi.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kmt.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://woh.gogol.net.cn

new Map(Object.entries(obj))
来源：http://jvw.sxryk.cn

[U112] JS：字符串补位
来源：http://nbs.gaohongyu789.top

"7".padStart(3, "0")
来源：http://hxe.jinghuilouyu.cn

[U113] JS：正则替换全部
来源：http://ycy.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://uff.cheryme.top

[U114] JS：JSON 深比较
来源：http://pip.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://otm.gzhubu.top

[U115] JS：生成 UUID
来源：http://urk.guannengcc.top

crypto.randomUUID()
来源：http://uty.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://ftp.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://wyh.xziqi.cn

[U117] JS：单元测试
来源：http://wrt.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://zqv.0kj1m.cn

[U118] JS：开发服务器
来源：http://wfq.havefunace.top

npm i -D vite;  npx vite
来源：http://ddv.zdqjudy.top

[U119] JS：生产构建
来源：http://vwr.yvedp.cn

npx vite build
来源：http://api.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://fpi.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://dzk.wangshuangyany.cn

================================================================================
来源：http://btj.snrcjt.cn

统计汇总
来源：http://zpw.sysykeji.top

================================================================================
来源：http://sfh.jlsjyb.cn

按语言统计（条）：
来源：http://cdd.dashuyun.cn

Python ......... 252
来源：http://aeu.hfpthk.cn

PHP ............ 252
来源：http://ojo.aibaodan.cn

JavaScript ..... 252
来源：http://ldy.316326.xyz

TypeScript ..... 212
来源：http://qol.sjlbkw.cn

Java ........... 212
来源：http://otv.cucudq.cn

Go ............. 212
来源：http://cet.cdnleiting.top

Ruby ........... 212
来源：http://kwe.svipenyu.cn

C# ............. 212
来源：http://ooo.meibo888.top

C .............. 30
来源：http://cwy.316326.xyz

C++ ............ 30
来源：http://npn.feifeiyinyue.top

SQL ............ 90
来源：http://isy.cqqwz.cn

Bash ........... 80
来源：http://eae.daxiang520.top

Kotlin ......... 15
来源：http://xff.hysaishi.cn

Swift .......... 15
来源：http://pxa.vehdjk.com

Lua ............ 10
来源：http://elr.dianchejie.cn

Perl ........... 10
来源：http://axq.hesvh.cn

Scala .......... 10
来源：http://fve.chenlongwang.top

------------------------------------
来源：http://bce.sweek.top

合计 ........... 2106 条
来源：http://ngq.birdmap.top

按章节统计：
来源：http://bsv.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://win.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bkz.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kjv.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nzn.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jfe.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bzb.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oql.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eig.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pbr.shanyushiyangtech.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qam.gotoacloud.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wqs.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eqb.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lne.fengsongda.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://igx.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zhc.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zwh.shuidangran.top

Q SQL 专题                              90
来源：http://liu.zhijiandao.cn

R Bash 专题                             80
来源：http://ixl.hnqzz.top

S C / C++ 专题                          60
来源：http://leu.yfazqb.com

T 其他语言补充                          60
来源：http://gur.nwbrower.top

U 高频实用片段                         120
来源：http://aqc.cashguo.top

------------------------------------
来源：http://hbv.chenlongwang.top

合计                                  2106 条
来源：http://ney.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://fsv.cucudq.cn

使用提醒
来源：http://vvv.gzhubu.top

--------------------------------------------------------------------------------
来源：http://mar.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qgb.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kfh.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fbf.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ebo.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kxy.snrcjt.cn

—— 文件结束 ——
来源：http://bif.hywenlv.cn

================================================================================
来源：http://wav.cdnleiting.top

程序语言常见例子速查手册（2024 版）
来源：http://iuz.ywan-chungtsiang.top

Common Programming Examples Cheat Book
来源：http://lbg.hongshengwenyu.top

================================================================================
来源：http://aav.yanxiufei.cn

【收录内容】
来源：http://ibu.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://poo.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ozc.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://osz.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lpu.vqdsnc.cn

【使用说明】
来源：http://cfz.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fjs.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zrt.zhaomingkeji.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ltv.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sck.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://trz.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lot.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lxt.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oac.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hcn.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wja.zhengqikj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sqt.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dtn.nwbrower.top

【文件统计】
来源：http://wou.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ulj.fengsongda.top

--------------------------------------------------------------------------------
来源：http://sgh.ivvv.top

目  录
来源：http://ekq.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://xum.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aji.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://efr.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://adj.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bvl.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yta.yangfankeji.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zvo.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xcv.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dnh.smart0.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://snz.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rvx.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nfv.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ygs.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qoe.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kye.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lzb.chenzaomai.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hln.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mxu.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://poa.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sqp.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xil.dashuyun.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rdc.gotoacloud.top

================================================================================
来源：http://ywj.zycfv.cn

A. 基础语法与类型
来源：http://eiz.jinyuanbaomall.cn

================================================================================
来源：http://pgb.shuidangran.top

[A01] Hello World
来源：http://zxe.52xcode.cn

Py:   print("Hello, World!")
来源：http://prw.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://npe.yonumen.top

JS:   console.log("Hello, World!");
来源：http://oyf.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nij.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://icp.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://zdq.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://kpl.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rdv.ppjwa.cn

[A02] 变量声明与赋值
来源：http://qxq.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qcv.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zsg.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fud.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gkl.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://txh.zhaomingkeji.xyz

Go:   name := "Alex"; age := 20
来源：http://owy.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://nef.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://vrq.aibaodan.cn

[A03] 常量定义
来源：http://sgk.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yvv.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://dxd.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://wox.c1oappe.top

TS:   const PI: number = 3.14159;
来源：http://vuw.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://wmy.ivvv.top

Go:   const PI = 3.14159
来源：http://btv.sweek.top

Ruby: PI = 3.14159
来源：http://nln.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://zhf.bjfxy.top

[A04] 判断变量类型
来源：http://jac.feifeiyinyue.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://eii.shuidangran.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dln.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wng.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://lva.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lkp.hfpthk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://icc.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cap.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://klz.yj20258.top

[A05] 整数除法与取模
来源：http://iyk.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cga.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jto.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://npv.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fkc.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://zcj.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://pni.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://trb.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://edt.nanxinkj.top

[A06] 字符串转数字
来源：http://xfa.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://frd.yongpay.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kfk.cqqwz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://awy.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://qdf.ctjpmb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://unk.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zdt.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://usx.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fgj.xziqi.cn

[A07] 数字转字符串
来源：http://vye.zhiwuduotai.top

Py:   str(42)
来源：http://xkq.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://lbs.yuxming.cn

JS:   String(42); (42).toString()
来源：http://kir.xziqi.cn

TS:   String(42)
来源：http://ryd.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ibe.cashguo.top

Go:   strconv.Itoa(42)
来源：http://swr.ctjpmb.com

Ruby: 42.to_s
来源：http://yot.yanxiufei.cn

C#:   42.ToString()
来源：http://jqr.zycfv.cn

[A08] 取整与四舍五入
来源：http://dej.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mnj.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dlu.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tmd.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ixx.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pbp.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dyu.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://udu.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://spw.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://hwv.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eds.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kre.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tyj.hysaishi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://myz.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fbg.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pyk.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dbb.ybcxt.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eai.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://ezu.hcnkem.com

Py:   import random; random.randint(1, 100)
来源：http://jlx.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://fmn.cheryme.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ajz.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ezp.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://yoo.ppjwa.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zso.316326.xyz

Ruby: rand(1..100)
来源：http://nbz.xylfe.cn

C#:   new Random().Next(1, 101)
来源：http://xar.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://hpg.guowangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://zjp.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ktp.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://ewp.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://rxf.zhoulong.xyz

Java: x > 0 ? "yes" : "no"
来源：http://etn.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ffz.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vte.jiagoushi.top

C#:   x > 0 ? "yes" : "no"
来源：http://jzz.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://kik.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qai.nanxuanxn.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zdh.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://tdx.yuxming.cn

TS:   `Hello, ${name}!`
来源：http://kje.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://fhj.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bqx.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://lcp.shanyushiyangtech.top

C#:   $"Hello, {name}!"
来源：http://kkd.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qmw.zycfv.cn

Py:   "第一行\n第二行"
来源：http://tvn.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://dsy.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://hkz.fengsongda.top

TS:   "第一行\n第二行"
来源：http://dkv.316326.xyz

Java: "第一行\n第二行"
来源：http://ila.hesvh.cn

Go:   "第一行\n第二行"
来源：http://fgo.pycfn.com

Ruby: "第一行\n第二行"
来源：http://nds.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://jdr.dianchejie.cn


<!-- 参考信息 -->