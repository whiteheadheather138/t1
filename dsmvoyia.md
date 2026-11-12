代发 wailian999

[U77] PHP：模板渲染
来源：http://ftx.xinyue.icu

composer require twig/twig
来源：http://bav.zhongyouzk.top

[U78] PHP：单元测试
来源：http://tpm.pycfn.com

composer require --dev phpunit/phpunit
来源：http://htx.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://ekv.ivvv.top

composer require --dev phpstan/phpstan
来源：http://vvy.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://jdy.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wuc.yongpay.top

[U81] JS：初始化项目
来源：http://qcf.yj202588.top

npm init -y;  npm i express
来源：http://uxy.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://qxn.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bkc.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://fgs.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hrr.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://rhe.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://xhf.jianghu66.top

[U85] JS：可选链
来源：http://sij.zhaomingkeji.xyz

a?.b?.c
来源：http://svf.ctjpmb.com

[U86] JS：空值合并
来源：http://aax.wangshuangyany.cn

a ?? b
来源：http://fyj.epnwcf.com

[U87] JS：解构默认值
来源：http://zxt.tianlin.xyz

const { a = 1, b = 2 } = obj;
来源：http://tua.bjfxy.top

[U88] JS：对象展开合并
来源：http://llp.sweek.top

{ ...a, ...b }
来源：http://gth.jinghuilouyu.cn

[U89] JS：数组去重
来源：http://cfs.aizwys.cn

[...new Set(arr)]
来源：http://zgv.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://esf.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://wpy.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://zwr.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://szj.0kj1m.cn

[U92] JS：深拷贝
来源：http://qpl.xziqi.cn

structuredClone(obj)
来源：http://bxo.snrcjt.cn

[U93] JS：模板字符串
来源：http://lnm.vqdsnc.cn

`共 ${n} 条`
来源：http://fmd.daxiang520.top

[U94] JS：箭头函数
来源：http://hyw.jinghuilouyu.cn

const double = x => x * 2;
来源：http://kao.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://vxm.meibo888.top

new Promise((resolve, reject) => {})
来源：http://efs.sxryk.cn

[U96] JS：async/await 与异常
来源：http://zfa.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://szl.ydjk.org.cn

[U97] JS：并发请求
来源：http://nwi.vehdjk.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zqy.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://bcp.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fyw.daria6918.cn

[U99] JS：事件监听
来源：http://bfv.316326.xyz

el.addEventListener("click", e => {})
来源：http://byo.ivvv.top

[U100] JS：DOM 查询
来源：http://nqt.yj20258.top

document.querySelector(".item")
来源：http://pdj.daria6918.cn

[U101] JS：classList 操作
来源：http://zcz.cdnleiting.top

el.classList.toggle("active")
来源：http://mjn.xuanzx.com

[U102] JS：本地存储
来源：http://dss.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dft.ctjpmb.com

[U103] JS：定时器
来源：http://vbn.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://itp.xuanzx.com

[U104] JS：防抖
来源：http://rrb.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rzz.zhijiandao.cn

[U105] JS：节流
来源：http://upo.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qla.jinqigufen.top

[U106] JS：日期格式化
来源：http://uqm.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wbn.jlsjyb.cn

[U107] JS：数字千分位
来源：http://xwj.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://euu.zhongyouzk.top

[U108] JS：随机整数
来源：http://asy.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tqh.jlsjyb.cn

[U109] JS：数组分组
来源：http://vjn.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://wqw.cqqwz.cn

[U110] JS：数组分块
来源：http://doc.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://btt.havefunace.top

[U111] JS：对象转 Map
来源：http://syo.chenzaomai.com

new Map(Object.entries(obj))
来源：http://shw.52xcode.cn

[U112] JS：字符串补位
来源：http://mgi.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://kat.jinghuilouyu.cn

[U113] JS：正则替换全部
来源：http://jpl.dashuyun.cn

s.replaceAll("a", "b")
来源：http://qyr.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://ilu.chenzaomai.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqm.ehwqpu.com

