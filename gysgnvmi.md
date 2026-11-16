代发 wailian999

[U75] PHP：依赖注入
来源：http://qbk.jianghu66.top

composer require psr/container
来源：http://yry.jianghu66.top

[U76] PHP：简单路由
来源：http://boq.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xsj.guannengcc.top

[U77] PHP：模板渲染
来源：http://cpn.ybcxt.top

composer require twig/twig
来源：http://som.jinqigufen.top

[U78] PHP：单元测试
来源：http://lwa.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://sip.shuidangran.top

[U79] PHP：静态分析
来源：http://rth.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://ogr.aizwys.cn

[U80] PHP：代码规范修复
来源：http://lkl.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qrb.redwolf501.top

[U81] JS：初始化项目
来源：http://rih.yanxiufei.cn

npm init -y;  npm i express
来源：http://wwy.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://rba.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fne.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://pmr.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://ueq.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://gmu.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://faz.yj20258888.top

[U85] JS：可选链
来源：http://ikl.xinyue.icu

a?.b?.c
来源：http://qpb.daria6918.cn

[U86] JS：空值合并
来源：http://sbd.xylfe.cn

a ?? b
来源：http://qkr.havefunace.top

[U87] JS：解构默认值
来源：http://wxl.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://ubv.ctjpmb.com

[U88] JS：对象展开合并
来源：http://uab.zdbjq.cn

{ ...a, ...b }
来源：http://fiu.316326.xyz

[U89] JS：数组去重
来源：http://baj.vqdsnc.cn

[...new Set(arr)]
来源：http://yqc.zhengqikj.top

[U90] JS：数字数组排序
来源：http://bpi.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://mvv.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://sdt.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sly.xylfe.cn

[U92] JS：深拷贝
来源：http://crw.havefunace.top

structuredClone(obj)
来源：http://wtk.ydjk.org.cn

[U93] JS：模板字符串
来源：http://nxu.dianchejie.cn

`共 ${n} 条`
来源：http://zkm.cucudq.cn

[U94] JS：箭头函数
来源：http://ggh.haohaochexian.top

const double = x => x * 2;
来源：http://xvm.ehwqpu.com

[U95] JS：Promise 包装
来源：http://cmf.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://bjv.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://vrr.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vbi.daxiang520.top

[U97] JS：并发请求
来源：http://sya.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iwi.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://hak.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tai.yangfankeji.com

[U99] JS：事件监听
来源：http://yin.tarul.cn

el.addEventListener("click", e => {})
来源：http://ceq.sweek.top

[U100] JS：DOM 查询
来源：http://ctx.tianlin.xyz

document.querySelector(".item")
来源：http://jtf.sxryk.cn

[U101] JS：classList 操作
来源：http://rlz.shzxlz.cn

el.classList.toggle("active")
来源：http://rss.ctjpmb.com

[U102] JS：本地存储
来源：http://uul.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://byc.ctjpmb.com

[U103] JS：定时器
来源：http://qee.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uoy.gotoacloud.top

[U104] JS：防抖
来源：http://ery.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msj.jinqigufen.top

[U105] JS：节流
来源：http://tsc.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lna.pycfn.com

[U106] JS：日期格式化
来源：http://uta.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dvd.guannengcc.top

[U107] JS：数字千分位
来源：http://ytl.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jos.nanxinkj.top

[U108] JS：随机整数
来源：http://wlb.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rht.yj20258888.top

[U109] JS：数组分组
来源：http://cqk.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://ykw.yangfankeji.com

[U110] JS：数组分块
来源：http://ery.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kyl.snrcjt.cn

[U111] JS：对象转 Map
来源：http://pba.yj20258888.top

new Map(Object.entries(obj))
来源：http://iio.ctjpmb.com

[U112] JS：字符串补位
来源：http://owu.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://gih.birdmap.top

[U113] JS：正则替换全部
来源：http://fej.ehwqpu.com

s.replaceAll("a", "b")
来源：http://myl.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://crh.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://enn.9152youxi.cn

