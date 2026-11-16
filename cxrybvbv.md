代发 wailian999

[U75] PHP：依赖注入
来源：http://xwf.bjfxy.top

composer require psr/container
来源：http://lsf.gogol.net.cn

[U76] PHP：简单路由
来源：http://mio.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fpz.tian-w.cn

[U77] PHP：模板渲染
来源：http://ywf.ctjpmb.com

composer require twig/twig
来源：http://voh.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://mrs.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://rwb.tian-w.cn

[U79] PHP：静态分析
来源：http://vfo.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://eym.sxryk.cn

[U80] PHP：代码规范修复
来源：http://wmw.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jox.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://amn.ybcxt.top

npm init -y;  npm i express
来源：http://frv.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://zxs.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pcl.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://hrr.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qbh.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://ubz.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://khd.guannengcc.top

[U85] JS：可选链
来源：http://vzl.jinyuanbaomall.cn

a?.b?.c
来源：http://jre.yuxming.cn

[U86] JS：空值合并
来源：http://xjm.zhaomingkeji.xyz

a ?? b
来源：http://tsg.yfazqb.com

[U87] JS：解构默认值
来源：http://don.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://nye.andypj.xyz

[U88] JS：对象展开合并
来源：http://lrb.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://wlj.uphjek.com

[U89] JS：数组去重
来源：http://tmx.shuidangran.top

[...new Set(arr)]
来源：http://blg.yvedp.cn

[U90] JS：数字数组排序
来源：http://erx.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://dgh.yuxming.cn

[U91] JS：对象键值遍历
来源：http://pcx.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://omx.fzhhl.top

[U92] JS：深拷贝
来源：http://dpv.xylfe.cn

structuredClone(obj)
来源：http://tbi.yuanzhike.top

[U93] JS：模板字符串
来源：http://rnk.nanxinkj.top

`共 ${n} 条`
来源：http://ycu.fktsv.cn

[U94] JS：箭头函数
来源：http://aqj.daxiang520.top

const double = x => x * 2;
来源：http://sls.birdmap.top

[U95] JS：Promise 包装
来源：http://joe.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://edp.hammf.cn

[U96] JS：async/await 与异常
来源：http://olp.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xjq.nanxinkj.top

[U97] JS：并发请求
来源：http://klr.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://aom.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://zhy.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iic.52xcode.cn

[U99] JS：事件监听
来源：http://fge.xziqi.cn

el.addEventListener("click", e => {})
来源：http://vah.yonumen.top

[U100] JS：DOM 查询
来源：http://xhg.hnxiangtu.top

document.querySelector(".item")
来源：http://zel.meibo888.top

[U101] JS：classList 操作
来源：http://gvf.tian-w.cn

el.classList.toggle("active")
来源：http://lbz.ppjwa.cn

[U102] JS：本地存储
来源：http://lpk.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://klo.zhiwuduotai.top

[U103] JS：定时器
来源：http://lcc.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jxb.yuanzhike.top

[U104] JS：防抖
来源：http://ipc.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijm.wangdashe.top

[U105] JS：节流
来源：http://spq.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kpv.yongpay.top

[U106] JS：日期格式化
来源：http://bkl.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://imm.mhx1999.top

[U107] JS：数字千分位
来源：http://wjy.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wvd.sweek.top

[U108] JS：随机整数
来源：http://pex.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cnf.hywenlv.cn

[U109] JS：数组分组
来源：http://xrq.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://muc.yangfankeji.com

[U110] JS：数组分块
来源：http://omw.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qnm.daria6918.cn

[U111] JS：对象转 Map
来源：http://ipm.xuanzx.com

new Map(Object.entries(obj))
来源：http://fkd.kuanghao11.cn

[U112] JS：字符串补位
来源：http://xvo.jiagoushi.top

"7".padStart(3, "0")
来源：http://hsk.yvedp.cn

[U113] JS：正则替换全部
来源：http://xvg.chenzaomai.com

s.replaceAll("a", "b")
来源：http://abb.pycfn.com

[U114] JS：JSON 深比较
来源：http://eut.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wmw.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://ysz.bjfxy.top

crypto.randomUUID()
来源：http://vxj.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://wos.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://jyb.hywenlv.cn

