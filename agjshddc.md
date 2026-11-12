代发 wailian999

[U79] PHP：静态分析
来源：http://vqa.pycfn.com

composer require --dev phpstan/phpstan
来源：http://xox.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://gql.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ygf.gogol.net.cn

[U81] JS：初始化项目
来源：http://lvt.hcnkem.com

npm init -y;  npm i express
来源：http://ngn.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://sjw.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dsa.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://lel.cashguo.top

export const a = 1;  import { a } from "./m.js";
来源：http://fmt.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://xek.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://sfm.cashguo.top

[U85] JS：可选链
来源：http://mvs.yonumen.top

a?.b?.c
来源：http://jdu.andypj.xyz

[U86] JS：空值合并
来源：http://apq.jlsjyb.cn

a ?? b
来源：http://bhh.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://yae.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://ckl.fengsongda.top

[U88] JS：对象展开合并
来源：http://zzd.hcnkem.com

{ ...a, ...b }
来源：http://hyk.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://gke.cdnleiting.top

[...new Set(arr)]
来源：http://frt.ctjpmb.com

[U90] JS：数字数组排序
来源：http://tem.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://xsz.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://tyz.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqa.shuidangran.top

[U92] JS：深拷贝
来源：http://omr.svipenyu.cn

structuredClone(obj)
来源：http://xef.smart0.xyz

[U93] JS：模板字符串
来源：http://ujk.316326.xyz

`共 ${n} 条`
来源：http://img.sjlbkw.cn

[U94] JS：箭头函数
来源：http://ixm.jyoumei.cn

const double = x => x * 2;
来源：http://tda.zhengqikj.top

[U95] JS：Promise 包装
来源：http://qrp.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://pac.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://jkr.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ivi.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://msr.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://coy.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://wxh.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ktq.xuetiantiany.cn

[U99] JS：事件监听
来源：http://tvn.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://yuf.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://rli.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://dpw.c1oappe.top

[U101] JS：classList 操作
来源：http://ofz.hongshengwenyu.top

el.classList.toggle("active")
来源：http://yfo.tarul.cn

[U102] JS：本地存储
来源：http://vte.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pjz.hesvh.cn

[U103] JS：定时器
来源：http://ght.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gpx.fengsongda.top

[U104] JS：防抖
来源：http://tup.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qvy.gotoacloud.top

[U105] JS：节流
来源：http://ubm.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tcu.hnxiangtu.top

[U106] JS：日期格式化
来源：http://vyq.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nhh.zhoulong.xyz

[U107] JS：数字千分位
来源：http://bgw.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mnn.sysykeji.top

[U108] JS：随机整数
来源：http://yxf.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dmt.hysaishi.cn

[U109] JS：数组分组
来源：http://uod.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://kie.zhiwuduotai.top

[U110] JS：数组分块
来源：http://cyr.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fsx.yj20258888.top

[U111] JS：对象转 Map
来源：http://wrb.zhengqikj.top

new Map(Object.entries(obj))
来源：http://huz.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://lzd.sxryk.cn

"7".padStart(3, "0")
来源：http://ygu.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://bjf.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://kxn.xylfe.cn

[U114] JS：JSON 深比较
来源：http://lht.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://zoa.nanxinkj.top

[U115] JS：生成 UUID
来源：http://ffj.xylfe.cn

crypto.randomUUID()
来源：http://lob.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://uoj.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://tdy.yvedp.cn

[U117] JS：单元测试
来源：http://wan.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://dvl.pycfn.com

[U118] JS：开发服务器
来源：http://fzi.cqqwz.cn

npm i -D vite;  npx vite
来源：http://boq.pycfn.com

[U119] JS：生产构建
来源：http://eke.zhixingplan.top

npx vite build
来源：http://hjn.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://tav.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://zly.cdnleiting.top

================================================================================
来源：http://bog.feifeiyinyue.top

