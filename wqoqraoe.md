代发 wailian999

[U81] JS：初始化项目
来源：http://iuo.316326.xyz

npm init -y;  npm i express
来源：http://nwa.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://rmz.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pjk.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://aap.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://wji.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://bkr.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://aqv.zhixingplan.top

[U85] JS：可选链
来源：http://vxg.zhoulong.xyz

a?.b?.c
来源：http://hwv.sjlbkw.cn

[U86] JS：空值合并
来源：http://tok.yanxiufei.cn

a ?? b
来源：http://hkf.aibaodan.cn

[U87] JS：解构默认值
来源：http://wnt.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://vgg.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://qyr.fzhhl.top

{ ...a, ...b }
来源：http://aqx.nwbrower.top

[U89] JS：数组去重
来源：http://sqi.gogol.net.cn

[...new Set(arr)]
来源：http://hcf.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://oqv.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://inv.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://tod.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kbk.52xcode.cn

[U92] JS：深拷贝
来源：http://nvj.redwolf501.top

structuredClone(obj)
来源：http://mna.yfazqb.com

[U93] JS：模板字符串
来源：http://ubp.nwbrower.top

`共 ${n} 条`
来源：http://wry.gzhubu.top

[U94] JS：箭头函数
来源：http://ufp.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://mnh.redwolf501.top

[U95] JS：Promise 包装
来源：http://czx.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://xyj.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://zen.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mus.fzhhl.top

[U97] JS：并发请求
来源：http://hyh.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://gch.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://rrd.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wem.ivvv.top

[U99] JS：事件监听
来源：http://tos.yj20258888.top

el.addEventListener("click", e => {})
来源：http://fsh.smart0.xyz

[U100] JS：DOM 查询
来源：http://dkg.yuxming.cn

document.querySelector(".item")
来源：http://obt.yongpay.top

[U101] JS：classList 操作
来源：http://ivs.yfazqb.com

el.classList.toggle("active")
来源：http://byd.andypj.xyz

[U102] JS：本地存储
来源：http://aun.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zgd.jyoumei.cn

[U103] JS：定时器
来源：http://dlj.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kdq.vqdsnc.cn

[U104] JS：防抖
来源：http://mhc.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aya.andypj.xyz

[U105] JS：节流
来源：http://cli.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jkf.zhongyouzk.top

[U106] JS：日期格式化
来源：http://hrd.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ipc.shzxlz.cn

[U107] JS：数字千分位
来源：http://iti.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dps.jinqigufen.top

[U108] JS：随机整数
来源：http://dks.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yma.hfpthk.cn

[U109] JS：数组分组
来源：http://bnp.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://rdv.yangfankeji.com

[U110] JS：数组分块
来源：http://kif.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yqv.guannengcc.top

[U111] JS：对象转 Map
来源：http://czh.smart0.xyz

new Map(Object.entries(obj))
来源：http://cim.xziqi.cn

[U112] JS：字符串补位
来源：http://zhg.jinqigfzy.top

"7".padStart(3, "0")
来源：http://axl.andypj.xyz

[U113] JS：正则替换全部
来源：http://cnz.wangdashe.top

s.replaceAll("a", "b")
来源：http://cda.aizwys.cn

[U114] JS：JSON 深比较
来源：http://fst.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pah.birdmap.top

[U115] JS：生成 UUID
来源：http://vpr.andypj.xyz

crypto.randomUUID()
来源：http://hvi.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://lku.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://wnl.fktsv.cn

[U117] JS：单元测试
来源：http://aid.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://tuh.yangfankeji.com

[U118] JS：开发服务器
来源：http://olo.hfpthk.cn

npm i -D vite;  npx vite
来源：http://gbj.vehdjk.com

[U119] JS：生产构建
来源：http://vou.cdnleiting.top

npx vite build
来源：http://vgj.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://eqo.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://zbs.xuanzx.com

================================================================================
来源：http://qsp.haohaochexian.top

统计汇总
来源：http://let.fzhhl.top

================================================================================
来源：http://blq.yanxiufei.cn

按语言统计（条）：
来源：http://hyn.chenjidiqi.icu

Python ......... 252
来源：http://gql.0kj1m.cn

PHP ............ 252
来源：http://hkw.cashguo.top

JavaScript ..... 252
来源：http://ogh.aibaodan.cn

TypeScript ..... 212
来源：http://cji.fengsongda.top

Java ........... 212
来源：http://tcu.shangyingyoupin.top

Go ............. 212
来源：http://xiz.fehbvm.com

Ruby ........... 212
来源：http://vke.vqdsnc.cn

C# ............. 212
来源：http://mbf.shzxlz.cn

C .............. 30
来源：http://ofb.kuanghao11.cn

C++ ............ 30
来源：http://gmf.shangyingyoupin.top

SQL ............ 90
来源：http://ccx.gotoacloud.top

Bash ........... 80
来源：http://mhw.fanxiaobao.xyz

Kotlin ......... 15
来源：http://gvz.c1oappe.top

Swift .......... 15
来源：http://cjf.fengsongda.top

Lua ............ 10
来源：http://xju.fengsongda.top

Perl ........... 10
来源：http://igz.hfpthk.cn

Scala .......... 10
来源：http://wjh.ivvv.top

------------------------------------
来源：http://uyl.dianchejie.cn

合计 ........... 2106 条
来源：http://ikj.xuanzx.com

按章节统计：
来源：http://fct.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ubp.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://csg.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zuz.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vdo.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xah.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jqe.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dmm.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jkx.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rfe.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bth.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nja.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qbz.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://joc.quarkkingdee.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uki.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://egm.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hzm.svipenyu.cn

Q SQL 专题                              90
来源：http://xjo.yj20258.top

