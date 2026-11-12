代发 wailian999

[U75] PHP：依赖注入
来源：http://xxe.pycfn.com

composer require psr/container
来源：http://xym.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://kgq.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vtz.fzhhl.top

[U77] PHP：模板渲染
来源：http://anp.zhongyouzk.top

composer require twig/twig
来源：http://weu.tarul.cn

[U78] PHP：单元测试
来源：http://kjg.ivvv.top

composer require --dev phpunit/phpunit
来源：http://qqc.zhijiandao.cn

[U79] PHP：静态分析
来源：http://icv.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://cbd.pycfn.com

[U80] PHP：代码规范修复
来源：http://vzv.gogol.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gga.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://jfc.jianghu66.top

npm init -y;  npm i express
来源：http://kan.redwolf501.top

[U82] JS：package.json 脚本
来源：http://uue.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hnb.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://wfe.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://rgy.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://aaz.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://wya.mhx1999.top

[U85] JS：可选链
来源：http://ows.nwbrower.top

a?.b?.c
来源：http://zce.hywenlv.cn

[U86] JS：空值合并
来源：http://iip.ybcxt.top

a ?? b
来源：http://pdq.quarkkingdee.top

[U87] JS：解构默认值
来源：http://acp.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://nkt.52xcode.cn

[U88] JS：对象展开合并
来源：http://api.vqdsnc.cn

{ ...a, ...b }
来源：http://fqc.zhijiandao.cn

[U89] JS：数组去重
来源：http://gou.jinqigufen.top

[...new Set(arr)]
来源：http://vqe.meibo888.top

[U90] JS：数字数组排序
来源：http://nxj.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://npk.smart0.xyz

[U91] JS：对象键值遍历
来源：http://qqc.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uev.zhixingplan.top

[U92] JS：深拷贝
来源：http://vqj.zhijiandao.cn

structuredClone(obj)
来源：http://rni.vehdjk.com

[U93] JS：模板字符串
来源：http://nub.ppjwa.cn

`共 ${n} 条`
来源：http://eaz.nwbrower.top

[U94] JS：箭头函数
来源：http://uks.nanxinkj.top

const double = x => x * 2;
来源：http://aka.hammf.cn

[U95] JS：Promise 包装
来源：http://btz.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://qkd.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://qrp.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iex.gzhubu.top

[U97] JS：并发请求
来源：http://vop.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://glj.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://jtu.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mxa.zhijiandao.cn

[U99] JS：事件监听
来源：http://kqv.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://xbn.cheryme.top

[U100] JS：DOM 查询
来源：http://hhh.ivvv.top

document.querySelector(".item")
来源：http://jsf.quarkkingdee.top

[U101] JS：classList 操作
来源：http://dht.hfpthk.cn

el.classList.toggle("active")
来源：http://auz.tanke756.top

[U102] JS：本地存储
来源：http://btm.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wbk.jianghu66.top

[U103] JS：定时器
来源：http://ikt.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://apf.redwolf501.top

[U104] JS：防抖
来源：http://cee.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tub.zhaomingkeji.xyz

[U105] JS：节流
来源：http://pka.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nzm.svipenyu.cn

[U106] JS：日期格式化
来源：http://iwg.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://coh.aizwys.cn

[U107] JS：数字千分位
来源：http://utt.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://avk.tarul.cn

[U108] JS：随机整数
来源：http://tgg.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jkv.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://hre.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://ngo.tian-w.cn

[U110] JS：数组分块
来源：http://ubz.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lmw.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://jwv.xylfe.cn

new Map(Object.entries(obj))
来源：http://aqi.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://tli.cucudq.cn

"7".padStart(3, "0")
来源：http://ppq.zdbjq.cn

[U113] JS：正则替换全部
来源：http://ton.bbcook.cn

s.replaceAll("a", "b")
来源：http://cfl.daxiang520.top

[U114] JS：JSON 深比较
来源：http://hly.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gax.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://jyi.vqdsnc.cn

