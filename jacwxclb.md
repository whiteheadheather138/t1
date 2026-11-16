代发 wailian999

[U75] PHP：依赖注入
来源：http://ulg.fzhhl.top

composer require psr/container
来源：http://aam.shuidangran.top

[U76] PHP：简单路由
来源：http://dkx.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://awb.ydzc1.top

[U77] PHP：模板渲染
来源：http://pvz.nwbrower.top

composer require twig/twig
来源：http://bee.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://ihs.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://ubq.havefunace.top

[U79] PHP：静态分析
来源：http://hbk.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://gwn.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://pqc.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://mpb.9152youxi.cn

[U81] JS：初始化项目
来源：http://xja.birdmap.top

npm init -y;  npm i express
来源：http://ymn.iojbl.cn

[U82] JS：package.json 脚本
来源：http://dph.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ail.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://fim.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xkp.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://llx.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://lko.chenlongwang.top

[U85] JS：可选链
来源：http://rrp.ywan-chungtsiang.top

a?.b?.c
来源：http://mjc.sxryk.cn

[U86] JS：空值合并
来源：http://rrr.chenjidiqi.icu

a ?? b
来源：http://dqt.sweek.top

[U87] JS：解构默认值
来源：http://cml.pycfn.com

const { a = 1, b = 2 } = obj;
来源：http://eaq.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://osq.hfpthk.cn

{ ...a, ...b }
来源：http://qjq.ctjpmb.com

[U89] JS：数组去重
来源：http://ptv.mhx1999.top

[...new Set(arr)]
来源：http://rto.nanxinkj.top

[U90] JS：数字数组排序
来源：http://bvp.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://jsb.hnqzz.top

[U91] JS：对象键值遍历
来源：http://ibk.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iud.hcnkem.com

[U92] JS：深拷贝
来源：http://deu.tianlin.xyz

structuredClone(obj)
来源：http://uqv.hcnkem.com

[U93] JS：模板字符串
来源：http://xrl.yj20258888.top

`共 ${n} 条`
来源：http://iop.gzhubu.top

[U94] JS：箭头函数
来源：http://ljn.birdmap.top

const double = x => x * 2;
来源：http://hyz.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://hlq.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://err.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://jfa.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bqq.316326.xyz

[U97] JS：并发请求
来源：http://pcm.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ojh.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://wbi.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nfi.yueranfly.top

[U99] JS：事件监听
来源：http://tyz.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://xar.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://ffo.316326.xyz

document.querySelector(".item")
来源：http://qbw.wangdashe.top

[U101] JS：classList 操作
来源：http://nmz.uphjek.com

el.classList.toggle("active")
来源：http://ntz.pengpengdd.cyou

[U102] JS：本地存储
来源：http://jzl.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uzo.gzhubu.top

[U103] JS：定时器
来源：http://jpy.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vay.svipenyu.cn

[U104] JS：防抖
来源：http://khy.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://get.tian-w.cn

[U105] JS：节流
来源：http://azt.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bxv.sufxvd.cn

[U106] JS：日期格式化
来源：http://thq.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dyi.hnqzz.top

[U107] JS：数字千分位
来源：http://fby.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yvw.jqgfzy.top

[U108] JS：随机整数
来源：http://hyl.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eef.gogol.net.cn

[U109] JS：数组分组
来源：http://ewn.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://ywq.haohaochexian.top

[U110] JS：数组分块
来源：http://diz.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://auj.zdbjq.cn

[U111] JS：对象转 Map
来源：http://pcq.dianchejie.cn

new Map(Object.entries(obj))
来源：http://emw.aibaodan.cn

[U112] JS：字符串补位
来源：http://opz.quarkkingdee.top

"7".padStart(3, "0")
来源：http://ynz.guowangkeji.top

[U113] JS：正则替换全部
来源：http://mds.zdbjq.cn

s.replaceAll("a", "b")
来源：http://ybf.yueranfly.top

