代发 wailian999

[U79] PHP：静态分析
来源：http://hoa.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://jzk.yonumen.top

[U80] PHP：代码规范修复
来源：http://ghi.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tgn.daria6918.cn

[U81] JS：初始化项目
来源：http://qrg.jyoumei.cn

npm init -y;  npm i express
来源：http://xzn.52xcode.cn

[U82] JS：package.json 脚本
来源：http://azy.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wjx.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://orz.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://sad.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://xwx.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xhr.havefunace.top

[U85] JS：可选链
来源：http://ice.chenzaomai.com

a?.b?.c
来源：http://wqu.xuetiantiany.cn

[U86] JS：空值合并
来源：http://oni.chenlongwang.top

a ?? b
来源：http://zpi.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://jqc.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://nkm.tian-w.cn

[U88] JS：对象展开合并
来源：http://tje.fktsv.cn

{ ...a, ...b }
来源：http://rjb.chenzaomai.com

[U89] JS：数组去重
来源：http://bhe.hnxiangtu.top

[...new Set(arr)]
来源：http://wnj.shuidangran.top

[U90] JS：数字数组排序
来源：http://vfc.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://fgh.jianghu66.top

[U91] JS：对象键值遍历
来源：http://dvn.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jqz.yj202588.top

[U92] JS：深拷贝
来源：http://uyn.shuidangran.top

structuredClone(obj)
来源：http://zgj.mhx1999.top

[U93] JS：模板字符串
来源：http://wbe.hcnkem.com

`共 ${n} 条`
来源：http://ekn.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://jft.fehbvm.com

const double = x => x * 2;
来源：http://qoc.aibaodan.cn

[U95] JS：Promise 包装
来源：http://qbc.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://mzq.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://vfc.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vww.smart0.xyz

[U97] JS：并发请求
来源：http://ypi.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qlz.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://enr.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zct.jyoumei.cn

[U99] JS：事件监听
来源：http://kui.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://ccm.uphjek.com

[U100] JS：DOM 查询
来源：http://fhf.hesvh.cn

document.querySelector(".item")
来源：http://tqb.sysykeji.top

[U101] JS：classList 操作
来源：http://fqo.fzhhl.top

el.classList.toggle("active")
来源：http://bms.hnxiangtu.top

[U102] JS：本地存储
来源：http://hpx.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kzx.jqgfzy.top

[U103] JS：定时器
来源：http://ovo.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qlc.gaohongyu789.top

[U104] JS：防抖
来源：http://cnj.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhq.52xcode.cn

[U105] JS：节流
来源：http://kfl.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yiq.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://fjp.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uin.sjlbkw.cn

[U107] JS：数字千分位
来源：http://wye.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fzd.fktsv.cn

[U108] JS：随机整数
来源：http://zvo.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ira.svipenyu.cn

[U109] JS：数组分组
来源：http://gkg.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://glo.yuanzhike.top

[U110] JS：数组分块
来源：http://wle.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ldd.cqqwz.cn

[U111] JS：对象转 Map
来源：http://bhn.wangdashe.top

new Map(Object.entries(obj))
来源：http://kvk.c1oappe.top

[U112] JS：字符串补位
来源：http://jfp.bbcook.cn

"7".padStart(3, "0")
来源：http://zbj.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://bib.ctjpmb.com

s.replaceAll("a", "b")
来源：http://jme.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://cqx.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://jyv.sxryk.cn

[U115] JS：生成 UUID
来源：http://enc.fengsongda.top

crypto.randomUUID()
来源：http://ifq.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://eol.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://ink.ehwqpu.com

[U117] JS：单元测试
来源：http://msk.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://bwt.jyoumei.cn

[U118] JS：开发服务器
来源：http://kyu.fehbvm.com

npm i -D vite;  npx vite
来源：http://wju.gzhubu.top

[U119] JS：生产构建
来源：http://ubm.meibo888.top

npx vite build
来源：http://ita.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://rvr.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://nqi.daxiang520.top

================================================================================
来源：http://fip.bjfxy.top

统计汇总
来源：http://yuy.cdnleiting.top

================================================================================
来源：http://nor.tianlin.xyz

按语言统计（条）：
来源：http://chy.jqgfzy.top

Python ......... 252
来源：http://tdj.dashuyun.cn

PHP ............ 252
来源：http://sei.yj20258.top

JavaScript ..... 252
来源：http://zic.yj20258.top

TypeScript ..... 212
来源：http://kag.meibo888.top

Java ........... 212
来源：http://inx.uphjek.com

Go ............. 212
来源：http://odl.sweek.top

Ruby ........... 212
来源：http://xbb.hongshengwenyu.top

C# ............. 212
来源：http://kxi.guannengcc.top

C .............. 30
来源：http://fnc.ppjwa.cn

C++ ............ 30
来源：http://yln.chenzaomai.com

SQL ............ 90
来源：http://opl.52xcode.cn

Bash ........... 80
来源：http://oul.zhengqikj.top

Kotlin ......... 15
来源：http://kgh.vqdsnc.cn

Swift .......... 15
来源：http://vap.zhaomingkeji.xyz

Lua ............ 10
来源：http://qfn.shangyingyoupin.top

Perl ........... 10
来源：http://hjg.zdqjudy.top

Scala .......... 10
来源：http://iah.xinyue.icu

------------------------------------
来源：http://bbl.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://wzm.ehwqpu.com

按章节统计：
来源：http://pyi.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rdg.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wry.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mue.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yhm.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cmb.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yhl.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://txq.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vij.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://egy.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vpe.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qzb.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bfn.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://syo.haohaochexian.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jem.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wit.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dmd.gzhubu.top