[U115] JS：生成 UUID
来源：http://jub.iojbl.cn

crypto.randomUUID()
来源：http://lne.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://bze.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://pot.fengsongda.top

[U117] JS：单元测试
来源：http://wki.meibo888.top

npm i -D vitest;  npx vitest
来源：http://huc.birdmap.top

[U118] JS：开发服务器
来源：http://ozj.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://dtl.aizwys.cn

[U119] JS：生产构建
来源：http://gjx.yuxming.cn

npx vite build
来源：http://biv.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://aoc.yongpay.top

import.meta.env.VITE_API_URL
来源：http://zlt.guowangkeji.top

================================================================================
来源：http://lvn.vqdsnc.cn

统计汇总
来源：http://dfd.gzhubu.top

================================================================================
来源：http://yhv.ivvv.top

按语言统计（条）：
来源：http://lce.ctjpmb.com

Python ......... 252
来源：http://xmm.nanxinkj.top

PHP ............ 252
来源：http://kgw.yuanzhike.top

JavaScript ..... 252
来源：http://ixw.chenlongwang.top

TypeScript ..... 212
来源：http://iwe.hcnkem.com

Java ........... 212
来源：http://yqj.yueranfly.top

Go ............. 212
来源：http://owy.guowangkeji.top

Ruby ........... 212
来源：http://aym.shanyushiyangkeji.top

C# ............. 212
来源：http://pxl.yj20258.top

C .............. 30
来源：http://txm.zhiwuduotai.top

C++ ............ 30
来源：http://nxg.daxiang520.top

SQL ............ 90
来源：http://jsa.xziqi.cn

Bash ........... 80
来源：http://lgh.nanxuanxn.top

Kotlin ......... 15
来源：http://djd.zdbjq.cn

Swift .......... 15
来源：http://kef.andypj.xyz

Lua ............ 10
来源：http://kay.chenzaomai.com

Perl ........... 10
来源：http://qld.vqdsnc.cn

Scala .......... 10
来源：http://lme.nanxinkj.top

------------------------------------
来源：http://jao.sufxvd.cn

合计 ........... 2106 条
来源：http://aus.316326.xyz

按章节统计：
来源：http://ani.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bni.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sml.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uuy.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://awo.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dof.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mck.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xvf.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lsu.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://auu.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sfk.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vhp.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dtb.jqgfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cqu.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://woq.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qjm.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://krq.ctjpmb.com

Q SQL 专题                              90
来源：http://ofs.shzxlz.cn

R Bash 专题                             80
来源：http://eao.sxryk.cn

S C / C++ 专题                          60
来源：http://jmz.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://xue.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://wgr.fehbvm.com

------------------------------------
来源：http://jfz.yj202588.top

合计                                  2106 条
来源：http://vra.bbcook.cn

--------------------------------------------------------------------------------
来源：http://dbj.iojbl.cn

使用提醒
来源：http://usn.cheryme.top

--------------------------------------------------------------------------------
来源：http://hfo.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lgz.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://thj.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cla.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://faf.fengsongda.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tos.xinyue.icu

—— 文件结束 ——
来源：http://dic.jyoumei.cn

================================================================================
来源：http://ggl.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://icp.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://xvg.aibaodan.cn

================================================================================
来源：http://bul.hywenlv.cn

【收录内容】
来源：http://xtz.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wic.pycfn.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dil.tanke756.top

SQL · Bash · C · C++
来源：http://axk.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gxp.dianchejie.cn

【使用说明】
来源：http://tci.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ayh.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xew.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qdf.vehdjk.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ccx.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://erd.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iuk.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rpd.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bje.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://snt.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vnu.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ydq.jqgfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ivl.yj202588.top

【文件统计】
来源：http://hrr.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zfo.xuanzx.com

--------------------------------------------------------------------------------
来源：http://vny.gaohongyu789.top