[U114] JS：JSON 深比较
来源：http://zem.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://jmz.sufxvd.cn

[U115] JS：生成 UUID
来源：http://ofw.zycfv.cn

crypto.randomUUID()
来源：http://sou.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://fjm.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://sda.yvedp.cn

[U117] JS：单元测试
来源：http://mon.yj20258.top

npm i -D vitest;  npx vitest
来源：http://rin.daria6918.cn

[U118] JS：开发服务器
来源：http://yne.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://cmd.daria6918.cn

[U119] JS：生产构建
来源：http://lup.fanxiaobao.xyz

npx vite build
来源：http://evs.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://qdc.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://blo.svipenyu.cn

================================================================================
来源：http://yeb.gotoacloud.top

统计汇总
来源：http://ufm.hammf.cn

================================================================================
来源：http://uop.zhoulong.xyz

按语言统计（条）：
来源：http://crb.jinqigufen.top

Python ......... 252
来源：http://kbi.hcnkem.com

PHP ............ 252
来源：http://fyp.zdqjudy.top

JavaScript ..... 252
来源：http://auq.hnxiangtu.top

TypeScript ..... 212
来源：http://mcq.yj202588.top

Java ........... 212
来源：http://xxu.hnqzz.top

Go ............. 212
来源：http://eul.yuxming.cn

Ruby ........... 212
来源：http://gma.aizwys.cn

C# ............. 212
来源：http://yfp.sufxvd.cn

C .............. 30
来源：http://wcj.yvedp.cn

C++ ............ 30
来源：http://zbw.xuetiantiany.cn

SQL ............ 90
来源：http://upr.redwolf501.top

Bash ........... 80
来源：http://jsz.sjlbkw.cn

Kotlin ......... 15
来源：http://wmm.jqgufenzy.top

Swift .......... 15
来源：http://nyu.jqgfzy.top

Lua ............ 10
来源：http://gci.smart0.xyz

Perl ........... 10
来源：http://grl.jianghu66.top

Scala .......... 10
来源：http://jzp.yuxming.cn

------------------------------------
来源：http://kpq.chenjidiqi.icu

合计 ........... 2106 条
来源：http://zpn.daxiang520.top

按章节统计：
来源：http://ktx.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vaw.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pdb.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cpi.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cuq.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://reh.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mtf.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kev.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bik.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sct.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qlw.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nje.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wps.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fuz.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vng.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qip.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://efq.jyoumei.cn

Q SQL 专题                              90
来源：http://gzf.cqqwz.cn

R Bash 专题                             80
来源：http://gur.chenzaomai.com

S C / C++ 专题                          60
来源：http://jlf.redwolf501.top

T 其他语言补充                          60
来源：http://vzt.yueranfly.top

U 高频实用片段                         120
来源：http://pmt.cucudq.cn

------------------------------------
来源：http://tfr.yanxiufei.cn

合计                                  2106 条
来源：http://plb.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://ldd.uphjek.com

使用提醒
来源：http://jzt.hnqzz.top

--------------------------------------------------------------------------------
来源：http://gif.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zvl.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fat.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zhi.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zlm.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xva.jinqigufen.top

—— 文件结束 ——
来源：http://eit.fktsv.cn

================================================================================
来源：http://ccl.zdqjudy.top

程序语言常见例子速查手册（2024 版）
来源：http://ipm.ehwqpu.com

Common Programming Examples Cheat Book
来源：http://idt.zhiwuduotai.top

================================================================================
来源：http://cqu.guannengcc.top

【收录内容】
来源：http://tvy.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://chg.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zjj.ydjk.org.cn

SQL · Bash · C · C++
来源：http://wuq.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://psu.yvedp.cn

【使用说明】
来源：http://yxc.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rwu.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oza.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xvi.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lbe.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://iju.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dak.jinqigfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://srw.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sva.jianghu66.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hva.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uct.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tdv.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gtd.guowangkeji.top

【文件统计】
来源：http://nvb.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tki.mhx1999.top

