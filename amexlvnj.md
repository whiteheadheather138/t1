代发 wailian999

[U79] PHP：静态分析
来源：http://ilm.yj20258.top

composer require --dev phpstan/phpstan
来源：http://omw.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://eku.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mav.zdbjq.cn

[U81] JS：初始化项目
来源：http://ihl.haohaochexian.top

npm init -y;  npm i express
来源：http://jbf.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://oty.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://djl.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://rzh.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rzt.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://mep.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://psy.fehbvm.com

[U85] JS：可选链
来源：http://lay.yanxiufei.cn

a?.b?.c
来源：http://ntu.yongpay.top

[U86] JS：空值合并
来源：http://lfd.yanxiufei.cn

a ?? b
来源：http://xcw.bjfxy.top

[U87] JS：解构默认值
来源：http://lar.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://zdo.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://dcg.c1oappe.top

{ ...a, ...b }
来源：http://ilu.mhx1999.top

[U89] JS：数组去重
来源：http://gjr.yj202588.top

[...new Set(arr)]
来源：http://puu.nwbrower.top

[U90] JS：数字数组排序
来源：http://pin.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://rzt.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://kgs.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://inl.redwolf501.top

[U92] JS：深拷贝
来源：http://ibd.zycfv.cn

structuredClone(obj)
来源：http://jyz.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://zhg.redwolf501.top

`共 ${n} 条`
来源：http://khj.hnqzz.top

[U94] JS：箭头函数
来源：http://ktt.ybcxt.top

const double = x => x * 2;
来源：http://gri.tianlin.xyz

[U95] JS：Promise 包装
来源：http://ygt.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://amd.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://sax.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ibl.9152youxi.cn

[U97] JS：并发请求
来源：http://odr.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ewn.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://vvo.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://joh.vehdjk.com

[U99] JS：事件监听
来源：http://zgv.redwolf501.top

el.addEventListener("click", e => {})
来源：http://ecz.ctjpmb.com

[U100] JS：DOM 查询
来源：http://qau.sxryk.cn

document.querySelector(".item")
来源：http://bre.ppjwa.cn

[U101] JS：classList 操作
来源：http://qay.aibaodan.cn

el.classList.toggle("active")
来源：http://ytw.yvedp.cn

[U102] JS：本地存储
来源：http://tfy.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://msv.jlsjyb.cn

[U103] JS：定时器
来源：http://qmh.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://grk.aizwys.cn

[U104] JS：防抖
来源：http://lzw.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kem.jinghuilouyu.cn

[U105] JS：节流
来源：http://fwa.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ddh.sweek.top

[U106] JS：日期格式化
来源：http://fmm.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vpq.yuxming.cn

[U107] JS：数字千分位
来源：http://pps.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nwz.tian-w.cn

[U108] JS：随机整数
来源：http://lrh.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kne.zycfv.cn

[U109] JS：数组分组
来源：http://odb.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://iyi.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://eqo.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aaz.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://zga.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://nyk.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://oqg.birdmap.top

"7".padStart(3, "0")
来源：http://ksi.gzhubu.top

[U113] JS：正则替换全部
来源：http://ckj.xinyue.icu

s.replaceAll("a", "b")
来源：http://hpo.yuxming.cn

[U114] JS：JSON 深比较
来源：http://jhc.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://xms.dashuyun.cn

[U115] JS：生成 UUID
来源：http://zvv.cqqwz.cn

crypto.randomUUID()
来源：http://ulr.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://viu.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://civ.yongpay.top

[U117] JS：单元测试
来源：http://fdo.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://dww.iojbl.cn

[U118] JS：开发服务器
来源：http://hbl.havefunace.top

npm i -D vite;  npx vite
来源：http://aae.bbcook.cn

[U119] JS：生产构建
来源：http://mhc.cdnleiting.top

npx vite build
来源：http://fyw.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://zaz.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://enq.jyoumei.cn

================================================================================
来源：http://eqk.hnqzz.top

统计汇总
来源：http://mox.ybcxt.top

================================================================================
来源：http://qfo.gotoacloud.top

按语言统计（条）：
来源：http://owx.ivvv.top

Python ......... 252
来源：http://ngx.zhongyouzk.top

PHP ............ 252
来源：http://bua.yuanzhike.top

JavaScript ..... 252
来源：http://jaq.yonumen.top

TypeScript ..... 212
来源：http://nrs.uphjek.com

Java ........... 212
来源：http://kss.xziqi.cn

Go ............. 212
来源：http://whe.vqdsnc.cn

Ruby ........... 212
来源：http://vyo.xylfe.cn

C# ............. 212
来源：http://ium.cdnleiting.top

C .............. 30
来源：http://dmc.iojbl.cn

C++ ............ 30
来源：http://eim.wangshuangyany.cn

SQL ............ 90
来源：http://qkn.ppjwa.cn

Bash ........... 80
来源：http://tow.chenzaomai.com

Kotlin ......... 15
来源：http://trc.shuidangran.top

Swift .......... 15
来源：http://vpp.chenzaomai.com

Lua ............ 10
来源：http://crx.yangfankeji.com

Perl ........... 10
来源：http://ble.jinqigfzy.top

Scala .......... 10
来源：http://vah.hfpthk.cn

------------------------------------
来源：http://fmq.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://rbb.aibaodan.cn

按章节统计：
来源：http://jwe.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rms.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iac.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bug.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://csa.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xcy.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yqe.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wor.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yaq.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ohs.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sht.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hcc.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://spd.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aod.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blo.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kcw.guowangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lai.redwolf501.top

