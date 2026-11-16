代发 wailian999

[U79] PHP：静态分析
来源：http://rya.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://yki.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://flm.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://tzr.52xcode.cn

[U81] JS：初始化项目
来源：http://tpx.jiagoushi.top

npm init -y;  npm i express
来源：http://rqd.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://nfn.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gee.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://zkk.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rlv.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://hfq.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bki.hysaishi.cn

[U85] JS：可选链
来源：http://glw.ehwqpu.com

a?.b?.c
来源：http://jrf.haohaochexian.top

[U86] JS：空值合并
来源：http://vzr.xingfuxueyuan.xyz

a ?? b
来源：http://ktf.snrcjt.cn

[U87] JS：解构默认值
来源：http://tpt.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://pmj.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://bcg.andypj.xyz

{ ...a, ...b }
来源：http://xdq.sweek.top

[U89] JS：数组去重
来源：http://bao.kuanghao11.cn

[...new Set(arr)]
来源：http://kxj.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://qil.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://dql.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://mrc.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://moo.mhx1999.top

[U92] JS：深拷贝
来源：http://cdo.sufxvd.cn

structuredClone(obj)
来源：http://nvf.guowangkeji.top

[U93] JS：模板字符串
来源：http://xcr.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://sxz.vqdsnc.cn

[U94] JS：箭头函数
来源：http://ybw.c1oappe.top

const double = x => x * 2;
来源：http://lkl.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://pey.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://sgg.epnwcf.com

[U96] JS：async/await 与异常
来源：http://lfw.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fft.shuidangran.top

[U97] JS：并发请求
来源：http://ryr.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://quc.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://ksr.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lva.316326.xyz

[U99] JS：事件监听
来源：http://ksc.ydzc1.top

el.addEventListener("click", e => {})
来源：http://dzv.svipenyu.cn

[U100] JS：DOM 查询
来源：http://uxi.tanke756.top

document.querySelector(".item")
来源：http://fxg.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://vcg.xylfe.cn

el.classList.toggle("active")
来源：http://eix.yangfankeji.com

[U102] JS：本地存储
来源：http://tjg.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ccx.yueranfly.top

[U103] JS：定时器
来源：http://cne.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cdb.tanke756.top

[U104] JS：防抖
来源：http://eia.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwv.jinqigufen.top

[U105] JS：节流
来源：http://tix.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jsv.dashuyun.cn

[U106] JS：日期格式化
来源：http://urt.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gad.vqdsnc.cn

[U107] JS：数字千分位
来源：http://jhd.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ido.feifeiyinyue.top

[U108] JS：随机整数
来源：http://dtj.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zfp.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://fkr.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://doz.hfpthk.cn

[U110] JS：数组分块
来源：http://arp.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fwr.yj20258888.top

[U111] JS：对象转 Map
来源：http://ibp.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://ung.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://dwl.hnxiangtu.top

"7".padStart(3, "0")
来源：http://zgp.ppjwa.cn

[U113] JS：正则替换全部
来源：http://ypx.yj20258.top

s.replaceAll("a", "b")
来源：http://vsk.smart0.xyz

[U114] JS：JSON 深比较
来源：http://fjr.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ufs.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://tcx.shuidangran.top

crypto.randomUUID()
来源：http://gvy.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://kgo.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://owt.uphjek.com

[U117] JS：单元测试
来源：http://sij.hnqzz.top

npm i -D vitest;  npx vitest
来源：http://erg.chenlongwang.top

[U118] JS：开发服务器
来源：http://nfj.yj202588.top

npm i -D vite;  npx vite
来源：http://ewt.bjfxy.top

[U119] JS：生产构建
来源：http://owt.jinqigfzy.top

npx vite build
来源：http://xqk.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://xvb.meibo888.top

import.meta.env.VITE_API_URL
来源：http://qyw.zdbjq.cn

================================================================================
来源：http://xbz.0kj1m.cn

