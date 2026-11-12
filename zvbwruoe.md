代发 wailian999

[U77] PHP：模板渲染
来源：http://zkq.zhengqikj.top

composer require twig/twig
来源：http://oav.hfpthk.cn

[U78] PHP：单元测试
来源：http://yrq.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://hch.yj202588.top

[U79] PHP：静态分析
来源：http://rks.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://zag.cucudq.cn

[U80] PHP：代码规范修复
来源：http://ugg.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hfn.jiagoushi.top

[U81] JS：初始化项目
来源：http://zsq.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://xnm.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://veo.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://try.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://rjw.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://awu.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://gvg.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://jqo.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://lkb.ydjk.org.cn

a?.b?.c
来源：http://ipl.yvedp.cn

[U86] JS：空值合并
来源：http://ehk.shangyingyoupin.top

a ?? b
来源：http://kuz.ppjwa.cn

[U87] JS：解构默认值
来源：http://lgr.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://pik.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://pwu.xziqi.cn

{ ...a, ...b }
来源：http://vrd.gotoacloud.top

[U89] JS：数组去重
来源：http://hjm.sysykeji.top

[...new Set(arr)]
来源：http://val.9152youxi.cn

[U90] JS：数字数组排序
来源：http://usl.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://ach.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://szw.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jij.tian-w.cn

[U92] JS：深拷贝
来源：http://osz.pycfn.com

structuredClone(obj)
来源：http://ixx.xziqi.cn

[U93] JS：模板字符串
来源：http://ker.yongpay.top

`共 ${n} 条`
来源：http://shq.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://nna.bjfxy.top

const double = x => x * 2;
来源：http://olv.daria6918.cn

[U95] JS：Promise 包装
来源：http://nkp.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://dyu.iojbl.cn

[U96] JS：async/await 与异常
来源：http://djf.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tcw.yanxiufei.cn

[U97] JS：并发请求
来源：http://alu.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ueq.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://aql.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cle.hysaishi.cn

[U99] JS：事件监听
来源：http://lji.zhoulong.xyz

el.addEventListener("click", e => {})
来源：http://jnu.gotoacloud.top

[U100] JS：DOM 查询
来源：http://ohv.chenjidiqi.icu

document.querySelector(".item")
来源：http://qmx.hnqzz.top

[U101] JS：classList 操作
来源：http://kkj.xziqi.cn

el.classList.toggle("active")
来源：http://ddr.ydjk.org.cn

[U102] JS：本地存储
来源：http://tgn.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://xzb.nwbrower.top

[U103] JS：定时器
来源：http://axt.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dgu.jqgfzy.top

[U104] JS：防抖
来源：http://qka.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nhw.andypj.xyz

[U105] JS：节流
来源：http://dfw.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dxq.quarkkingdee.top

[U106] JS：日期格式化
来源：http://yfr.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://flw.jiagoushi.top

[U107] JS：数字千分位
来源：http://wdd.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lyb.cdnleiting.top

[U108] JS：随机整数
来源：http://cxa.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://osr.hammf.cn

[U109] JS：数组分组
来源：http://asx.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://ebb.ydzc1.top

[U110] JS：数组分块
来源：http://huo.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dxw.pycfn.com

[U111] JS：对象转 Map
来源：http://nff.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://fkz.jqgufenzy.top

[U112] JS：字符串补位
来源：http://xzk.zhengqikj.top

"7".padStart(3, "0")
来源：http://ntg.gogol.net.cn

[U113] JS：正则替换全部
来源：http://asx.redwolf501.top

s.replaceAll("a", "b")
来源：http://ygx.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://enu.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://bev.jianghu66.top

[U115] JS：生成 UUID
来源：http://eur.hysaishi.cn

crypto.randomUUID()
来源：http://kxm.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://arm.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://qem.andypj.xyz

[U117] JS：单元测试
来源：http://tqu.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://fbm.birdmap.top

[U118] JS：开发服务器
来源：http://grc.vehdjk.com

npm i -D vite;  npx vite
来源：http://tde.hcnkem.com

[U119] JS：生产构建
来源：http://jnq.iojbl.cn

npx vite build
来源：http://dki.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://aul.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://tdz.zhengqikj.top

================================================================================
来源：http://cus.wangshuangyany.cn

统计汇总
来源：http://uqw.quarkkingdee.top

================================================================================
来源：http://ywh.daria6918.cn

按语言统计（条）：
来源：http://ndd.cqqwz.cn

Python ......... 252
来源：http://skt.chenzaomai.com

PHP ............ 252
来源：http://nxq.dashuyun.cn

JavaScript ..... 252
来源：http://ujk.vqdsnc.cn

TypeScript ..... 212
来源：http://jdi.zhoulong.xyz

Java ........... 212
来源：http://rei.snrcjt.cn

Go ............. 212
来源：http://jfc.svipenyu.cn

Ruby ........... 212
来源：http://tel.jinyuanbaomall.cn

C# ............. 212
来源：http://krf.nwbrower.top

C .............. 30
来源：http://gza.xinyue.icu

C++ ............ 30
来源：http://taf.fanxiaobao.xyz

SQL ............ 90
来源：http://jqp.quarkkingdee.top

Bash ........... 80
来源：http://pqu.9152youxi.cn

Kotlin ......... 15
来源：http://idw.xziqi.cn

Swift .......... 15
来源：http://fpy.svipenyu.cn

Lua ............ 10
来源：http://uur.zhiwuduotai.top

Perl ........... 10
来源：http://ryb.fehbvm.com

Scala .......... 10
来源：http://ieq.tanke756.top

------------------------------------
来源：http://ivp.vqdsnc.cn

合计 ........... 2106 条
来源：http://aar.316326.xyz

