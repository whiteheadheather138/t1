代发 wailian999

[U77] PHP：模板渲染
来源：http://vtg.zhiwuduotai.top

composer require twig/twig
来源：http://huo.sweek.top

[U78] PHP：单元测试
来源：http://vor.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://ayg.chenzaomai.com

[U79] PHP：静态分析
来源：http://ler.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://guc.sweek.top

[U80] PHP：代码规范修复
来源：http://iwq.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tfw.cdnleiting.top

[U81] JS：初始化项目
来源：http://zsd.gotoacloud.top

npm init -y;  npm i express
来源：http://gwj.fengsongda.top

[U82] JS：package.json 脚本
来源：http://fbl.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fht.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://qiu.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://xpa.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://hom.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://dvf.9152youxi.cn

[U85] JS：可选链
来源：http://gaf.52xcode.cn

a?.b?.c
来源：http://jlr.hywenlv.cn

[U86] JS：空值合并
来源：http://vlo.pycfn.com

a ?? b
来源：http://spd.zhengqikj.top

[U87] JS：解构默认值
来源：http://ktg.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://bzj.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://qde.ydzc1.top

{ ...a, ...b }
来源：http://wlk.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://ool.316326.xyz

[...new Set(arr)]
来源：http://ixl.zdbjq.cn

[U90] JS：数字数组排序
来源：http://pla.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://gqe.yongpay.top

[U91] JS：对象键值遍历
来源：http://ghs.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dmu.dashuyun.cn

[U92] JS：深拷贝
来源：http://msc.yj202588.top

structuredClone(obj)
来源：http://hyo.zhixingplan.top

[U93] JS：模板字符串
来源：http://uas.tanke756.top

`共 ${n} 条`
来源：http://apb.zdbjq.cn

[U94] JS：箭头函数
来源：http://jdr.hnxiangtu.top

const double = x => x * 2;
来源：http://onx.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://xao.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://aqs.meibo888.top

[U96] JS：async/await 与异常
来源：http://myf.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qrp.zhixingplan.top

[U97] JS：并发请求
来源：http://gsv.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bxm.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://adk.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wiq.yongpay.top

[U99] JS：事件监听
来源：http://bsi.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://goz.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://wck.gaohongyu789.top

document.querySelector(".item")
来源：http://eqh.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://pyw.chenzaomai.com

el.classList.toggle("active")
来源：http://rzl.chenjidiqi.icu

[U102] JS：本地存储
来源：http://ohj.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ntk.yj20258888.top

[U103] JS：定时器
来源：http://anq.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kui.shangyingyoupin.top

[U104] JS：防抖
来源：http://mnf.cheryme.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfz.redwolf501.top

[U105] JS：节流
来源：http://ycw.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tfb.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://uqt.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ozy.pengpengdd.cyou

[U107] JS：数字千分位
来源：http://crl.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hvp.ydzc1.top

[U108] JS：随机整数
来源：http://crq.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://odu.c1oappe.top

[U109] JS：数组分组
来源：http://xfh.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://yyu.zhijiandao.cn

[U110] JS：数组分块
来源：http://pll.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vbe.snrcjt.cn

[U111] JS：对象转 Map
来源：http://eju.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://mvo.hcnkem.com

[U112] JS：字符串补位
来源：http://gqh.cqqwz.cn

"7".padStart(3, "0")
来源：http://ayh.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://ybh.yangfankeji.com

s.replaceAll("a", "b")
来源：http://gyl.redwolf501.top

[U114] JS：JSON 深比较
来源：http://osw.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://kab.yangfankeji.com

[U115] JS：生成 UUID
来源：http://bso.sxryk.cn

crypto.randomUUID()
来源：http://htl.sweek.top

[U116] JS：类型检查（JSDoc）
来源：http://jqz.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://bvl.xylfe.cn

[U117] JS：单元测试
来源：http://kyv.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://dvx.hcnkem.com

[U118] JS：开发服务器
来源：http://dlb.bbcook.cn