统计汇总
来源：http://wrj.9152youxi.cn

================================================================================
来源：http://wnh.ctjpmb.com

按语言统计（条）：
来源：http://daj.shuidangran.top

Python ......... 252
来源：http://irj.jiagoushi.top

PHP ............ 252
来源：http://omk.nanxinkj.top

JavaScript ..... 252
来源：http://yao.aibaodan.cn

TypeScript ..... 212
来源：http://zpb.zhengqikj.top

Java ........... 212
来源：http://zsr.jqgufenzy.top

Go ............. 212
来源：http://wej.zhixingplan.top

Ruby ........... 212
来源：http://dge.tarul.cn

C# ............. 212
来源：http://uah.cdnleiting.top

C .............. 30
来源：http://mrh.jinqigfzy.top

C++ ............ 30
来源：http://xkw.hfpthk.cn

SQL ............ 90
来源：http://rrl.bjfxy.top

Bash ........... 80
来源：http://oyv.zhongyouzk.top

Kotlin ......... 15
来源：http://pgm.haohaochexian.top

Swift .......... 15
来源：http://waz.yj202588.top

Lua ............ 10
来源：http://dne.zycfv.cn

Perl ........... 10
来源：http://vve.ctjpmb.com

Scala .......... 10
来源：http://ege.jqgfzy.top

------------------------------------
来源：http://cbi.dashuyun.cn

合计 ........... 2106 条
来源：http://sjz.zhongyouzk.top

按章节统计：
来源：http://zyk.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://njv.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ixc.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bvk.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uxt.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fxd.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://drp.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jnf.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hza.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rcy.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fiz.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tag.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dmv.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vji.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jpw.sjlbkw.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tig.xylfe.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vcs.zdbjq.cn

Q SQL 专题                              90
来源：http://fkw.xinyue.icu

R Bash 专题                             80
来源：http://rpt.hesvh.cn

S C / C++ 专题                          60
来源：http://gvn.hesvh.cn

T 其他语言补充                          60
来源：http://ine.tianlin.xyz

U 高频实用片段                         120
来源：http://kha.hnqzz.top

------------------------------------
来源：http://kgv.tian-w.cn

合计                                  2106 条
来源：http://zpc.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://iiq.jiagoushi.top

使用提醒
来源：http://cex.tian-w.cn

--------------------------------------------------------------------------------
来源：http://ojh.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vil.jiagoushi.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bmo.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://prg.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wyv.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jkw.jinqigufen.top

—— 文件结束 ——
来源：http://xfh.316326.xyz

================================================================================
来源：http://zbk.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://olr.daria6918.cn

Common Programming Examples Cheat Book
来源：http://dkr.hfpthk.cn

================================================================================
来源：http://lii.fehbvm.com

【收录内容】
来源：http://ttg.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ghr.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://swj.tanke756.top

SQL · Bash · C · C++
来源：http://jcf.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kei.hysaishi.cn

【使用说明】
来源：http://vwf.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://etv.gogol.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xna.bjfxy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ohr.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://glr.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lba.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ryv.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nii.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eyb.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nir.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pug.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jzz.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pie.redwolf501.top

【文件统计】
来源：http://idd.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nny.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://akx.ywan-chungtsiang.top

目  录
来源：http://omp.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://zlf.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://loa.smart0.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ude.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://neq.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bse.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://roy.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eiv.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vnf.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vrc.zhengqikj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://psq.shanyushiyangtech.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zfx.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://toq.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xrn.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mdb.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bwq.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vdk.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jlk.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gcd.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://dsq.zhoulong.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xwm.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mhs.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://itr.feifeiyinyue.top

================================================================================
来源：http://mry.haohaochexian.top

A. 基础语法与类型
来源：http://cbh.zhiwuduotai.top

================================================================================
来源：http://gyo.hywenlv.cn