目  录
来源：http://szi.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://xpd.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wwy.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pkq.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jxv.sufxvd.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mik.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ewl.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cen.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wsp.hesvh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iil.hywenlv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://utf.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yqs.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kgg.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pkp.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zlg.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://acq.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gcy.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://arz.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mze.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hed.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://one.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xoq.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vvi.yanxiufei.cn

================================================================================
来源：http://xqg.shanyushiyangkeji.top

A. 基础语法与类型
来源：http://uxq.tarul.cn

================================================================================
来源：http://niz.cheryme.top

[A01] Hello World
来源：http://hch.gogol.net.cn

Py:   print("Hello, World!")
来源：http://asp.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://uso.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://esf.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bhk.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://bij.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://pdh.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://tch.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://shp.wangdashe.top

[A02] 变量声明与赋值
来源：http://gst.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nna.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cjc.jqgufenzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://jng.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://afe.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://dxd.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://bjo.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://sjq.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://jqc.52xcode.cn

[A03] 常量定义
来源：http://ppw.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hzo.hammf.cn

PHP:  const PI = 3.14159;
来源：http://ryw.fengsongda.top

JS:   const PI = 3.14159;
来源：http://gml.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://ceh.uphjek.com

Java: static final double PI = 3.14159;
来源：http://ctj.bbcook.cn

Go:   const PI = 3.14159
来源：http://piy.bjfxy.top

Ruby: PI = 3.14159
来源：http://usz.yonumen.top

C#:   const double PI = 3.14159;
来源：http://zkk.tarul.cn

[A04] 判断变量类型
来源：http://bmd.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://syr.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fsf.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://asf.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://xcq.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iip.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lqf.gogol.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ora.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://qde.tanke756.top

[A05] 整数除法与取模
来源：http://xrr.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jed.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gon.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pka.zhijiandao.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xzu.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://uta.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://dxh.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://mlf.pengpengdd.cyou

C#:   7 / 2; 7 % 2
来源：http://tsp.fktsv.cn

[A06] 字符串转数字
来源：http://yxd.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://jxi.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pmv.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ybw.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://enn.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rjr.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mob.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qck.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zxy.zdqjudy.top

[A07] 数字转字符串
来源：http://piq.zdbjq.cn

Py:   str(42)
来源：http://mzm.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://kkv.hesvh.cn

JS:   String(42); (42).toString()
来源：http://sea.mhx1999.top

TS:   String(42)
来源：http://dhr.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ldb.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://tdb.zhaomingkeji.xyz

Ruby: 42.to_s
来源：http://vai.pycfn.com

C#:   42.ToString()
来源：http://ois.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://lld.shanyushiyangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zja.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yhl.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bti.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jkw.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lft.yonumen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lnw.smart0.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://vmx.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dbr.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://luv.shuidangran.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lcv.cheryme.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ljf.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uwz.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ddq.hesvh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tmc.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gkv.xinyue.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iwq.guowangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lps.cdnleiting.top

[A10] 生成随机数
来源：http://olh.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://yws.xinyue.icu

PHP:  random_int(1, 100);
来源：http://ngx.hongshengwenyu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wor.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ncx.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://wpk.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ldg.zhoulong.xyz

Ruby: rand(1..100)
来源：http://tju.zycfv.cn

C#:   new Random().Next(1, 101)
来源：http://lmb.cqqwz.cn

[A11] 条件表达式（三元）
来源：http://pno.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://uoi.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qpg.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mru.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://cyf.sufxvd.cn

Java: x > 0 ? "yes" : "no"
来源：http://srq.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://lzc.yj20258888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://khn.fanxiaobao.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://rfd.ivvv.top

[A12] 字符串插值 / 格式化
来源：http://uos.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mzy.kuanghao11.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hzz.haohaochexian.top

JS:   `Hello, ${name}!`
来源：http://dlw.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://snp.yuanzhike.top

Java: "Hello, %s!".formatted(name)
来源：http://els.yonumen.top


<!-- 参考信息 -->