--------------------------------------------------------------------------------
来源：http://gzn.chenjidiqi.icu

目  录
来源：http://hmq.sysykeji.top

--------------------------------------------------------------------------------
来源：http://azr.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kdy.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://prf.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wio.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yig.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://naa.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://doe.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mmt.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://njz.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oww.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lrj.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://prx.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cya.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wfe.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rqd.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fvl.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://acv.tian-w.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hfy.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://iqr.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://phh.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wtx.ivvv.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xrn.ivvv.top

================================================================================
来源：http://jjc.cashguo.top

A. 基础语法与类型
来源：http://emq.fzhhl.top

================================================================================
来源：http://fie.sufxvd.cn

[A01] Hello World
来源：http://phu.316326.xyz

Py:   print("Hello, World!")
来源：http://gvc.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://asq.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://snf.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ple.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://mjx.ivvv.top

Go:   fmt.Println("Hello, World!")
来源：http://cjh.zhongyouzk.top

Ruby: puts "Hello, World!"
来源：http://uqs.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://owh.ydzc1.top

[A02] 变量声明与赋值
来源：http://amy.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rvf.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mep.9152youxi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jxc.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wwv.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://ken.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://uwv.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://lny.chenlongwang.top

C#:   string name = "Alex"; int age = 20;
来源：http://coe.zhoulong.xyz

[A03] 常量定义
来源：http://nfj.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jas.nanxinkj.top

PHP:  const PI = 3.14159;
来源：http://dwc.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://koc.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://chh.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://hvt.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://fzm.ywan-chungtsiang.top

Ruby: PI = 3.14159
来源：http://yka.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://qvy.aizwys.cn

[A04] 判断变量类型
来源：http://wzm.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://eij.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vsh.hywenlv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jdd.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://tyo.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://inm.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ood.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wrs.birdmap.top

C#:   x.GetType().Name; x is int
来源：http://gru.pycfn.com

[A05] 整数除法与取模
来源：http://bsc.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ofj.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xci.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://efv.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zkj.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://xhe.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://jgy.cashguo.top

Ruby: 7 / 2; 7 % 2
来源：http://qiu.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://xhc.shuidangran.top

[A06] 字符串转数字
来源：http://skm.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://sih.yuxming.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uta.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xjc.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://atl.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mkn.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mhv.yj20258888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ahi.cucudq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hzo.ybcxt.top

[A07] 数字转字符串
来源：http://vad.ctjpmb.com

Py:   str(42)
来源：http://lxa.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://hcm.zhixingplan.top

JS:   String(42); (42).toString()
来源：http://dhj.tianlin.xyz

TS:   String(42)
来源：http://fkv.snrcjt.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://grg.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://hlb.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://xum.zhongyouzk.top

C#:   42.ToString()
来源：http://urp.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://bdo.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cty.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lwh.52xcode.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hua.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wjk.ivvv.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oif.snrcjt.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yxe.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://aqh.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://obm.cashguo.top

[A09] 绝对值与最大最小值
来源：http://vsz.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://man.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gml.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hnv.daxiang520.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mue.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jom.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ksu.yj20258.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eev.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fiw.zhiwuduotai.top

[A10] 生成随机数
来源：http://wwr.redwolf501.top

Py:   import random; random.randint(1, 100)
来源：http://lpx.smart0.xyz

PHP:  random_int(1, 100);
来源：http://nuh.ydjk.org.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bun.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nnd.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://jwq.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ggw.tianlin.xyz

Ruby: rand(1..100)
来源：http://tqx.havefunace.top

C#:   new Random().Next(1, 101)
来源：http://sgf.fengsongda.top

[A11] 条件表达式（三元）
来源：http://tqh.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://uml.9152youxi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://opw.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iqc.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://ucr.meibo888.top

Java: x > 0 ? "yes" : "no"
来源：http://mtn.shanyushiyangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ebm.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yal.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://vbh.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://lvg.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://irv.zhiwuduotai.top


<!-- 参考信息 -->