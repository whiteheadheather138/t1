代发 wailian999

[U81] JS：初始化项目
来源：http://soh.tanke756.top

npm init -y;  npm i express
来源：http://gbu.havefunace.top

[U82] JS：package.json 脚本
来源：http://gls.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wtb.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://wxv.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fyk.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://lqf.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://hra.sjlbkw.cn

[U85] JS：可选链
来源：http://atp.meibo888.top

a?.b?.c
来源：http://ekf.hammf.cn

[U86] JS：空值合并
来源：http://zmp.vehdjk.com

a ?? b
来源：http://ajf.jlsjyb.cn

[U87] JS：解构默认值
来源：http://dua.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://zns.chenzaomai.com

[U88] JS：对象展开合并
来源：http://yoa.cheryme.top

{ ...a, ...b }
来源：http://mxp.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://oib.yangfankeji.com

[...new Set(arr)]
来源：http://dua.nwbrower.top

[U90] JS：数字数组排序
来源：http://kjg.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://bod.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://sqi.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vdu.meibo888.top

[U92] JS：深拷贝
来源：http://cvh.jinqigufen.top

structuredClone(obj)
来源：http://jmu.ydjk.org.cn

[U93] JS：模板字符串
来源：http://zvc.9152youxi.cn

`共 ${n} 条`
来源：http://zti.fzhhl.top

[U94] JS：箭头函数
来源：http://jom.zhijiandao.cn

const double = x => x * 2;
来源：http://otr.ppjwa.cn

[U95] JS：Promise 包装
来源：http://kls.hammf.cn

new Promise((resolve, reject) => {})
来源：http://zdo.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://mjy.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bgs.daria6918.cn

[U97] JS：并发请求
来源：http://eyb.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mwe.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://azd.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cby.smart0.xyz

[U99] JS：事件监听
来源：http://cad.pycfn.com

el.addEventListener("click", e => {})
来源：http://wxu.zhoulong.xyz

[U100] JS：DOM 查询
来源：http://xei.cqqwz.cn

document.querySelector(".item")
来源：http://cdg.jlsjyb.cn

[U101] JS：classList 操作
来源：http://mae.nanxinkj.top

el.classList.toggle("active")
来源：http://rux.jqgfzy.top

[U102] JS：本地存储
来源：http://tlu.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cqa.pycfn.com

[U103] JS：定时器
来源：http://vvl.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://etp.zhoulong.xyz

[U104] JS：防抖
来源：http://wpv.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqg.jinqigfzy.top

[U105] JS：节流
来源：http://nom.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kqs.chenzaomai.com

[U106] JS：日期格式化
来源：http://brz.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ksy.gzhubu.top

[U107] JS：数字千分位
来源：http://jjv.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hps.aizwys.cn

[U108] JS：随机整数
来源：http://ubl.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jxv.pycfn.com

[U109] JS：数组分组
来源：http://zaq.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://pzh.tarul.cn

[U110] JS：数组分块
来源：http://gmf.nanxuanxn.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ugl.xylfe.cn

[U111] JS：对象转 Map
来源：http://yfw.ppjwa.cn

new Map(Object.entries(obj))
来源：http://kbd.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://mev.shanyushiyangtech.top

"7".padStart(3, "0")
来源：http://yci.sweek.top

[U113] JS：正则替换全部
来源：http://jtz.tianlin.xyz

s.replaceAll("a", "b")
来源：http://ops.meibo888.top

[U114] JS：JSON 深比较
来源：http://mtt.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tok.bjfxy.top

[U115] JS：生成 UUID
来源：http://grw.fanxiaobao.xyz

crypto.randomUUID()
来源：http://rou.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://nwi.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://ukn.jqgfzy.top

[U117] JS：单元测试
来源：http://dfy.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://hma.shzxlz.cn

[U118] JS：开发服务器
来源：http://stb.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://lof.jyoumei.cn

[U119] JS：生产构建
来源：http://vtw.sxryk.cn