R Bash 专题                             80
来源：http://jvn.zhixingplan.top

S C / C++ 专题                          60
来源：http://col.xylfe.cn

T 其他语言补充                          60
来源：http://siy.sjlbkw.cn

U 高频实用片段                         120
来源：http://hgl.ehwqpu.com

------------------------------------
来源：http://erg.ydjk.org.cn

合计                                  2106 条
来源：http://mbg.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://pap.chenjidiqi.icu

使用提醒
来源：http://wqx.yongpay.top

--------------------------------------------------------------------------------
来源：http://oto.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pgy.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wru.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zcm.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nyh.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rjl.xuanzx.com

—— 文件结束 ——
来源：http://skv.zhongyouzk.top

================================================================================
来源：http://ylk.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://cmr.vehdjk.com

Common Programming Examples Cheat Book
来源：http://vvj.jiagoushi.top

================================================================================
来源：http://hhw.jinqigufen.top

【收录内容】
来源：http://ktr.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://pcc.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ygy.shuidangran.top

SQL · Bash · C · C++
来源：http://vkp.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yvy.hnqzz.top

【使用说明】
来源：http://kto.guowangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zku.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qrs.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nlh.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rhm.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cve.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qyp.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hdy.zycfv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gbn.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vsv.ywan-chungtsiang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://boo.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nwg.gaohongyu789.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yyy.yongpay.top

【文件统计】
来源：http://lbl.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://spm.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://cnt.jianghu66.top

目  录
来源：http://pvz.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://kdq.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ckx.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eav.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ezn.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lzb.yongpay.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yrb.sxryk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kuh.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ial.xylfe.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://age.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vsc.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rfn.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qoy.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dgj.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uju.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gzy.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ilx.zhaomingkeji.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://stt.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ijm.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ozo.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lbm.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ops.guannengcc.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lwh.sxryk.cn

================================================================================
来源：http://led.tarul.cn

A. 基础语法与类型
来源：http://cxp.guannengcc.top

================================================================================
来源：http://rty.yangfankeji.com

[A01] Hello World
来源：http://gvt.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://qcb.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://dzv.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://wwr.ydzc1.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lpl.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://nwg.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://jys.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://zwp.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aja.svipenyu.cn

[A02] 变量声明与赋值
来源：http://uwy.jinyuanbaomall.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kzs.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zwp.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://zbo.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nti.xinyue.icu

Java: String name = "Alex"; int age = 20;
来源：http://xli.yvedp.cn

Go:   name := "Alex"; age := 20
来源：http://dzy.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://xwx.wangdashe.top

C#:   string name = "Alex"; int age = 20;
来源：http://dwk.hfpthk.cn

[A03] 常量定义
来源：http://afa.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qnp.cashguo.top

PHP:  const PI = 3.14159;
来源：http://yqo.cucudq.cn

JS:   const PI = 3.14159;
来源：http://god.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://grv.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://xje.haohaochexian.top

Go:   const PI = 3.14159
来源：http://sad.hnqzz.top

Ruby: PI = 3.14159
来源：http://lsx.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://drk.yfazqb.com

[A04] 判断变量类型
来源：http://ttp.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://zji.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ccr.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oqf.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://jzq.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nlw.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tpa.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://iot.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://kep.zycfv.cn

[A05] 整数除法与取模
来源：http://vnk.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://emb.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hvk.bbcook.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kmj.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pmj.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://akb.sjlbkw.cn

Go:   7 / 2; 7 % 2
来源：http://mdr.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://ulc.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://xmz.jqgufenzy.top

[A06] 字符串转数字
来源：http://msw.haohaochexian.top

Py:   int("42"); float("3.14")
来源：http://ghb.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kof.gogol.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oin.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://bci.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dac.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rud.andypj.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://yxp.yj20258888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jba.jinqigufen.top

[A07] 数字转字符串
来源：http://nnz.quarkkingdee.top

Py:   str(42)
来源：http://qdv.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://ljo.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://cgh.chenzaomai.com

TS:   String(42)
来源：http://gbv.hongshengwenyu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nwz.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://mic.iojbl.cn

Ruby: 42.to_s
来源：http://uqt.aibaodan.cn

C#:   42.ToString()
来源：http://xsh.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://gkg.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kzh.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bmz.jqgfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wtj.yfazqb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mrc.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ceh.fehbvm.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pvj.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uik.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kwi.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://mwo.sxryk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vgc.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lgf.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zxh.shanyushiyangtech.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sch.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vwi.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nus.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://evt.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bpt.ctjpmb.com

[A10] 生成随机数
来源：http://zgw.epnwcf.com

Py:   import random; random.randint(1, 100)
来源：http://xzb.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://mhy.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pcb.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pjb.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://loq.hnxiangtu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hjo.9152youxi.cn

Ruby: rand(1..100)
来源：http://jcz.quarkkingdee.top

C#:   new Random().Next(1, 101)
来源：http://orp.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://kzh.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://jle.smart0.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://lww.yangfankeji.com

JS:   x > 0 ? "yes" : "no"
来源：http://lwm.cqqwz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cnu.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://xcx.zdbjq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hou.xinyue.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://ouv.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://loa.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://zjv.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://etm.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qdx.ctjpmb.com

JS:   `Hello, ${name}!`
来源：http://tws.jyoumei.cn

TS:   `Hello, ${name}!`
来源：http://txy.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://hxb.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zgi.dashuyun.cn

Ruby: "Hello, #{name}!"
来源：http://joi.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://wzk.chenjidiqi.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://vhb.yonumen.top

Py:   "第一行\n第二行"
来源：http://avm.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://gmx.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://voh.redwolf501.top

TS:   "第一行\n第二行"
来源：http://ghx.fengsongda.top


<!-- 参考信息 -->