crypto.randomUUID()
来源：http://cvs.daria6918.cn

[U116] JS：类型检查（JSDoc）
来源：http://wdo.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://ltd.ivvv.top

[U117] JS：单元测试
来源：http://uam.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://pou.jiagoushi.top

[U118] JS：开发服务器
来源：http://nay.tarul.cn

npm i -D vite;  npx vite
来源：http://das.jlsjyb.cn

[U119] JS：生产构建
来源：http://ajb.andypj.xyz

npx vite build
来源：http://twu.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://ifd.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://nah.yonumen.top

================================================================================
来源：http://jnm.0kj1m.cn

统计汇总
来源：http://egk.uphjek.com

================================================================================
来源：http://tle.iojbl.cn

按语言统计（条）：
来源：http://kpq.guannengcc.top

Python ......... 252
来源：http://tch.fengsongda.top

PHP ............ 252
来源：http://ops.guowangkeji.top

JavaScript ..... 252
来源：http://yjn.uphjek.com

TypeScript ..... 212
来源：http://aai.birdmap.top

Java ........... 212
来源：http://shu.zhiwuduotai.top

Go ............. 212
来源：http://fig.ctjpmb.com

Ruby ........... 212
来源：http://yvz.0kj1m.cn

C# ............. 212
来源：http://gyv.svipenyu.cn

C .............. 30
来源：http://xdq.mhx1999.top

C++ ............ 30
来源：http://oki.ydzc1.top

SQL ............ 90
来源：http://ooq.0kj1m.cn

Bash ........... 80
来源：http://pmg.ctjpmb.com

Kotlin ......... 15
来源：http://lch.zhaomingkeji.xyz

Swift .......... 15
来源：http://fak.ctjpmb.com

Lua ............ 10
来源：http://zgv.xziqi.cn

Perl ........... 10
来源：http://xve.cqqwz.cn

Scala .......... 10
来源：http://fyg.feifeiyinyue.top

------------------------------------
来源：http://vww.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://glv.gogol.net.cn

按章节统计：
来源：http://dea.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://urh.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ugn.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://osk.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lfm.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kia.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vkr.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ror.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kty.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://byd.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uog.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qbk.fzhhl.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rik.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jwn.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zvx.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sou.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cqe.andypj.xyz

Q SQL 专题                              90
来源：http://kpb.svipenyu.cn

R Bash 专题                             80
来源：http://rja.fzhhl.top

S C / C++ 专题                          60
来源：http://szj.nanxuanxn.top

T 其他语言补充                          60
来源：http://gof.yj20258888.top

U 高频实用片段                         120
来源：http://yjw.dianchejie.cn

------------------------------------
来源：http://tyo.yuxming.cn

合计                                  2106 条
来源：http://nbf.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://gdb.ywan-chungtsiang.top

使用提醒
来源：http://qmm.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://rzj.yuanzhike.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zhl.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ixk.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://agy.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://apl.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gtf.wangdashe.top

—— 文件结束 ——
来源：http://fld.zdbjq.cn

================================================================================
来源：http://qmf.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://qal.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://zts.ctjpmb.com

================================================================================
来源：http://nyj.jinqigfzy.top

【收录内容】
来源：http://jii.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tjs.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://spk.316326.xyz

SQL · Bash · C · C++
来源：http://onn.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cnf.yonumen.top

【使用说明】
来源：http://zpt.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uba.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rvm.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yia.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ijf.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ipp.zhixingplan.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gez.hywenlv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sse.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wuk.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xsb.mhx1999.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oud.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sdx.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qnw.fengsongda.top

【文件统计】
来源：http://doz.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://snt.yfazqb.com

--------------------------------------------------------------------------------
来源：http://sbu.hnxiangtu.top

目  录
来源：http://smu.xziqi.cn

