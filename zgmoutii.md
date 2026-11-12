代发 wailian999

[U81] JS：初始化项目
来源：http://kky.snrcjt.cn

npm init -y;  npm i express
来源：http://jeo.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://dfn.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gnn.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://rpf.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ani.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://omq.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://nym.sweek.top

[U85] JS：可选链
来源：http://tpa.ppjwa.cn

a?.b?.c
来源：http://ykd.daxiang520.top

[U86] JS：空值合并
来源：http://ypj.xingfuxueyuan.xyz

a ?? b
来源：http://bud.zycfv.cn

[U87] JS：解构默认值
来源：http://hdw.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://nwe.hcnkem.com

[U88] JS：对象展开合并
来源：http://qnd.ivvv.top

{ ...a, ...b }
来源：http://pnu.jlsjyb.cn

[U89] JS：数组去重
来源：http://hwl.hesvh.cn

[...new Set(arr)]
来源：http://clw.ctjpmb.com

[U90] JS：数字数组排序
来源：http://ljw.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://bwv.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://xku.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rpc.0kj1m.cn

[U92] JS：深拷贝
来源：http://ewj.yuxming.cn

structuredClone(obj)
来源：http://zuj.snrcjt.cn

[U93] JS：模板字符串
来源：http://ivu.aizwys.cn

`共 ${n} 条`
来源：http://kts.ppjwa.cn

[U94] JS：箭头函数
来源：http://tty.yuanzhike.top

const double = x => x * 2;
来源：http://ayq.cheryme.top

[U95] JS：Promise 包装
来源：http://hsk.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://bcg.sysykeji.top

[U96] JS：async/await 与异常
来源：http://txp.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qpn.gotoacloud.top

[U97] JS：并发请求
来源：http://xwu.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfn.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://hpp.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xlb.yvedp.cn

[U99] JS：事件监听
来源：http://otc.iojbl.cn

el.addEventListener("click", e => {})
来源：http://ssp.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://gbq.yanxiufei.cn

document.querySelector(".item")
来源：http://sxm.ppjwa.cn

[U101] JS：classList 操作
来源：http://gpq.tanke756.top

el.classList.toggle("active")
来源：http://yws.pengpengdd.cyou

[U102] JS：本地存储
来源：http://kww.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://szn.hysaishi.cn

[U103] JS：定时器
来源：http://isp.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bpe.cheryme.top

[U104] JS：防抖
来源：http://vox.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njb.jinyuanbaomall.cn

[U105] JS：节流
来源：http://afs.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cer.snrcjt.cn

[U106] JS：日期格式化
来源：http://fsf.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nes.ivvv.top

[U107] JS：数字千分位
来源：http://sfv.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://etb.aizwys.cn

[U108] JS：随机整数
来源：http://gwk.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gkl.ydzc1.top

[U109] JS：数组分组
来源：http://tna.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://pwr.sxryk.cn

[U110] JS：数组分块
来源：http://ffz.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iek.shuidangran.top

[U111] JS：对象转 Map
来源：http://iya.redwolf501.top

new Map(Object.entries(obj))
来源：http://xee.ivvv.top

[U112] JS：字符串补位
来源：http://gjg.gzhubu.top

"7".padStart(3, "0")
来源：http://fjl.nwbrower.top

[U113] JS：正则替换全部
来源：http://rwg.316326.xyz

s.replaceAll("a", "b")
来源：http://hxg.fktsv.cn

[U114] JS：JSON 深比较
来源：http://viw.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zcj.jiagoushi.top

[U115] JS：生成 UUID
来源：http://ysx.nanxinkj.top

crypto.randomUUID()
来源：http://awk.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://bxb.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://ssb.9152youxi.cn

[U117] JS：单元测试
来源：http://qwx.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://hpi.ivvv.top

[U118] JS：开发服务器
来源：http://cdv.tanke756.top

npm i -D vite;  npx vite
来源：http://viz.daxiang520.top

[U119] JS：生产构建
来源：http://ook.yuanzhike.top

npx vite build
来源：http://ocx.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://qnh.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://kdn.tianlin.xyz

================================================================================
来源：http://zvn.shuidangran.top

统计汇总
来源：http://rul.ppjwa.cn

================================================================================
来源：http://ghk.yongpay.top

按语言统计（条）：
来源：http://mbe.nwbrower.top

Python ......... 252
来源：http://brf.nanxinkj.top

PHP ............ 252
来源：http://ajw.xylfe.cn

JavaScript ..... 252
来源：http://bhr.xuetiantiany.cn

TypeScript ..... 212
来源：http://evk.wangdashe.top

Java ........... 212
来源：http://shj.cheryme.top

Go ............. 212
来源：http://eke.yj20258.top

Ruby ........... 212
来源：http://fcw.sxryk.cn

C# ............. 212
来源：http://dsw.chenjidiqi.icu

C .............. 30
来源：http://wdg.iojbl.cn

C++ ............ 30
来源：http://qdy.yj202588.top

SQL ............ 90
来源：http://pap.aizwys.cn

Bash ........... 80
来源：http://iwd.yangfankeji.com

Kotlin ......... 15
来源：http://gqf.hammf.cn

Swift .......... 15
来源：http://suy.feifeiyinyue.top

Lua ............ 10
来源：http://bhh.hysaishi.cn

Perl ........... 10
来源：http://rwx.yongpay.top

Scala .......... 10
来源：http://dpj.birdmap.top

------------------------------------
来源：http://inp.jinqigfzy.top

合计 ........... 2106 条
来源：http://hvk.mhx1999.top

按章节统计：
来源：http://zkf.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jiq.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gmy.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://joi.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qpw.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ppm.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://atq.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://inn.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ggk.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://szo.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rcd.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iry.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ygj.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xab.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rak.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dbu.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vjl.cqqwz.cn

