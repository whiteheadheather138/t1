代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://cru.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://zpy.316326.xyz

[U74] PHP：读取环境变量
来源：http://icw.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://pai.cdnleiting.top

[U75] PHP：依赖注入
来源：http://xus.xuetiantiany.cn

composer require psr/container
来源：http://fom.zhongyouzk.top

[U76] PHP：简单路由
来源：http://ywt.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ttd.c1oappe.top

[U77] PHP：模板渲染
来源：http://ptz.chenzaomai.com

composer require twig/twig
来源：http://qso.hammf.cn

[U78] PHP：单元测试
来源：http://eyt.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://uok.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://imu.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://sfa.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://fef.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://neq.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://dmi.andypj.xyz

npm init -y;  npm i express
来源：http://jah.sweek.top

[U82] JS：package.json 脚本
来源：http://guw.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jlv.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://tmy.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://mzr.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://sbz.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://hln.fanxiaobao.xyz

[U85] JS：可选链
来源：http://fql.tarul.cn

a?.b?.c
来源：http://pvq.smart0.xyz

[U86] JS：空值合并
来源：http://aoa.mhx1999.top

a ?? b
来源：http://vgl.haohaochexian.top

[U87] JS：解构默认值
来源：http://iil.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://owx.sxryk.cn

[U88] JS：对象展开合并
来源：http://hiw.uphjek.com

{ ...a, ...b }
来源：http://rel.epnwcf.com

[U89] JS：数组去重
来源：http://vsy.yonumen.top

[...new Set(arr)]
来源：http://sah.yongpay.top

[U90] JS：数字数组排序
来源：http://hwj.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://dab.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://wsd.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ost.pycfn.com

[U92] JS：深拷贝
来源：http://fsy.yj20258.top

structuredClone(obj)
来源：http://lzc.jqgufenzy.top

[U93] JS：模板字符串
来源：http://pqw.ivvv.top

`共 ${n} 条`
来源：http://ond.ydjk.org.cn

[U94] JS：箭头函数
来源：http://rxw.xinyue.icu

const double = x => x * 2;
来源：http://exh.havefunace.top

[U95] JS：Promise 包装
来源：http://dhx.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://kjr.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://zqz.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://idj.yfazqb.com

[U97] JS：并发请求
来源：http://jqg.jqgfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://slf.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://qkt.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zej.jianghu66.top

[U99] JS：事件监听
来源：http://uao.aizwys.cn

el.addEventListener("click", e => {})
来源：http://zji.ybcxt.top

[U100] JS：DOM 查询
来源：http://kxg.sjlbkw.cn

document.querySelector(".item")
来源：http://smj.ppjwa.cn

[U101] JS：classList 操作
来源：http://rys.gogol.net.cn

el.classList.toggle("active")
来源：http://nqz.guowangkeji.top

[U102] JS：本地存储
来源：http://mbb.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ikz.ybcxt.top

[U103] JS：定时器
来源：http://jxy.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zeq.sxryk.cn

[U104] JS：防抖
来源：http://kvp.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aop.iojbl.cn

[U105] JS：节流
来源：http://uij.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hkm.sweek.top

[U106] JS：日期格式化
来源：http://sik.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sfl.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://sgi.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ovs.jyoumei.cn

[U108] JS：随机整数
来源：http://hce.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://djk.bbcook.cn

[U109] JS：数组分组
来源：http://ilo.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://vbq.andypj.xyz

[U110] JS：数组分块
来源：http://qns.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qgd.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://xpl.bbcook.cn

new Map(Object.entries(obj))
来源：http://igf.yonumen.top

[U112] JS：字符串补位
来源：http://lhl.iojbl.cn

"7".padStart(3, "0")
来源：http://pzt.xziqi.cn

[U113] JS：正则替换全部
来源：http://apn.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://gaf.hcnkem.com

[U114] JS：JSON 深比较
来源：http://mzh.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xpi.sxryk.cn

