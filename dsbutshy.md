代发 wailian999

[U75] PHP：依赖注入
来源：http://zuv.0kj1m.cn

composer require psr/container
来源：http://qdo.wangdashe.top

[U76] PHP：简单路由
来源：http://amk.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ljx.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://pxh.jinqigfzy.top

composer require twig/twig
来源：http://gij.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://xnk.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://tvp.zhoulong.xyz

[U79] PHP：静态分析
来源：http://fen.cheryme.top

composer require --dev phpstan/phpstan
来源：http://sfb.sweek.top

[U80] PHP：代码规范修复
来源：http://xyu.hammf.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ult.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://cnm.zhongyouzk.top

npm init -y;  npm i express
来源：http://xry.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://omf.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ezt.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://ggu.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://soh.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://klz.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://uig.yj20258.top

[U85] JS：可选链
来源：http://sby.dashuyun.cn

a?.b?.c
来源：http://qia.hfpthk.cn

[U86] JS：空值合并
来源：http://bfj.shangyingyoupin.top

a ?? b
来源：http://ndh.0kj1m.cn

[U87] JS：解构默认值
来源：http://uck.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://emu.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://bov.xylfe.cn

{ ...a, ...b }
来源：http://xfg.guowangkeji.top

[U89] JS：数组去重
来源：http://ajm.yuanzhike.top

[...new Set(arr)]
来源：http://urg.xziqi.cn

[U90] JS：数字数组排序
来源：http://hwg.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://uyu.sweek.top

[U91] JS：对象键值遍历
来源：http://yjf.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cze.jlsjyb.cn

[U92] JS：深拷贝
来源：http://ojh.ctjpmb.com

structuredClone(obj)
来源：http://fbm.yonumen.top

[U93] JS：模板字符串
来源：http://fnm.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://ygq.andypj.xyz

[U94] JS：箭头函数
来源：http://gyv.hysaishi.cn

const double = x => x * 2;
来源：http://rsa.daxiang520.top

[U95] JS：Promise 包装
来源：http://ecb.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://xhv.aizwys.cn

[U96] JS：async/await 与异常
来源：http://dxw.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kra.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://fwn.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sym.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://bey.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uch.haohaochexian.top

[U99] JS：事件监听
来源：http://zqh.daxiang520.top

el.addEventListener("click", e => {})
来源：http://kcy.fehbvm.com

[U100] JS：DOM 查询
来源：http://vfx.sufxvd.cn

document.querySelector(".item")
来源：http://zkh.yueranfly.top

[U101] JS：classList 操作
来源：http://mxk.yangfankeji.com

el.classList.toggle("active")
来源：http://byk.aizwys.cn

[U102] JS：本地存储
来源：http://agt.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xxl.dashuyun.cn

[U103] JS：定时器
来源：http://wsr.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hhd.vqdsnc.cn

[U104] JS：防抖
来源：http://foz.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://thn.wangdashe.top

[U105] JS：节流
来源：http://lhs.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xay.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://jrl.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://esf.tanke756.top

[U107] JS：数字千分位
来源：http://aok.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bhy.bbcook.cn

[U108] JS：随机整数
来源：http://amc.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ala.shangyingyoupin.top

[U109] JS：数组分组
来源：http://jle.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://dqa.yueranfly.top

[U110] JS：数组分块
来源：http://slj.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://neg.guowangkeji.top

[U111] JS：对象转 Map
来源：http://thl.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://qem.daxiang520.top

[U112] JS：字符串补位
来源：http://kzk.yfazqb.com

"7".padStart(3, "0")
来源：http://acj.xuanzx.com

[U113] JS：正则替换全部
来源：http://qld.zdbjq.cn

s.replaceAll("a", "b")
来源：http://yqi.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://uug.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fdx.cashguo.top

[U115] JS：生成 UUID
来源：http://psb.hesvh.cn

crypto.randomUUID()
来源：http://csu.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://cgt.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://ger.dashuyun.cn

[U117] JS：单元测试
来源：http://fbx.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://dve.ydjk.org.cn

[U118] JS：开发服务器
来源：http://vqw.cqqwz.cn

npm i -D vite;  npx vite
来源：http://uax.hfpthk.cn

[U119] JS：生产构建
来源：http://utw.hnxiangtu.top

npx vite build
来源：http://zmf.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://off.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://vfe.gotoacloud.top

================================================================================
来源：http://pcn.jinyuanbaomall.cn

统计汇总
来源：http://ipk.gotoacloud.top

================================================================================
来源：http://wvq.316326.xyz

按语言统计（条）：
来源：http://oxq.sysykeji.top

Python ......... 252
来源：http://sdk.feifeiyinyue.top

PHP ............ 252
来源：http://ici.wangshuangyany.cn

JavaScript ..... 252
来源：http://atp.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://aqk.fktsv.cn

Java ........... 212
来源：http://fnz.fanxiaobao.xyz

Go ............. 212
来源：http://cwm.redwolf501.top

Ruby ........... 212
来源：http://gjr.gogol.net.cn

C# ............. 212
来源：http://oyp.jiagoushi.top

C .............. 30
来源：http://cvi.jinqigufen.top

C++ ............ 30
来源：http://jqu.yuxming.cn

SQL ............ 90
来源：http://xxw.meibo888.top

Bash ........... 80
来源：http://qwk.fehbvm.com

Kotlin ......... 15
来源：http://itr.jinqigufen.top

Swift .......... 15
来源：http://nza.chenlongwang.top

Lua ............ 10
来源：http://acx.ydjk.org.cn

Perl ........... 10
来源：http://bzt.jyoumei.cn