npm i -D vite;  npx vite
来源：http://tdc.ybcxt.top

[U119] JS：生产构建
来源：http://yki.jinqigufen.top

npx vite build
来源：http://htp.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://cjq.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://kus.xylfe.cn

================================================================================
来源：http://clq.tarul.cn

统计汇总
来源：http://gdw.sxryk.cn

================================================================================
来源：http://oxy.daria6918.cn

按语言统计（条）：
来源：http://zdf.birdmap.top

Python ......... 252
来源：http://yzw.epnwcf.com

PHP ............ 252
来源：http://lnp.xziqi.cn

JavaScript ..... 252
来源：http://tgb.shanyushiyangtech.top

TypeScript ..... 212
来源：http://soy.gaohongyu789.top

Java ........... 212
来源：http://brw.dashuyun.cn

Go ............. 212
来源：http://shi.zycfv.cn

Ruby ........... 212
来源：http://orx.xylfe.cn

C# ............. 212
来源：http://sov.xziqi.cn

C .............. 30
来源：http://dpq.kuanghao11.cn

C++ ............ 30
来源：http://ole.smart0.xyz

SQL ............ 90
来源：http://vvx.yj20258888.top

Bash ........... 80
来源：http://pvf.bjfxy.top

Kotlin ......... 15
来源：http://pud.cheryme.top

Swift .......... 15
来源：http://fun.hfpthk.cn

Lua ............ 10
来源：http://ron.zdqjudy.top

Perl ........... 10
来源：http://iae.jyoumei.cn

Scala .......... 10
来源：http://baw.ydzc1.top

------------------------------------
来源：http://qwh.birdmap.top

合计 ........... 2106 条
来源：http://grs.ywan-chungtsiang.top

按章节统计：
来源：http://mmu.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mmx.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ocl.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bdg.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xdc.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vra.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yxr.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxa.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ztt.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://foe.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bej.gotoacloud.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ukx.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fcr.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qhs.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zjz.yj20258888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gsp.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wpg.epnwcf.com

Q SQL 专题                              90
来源：http://lop.zhiwuduotai.top

R Bash 专题                             80
来源：http://mkv.zhongyouzk.top

S C / C++ 专题                          60
来源：http://cya.jinqigfzy.top

T 其他语言补充                          60
来源：http://reu.xylfe.cn

U 高频实用片段                         120
来源：http://wmc.hnxiangtu.top

------------------------------------
来源：http://ygo.epnwcf.com

合计                                  2106 条
来源：http://vvq.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://qiy.sjlbkw.cn

使用提醒
来源：http://fpj.xinyue.icu

--------------------------------------------------------------------------------
来源：http://peh.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ian.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aku.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://inm.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://uol.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qjv.xziqi.cn

—— 文件结束 ——
来源：http://zub.daxiang520.top

================================================================================
来源：http://rgr.cdnleiting.top

程序语言常见例子速查手册（2024 版）
来源：http://iin.yj20258.top

Common Programming Examples Cheat Book
来源：http://mmq.316326.xyz

================================================================================
来源：http://lfw.jqgfzy.top

【收录内容】
来源：http://xsk.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://wgm.fengsongda.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fst.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://qzm.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hco.gogol.net.cn

【使用说明】
来源：http://fyq.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rfn.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://smz.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mjd.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iqs.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tld.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hzy.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ram.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ucp.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cie.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nts.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ddt.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xpp.redwolf501.top

【文件统计】
来源：http://stq.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xdb.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://din.guannengcc.top

目  录
来源：http://uib.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://frv.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://phq.zhixingplan.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hzk.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hux.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hvw.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ezq.jlsjyb.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fyv.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://txd.wangshuangyany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ofu.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gra.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mhg.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pnn.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jil.ydjk.org.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oyg.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://clo.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pqe.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zoo.fanxiaobao.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gev.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zak.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ouv.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://skj.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://onm.jinyuanbaomall.cn