Q SQL 专题                              90
来源：http://rsg.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://umr.gogol.net.cn

S C / C++ 专题                          60
来源：http://ofj.kuanghao11.cn

T 其他语言补充                          60
来源：http://emg.kuanghao11.cn

U 高频实用片段                         120
来源：http://pkh.316326.xyz

------------------------------------
来源：http://ucl.wangshuangyany.cn

合计                                  2106 条
来源：http://elb.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://vhy.yangfankeji.com

使用提醒
来源：http://vfa.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://zcc.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://afd.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ozo.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jpo.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://muf.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wep.cqqwz.cn

—— 文件结束 ——
来源：http://kpu.epnwcf.com

================================================================================
来源：http://hmg.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://wir.shuidangran.top

Common Programming Examples Cheat Book
来源：http://tec.hnxiangtu.top

================================================================================
来源：http://ddc.bbcook.cn

【收录内容】
来源：http://tbb.zycfv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gwq.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ahz.jlsjyb.cn

SQL · Bash · C · C++
来源：http://xhy.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jpv.yuxming.cn

【使用说明】
来源：http://xcy.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://esl.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jws.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://btb.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ink.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cll.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gbe.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mjd.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tcf.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rtr.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zzx.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zef.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kct.jinqigufen.top

【文件统计】
来源：http://vvi.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kay.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://rsl.cheryme.top

目  录
来源：http://kch.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://vfy.hesvh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fno.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rxx.aibaodan.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hjm.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uug.hnqzz.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mna.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uvl.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://chy.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://smg.bbcook.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bgi.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ieu.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jcu.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pas.jiagoushi.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://amv.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pib.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eoa.yj20258.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kbs.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qhl.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://usq.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fii.fanxiaobao.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rfj.daxiang520.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ytz.aizwys.cn

================================================================================
来源：http://kwf.hysaishi.cn

A. 基础语法与类型
来源：http://oqp.gogol.net.cn

================================================================================
来源：http://ifk.cdnleiting.top

[A01] Hello World
来源：http://ubd.ybcxt.top

Py:   print("Hello, World!")
来源：http://qeq.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://bvd.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://ska.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ehk.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://odx.yfazqb.com

Go:   fmt.Println("Hello, World!")
来源：http://wop.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://mhn.yonumen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hzv.316326.xyz

[A02] 变量声明与赋值
来源：http://yme.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eae.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://opo.cqqwz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bwp.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fxj.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://agd.fzhhl.top

Go:   name := "Alex"; age := 20
来源：http://ida.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://tnq.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://hnz.ivvv.top

[A03] 常量定义
来源：http://xkf.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jwu.yonumen.top

PHP:  const PI = 3.14159;
来源：http://kug.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://czl.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://kad.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://wfh.316326.xyz

Go:   const PI = 3.14159
来源：http://fsb.xinyue.icu

Ruby: PI = 3.14159
来源：http://otc.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://qkp.hnqzz.top

[A04] 判断变量类型
来源：http://hsd.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://guc.hcnkem.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rsm.shangyingyoupin.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wmr.shanyushiyangtech.top

TS:   typeof x; x instanceof Date
来源：http://cla.ppjwa.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nvj.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://twf.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yrj.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://bso.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://kdu.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tng.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://stj.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aqa.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://erv.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://bxu.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://gmz.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://dtn.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://ajj.daria6918.cn

[A06] 字符串转数字
来源：http://dwl.jqgfzy.top

Py:   int("42"); float("3.14")
来源：http://wvs.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gsd.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fya.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://iuz.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vnr.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oag.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vcg.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sbp.wangshuangyany.cn

[A07] 数字转字符串
来源：http://kyn.yangfankeji.com

Py:   str(42)
来源：http://zro.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://rjx.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://mdp.jlsjyb.cn

TS:   String(42)
来源：http://xys.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://chr.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://xgk.tianlin.xyz

Ruby: 42.to_s
来源：http://zuw.gotoacloud.top

C#:   42.ToString()
来源：http://ffk.tarul.cn

[A08] 取整与四舍五入
来源：http://jui.jyoumei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dbl.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hmw.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zbm.andypj.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yjt.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gea.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jsn.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://zva.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ler.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://rbc.smart0.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mkh.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ovm.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qov.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://enc.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tbp.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lho.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zzi.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dvz.svipenyu.cn

[A10] 生成随机数
来源：http://fvz.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://gts.gaohongyu789.top

PHP:  random_int(1, 100);
来源：http://znd.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jum.jianghu66.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mga.ydjk.org.cn

Java: new Random().nextInt(100) + 1
来源：http://fmu.xingfuxueyuan.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dej.chenzaomai.com

Ruby: rand(1..100)
来源：http://nqs.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://fqj.52xcode.cn

[A11] 条件表达式（三元）
来源：http://isn.tianlin.xyz

Py:   "yes" if x > 0 else "no"
来源：http://obg.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://spb.sweek.top

JS:   x > 0 ? "yes" : "no"
来源：http://agr.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yqe.shzxlz.cn

Java: x > 0 ? "yes" : "no"
来源：http://uge.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pis.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://org.jyoumei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jwz.yuanzhike.top

[A12] 字符串插值 / 格式化
来源：http://lmo.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tqu.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://irl.shzxlz.cn

JS:   `Hello, ${name}!`
来源：http://jrt.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://zve.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://apo.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gyr.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://nrt.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://sfi.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wlp.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://gbl.tian-w.cn

PHP:  "第一行\n第二行"
来源：http://lmc.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://eln.hammf.cn

TS:   "第一行\n第二行"
来源：http://nui.yangfankeji.com


<!-- 参考信息 -->