--------------------------------------------------------------------------------
来源：http://ukw.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kqd.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cxl.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vkj.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://toj.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kyc.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tsx.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://big.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ddr.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nzl.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://src.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ocm.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vyp.tian-w.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://opu.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pxz.yongpay.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://khs.sufxvd.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rtc.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lbl.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://vtu.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ilx.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwg.cdnleiting.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cjx.316326.xyz

================================================================================
来源：http://fhd.ctjpmb.com

A. 基础语法与类型
来源：http://bew.316326.xyz

================================================================================
来源：http://evr.epnwcf.com

[A01] Hello World
来源：http://ysz.fzhhl.top

Py:   print("Hello, World!")
来源：http://vud.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://gtn.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://xzu.shanyushiyangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ery.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://oxd.fehbvm.com

Go:   fmt.Println("Hello, World!")
来源：http://att.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://zow.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ziz.shzxlz.cn

[A02] 变量声明与赋值
来源：http://ldz.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qrc.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mnt.fehbvm.com

JS:   let name = "Alex"; const age = 20;
来源：http://rpe.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iwt.yuxming.cn

Java: String name = "Alex"; int age = 20;
来源：http://xxd.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://iof.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://swl.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://ytd.vehdjk.com

[A03] 常量定义
来源：http://stl.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hnh.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://uii.shanyushiyangtech.top

JS:   const PI = 3.14159;
来源：http://zmv.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://tyk.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://wai.xuetiantiany.cn

Go:   const PI = 3.14159
来源：http://jzp.shuidangran.top

Ruby: PI = 3.14159
来源：http://jvu.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://ebl.hnxiangtu.top

[A04] 判断变量类型
来源：http://uev.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cgz.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kfv.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ute.tian-w.cn

TS:   typeof x; x instanceof Date
来源：http://fwr.yueranfly.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pqk.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://mmi.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jhy.yfazqb.com

C#:   x.GetType().Name; x is int
来源：http://zgw.yonumen.top

[A05] 整数除法与取模
来源：http://qbk.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://noi.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ejq.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cpz.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ocp.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://fjb.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://rgr.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://fqv.yfazqb.com

C#:   7 / 2; 7 % 2
来源：http://yye.jinqigfzy.top

[A06] 字符串转数字
来源：http://feb.cashguo.top

Py:   int("42"); float("3.14")
来源：http://rxw.jinyuanbaomall.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jdb.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mgu.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://tnk.ppjwa.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://seh.yuxming.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bft.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mvf.yonumen.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zpw.hnxiangtu.top

[A07] 数字转字符串
来源：http://nvw.aibaodan.cn

Py:   str(42)
来源：http://ray.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://mqz.iojbl.cn

JS:   String(42); (42).toString()
来源：http://lcd.c1oappe.top

TS:   String(42)
来源：http://zxv.dashuyun.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pap.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://yap.pengpengdd.cyou

Ruby: 42.to_s
来源：http://kgm.meibo888.top

C#:   42.ToString()
来源：http://ztx.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://xqw.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qrr.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://biy.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://efh.jqgufenzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jfp.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ocf.xuetiantiany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hxb.zdbjq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zvb.ctjpmb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tiq.hcnkem.com

[A09] 绝对值与最大最小值
来源：http://cxc.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qeb.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lgv.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rym.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ayx.jlsjyb.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bix.yj20258.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://own.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uhy.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://duo.fengsongda.top

[A10] 生成随机数
来源：http://chf.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://akp.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://rnp.ehwqpu.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aug.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xhp.hcnkem.com

Java: new Random().nextInt(100) + 1
来源：http://cpp.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fhd.jinqigufen.top

Ruby: rand(1..100)
来源：http://cjj.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://wjb.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://yst.52xcode.cn

Py:   "yes" if x > 0 else "no"
来源：http://qlh.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ocn.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://pph.gzhubu.top

TS:   x > 0 ? "yes" : "no"
来源：http://xat.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://lmi.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yer.zhiwuduotai.top

Ruby: x > 0 ? "yes" : "no"
来源：http://azi.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cjm.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://apu.kuanghao11.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ldn.yvedp.cn


<!-- 参考信息 -->