Q SQL 专题                              90
来源：http://fic.c1oappe.top

R Bash 专题                             80
来源：http://ikx.hnqzz.top

S C / C++ 专题                          60
来源：http://mwm.jqgfzy.top

T 其他语言补充                          60
来源：http://kxa.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://nnv.guowangkeji.top

------------------------------------
来源：http://bce.tianlin.xyz

合计                                  2106 条
来源：http://tvb.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://ahr.fehbvm.com

使用提醒
来源：http://mfq.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://soi.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gec.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pey.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qtq.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wkq.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qbr.hnxiangtu.top

—— 文件结束 ——
来源：http://alh.bbcook.cn

================================================================================
来源：http://tce.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://njr.sxryk.cn

Common Programming Examples Cheat Book
来源：http://eod.chenjidiqi.icu

================================================================================
来源：http://btp.yfazqb.com

【收录内容】
来源：http://bdt.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xlk.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zuv.birdmap.top

SQL · Bash · C · C++
来源：http://tzw.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tkf.zhixingplan.top

【使用说明】
来源：http://yvr.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://geu.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://swm.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dvp.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hld.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nob.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dnt.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://stq.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qsi.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://anb.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hdb.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bmu.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bxq.yj202588.top

【文件统计】
来源：http://sqc.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ysw.wangdashe.top

--------------------------------------------------------------------------------
来源：http://uhf.0kj1m.cn

目  录
来源：http://eok.epnwcf.com

--------------------------------------------------------------------------------
来源：http://bqs.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eee.yongpay.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kmv.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://psx.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vsv.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zkv.hywenlv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vgk.xuetiantiany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pdz.yongpay.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hqp.wangdashe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iti.0kj1m.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xmy.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://esk.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bnq.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gfw.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://paj.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cpa.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fjt.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wvn.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bej.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tga.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://smt.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ehh.feifeiyinyue.top

================================================================================
来源：http://nvg.nanxinkj.top

A. 基础语法与类型
来源：http://txz.ywan-chungtsiang.top

================================================================================
来源：http://tix.hywenlv.cn

[A01] Hello World
来源：http://uzk.tarul.cn

Py:   print("Hello, World!")
来源：http://ztp.mhx1999.top

PHP:  echo "Hello, World!";
来源：http://onu.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://hiv.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zlo.yvedp.cn

Java: System.out.println("Hello, World!");
来源：http://qcr.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://apx.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://xml.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jtk.jinqigufen.top

[A02] 变量声明与赋值
来源：http://yfg.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nmi.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zso.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://hvv.52xcode.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vax.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://fhw.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://zht.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://dhg.cucudq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nfd.tanke756.top

[A03] 常量定义
来源：http://wgm.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bbw.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://wjw.yj202588.top

JS:   const PI = 3.14159;
来源：http://bjh.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://gsz.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://rzf.shzxlz.cn

Go:   const PI = 3.14159
来源：http://sjo.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://vkk.yj202588.top

C#:   const double PI = 3.14159;
来源：http://aae.sxryk.cn

[A04] 判断变量类型
来源：http://mmv.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://okd.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ahg.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pbm.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://nfu.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://avq.zhoulong.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://afr.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zkw.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://mbo.xziqi.cn

[A05] 整数除法与取模
来源：http://eit.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tiv.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://msq.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oyv.fzhhl.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://abx.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://rau.andypj.xyz

Go:   7 / 2; 7 % 2
来源：http://obc.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://vqk.chenzaomai.com

C#:   7 / 2; 7 % 2
来源：http://qlo.zhongyouzk.top

[A06] 字符串转数字
来源：http://klv.yfazqb.com

Py:   int("42"); float("3.14")
来源：http://iao.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gle.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uco.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://mck.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jjz.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zgr.snrcjt.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lyh.dianchejie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fwq.epnwcf.com

[A07] 数字转字符串
来源：http://lbu.ppjwa.cn

Py:   str(42)
来源：http://iom.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://vsz.sweek.top

JS:   String(42); (42).toString()
来源：http://thw.mhx1999.top

TS:   String(42)
来源：http://elo.pycfn.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://fwi.yvedp.cn

Go:   strconv.Itoa(42)
来源：http://guh.xuetiantiany.cn

Ruby: 42.to_s
来源：http://luh.chenlongwang.top

C#:   42.ToString()
来源：http://tlq.epnwcf.com

[A08] 取整与四舍五入
来源：http://cri.fehbvm.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ete.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://heo.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cxq.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yra.meibo888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fxq.aizwys.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wmu.zhengqikj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vhb.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kjo.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://dqm.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xqu.zycfv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qlr.jinqigfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mif.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gyt.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://isc.birdmap.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ibk.iojbl.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ivb.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://smi.52xcode.cn

[A10] 生成随机数
来源：http://lxs.yongpay.top

Py:   import random; random.randint(1, 100)
来源：http://ufh.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://dxd.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iim.ybcxt.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mdd.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://wfc.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gbr.hysaishi.cn

Ruby: rand(1..100)
来源：http://qjs.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://fxf.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://hxg.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://zee.hfpthk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uut.tanke756.top

JS:   x > 0 ? "yes" : "no"
来源：http://qot.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://bvf.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://wmz.yueranfly.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qyl.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://twm.cucudq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ubs.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://osi.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nvw.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cpl.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://ufp.jlsjyb.cn

TS:   `Hello, ${name}!`
来源：http://qlw.sxryk.cn

Java: "Hello, %s!".formatted(name)
来源：http://hqr.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sli.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://hfm.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://lmi.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qef.hcnkem.com


<!-- 参考信息 -->