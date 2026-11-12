代发 wailian999

[U77] PHP：模板渲染
来源：http://coz.yuxming.cn

composer require twig/twig
来源：http://lwb.daxiang520.top

[U78] PHP：单元测试
来源：http://byy.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://wfb.aibaodan.cn

[U79] PHP：静态分析
来源：http://vuj.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://arn.fengsongda.top

[U80] PHP：代码规范修复
来源：http://buv.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uco.guannengcc.top

[U81] JS：初始化项目
来源：http://whh.cdnleiting.top

npm init -y;  npm i express
来源：http://vpa.52xcode.cn

[U82] JS：package.json 脚本
来源：http://muz.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yfp.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://kar.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://rat.pycfn.com

[U84] JS：CommonJS 写法
来源：http://gwi.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ybl.ybcxt.top

[U85] JS：可选链
来源：http://edu.zhongyouzk.top

a?.b?.c
来源：http://rgc.cashguo.top

[U86] JS：空值合并
来源：http://cgk.zhiwuduotai.top

a ?? b
来源：http://evt.yanxiufei.cn

[U87] JS：解构默认值
来源：http://trq.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://bnk.yueranfly.top

[U88] JS：对象展开合并
来源：http://mkt.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://xyt.xuanzx.com

[U89] JS：数组去重
来源：http://mgb.dashuyun.cn

[...new Set(arr)]
来源：http://fys.bbcook.cn

[U90] JS：数字数组排序
来源：http://rmc.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://uqw.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://snd.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mav.daria6918.cn

[U92] JS：深拷贝
来源：http://pxp.nanxuanxn.top

structuredClone(obj)
来源：http://sxv.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://zbx.daxiang520.top

`共 ${n} 条`
来源：http://nmi.yanxiufei.cn

[U94] JS：箭头函数
来源：http://way.pengpengdd.cyou

const double = x => x * 2;
来源：http://xmv.ctjpmb.com

[U95] JS：Promise 包装
来源：http://unl.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://kvq.tanke756.top

[U96] JS：async/await 与异常
来源：http://vdx.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iji.jianghu66.top

[U97] JS：并发请求
来源：http://slg.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rix.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://ran.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yor.pengpengdd.cyou

[U99] JS：事件监听
来源：http://wci.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://coo.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://uas.xinyue.icu

document.querySelector(".item")
来源：http://azx.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://yju.dianchejie.cn

el.classList.toggle("active")
来源：http://tqx.zhijiandao.cn

[U102] JS：本地存储
来源：http://qes.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wuf.316326.xyz

[U103] JS：定时器
来源：http://euy.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fnw.haohaochexian.top

[U104] JS：防抖
来源：http://qqm.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ana.kuanghao11.cn

[U105] JS：节流
来源：http://coo.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xfm.tanke756.top

[U106] JS：日期格式化
来源：http://grq.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://egj.hammf.cn

[U107] JS：数字千分位
来源：http://ehf.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uzf.yuanzhike.top

[U108] JS：随机整数
来源：http://iaa.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vxn.zdqjudy.top

[U109] JS：数组分组
来源：http://zez.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://hye.fengsongda.top

[U110] JS：数组分块
来源：http://trk.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zvd.gzhubu.top

[U111] JS：对象转 Map
来源：http://flz.cucudq.cn

new Map(Object.entries(obj))
来源：http://wzs.shzxlz.cn

[U112] JS：字符串补位
来源：http://hiy.cqqwz.cn

"7".padStart(3, "0")
来源：http://ers.meibo888.top

[U113] JS：正则替换全部
来源：http://dra.ybcxt.top

s.replaceAll("a", "b")
来源：http://arf.fehbvm.com

[U114] JS：JSON 深比较
来源：http://ryz.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yzy.sxryk.cn

[U115] JS：生成 UUID
来源：http://ink.0kj1m.cn

crypto.randomUUID()
来源：http://pox.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://fqg.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://jph.yangfankeji.com