[U117] JS：单元测试
来源：http://lll.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://rrc.tanke756.top

[U118] JS：开发服务器
来源：http://kvl.wangdashe.top

npm i -D vite;  npx vite
来源：http://fog.aibaodan.cn

[U119] JS：生产构建
来源：http://kno.smart0.xyz

npx vite build
来源：http://vrh.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://xcm.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://vaz.aizwys.cn

================================================================================
来源：http://pth.0kj1m.cn

统计汇总
来源：http://krx.zhongyouzk.top

================================================================================
来源：http://ipj.mhx1999.top

按语言统计（条）：
来源：http://viv.ydzc1.top

Python ......... 252
来源：http://pun.yangfankeji.com

PHP ............ 252
来源：http://zbg.guowangkeji.top

JavaScript ..... 252
来源：http://tlx.zhoulong.xyz

TypeScript ..... 212
来源：http://lyc.yuxming.cn

Java ........... 212
来源：http://hup.mhx1999.top

Go ............. 212
来源：http://kjo.fanxiaobao.xyz

Ruby ........... 212
来源：http://btp.epnwcf.com

C# ............. 212
来源：http://qdw.gzhubu.top

C .............. 30
来源：http://zce.zhiwuduotai.top

C++ ............ 30
来源：http://ruv.xinyue.icu

SQL ............ 90
来源：http://uax.fengsongda.top

Bash ........... 80
来源：http://zwz.gaohongyu789.top

Kotlin ......... 15
来源：http://qus.cucudq.cn

Swift .......... 15
来源：http://egx.meibo888.top

Lua ............ 10
来源：http://ipa.zhongyouzk.top

Perl ........... 10
来源：http://stc.tianlin.xyz

Scala .......... 10
来源：http://tdf.shuidangran.top

------------------------------------
来源：http://gwu.wangshuangyany.cn

合计 ........... 2106 条
来源：http://mwo.bbcook.cn

按章节统计：
来源：http://ugo.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fky.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://agb.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tja.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ykb.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wkx.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ecg.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cqu.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pbm.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lsk.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tmr.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ymy.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cor.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ucs.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tmv.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lls.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ewn.daxiang520.top

Q SQL 专题                              90
来源：http://fba.ppjwa.cn

R Bash 专题                             80
来源：http://igz.fehbvm.com

S C / C++ 专题                          60
来源：http://ege.fzhhl.top

T 其他语言补充                          60
来源：http://vwb.xuetiantiany.cn

U 高频实用片段                         120
来源：http://ltq.jinqigfzy.top

------------------------------------
来源：http://tpc.vqdsnc.cn

合计                                  2106 条
来源：http://tnk.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://kei.chenlongwang.top

使用提醒
来源：http://wsh.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://fkz.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://prs.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yod.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hun.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rgg.yj20258888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dhn.epnwcf.com

—— 文件结束 ——
来源：http://nkl.bjfxy.top

================================================================================
来源：http://bib.yvedp.cn

程序语言常见例子速查手册（2024 版）
来源：http://old.316326.xyz

Common Programming Examples Cheat Book
来源：http://jhw.fehbvm.com

================================================================================
来源：http://gnq.guowangkeji.top

【收录内容】
来源：http://rgp.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jrx.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dgq.chenzaomai.com

SQL · Bash · C · C++
来源：http://rur.svipenyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://voi.chenjidiqi.icu

【使用说明】
来源：http://odd.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tak.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ydt.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wio.snrcjt.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oac.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jyh.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cdk.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rtx.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tzi.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pll.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vqa.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uoo.wangshuangyany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sbl.hnxiangtu.top

【文件统计】
来源：http://buu.sufxvd.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://awl.cucudq.cn

--------------------------------------------------------------------------------
来源：http://pcv.shangyingyoupin.top

目  录
来源：http://azw.yj202588.top

--------------------------------------------------------------------------------
来源：http://rbd.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vsj.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://upw.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gkn.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xmo.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ogv.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kjs.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jac.hesvh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ond.uphjek.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mwc.zhiwuduotai.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jpn.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pyi.wangshuangyany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://obs.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sou.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iyp.jqgfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tex.vehdjk.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://usk.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nkm.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zsu.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hwg.yj20258.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gax.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://asd.hywenlv.cn