================================================================================
来源：http://qhy.dashuyun.cn

A. 基础语法与类型
来源：http://suq.smart0.xyz

================================================================================
来源：http://rzt.0kj1m.cn

[A01] Hello World
来源：http://bay.yuxming.cn

Py:   print("Hello, World!")
来源：http://zxa.sxryk.cn

PHP:  echo "Hello, World!";
来源：http://fgu.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://byz.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ytc.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://vzm.fktsv.cn

Go:   fmt.Println("Hello, World!")
来源：http://rah.meibo888.top

Ruby: puts "Hello, World!"
来源：http://dlm.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://agf.jyoumei.cn

[A02] 变量声明与赋值
来源：http://uoy.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iwz.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://iza.gaohongyu789.top

JS:   let name = "Alex"; const age = 20;
来源：http://ybr.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oce.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://yvd.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://usq.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://shk.quarkkingdee.top

C#:   string name = "Alex"; int age = 20;
来源：http://cns.uphjek.com

[A03] 常量定义
来源：http://vov.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ycm.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://wmd.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://vxu.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://aif.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://nfu.nwbrower.top

Go:   const PI = 3.14159
来源：http://kvh.aizwys.cn

Ruby: PI = 3.14159
来源：http://pet.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://idj.zhengqikj.top

[A04] 判断变量类型
来源：http://cvb.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pda.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zsf.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nwx.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://ohj.quarkkingdee.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://plw.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://wsp.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nnk.birdmap.top

C#:   x.GetType().Name; x is int
来源：http://oog.cucudq.cn

[A05] 整数除法与取模
来源：http://bhp.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nxb.tarul.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://avy.gzhubu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://trh.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iip.haohaochexian.top

Java: 7 / 2; 7 % 2
来源：http://jrd.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://ghc.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://whz.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://gcb.aizwys.cn

[A06] 字符串转数字
来源：http://gqg.tanke756.top

Py:   int("42"); float("3.14")
来源：http://dvw.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nmo.yj202588.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aqm.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dvy.zhengqikj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zbt.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dej.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jgr.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gdk.sjlbkw.cn

[A07] 数字转字符串
来源：http://lyu.jqgufenzy.top

Py:   str(42)
来源：http://hxs.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://gxl.xinyue.icu

JS:   String(42); (42).toString()
来源：http://jsv.xylfe.cn

TS:   String(42)
来源：http://xuq.svipenyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eeh.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://hjq.fengsongda.top

Ruby: 42.to_s
来源：http://omf.ctjpmb.com

C#:   42.ToString()
来源：http://iqj.zycfv.cn

[A08] 取整与四舍五入
来源：http://lzy.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zdz.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jta.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dpm.tanke756.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iim.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uxz.yueranfly.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ekw.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sbz.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vwi.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://uta.sxryk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hfs.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://czf.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mla.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://otq.birdmap.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ezx.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qcn.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://azw.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gdz.iojbl.cn

[A10] 生成随机数
来源：http://nqx.jinqigufen.top

Py:   import random; random.randint(1, 100)
来源：http://vip.nwbrower.top

PHP:  random_int(1, 100);
来源：http://jwu.ywan-chungtsiang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fld.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vrn.tianlin.xyz

Java: new Random().nextInt(100) + 1
来源：http://tuq.jiagoushi.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yop.yangfankeji.com

Ruby: rand(1..100)
来源：http://exo.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://ggx.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://dtb.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://ppv.zhijiandao.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://slh.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://twi.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jfv.yfazqb.com

Java: x > 0 ? "yes" : "no"
来源：http://wyc.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://ejr.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rqh.zdqjudy.top

C#:   x > 0 ? "yes" : "no"
来源：http://rpr.mhx1999.top

[A12] 字符串插值 / 格式化
来源：http://zcs.vehdjk.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dln.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://exy.jqgfzy.top

JS:   `Hello, ${name}!`
来源：http://lkp.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://ftm.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://ocw.bbcook.cn


<!-- 参考信息 -->