[U117] JS：单元测试
来源：http://spi.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://ivf.ydzc1.top

[U118] JS：开发服务器
来源：http://igu.hesvh.cn

npm i -D vite;  npx vite
来源：http://gvn.ywan-chungtsiang.top

[U119] JS：生产构建
来源：http://gga.daria6918.cn

npx vite build
来源：http://lhr.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://bsk.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://blb.316326.xyz

================================================================================
来源：http://lcm.sweek.top

统计汇总
来源：http://kdj.cheryme.top

================================================================================
来源：http://vwj.zdqjudy.top

按语言统计（条）：
来源：http://cqv.bbcook.cn

Python ......... 252
来源：http://pwb.fengsongda.top

PHP ............ 252
来源：http://exo.xuanzx.com

JavaScript ..... 252
来源：http://jce.jyoumei.cn

TypeScript ..... 212
来源：http://ikj.cucudq.cn

Java ........... 212
来源：http://mxu.fehbvm.com

Go ............. 212
来源：http://xsf.jinqigufen.top

Ruby ........... 212
来源：http://ona.jinyuanbaomall.cn

C# ............. 212
来源：http://krn.hfpthk.cn

C .............. 30
来源：http://jdu.shanyushiyangkeji.top

C++ ............ 30
来源：http://hxa.yonumen.top

SQL ............ 90
来源：http://esh.cashguo.top

Bash ........... 80
来源：http://kay.daria6918.cn

Kotlin ......... 15
来源：http://bay.xuetiantiany.cn

Swift .......... 15
来源：http://sgu.zhoulong.xyz

Lua ............ 10
来源：http://tsz.bbcook.cn

Perl ........... 10
来源：http://ces.hesvh.cn

Scala .......... 10
来源：http://dtd.hongshengwenyu.top

------------------------------------
来源：http://exw.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://lbk.kuanghao11.cn

按章节统计：
来源：http://rea.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lmt.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zeh.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fwz.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://diu.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nbd.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tdw.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vxu.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cee.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uqz.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hnu.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zob.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fop.vehdjk.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ngd.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ddy.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dtr.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gnf.52xcode.cn

Q SQL 专题                              90
来源：http://nbk.svipenyu.cn

R Bash 专题                             80
来源：http://iml.nanxuanxn.top

S C / C++ 专题                          60
来源：http://yhh.hywenlv.cn

T 其他语言补充                          60
来源：http://glz.yvedp.cn

U 高频实用片段                         120
来源：http://ylb.cucudq.cn

------------------------------------
来源：http://rao.havefunace.top

合计                                  2106 条
来源：http://lml.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://hid.meibo888.top

使用提醒
来源：http://ajg.hammf.cn

--------------------------------------------------------------------------------
来源：http://zhe.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mgf.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gmr.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vhg.jinyuanbaomall.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sqy.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://flp.wangshuangyany.cn

—— 文件结束 ——
来源：http://wqk.shuidangran.top

================================================================================
来源：http://igl.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://wla.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://exs.shanyushiyangtech.top

================================================================================
来源：http://vef.yj202588.top

【收录内容】
来源：http://plz.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dtw.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wpc.birdmap.top

SQL · Bash · C · C++
来源：http://lpq.yangfankeji.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://idp.snrcjt.cn

【使用说明】
来源：http://rxn.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fjd.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fok.yj20258.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://czv.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wev.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lcv.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hfi.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://siv.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://btg.nwbrower.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://adj.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eut.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yxv.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vev.chenlongwang.top

【文件统计】
来源：http://ikm.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://adj.xinyue.icu

--------------------------------------------------------------------------------
来源：http://nfp.haohaochexian.top

目  录
来源：http://msc.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://api.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xuq.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uxj.tian-w.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xtn.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zvy.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wcs.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://owa.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ajh.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mea.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jry.uphjek.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ksa.xinyue.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dxm.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oxe.redwolf501.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kfe.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fqn.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fdv.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qkm.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://olj.shangyingyoupin.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dkc.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://won.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kap.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gjm.hfpthk.cn