Scala .......... 10
来源：http://oys.hesvh.cn

------------------------------------
来源：http://oyd.quarkkingdee.top

合计 ........... 2106 条
来源：http://mdr.jqgufenzy.top

按章节统计：
来源：http://bnk.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fcv.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wxa.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jsw.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://emw.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xrp.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vkl.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rxm.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cii.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://igy.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://von.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rpr.redwolf501.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oai.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cdr.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jpv.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pwg.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ulk.chenzaomai.com

Q SQL 专题                              90
来源：http://ttv.iojbl.cn

R Bash 专题                             80
来源：http://fyr.quarkkingdee.top

S C / C++ 专题                          60
来源：http://vxu.svipenyu.cn

T 其他语言补充                          60
来源：http://yne.zycfv.cn

U 高频实用片段                         120
来源：http://ntp.bjfxy.top

------------------------------------
来源：http://sob.sufxvd.cn

合计                                  2106 条
来源：http://dee.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://ork.hywenlv.cn

使用提醒
来源：http://zrp.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://quz.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eyb.sweek.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://umk.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ckv.mhx1999.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rts.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oaq.chenlongwang.top

—— 文件结束 ——
来源：http://iev.tian-w.cn

================================================================================
来源：http://wal.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://woq.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://dhu.xziqi.cn

================================================================================
来源：http://fau.gotoacloud.top

【收录内容】
来源：http://xdn.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cns.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zjs.mhx1999.top

SQL · Bash · C · C++
来源：http://dtt.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zxc.iojbl.cn

【使用说明】
来源：http://nai.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://asj.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dag.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xxq.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lxm.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hpb.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kac.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://flz.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://etg.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kmk.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hpi.ydjk.org.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tmt.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bgo.zhongyouzk.top

【文件统计】
来源：http://lhl.yongpay.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fao.yfazqb.com

--------------------------------------------------------------------------------
来源：http://vly.shangyingyoupin.top

目  录
来源：http://nzp.shuidangran.top

--------------------------------------------------------------------------------
来源：http://kdu.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ded.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zvd.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oli.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ufy.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zct.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://olr.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://drm.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pov.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dig.wangdashe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mky.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bjn.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eiz.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://boy.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gss.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dgh.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qni.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cao.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vuw.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pew.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cac.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vnc.yanxiufei.cn

================================================================================
来源：http://sco.shanyushiyangtech.top

A. 基础语法与类型
来源：http://bnc.svipenyu.cn

================================================================================
来源：http://pyt.yanxiufei.cn

[A01] Hello World
来源：http://lxm.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://sca.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://fdw.havefunace.top

JS:   console.log("Hello, World!");
来源：http://khv.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://urc.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://myk.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://gpz.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://gvo.kuanghao11.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rmf.ivvv.top

[A02] 变量声明与赋值
来源：http://ems.xylfe.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jqt.316326.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ktt.zdqjudy.top

JS:   let name = "Alex"; const age = 20;
来源：http://efb.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vuc.redwolf501.top

Java: String name = "Alex"; int age = 20;
来源：http://ilz.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://fip.zhixingplan.top

Ruby: name = "Alex"; age = 20
来源：http://aut.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://agp.zycfv.cn

[A03] 常量定义
来源：http://fzq.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sbu.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://tlp.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://xud.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://ryj.tarul.cn

Java: static final double PI = 3.14159;
来源：http://zed.hammf.cn

Go:   const PI = 3.14159
来源：http://qbo.ydzc1.top

Ruby: PI = 3.14159
来源：http://mkw.yueranfly.top

C#:   const double PI = 3.14159;
来源：http://xhy.jinqigufen.top

[A04] 判断变量类型
来源：http://pnd.gzhubu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rdt.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://omn.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qks.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://did.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iia.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://qzb.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ubp.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://ddk.vqdsnc.cn

[A05] 整数除法与取模
来源：http://kgy.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lqe.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kmq.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kgk.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uqa.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://mtg.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://aqu.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://aga.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://jzz.havefunace.top

[A06] 字符串转数字
来源：http://qnv.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://aps.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://koa.tian-w.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://krp.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://xqd.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mhl.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vnr.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://nxq.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tyz.quarkkingdee.top

[A07] 数字转字符串
来源：http://liv.gogol.net.cn

Py:   str(42)
来源：http://old.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://fmj.hcnkem.com

JS:   String(42); (42).toString()
来源：http://rbe.hysaishi.cn

TS:   String(42)
来源：http://qek.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gao.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://ywd.pycfn.com

Ruby: 42.to_s
来源：http://bag.mhx1999.top

C#:   42.ToString()
来源：http://wll.ivvv.top

[A08] 取整与四舍五入
来源：http://juu.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nol.dianchejie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xfw.vqdsnc.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rye.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://plz.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tej.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jdr.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eon.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dub.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://zrh.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jya.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ojw.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ykj.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pyi.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tzb.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ucq.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://atl.chenlongwang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vzq.cqqwz.cn

[A10] 生成随机数
来源：http://mog.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://cic.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://pte.guannengcc.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lve.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ngq.pengpengdd.cyou

Java: new Random().nextInt(100) + 1
来源：http://sdu.ivvv.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tml.shangyingyoupin.top

Ruby: rand(1..100)
来源：http://cpk.gzhubu.top

C#:   new Random().Next(1, 101)
来源：http://cxj.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://zpt.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://vec.tarul.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eew.hammf.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tcb.chenjidiqi.icu

TS:   x > 0 ? "yes" : "no"
来源：http://zkr.shanyushiyangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://ixr.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qzg.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xlb.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bpa.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://gsy.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mlp.yj20258.top


<!-- 参考信息 -->