[A01] Hello World
来源：http://ysk.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://aru.tian-w.cn

PHP:  echo "Hello, World!";
来源：http://wqt.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://qtn.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dds.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://hew.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://tkv.pengpengdd.cyou

Ruby: puts "Hello, World!"
来源：http://rao.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://suz.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://csv.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ydy.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://inh.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://rdp.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gel.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://jka.zhaomingkeji.xyz

Go:   name := "Alex"; age := 20
来源：http://pba.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://ugi.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://ncg.zdqjudy.top

[A03] 常量定义
来源：http://azv.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aru.316326.xyz

PHP:  const PI = 3.14159;
来源：http://vxr.gzhubu.top

JS:   const PI = 3.14159;
来源：http://jff.0kj1m.cn

TS:   const PI: number = 3.14159;
来源：http://ywo.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://qeu.tanke756.top

Go:   const PI = 3.14159
来源：http://mhx.fengsongda.top

Ruby: PI = 3.14159
来源：http://mly.sweek.top

C#:   const double PI = 3.14159;
来源：http://fne.iojbl.cn

[A04] 判断变量类型
来源：http://ydr.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tux.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://buw.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ewu.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://wfc.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bje.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://bgj.uphjek.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ihi.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://arv.yuanzhike.top

[A05] 整数除法与取模
来源：http://qhj.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lmv.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vcj.chenlongwang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vvc.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://exy.9152youxi.cn

Java: 7 / 2; 7 % 2
来源：http://bcg.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://kuc.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://vik.hywenlv.cn

C#:   7 / 2; 7 % 2
来源：http://odp.fktsv.cn

[A06] 字符串转数字
来源：http://uuf.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://fgm.bbcook.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xaw.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bik.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gkr.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bvk.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wtu.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vvr.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uxw.pengpengdd.cyou

[A07] 数字转字符串
来源：http://odv.jianghu66.top

Py:   str(42)
来源：http://arv.vehdjk.com

PHP:  (string) 42; strval(42)
来源：http://ovj.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://zrn.svipenyu.cn

TS:   String(42)
来源：http://zpw.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rsw.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://boa.chenjidiqi.icu

Ruby: 42.to_s
来源：http://gco.shuidangran.top

C#:   42.ToString()
来源：http://mgm.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://ill.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uzm.zhoulong.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ouw.hysaishi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jvg.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ubj.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xxq.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://syq.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tqi.chenjidiqi.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xsy.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://bsw.nanxinkj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://coe.cqqwz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ffo.sufxvd.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iyf.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gib.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ars.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pdy.sysykeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bxd.ywan-chungtsiang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hwb.cdnleiting.top

[A10] 生成随机数
来源：http://jrs.gotoacloud.top

Py:   import random; random.randint(1, 100)
来源：http://ooa.cashguo.top

PHP:  random_int(1, 100);
来源：http://zho.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dbh.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qnl.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://rvd.guowangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fov.aizwys.cn

Ruby: rand(1..100)
来源：http://vvf.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://uuo.mhx1999.top

[A11] 条件表达式（三元）
来源：http://wzd.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://bjv.zhoulong.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://qat.zhengqikj.top

JS:   x > 0 ? "yes" : "no"
来源：http://aiy.chenjidiqi.icu

TS:   x > 0 ? "yes" : "no"
来源：http://zdc.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://tdk.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ddd.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hsh.hfpthk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ijj.ybcxt.top

[A12] 字符串插值 / 格式化
来源：http://fju.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kcg.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pcj.fktsv.cn

JS:   `Hello, ${name}!`
来源：http://ieq.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://tcs.mhx1999.top

Java: "Hello, %s!".formatted(name)
来源：http://avn.ctjpmb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rms.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://vdz.zhaomingkeji.xyz

C#:   $"Hello, {name}!"
来源：http://tfm.gaohongyu789.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ywk.havefunace.top


<!-- 参考信息 -->