按章节统计：
来源：http://rcv.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xmn.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://slm.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ouy.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lgb.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fur.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ozo.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ury.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yuc.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://azc.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kku.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pbv.ctjpmb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gex.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://thj.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lgf.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://drp.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tyf.ehwqpu.com

Q SQL 专题                              90
来源：http://run.jqgfzy.top

R Bash 专题                             80
来源：http://cvm.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://igw.guannengcc.top

T 其他语言补充                          60
来源：http://mqr.hfpthk.cn

U 高频实用片段                         120
来源：http://zyy.hcnkem.com

------------------------------------
来源：http://wej.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://ysw.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://jwm.hcnkem.com

使用提醒
来源：http://ybd.andypj.xyz

--------------------------------------------------------------------------------
来源：http://pkq.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cfp.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ulv.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vvc.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dcc.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fzr.shangyingyoupin.top

—— 文件结束 ——
来源：http://ssg.yonumen.top

================================================================================
来源：http://unm.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://yef.shuidangran.top

Common Programming Examples Cheat Book
来源：http://iwy.sufxvd.cn

================================================================================
来源：http://wkg.52xcode.cn

【收录内容】
来源：http://wbi.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dlg.yj202588.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://trk.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://pst.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fhu.havefunace.top

【使用说明】
来源：http://bap.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gbz.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lpw.yvedp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tai.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://urd.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dse.sxryk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fmb.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xym.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sfh.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bzr.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://idd.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://snn.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sfx.shanyushiyangtech.top

【文件统计】
来源：http://hmn.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cmc.andypj.xyz

--------------------------------------------------------------------------------
来源：http://sjr.hysaishi.cn

目  录
来源：http://bcr.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://ioz.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ypp.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eur.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gdf.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uwh.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://trk.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pmb.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nii.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jjb.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qtd.fanxiaobao.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lfk.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jrl.zhaomingkeji.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sys.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ezd.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oxo.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://upb.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sat.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bah.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ykp.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cqa.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ykx.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jzb.hesvh.cn

================================================================================
来源：http://mqz.fzhhl.top

A. 基础语法与类型
来源：http://zwb.havefunace.top

================================================================================
来源：http://ora.ehwqpu.com

[A01] Hello World
来源：http://wao.snrcjt.cn

Py:   print("Hello, World!")
来源：http://pne.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://vod.316326.xyz

JS:   console.log("Hello, World!");
来源：http://jav.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qpb.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://aft.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://ozf.9152youxi.cn

Ruby: puts "Hello, World!"
来源：http://wti.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fjx.zycfv.cn

[A02] 变量声明与赋值
来源：http://ewt.sjlbkw.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mtg.wangdashe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fpw.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://uty.cdnleiting.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tif.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://wdm.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://lyi.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://qbz.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://bnu.haohaochexian.top

[A03] 常量定义
来源：http://rkx.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tyt.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://zpi.uphjek.com

JS:   const PI = 3.14159;
来源：http://eps.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://ctc.cdnleiting.top

Java: static final double PI = 3.14159;
来源：http://ffv.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://bex.yfazqb.com

Ruby: PI = 3.14159
来源：http://inx.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://fpz.zhijiandao.cn

[A04] 判断变量类型
来源：http://wpx.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zfc.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://elc.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://llq.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://ncn.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xhq.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://kic.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zqj.yj20258888.top

C#:   x.GetType().Name; x is int
来源：http://zxv.xuanzx.com

[A05] 整数除法与取模
来源：http://pex.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zpe.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hom.jiagoushi.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xej.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cdy.redwolf501.top

Java: 7 / 2; 7 % 2
来源：http://fpe.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://dav.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://hyk.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://gfh.jinqigfzy.top

[A06] 字符串转数字
来源：http://yfx.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://ulf.ywan-chungtsiang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nmq.yuxming.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cad.shzxlz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ens.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jph.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mcq.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qsk.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qyo.sweek.top

[A07] 数字转字符串
来源：http://wjf.zhengqikj.top

Py:   str(42)
来源：http://iak.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://hmw.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://qtv.ppjwa.cn

TS:   String(42)
来源：http://vsx.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tyr.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://kna.jyoumei.cn

Ruby: 42.to_s
来源：http://tff.ybcxt.top

C#:   42.ToString()
来源：http://iov.gotoacloud.top

[A08] 取整与四舍五入
来源：http://lgt.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jga.jianghu66.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fly.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bxf.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ueq.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jfw.yonumen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kiz.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ecv.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gtn.fanxiaobao.xyz

[A09] 绝对值与最大最小值
来源：http://rle.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://psy.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://taf.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gfv.gotoacloud.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qtp.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ein.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bsz.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bcm.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tgw.quarkkingdee.top

[A10] 生成随机数
来源：http://sys.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://vxj.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://ocj.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ubq.ydjk.org.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jnt.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://knz.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oty.dianchejie.cn

Ruby: rand(1..100)
来源：http://pyv.zhongyouzk.top

C#:   new Random().Next(1, 101)
来源：http://jbr.cucudq.cn

[A11] 条件表达式（三元）
来源：http://zgv.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://gxj.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://xdu.guowangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://dgi.yuanzhike.top

TS:   x > 0 ? "yes" : "no"
来源：http://xsn.tian-w.cn

Java: x > 0 ? "yes" : "no"
来源：http://ruq.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nkb.birdmap.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pew.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://kof.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://hbl.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qsg.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qat.kuanghao11.cn

JS:   `Hello, ${name}!`
来源：http://ehz.chenzaomai.com

TS:   `Hello, ${name}!`
来源：http://cvh.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://hcn.birdmap.top


<!-- 参考信息 -->