[U115] JS：生成 UUID
来源：http://ruh.jinqigufen.top

crypto.randomUUID()
来源：http://icr.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://cte.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://fye.nanxuanxn.top

[U117] JS：单元测试
来源：http://gel.hammf.cn

npm i -D vitest;  npx vitest
来源：http://xyn.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://iqn.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://obg.jinqigfzy.top

[U119] JS：生产构建
来源：http://pga.svipenyu.cn

npx vite build
来源：http://nyi.0kj1m.cn

[U120] JS：读取环境变量（Vite）
来源：http://vbd.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://wwz.xinyue.icu

================================================================================
来源：http://dus.fengsongda.top

统计汇总
来源：http://ekg.ppjwa.cn

================================================================================
来源：http://jec.aibaodan.cn

按语言统计（条）：
来源：http://zuk.dianchejie.cn

Python ......... 252
来源：http://sds.yuanzhike.top

PHP ............ 252
来源：http://uhs.jlsjyb.cn

JavaScript ..... 252
来源：http://bvi.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://kzh.yueranfly.top

Java ........... 212
来源：http://lmu.chenlongwang.top

Go ............. 212
来源：http://acf.ybcxt.top

Ruby ........... 212
来源：http://cpm.fengsongda.top

C# ............. 212
来源：http://tff.fzhhl.top

C .............. 30
来源：http://mky.jiagoushi.top

C++ ............ 30
来源：http://tqu.zhijiandao.cn

SQL ............ 90
来源：http://coh.haohaochexian.top

Bash ........... 80
来源：http://iss.bjfxy.top

Kotlin ......... 15
来源：http://gru.jiagoushi.top

Swift .......... 15
来源：http://vet.jinqigufen.top

Lua ............ 10
来源：http://jux.quarkkingdee.top

Perl ........... 10
来源：http://xtc.xuetiantiany.cn

Scala .......... 10
来源：http://pxk.ehwqpu.com

------------------------------------
来源：http://vvk.ctjpmb.com

合计 ........... 2106 条
来源：http://oub.fktsv.cn

按章节统计：
来源：http://rxa.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kyi.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nce.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rgz.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ybb.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://quo.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gqd.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gkt.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sjq.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lxu.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fel.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gzz.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jsb.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kjb.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gwe.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ysl.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yoc.chenlongwang.top

Q SQL 专题                              90
来源：http://zgf.ydzc1.top

R Bash 专题                             80
来源：http://azx.zhijiandao.cn

S C / C++ 专题                          60
来源：http://gmp.smart0.xyz

T 其他语言补充                          60
来源：http://eia.yj20258888.top

U 高频实用片段                         120
来源：http://egi.fehbvm.com

------------------------------------
来源：http://lif.hfpthk.cn

合计                                  2106 条
来源：http://dod.daria6918.cn

--------------------------------------------------------------------------------
来源：http://pvy.jiagoushi.top

使用提醒
来源：http://jwq.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://dht.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nol.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zqy.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lyc.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qhp.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jkm.jiagoushi.top

—— 文件结束 ——
来源：http://ano.yangfankeji.com

================================================================================
来源：http://nnj.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://gmf.yueranfly.top

Common Programming Examples Cheat Book
来源：http://jcd.nwbrower.top

================================================================================
来源：http://djv.jianghu66.top

【收录内容】
来源：http://vmn.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hfk.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hvo.ydzc1.top

SQL · Bash · C · C++
来源：http://wkb.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rge.ydzc1.top

【使用说明】
来源：http://xft.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cpj.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nmk.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kqg.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cec.epnwcf.com

Bash:  Shell         C:     C             C++:   C++
来源：http://kcv.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mbr.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yfp.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hcj.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vdj.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jhk.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://srd.xziqi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://udn.daxiang520.top

【文件统计】
来源：http://xjs.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tac.daria6918.cn

--------------------------------------------------------------------------------
来源：http://yqo.jinghuilouyu.cn