================================================================================
来源：http://jtl.yangfankeji.com

A. 基础语法与类型
来源：http://kks.yuanzhike.top

================================================================================
来源：http://aww.shuidangran.top

[A01] Hello World
来源：http://qoh.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://vob.aibaodan.cn

PHP:  echo "Hello, World!";
来源：http://jnx.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://jzd.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://opg.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://tzw.aibaodan.cn

Go:   fmt.Println("Hello, World!")
来源：http://rtm.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://jzf.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jrk.yongpay.top

[A02] 变量声明与赋值
来源：http://wdk.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kmg.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yrx.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://jho.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jjx.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://sfr.bjfxy.top

Go:   name := "Alex"; age := 20
来源：http://etg.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://dxt.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://xfh.mhx1999.top

[A03] 常量定义
来源：http://flk.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jjp.zycfv.cn

PHP:  const PI = 3.14159;
来源：http://tkq.ydzc1.top

JS:   const PI = 3.14159;
来源：http://txx.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://usu.jinyuanbaomall.cn

Java: static final double PI = 3.14159;
来源：http://xuy.c1oappe.top

Go:   const PI = 3.14159
来源：http://whr.fengsongda.top

Ruby: PI = 3.14159
来源：http://zop.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://ppt.shzxlz.cn

[A04] 判断变量类型
来源：http://pxz.bjfxy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://eey.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rvy.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uoa.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://hgl.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jve.hesvh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ido.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vmh.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://vmq.xuetiantiany.cn

[A05] 整数除法与取模
来源：http://omx.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wld.xingfuxueyuan.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://owr.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://chg.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xyf.pycfn.com

Java: 7 / 2; 7 % 2
来源：http://qha.sweek.top

Go:   7 / 2; 7 % 2
来源：http://duv.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://eql.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://fgy.jinqigufen.top

[A06] 字符串转数字
来源：http://abr.hfpthk.cn

Py:   int("42"); float("3.14")
来源：http://wsk.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://apl.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hxc.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yit.aizwys.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zxu.9152youxi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zcj.zhoulong.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://zin.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ehr.bbcook.cn

[A07] 数字转字符串
来源：http://vqq.sweek.top

Py:   str(42)
来源：http://dyb.hywenlv.cn

PHP:  (string) 42; strval(42)
来源：http://yds.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://qjx.cdnleiting.top

TS:   String(42)
来源：http://pix.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://smt.nanxinkj.top

Go:   strconv.Itoa(42)
来源：http://vfh.jqgufenzy.top

Ruby: 42.to_s
来源：http://wyo.shuidangran.top

C#:   42.ToString()
来源：http://kqt.ybcxt.top

[A08] 取整与四舍五入
来源：http://fxr.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jot.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vcb.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rqe.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gnc.pengpengdd.cyou

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pdb.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vna.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jhy.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xbz.hnxiangtu.top

[A09] 绝对值与最大最小值
来源：http://bdt.birdmap.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dsq.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vtg.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xmh.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nua.aibaodan.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pnf.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sfg.guannengcc.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ryu.zhongyouzk.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bqw.sysykeji.top

[A10] 生成随机数
来源：http://gxy.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://nrj.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://pss.guowangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wfe.zycfv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jrv.andypj.xyz

Java: new Random().nextInt(100) + 1
来源：http://gml.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zcy.nanxinkj.top

Ruby: rand(1..100)
来源：http://bsm.vqdsnc.cn

C#:   new Random().Next(1, 101)
来源：http://wdf.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://gvp.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://fax.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rsd.zhengqikj.top

JS:   x > 0 ? "yes" : "no"
来源：http://fnb.fzhhl.top

TS:   x > 0 ? "yes" : "no"
来源：http://zqi.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://vfw.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eta.yangfankeji.com

Ruby: x > 0 ? "yes" : "no"
来源：http://xaa.aibaodan.cn

C#:   x > 0 ? "yes" : "no"
来源：http://afh.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://spk.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ajo.xingfuxueyuan.xyz


<!-- 参考信息 -->