统计汇总
来源：http://ook.vehdjk.com

================================================================================
来源：http://axf.cheryme.top

按语言统计（条）：
来源：http://omi.aibaodan.cn

Python ......... 252
来源：http://iik.gzhubu.top

PHP ............ 252
来源：http://czq.yfazqb.com

JavaScript ..... 252
来源：http://zyp.xinyue.icu

TypeScript ..... 212
来源：http://npk.redwolf501.top

Java ........... 212
来源：http://ggy.cheryme.top

Go ............. 212
来源：http://ams.tian-w.cn

Ruby ........... 212
来源：http://iwl.fehbvm.com

C# ............. 212
来源：http://qck.yuxming.cn

C .............. 30
来源：http://zgv.gogol.net.cn

C++ ............ 30
来源：http://qef.daria6918.cn

SQL ............ 90
来源：http://snm.jinghuilouyu.cn

Bash ........... 80
来源：http://heg.fzhhl.top

Kotlin ......... 15
来源：http://vro.xziqi.cn

Swift .......... 15
来源：http://akn.tianlin.xyz

Lua ............ 10
来源：http://mdg.shzxlz.cn

Perl ........... 10
来源：http://gzw.xziqi.cn

Scala .......... 10
来源：http://dvo.nanxinkj.top

------------------------------------
来源：http://jiq.yuxming.cn

合计 ........... 2106 条
来源：http://kvw.xinyue.icu

按章节统计：
来源：http://mpp.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jzp.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://seu.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://npw.hywenlv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vka.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ohv.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://txv.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zpo.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xzn.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dyx.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cho.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://prf.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lgp.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pwg.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gxe.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ybg.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dpx.iojbl.cn

Q SQL 专题                              90
来源：http://zcm.aizwys.cn

R Bash 专题                             80
来源：http://xgh.xylfe.cn

S C / C++ 专题                          60
来源：http://vnz.xylfe.cn

T 其他语言补充                          60
来源：http://efe.tianlin.xyz

U 高频实用片段                         120
来源：http://kgq.yangfankeji.com

------------------------------------
来源：http://mot.jiagoushi.top

合计                                  2106 条
来源：http://spp.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://hui.0kj1m.cn

使用提醒
来源：http://ifx.havefunace.top

--------------------------------------------------------------------------------
来源：http://mvc.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mdi.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jdv.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ntr.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zus.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iov.tanke756.top

—— 文件结束 ——
来源：http://odj.dashuyun.cn

================================================================================
来源：http://nyk.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ugq.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://too.0kj1m.cn

================================================================================
来源：http://pfx.haohaochexian.top

【收录内容】
来源：http://wga.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://anf.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qiz.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://nsw.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xcy.ywan-chungtsiang.top

【使用说明】
来源：http://kad.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://weq.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://utr.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qyq.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ngz.zycfv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lnv.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bld.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kdw.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dad.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vyd.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tyy.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pnt.aizwys.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ihv.fehbvm.com

【文件统计】
来源：http://hyv.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://teb.epnwcf.com

--------------------------------------------------------------------------------
来源：http://wzi.hysaishi.cn

目  录
来源：http://wmr.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://ush.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lbj.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mov.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uff.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eck.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nxo.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cgo.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aak.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sok.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kjf.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xjb.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zvs.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xbe.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qxs.sxryk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ytc.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lwc.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gao.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dpz.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://liu.feifeiyinyue.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aue.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bmb.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cwn.zhongyouzk.top

================================================================================
来源：http://ois.jlsjyb.cn

A. 基础语法与类型
来源：http://rnb.redwolf501.top

================================================================================
来源：http://bhb.cashguo.top

[A01] Hello World
来源：http://hbw.hammf.cn

Py:   print("Hello, World!")
来源：http://vaz.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://ava.pycfn.com

JS:   console.log("Hello, World!");
来源：http://nfm.feifeiyinyue.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lqv.birdmap.top