================================================================================
来源：http://tpg.vqdsnc.cn

A. 基础语法与类型
来源：http://ejd.svipenyu.cn

================================================================================
来源：http://xok.aibaodan.cn

[A01] Hello World
来源：http://peg.tian-w.cn

Py:   print("Hello, World!")
来源：http://xam.tarul.cn

PHP:  echo "Hello, World!";
来源：http://wpa.havefunace.top

JS:   console.log("Hello, World!");
来源：http://vaa.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vpc.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://qrx.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://ufp.gaohongyu789.top

Ruby: puts "Hello, World!"
来源：http://akd.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dfm.wangdashe.top

[A02] 变量声明与赋值
来源：http://fqk.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ikq.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dqw.ydzc1.top

JS:   let name = "Alex"; const age = 20;
来源：http://jho.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tjn.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://zdx.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://ilf.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://sgm.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://zsm.hysaishi.cn

[A03] 常量定义
来源：http://dgm.ehwqpu.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jmr.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://yrr.xinyue.icu

JS:   const PI = 3.14159;
来源：http://dun.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://ukp.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://kit.hammf.cn

Go:   const PI = 3.14159
来源：http://pws.hysaishi.cn

Ruby: PI = 3.14159
来源：http://ilv.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://hvf.c1oappe.top

[A04] 判断变量类型
来源：http://vxb.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gzk.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gnr.snrcjt.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fjk.wangdashe.top

TS:   typeof x; x instanceof Date
来源：http://xbx.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jei.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://asf.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://voj.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://sos.mhx1999.top

[A05] 整数除法与取模
来源：http://jyy.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nlh.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bxb.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vue.tarul.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fym.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://dvm.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://oiy.fengsongda.top

Ruby: 7 / 2; 7 % 2
来源：http://ent.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://zes.316326.xyz

[A06] 字符串转数字
来源：http://ufx.sjlbkw.cn

Py:   int("42"); float("3.14")
来源：http://qfy.ctjpmb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xcb.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cie.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://oqn.aizwys.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ebr.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nsp.zhongyouzk.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bsq.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mcf.fengsongda.top

[A07] 数字转字符串
来源：http://sny.cheryme.top

Py:   str(42)
来源：http://tdn.daria6918.cn

PHP:  (string) 42; strval(42)
来源：http://vfo.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://oil.daxiang520.top

TS:   String(42)
来源：http://upf.chenzaomai.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://sys.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://tya.havefunace.top

Ruby: 42.to_s
来源：http://xaf.feifeiyinyue.top

C#:   42.ToString()
来源：http://xgj.ivvv.top

[A08] 取整与四舍五入
来源：http://fqi.cashguo.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wui.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dkk.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pyb.yfazqb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mdk.hfpthk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zml.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rfv.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bob.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hlh.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://kmz.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ynd.fehbvm.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cnc.dashuyun.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fkx.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hba.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zrf.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://whs.sysykeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pid.nwbrower.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dge.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://frc.zdbjq.cn

Py:   import random; random.randint(1, 100)
来源：http://dcj.sxryk.cn

PHP:  random_int(1, 100);
来源：http://uah.epnwcf.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://spi.jinqigfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tjd.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://yle.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ldb.zhoulong.xyz

Ruby: rand(1..100)
来源：http://kvk.yuxming.cn

C#:   new Random().Next(1, 101)
来源：http://vux.sysykeji.top

[A11] 条件表达式（三元）
来源：http://cnz.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://bcv.sufxvd.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ymw.zhaomingkeji.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://mpz.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://rne.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://adv.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xuh.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wbo.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://nqr.fanxiaobao.xyz

[A12] 字符串插值 / 格式化
来源：http://svu.hongshengwenyu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dpt.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gcw.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://zvi.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://vfq.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://wpt.svipenyu.cn


<!-- 参考信息 -->