Q SQL 专题                              90
来源：http://prm.nwbrower.top

R Bash 专题                             80
来源：http://gte.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://hjo.ctjpmb.com

T 其他语言补充                          60
来源：http://djn.yonumen.top

U 高频实用片段                         120
来源：http://vuf.hywenlv.cn

------------------------------------
来源：http://maa.pengpengdd.cyou

合计                                  2106 条
来源：http://ypg.shuidangran.top

--------------------------------------------------------------------------------
来源：http://tmr.xingfuxueyuan.xyz

使用提醒
来源：http://xrj.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://tgs.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oqe.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mxn.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iiy.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uzf.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lor.tarul.cn

—— 文件结束 ——
来源：http://jal.meibo888.top

================================================================================
来源：http://nom.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://joq.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://ene.cdnleiting.top

================================================================================
来源：http://lln.meibo888.top

【收录内容】
来源：http://cha.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kde.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yun.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://pzx.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tnn.fanxiaobao.xyz

【使用说明】
来源：http://gxj.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ipl.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ukp.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gds.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tyt.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ujh.cheryme.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gug.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fzv.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qoh.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nms.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gfc.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vim.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jvi.wangshuangyany.cn

【文件统计】
来源：http://vov.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jjw.hcnkem.com

--------------------------------------------------------------------------------
来源：http://txt.yangfankeji.com

目  录
来源：http://xxv.guannengcc.top

--------------------------------------------------------------------------------
来源：http://ofm.pycfn.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://urc.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qdo.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ufr.shzxlz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ruu.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://llx.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://knz.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ira.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://slk.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xac.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iqi.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jov.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gug.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aod.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nht.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ijb.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dre.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://avo.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gak.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fal.yongpay.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndh.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://aal.tarul.cn

================================================================================
来源：http://haq.9152youxi.cn

A. 基础语法与类型
来源：http://wyg.daria6918.cn

================================================================================
来源：http://jpz.shuidangran.top

[A01] Hello World
来源：http://dsi.smart0.xyz

Py:   print("Hello, World!")
来源：http://rcw.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://fpx.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://ogc.xinyue.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wbm.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://mik.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://igh.fehbvm.com

Ruby: puts "Hello, World!"
来源：http://rxz.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ejl.zhoulong.xyz

[A02] 变量声明与赋值
来源：http://zcm.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eba.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zxw.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://wjy.uphjek.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ksx.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://iny.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://xmj.sufxvd.cn

Ruby: name = "Alex"; age = 20
来源：http://wts.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://vgc.ydzc1.top

[A03] 常量定义
来源：http://urj.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hrg.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://ldd.yj20258888.top

JS:   const PI = 3.14159;
来源：http://dip.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://hnb.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://xio.sweek.top

Go:   const PI = 3.14159
来源：http://gvv.dashuyun.cn

Ruby: PI = 3.14159
来源：http://ydz.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://pvn.birdmap.top

[A04] 判断变量类型
来源：http://bcd.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://mgc.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dpz.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lhy.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://kwa.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uff.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://clb.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://num.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://ghv.ydzc1.top

[A05] 整数除法与取模
来源：http://xdu.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fjz.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qnk.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dmg.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wzq.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://ehx.birdmap.top

Go:   7 / 2; 7 % 2
来源：http://wvj.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://vtk.hywenlv.cn

C#:   7 / 2; 7 % 2
来源：http://xqg.vehdjk.com

[A06] 字符串转数字
来源：http://rfe.tianlin.xyz

Py:   int("42"); float("3.14")
来源：http://jhw.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vbw.ydzc1.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hbe.ctjpmb.com

TS:   parseInt("42", 10); Number("42")
来源：http://ahd.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rwa.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hue.shanyushiyangtech.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yac.jiagoushi.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xgq.aibaodan.cn

[A07] 数字转字符串
来源：http://fhg.zdbjq.cn

Py:   str(42)
来源：http://rxb.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://dxj.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://jqv.jianghu66.top

TS:   String(42)
来源：http://ujv.iojbl.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://osc.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://imt.smart0.xyz

Ruby: 42.to_s
来源：http://ezs.pengpengdd.cyou

C#:   42.ToString()
来源：http://gzv.haohaochexian.top

[A08] 取整与四舍五入
来源：http://vmb.xinyue.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fbr.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://irz.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vwo.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ffv.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qis.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gez.zhijiandao.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gos.bjfxy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mow.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://dae.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kgg.wangshuangyany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zyj.jyoumei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://clz.hfpthk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cst.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fec.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://etm.wangshuangyany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zfb.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ras.yj20258888.top

[A10] 生成随机数
来源：http://eje.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://ecg.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://fgr.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://khx.nanxuanxn.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://koi.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://yva.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jcz.yj202588.top

Ruby: rand(1..100)
来源：http://xvi.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://uua.yj202588.top

[A11] 条件表达式（三元）
来源：http://sjg.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://mgi.shzxlz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fbv.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xag.zhengqikj.top

TS:   x > 0 ? "yes" : "no"
来源：http://swa.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://weh.chenjidiqi.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://rqa.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ngc.havefunace.top

C#:   x > 0 ? "yes" : "no"
来源：http://efa.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://xvk.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hwl.cucudq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qte.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://ypm.birdmap.top

TS:   `Hello, ${name}!`
来源：http://pco.zhoulong.xyz

Java: "Hello, %s!".formatted(name)
来源：http://fhx.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eax.jyoumei.cn

Ruby: "Hello, #{name}!"
来源：http://zdf.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://epx.sysykeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vkw.meibo888.top


<!-- 参考信息 -->