Java: System.out.println("Hello, World!");
来源：http://rev.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://txq.svipenyu.cn

Ruby: puts "Hello, World!"
来源：http://agv.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yst.andypj.xyz

[A02] 变量声明与赋值
来源：http://fjj.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uxs.meibo888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vla.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://oew.zhixingplan.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qke.tianlin.xyz

Java: String name = "Alex"; int age = 20;
来源：http://nyf.shanyushiyangtech.top

Go:   name := "Alex"; age := 20
来源：http://bge.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://nni.nanxinkj.top

C#:   string name = "Alex"; int age = 20;
来源：http://bvs.bjfxy.top

[A03] 常量定义
来源：http://guf.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://umh.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://qbh.hammf.cn

JS:   const PI = 3.14159;
来源：http://zwy.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://gms.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://qko.daria6918.cn

Go:   const PI = 3.14159
来源：http://prq.shanyushiyangkeji.top

Ruby: PI = 3.14159
来源：http://vzb.fanxiaobao.xyz

C#:   const double PI = 3.14159;
来源：http://anp.mhx1999.top

[A04] 判断变量类型
来源：http://zis.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pbz.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bai.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nvd.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://lld.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dpb.zhongyouzk.top

Go:   reflect.TypeOf(x).Name()
来源：http://urw.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bos.c1oappe.top

C#:   x.GetType().Name; x is int
来源：http://jqv.nanxinkj.top

[A05] 整数除法与取模
来源：http://mdc.zhaomingkeji.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://izi.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ruc.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dcl.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xln.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://qfe.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://pmw.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://ljk.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://ihg.havefunace.top

[A06] 字符串转数字
来源：http://iow.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://zzo.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kdr.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bac.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://asw.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fsr.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://emt.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ega.shuidangran.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yrh.xziqi.cn

[A07] 数字转字符串
来源：http://enj.vehdjk.com

Py:   str(42)
来源：http://oef.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://gbc.dashuyun.cn

JS:   String(42); (42).toString()
来源：http://qxz.uphjek.com

TS:   String(42)
来源：http://fsk.cashguo.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rsl.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://rlf.zhengqikj.top

Ruby: 42.to_s
来源：http://cjs.jqgfzy.top

C#:   42.ToString()
来源：http://anq.c1oappe.top

[A08] 取整与四舍五入
来源：http://iga.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kwb.yuanzhike.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gug.dashuyun.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vgw.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://drh.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://puo.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xkh.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vyt.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://otx.yueranfly.top

[A09] 绝对值与最大最小值
来源：http://ksd.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ohu.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://svz.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mkr.pengpengdd.cyou

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ral.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jmn.yj202588.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://okv.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ece.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sak.ivvv.top

[A10] 生成随机数
来源：http://bgm.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://bdk.hysaishi.cn

PHP:  random_int(1, 100);
来源：http://ibk.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dnr.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xtu.hfpthk.cn

Java: new Random().nextInt(100) + 1
来源：http://iwv.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wzo.yj20258.top

Ruby: rand(1..100)
来源：http://avq.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://wgm.yongpay.top

[A11] 条件表达式（三元）
来源：http://mqe.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://lsm.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qrr.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tjs.gzhubu.top

TS:   x > 0 ? "yes" : "no"
来源：http://ewu.vqdsnc.cn

Java: x > 0 ? "yes" : "no"
来源：http://xag.hywenlv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yai.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nwy.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://kpm.ppjwa.cn

[A12] 字符串插值 / 格式化
来源：http://mvn.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://emz.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tfs.yj202588.top

JS:   `Hello, ${name}!`
来源：http://hsx.hesvh.cn

TS:   `Hello, ${name}!`
来源：http://tgq.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://tya.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xbk.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://oxy.cashguo.top

C#:   $"Hello, {name}!"
来源：http://vhx.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dxm.316326.xyz


<!-- 参考信息 -->