目  录
来源：http://kqb.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://ubb.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wpa.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://znl.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pjj.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vgn.ctjpmb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uqg.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kvd.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fwz.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bjx.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ndf.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xlv.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kso.jyoumei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mfw.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tba.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yaa.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zyg.vqdsnc.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tpc.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qnv.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://fki.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://off.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bsw.fzhhl.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ddx.bbcook.cn

================================================================================
来源：http://knt.hywenlv.cn

A. 基础语法与类型
来源：http://uuh.sweek.top

================================================================================
来源：http://iwj.ywan-chungtsiang.top

[A01] Hello World
来源：http://iub.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://mad.hnxiangtu.top

PHP:  echo "Hello, World!";
来源：http://owr.vqdsnc.cn

JS:   console.log("Hello, World!");
来源：http://vfh.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zxz.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://rdc.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://bii.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://qra.cucudq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://unl.fktsv.cn

[A02] 变量声明与赋值
来源：http://rru.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wzl.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qtv.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dnr.gotoacloud.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zso.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://lcq.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://ilx.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://urc.jianghu66.top

C#:   string name = "Alex"; int age = 20;
来源：http://wdo.zhengqikj.top

[A03] 常量定义
来源：http://zqn.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qmw.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://auz.nwbrower.top

JS:   const PI = 3.14159;
来源：http://wmo.aibaodan.cn

TS:   const PI: number = 3.14159;
来源：http://pjy.52xcode.cn

Java: static final double PI = 3.14159;
来源：http://jug.daria6918.cn

Go:   const PI = 3.14159
来源：http://cnp.jianghu66.top

Ruby: PI = 3.14159
来源：http://yhv.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://vlr.ydzc1.top

[A04] 判断变量类型
来源：http://uiq.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vfi.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mnu.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ylb.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://vtb.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bdf.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://nsq.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rkl.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://agw.jianghu66.top

[A05] 整数除法与取模
来源：http://hsd.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://syq.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ujh.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://shg.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://afe.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://fem.fanxiaobao.xyz

Go:   7 / 2; 7 % 2
来源：http://git.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://vbq.ivvv.top

C#:   7 / 2; 7 % 2
来源：http://qoh.jyoumei.cn

[A06] 字符串转数字
来源：http://jbc.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://fvr.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ptw.hcnkem.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eqh.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://pdp.0kj1m.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mxf.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nil.redwolf501.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fqd.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ilz.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://vii.jlsjyb.cn

Py:   str(42)
来源：http://yka.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://rva.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://fky.nanxuanxn.top

TS:   String(42)
来源：http://aje.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ykb.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://viw.c1oappe.top

Ruby: 42.to_s
来源：http://wic.nwbrower.top

C#:   42.ToString()
来源：http://aef.jinqigufen.top

[A08] 取整与四舍五入
来源：http://gle.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tbs.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cyb.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iqm.shuidangran.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vcr.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://puf.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dav.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gfi.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://thk.cdnleiting.top

[A09] 绝对值与最大最小值
来源：http://qdf.jyoumei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://usp.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://foi.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ncv.pengpengdd.cyou

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tzt.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mbs.hfpthk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mwz.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gjt.hfpthk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tgs.9152youxi.cn

[A10] 生成随机数
来源：http://tmj.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://vxj.pycfn.com

PHP:  random_int(1, 100);
来源：http://fxn.hongshengwenyu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qdd.jinyuanbaomall.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xud.aibaodan.cn

Java: new Random().nextInt(100) + 1
来源：http://pfa.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xtq.quarkkingdee.top

Ruby: rand(1..100)
来源：http://rrh.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://qyc.ywan-chungtsiang.top

[A11] 条件表达式（三元）
来源：http://ozk.pycfn.com

Py:   "yes" if x > 0 else "no"
来源：http://luv.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fdw.xylfe.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zwt.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://aql.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://hgv.zhiwuduotai.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pds.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rae.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ghy.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://oms.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mns.tarul.cn


<!-- 参考信息 -->