[U115] JS：生成 UUID
来源：http://eiu.haohaochexian.top

crypto.randomUUID()
来源：http://gmq.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://liq.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://mbg.jiagoushi.top

[U117] JS：单元测试
来源：http://otm.yongpay.top

npm i -D vitest;  npx vitest
来源：http://jrq.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://osm.yj20258.top

npm i -D vite;  npx vite
来源：http://tfq.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://eoa.hammf.cn

npx vite build
来源：http://hmx.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://bxv.yj202588.top

import.meta.env.VITE_API_URL
来源：http://szb.tian-w.cn

================================================================================
来源：http://bgh.shanyushiyangkeji.top

统计汇总
来源：http://tyr.tarul.cn

================================================================================
来源：http://vkp.jiagoushi.top

按语言统计（条）：
来源：http://cwx.chenzaomai.com

Python ......... 252
来源：http://afa.hesvh.cn

PHP ............ 252
来源：http://zwf.vehdjk.com

JavaScript ..... 252
来源：http://byq.fehbvm.com

TypeScript ..... 212
来源：http://gko.guowangkeji.top

Java ........... 212
来源：http://okh.jinqigfzy.top

Go ............. 212
来源：http://rls.chenzaomai.com

Ruby ........... 212
来源：http://cgf.9152youxi.cn

C# ............. 212
来源：http://tpv.guannengcc.top

C .............. 30
来源：http://lqo.yueranfly.top

C++ ............ 30
来源：http://com.gzhubu.top

SQL ............ 90
来源：http://ljn.dianchejie.cn

Bash ........... 80
来源：http://evp.fanxiaobao.xyz

Kotlin ......... 15
来源：http://xsx.daria6918.cn

Swift .......... 15
来源：http://zsc.jinqigfzy.top

Lua ............ 10
来源：http://hru.hcnkem.com

Perl ........... 10
来源：http://vfj.yj20258888.top

Scala .......... 10
来源：http://prr.jinqigfzy.top

------------------------------------
来源：http://epo.hesvh.cn

合计 ........... 2106 条
来源：http://ecf.sufxvd.cn

按章节统计：
来源：http://weg.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xyx.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hyk.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iwd.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hox.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bow.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qth.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pyu.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://guf.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vbl.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eds.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kuf.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xvy.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://unn.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hpv.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bfp.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ueo.jinqigfzy.top

Q SQL 专题                              90
来源：http://oja.redwolf501.top

R Bash 专题                             80
来源：http://zyi.zhiwuduotai.top

S C / C++ 专题                          60
来源：http://kmb.vehdjk.com

T 其他语言补充                          60
来源：http://ftv.52xcode.cn

U 高频实用片段                         120
来源：http://vup.9152youxi.cn

------------------------------------
来源：http://eox.ivvv.top

合计                                  2106 条
来源：http://zkl.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://sgv.hnxiangtu.top

使用提醒
来源：http://igp.hnqzz.top

--------------------------------------------------------------------------------
来源：http://kkg.chenjidiqi.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bpd.gaohongyu789.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tia.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hfn.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://arj.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wyi.ywan-chungtsiang.top

—— 文件结束 ——
来源：http://rpc.0kj1m.cn

================================================================================
来源：http://weh.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://wgi.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://oks.cucudq.cn

================================================================================
来源：http://wxj.epnwcf.com

【收录内容】
来源：http://znp.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gsh.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wqu.zycfv.cn

SQL · Bash · C · C++
来源：http://hkg.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://piu.fanxiaobao.xyz

【使用说明】
来源：http://dqk.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://onu.smart0.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rce.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pcf.zdqjudy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ptw.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nyp.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ksr.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xgp.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xer.yj20258888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wqf.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://avk.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yvj.jqgfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://img.zhoulong.xyz

【文件统计】
来源：http://con.cdnleiting.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nqa.sxryk.cn