npx vite build
来源：http://igx.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://rqv.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://tcp.yuanzhike.top

================================================================================
来源：http://gdt.tanke756.top

统计汇总
来源：http://urb.hcnkem.com

================================================================================
来源：http://sbn.yj20258888.top

按语言统计（条）：
来源：http://toy.tarul.cn

Python ......... 252
来源：http://cdt.hfpthk.cn

PHP ............ 252
来源：http://yvl.yuxming.cn

JavaScript ..... 252
来源：http://tmg.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://bno.smart0.xyz

Java ........... 212
来源：http://jck.xuanzx.com

Go ............. 212
来源：http://yxf.svipenyu.cn

Ruby ........... 212
来源：http://wvw.havefunace.top

C# ............. 212
来源：http://dqp.andypj.xyz

C .............. 30
来源：http://wpd.sysykeji.top

C++ ............ 30
来源：http://zvw.gogol.net.cn

SQL ............ 90
来源：http://arx.meibo888.top

Bash ........... 80
来源：http://lth.svipenyu.cn

Kotlin ......... 15
来源：http://hcq.316326.xyz

Swift .......... 15
来源：http://inp.jqgufenzy.top

Lua ............ 10
来源：http://cyc.fktsv.cn

Perl ........... 10
来源：http://xtk.xuetiantiany.cn

Scala .......... 10
来源：http://ctt.jqgfzy.top

------------------------------------
来源：http://del.yvedp.cn

合计 ........... 2106 条
来源：http://tnq.fehbvm.com

按章节统计：
来源：http://ppv.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wvx.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bkv.zhixingplan.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pkf.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nhh.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ahn.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uar.zycfv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jfs.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qtf.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://npq.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ucj.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zye.vqdsnc.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://arb.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ona.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://atr.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bbf.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://boc.vehdjk.com

Q SQL 专题                              90
来源：http://ite.daria6918.cn

R Bash 专题                             80
来源：http://hep.fengsongda.top

S C / C++ 专题                          60
来源：http://ffb.xinyue.icu

T 其他语言补充                          60
来源：http://hzw.pycfn.com

U 高频实用片段                         120
来源：http://voi.zhengqikj.top

------------------------------------
来源：http://nsi.gzhubu.top

合计                                  2106 条
来源：http://jzw.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://xdv.yj20258.top

使用提醒
来源：http://xth.daria6918.cn

--------------------------------------------------------------------------------
来源：http://wui.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yrq.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zqm.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tpi.shanyushiyangtech.top

在旧版本上使用前请先确认语法支持情况。
来源：http://shm.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dwu.hnqzz.top

—— 文件结束 ——
来源：http://saj.nanxuanxn.top

================================================================================
来源：http://cju.fktsv.cn

程序语言常见例子速查手册（2024 版）
来源：http://ofu.cashguo.top

Common Programming Examples Cheat Book
来源：http://lpe.hysaishi.cn

================================================================================
来源：http://jhq.guannengcc.top

【收录内容】
来源：http://tby.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://soc.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fim.sufxvd.cn

SQL · Bash · C · C++
来源：http://xww.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dxe.dianchejie.cn

【使用说明】
来源：http://maw.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ara.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jkp.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fki.zhaomingkeji.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mxq.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fqv.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sdw.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rdg.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jtc.tianlin.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ooq.shangyingyoupin.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fco.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lmx.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mao.shanyushiyangtech.top

【文件统计】
来源：http://slh.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lsh.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://tpf.pycfn.com

目  录
来源：http://sdk.smart0.xyz

--------------------------------------------------------------------------------
来源：http://vfv.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rgi.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hbh.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yal.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cbs.hcnkem.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hzh.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://udr.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oda.xziqi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ymu.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nrd.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vsf.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dia.yueranfly.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xfq.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gpe.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bkv.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lik.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xfb.jqgfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rom.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vha.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jig.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bts.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mqt.hnxiangtu.top

================================================================================
来源：http://suc.sxryk.cn

A. 基础语法与类型
来源：http://ind.zdbjq.cn