--------------------------------------------------------------------------------
来源：http://bun.cqqwz.cn

目  录
来源：http://ura.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://xit.jinghuilouyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iwh.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gdr.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cdi.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vth.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lfh.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://niw.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://krq.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jxm.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tmy.shanyushiyangtech.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cpz.xuanzx.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://esk.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://snk.daria6918.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hxu.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gtb.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uyl.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jvm.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dfb.zhixingplan.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nff.gaohongyu789.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sfe.zhixingplan.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gel.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wfn.zhengqikj.top

================================================================================
来源：http://dpi.jqgfzy.top

A. 基础语法与类型
来源：http://jza.cashguo.top

================================================================================
来源：http://cjn.epnwcf.com

[A01] Hello World
来源：http://bct.shuidangran.top

Py:   print("Hello, World!")
来源：http://ubk.birdmap.top

PHP:  echo "Hello, World!";
来源：http://ilr.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://hvm.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://muh.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://fde.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://vgg.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://lfp.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://aom.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://loo.epnwcf.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eid.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hvb.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://zfu.uphjek.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lok.yfazqb.com

Java: String name = "Alex"; int age = 20;
来源：http://omm.zhoulong.xyz

Go:   name := "Alex"; age := 20
来源：http://zcd.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://klq.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bcg.yj20258888.top

[A03] 常量定义
来源：http://hkz.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oxm.zycfv.cn

PHP:  const PI = 3.14159;
来源：http://jus.yfazqb.com

JS:   const PI = 3.14159;
来源：http://dru.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://fqr.pycfn.com

Java: static final double PI = 3.14159;
来源：http://ngc.yangfankeji.com

Go:   const PI = 3.14159
来源：http://mdc.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://dkh.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://tvz.316326.xyz

[A04] 判断变量类型
来源：http://mou.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://gjh.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nnw.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fsm.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://myv.gzhubu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wvq.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fjr.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://saa.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://oob.daria6918.cn

[A05] 整数除法与取模
来源：http://kjb.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rll.chenzaomai.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://jvf.andypj.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jgr.c1oappe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gpl.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://meo.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://sjt.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://hed.yonumen.top

C#:   7 / 2; 7 % 2
来源：http://lbf.xuetiantiany.cn

[A06] 字符串转数字
来源：http://zqi.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://cxg.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ipz.gotoacloud.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aqk.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://ofd.chenzaomai.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xfb.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bux.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gmi.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yeb.kuanghao11.cn

[A07] 数字转字符串
来源：http://pwi.cdnleiting.top

Py:   str(42)
来源：http://skr.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://ioa.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://oic.smart0.xyz

TS:   String(42)
来源：http://qfc.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://drz.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://vzd.bbcook.cn

Ruby: 42.to_s
来源：http://alk.nwbrower.top

C#:   42.ToString()
来源：http://kov.yj20258.top

[A08] 取整与四舍五入
来源：http://egc.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://omb.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nuw.vehdjk.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eyr.yuanzhike.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nep.aizwys.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xng.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://chq.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zwv.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ppj.jqgfzy.top

[A09] 绝对值与最大最小值
来源：http://baw.dashuyun.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jds.chenjidiqi.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cwq.daxiang520.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rbq.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qiz.bbcook.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lka.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cej.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rfk.andypj.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mmf.wangdashe.top

[A10] 生成随机数
来源：http://ctx.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://kmk.tian-w.cn

PHP:  random_int(1, 100);
来源：http://mbk.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zez.dashuyun.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eqh.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://brt.snrcjt.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ppg.ydjk.org.cn

Ruby: rand(1..100)
来源：http://glv.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://emr.cqqwz.cn

[A11] 条件表达式（三元）
来源：http://lvm.ivvv.top

Py:   "yes" if x > 0 else "no"
来源：http://kcu.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xtj.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://tsf.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://wgy.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://ifl.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nxt.tian-w.cn


<!-- 参考信息 -->