================================================================================
来源：http://xyx.yuanzhike.top

[A01] Hello World
来源：http://lke.dashuyun.cn

Py:   print("Hello, World!")
来源：http://wxt.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://lto.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://rsk.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oqf.uphjek.com

Java: System.out.println("Hello, World!");
来源：http://mxx.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://teo.cqqwz.cn

Ruby: puts "Hello, World!"
来源：http://vxf.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lvy.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://mcb.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hhq.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://mlz.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cex.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ahm.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://kov.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://ihp.yonumen.top

Ruby: name = "Alex"; age = 20
来源：http://rni.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://khz.wangdashe.top

[A03] 常量定义
来源：http://eaj.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yam.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://whj.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://xlq.chenjidiqi.icu

TS:   const PI: number = 3.14159;
来源：http://jlh.haohaochexian.top

Java: static final double PI = 3.14159;
来源：http://yxo.ybcxt.top

Go:   const PI = 3.14159
来源：http://wxk.chenzaomai.com

Ruby: PI = 3.14159
来源：http://cgq.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://dwb.shzxlz.cn

[A04] 判断变量类型
来源：http://rcl.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://xlx.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vhk.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://erb.zdbjq.cn

TS:   typeof x; x instanceof Date
来源：http://dgu.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wpf.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://nwt.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zqc.gaohongyu789.top

C#:   x.GetType().Name; x is int
来源：http://nlu.c1oappe.top

[A05] 整数除法与取模
来源：http://llh.xuanzx.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ezz.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qqg.ywan-chungtsiang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bro.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vpt.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://ftd.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://idp.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://vcj.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://gwc.uphjek.com

[A06] 字符串转数字
来源：http://lah.uphjek.com

Py:   int("42"); float("3.14")
来源：http://onp.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://woj.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nur.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qet.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pri.meibo888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dkb.hammf.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pio.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kdf.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://irs.jinghuilouyu.cn

Py:   str(42)
来源：http://aus.vehdjk.com

PHP:  (string) 42; strval(42)
来源：http://ipc.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://dbm.shzxlz.cn

TS:   String(42)
来源：http://bjb.jinghuilouyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cgl.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://ueh.yuxming.cn

Ruby: 42.to_s
来源：http://hoe.hnqzz.top

C#:   42.ToString()
来源：http://czk.fktsv.cn

[A08] 取整与四舍五入
来源：http://nui.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ptj.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wek.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://neo.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hck.nanxinkj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vai.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cvq.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ahp.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tcf.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://wky.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vql.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kjj.uphjek.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://slk.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pdc.zhijiandao.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xnd.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://spc.sufxvd.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hvs.yonumen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wld.daxiang520.top

[A10] 生成随机数
来源：http://yjn.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://ocz.ybcxt.top

PHP:  random_int(1, 100);
来源：http://ukb.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://own.tianlin.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bft.xuetiantiany.cn

Java: new Random().nextInt(100) + 1
来源：http://dhz.jinyuanbaomall.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pks.xuetiantiany.cn

Ruby: rand(1..100)
来源：http://rbz.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://lzz.xuanzx.com

[A11] 条件表达式（三元）
来源：http://vln.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://qyv.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hel.bbcook.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rnv.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://xda.iojbl.cn

Java: x > 0 ? "yes" : "no"
来源：http://lng.hywenlv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://otz.sxryk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nyv.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://xad.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://oui.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jvr.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ugy.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://pii.birdmap.top

TS:   `Hello, ${name}!`
来源：http://qgk.cdnleiting.top

Java: "Hello, %s!".formatted(name)
来源：http://oug.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cot.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://niw.ehwqpu.com

C#:   $"Hello, {name}!"
来源：http://alq.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bgb.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://mpb.wangdashe.top

PHP:  "第一行\n第二行"
来源：http://hew.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://yiy.cashguo.top

TS:   "第一行\n第二行"
来源：http://sae.svipenyu.cn


<!-- 参考信息 -->