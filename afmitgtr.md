代发 wailian999

[U71] PHP：抛出异常
来源：http://ogo.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://fxm.yueranfly.top

[U72] PHP：写错误日志
来源：http://gar.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://wcf.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://qkk.yj20258.top

parse_ini_file("config.ini", true)
来源：http://wjp.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://hnr.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://inu.aibaodan.cn

[U75] PHP：依赖注入
来源：http://xgy.bbcook.cn

composer require psr/container
来源：http://ogy.bbcook.cn

[U76] PHP：简单路由
来源：http://pti.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gbl.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://tcf.ctjpmb.com

composer require twig/twig
来源：http://ljd.havefunace.top

[U78] PHP：单元测试
来源：http://rbc.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://rrt.jqgfzy.top

[U79] PHP：静态分析
来源：http://sep.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://dlc.yj202588.top

[U80] PHP：代码规范修复
来源：http://rvg.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ibz.hcnkem.com

[U81] JS：初始化项目
来源：http://wme.dashuyun.cn

npm init -y;  npm i express
来源：http://blt.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://yqm.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uid.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://gfy.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://gtk.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://qyb.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rxx.zycfv.cn

[U85] JS：可选链
来源：http://noh.jiagoushi.top

a?.b?.c
来源：http://ixl.pengpengdd.cyou

[U86] JS：空值合并
来源：http://ijm.iojbl.cn

a ?? b
来源：http://rkz.havefunace.top

[U87] JS：解构默认值
来源：http://scx.vqdsnc.cn

const { a = 1, b = 2 } = obj;
来源：http://byb.smart0.xyz

[U88] JS：对象展开合并
来源：http://pbz.yonumen.top

{ ...a, ...b }
来源：http://mjg.bbcook.cn

[U89] JS：数组去重
来源：http://xao.ctjpmb.com

[...new Set(arr)]
来源：http://ndd.chenzaomai.com

[U90] JS：数字数组排序
来源：http://vxx.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://xzg.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://lvx.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wvt.xuetiantiany.cn

[U92] JS：深拷贝
来源：http://pol.guannengcc.top

structuredClone(obj)
来源：http://kim.snrcjt.cn

[U93] JS：模板字符串
来源：http://ngw.bbcook.cn

`共 ${n} 条`
来源：http://wwl.cucudq.cn

[U94] JS：箭头函数
来源：http://ttq.cheryme.top

const double = x => x * 2;
来源：http://tdo.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://koj.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://zlc.hesvh.cn

[U96] JS：async/await 与异常
来源：http://ipd.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bay.zycfv.cn

[U97] JS：并发请求
来源：http://lnh.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wzw.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://jfa.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mqc.hywenlv.cn

[U99] JS：事件监听
来源：http://cmr.yj20258.top

el.addEventListener("click", e => {})
来源：http://mjk.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://cge.cashguo.top

document.querySelector(".item")
来源：http://tda.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://pnr.jyoumei.cn

el.classList.toggle("active")
来源：http://srw.zycfv.cn

[U102] JS：本地存储
来源：http://vfs.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tbb.birdmap.top

[U103] JS：定时器
来源：http://uul.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nht.jlsjyb.cn

[U104] JS：防抖
来源：http://wnx.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://scw.jinghuilouyu.cn

[U105] JS：节流
来源：http://nyg.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bgk.yonumen.top

[U106] JS：日期格式化
来源：http://kkq.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hsh.jinqigfzy.top

[U107] JS：数字千分位
来源：http://sgy.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zuz.tarul.cn

[U108] JS：随机整数
来源：http://vvo.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uts.yangfankeji.com

[U109] JS：数组分组
来源：http://chf.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://rkp.kuanghao11.cn

[U110] JS：数组分块
来源：http://hef.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uyn.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://rmr.yueranfly.top

new Map(Object.entries(obj))
来源：http://slm.xuanzx.com

[U112] JS：字符串补位
来源：http://sar.sufxvd.cn

"7".padStart(3, "0")
来源：http://jpq.gzhubu.top

[U113] JS：正则替换全部
来源：http://buf.hnqzz.top

s.replaceAll("a", "b")
来源：http://nky.andypj.xyz

[U114] JS：JSON 深比较
来源：http://caq.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lbo.svipenyu.cn

[U115] JS：生成 UUID
来源：http://rze.gotoacloud.top

crypto.randomUUID()
来源：http://rvk.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://oup.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://nnp.andypj.xyz

[U117] JS：单元测试
来源：http://vpv.316326.xyz

npm i -D vitest;  npx vitest
来源：http://gtq.ctjpmb.com

[U118] JS：开发服务器
来源：http://nlc.yuanzhike.top

npm i -D vite;  npx vite
来源：http://etr.xylfe.cn

[U119] JS：生产构建
来源：http://jfh.ehwqpu.com

npx vite build
来源：http://cme.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://ysf.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://jzc.gogol.net.cn

================================================================================
来源：http://nwx.zhongyouzk.top

统计汇总
来源：http://drx.havefunace.top

================================================================================
来源：http://zij.aizwys.cn

按语言统计（条）：
来源：http://gmh.nanxinkj.top

Python ......... 252
来源：http://qnm.yonumen.top

PHP ............ 252
来源：http://ovq.fengsongda.top

JavaScript ..... 252
来源：http://nhf.cashguo.top

TypeScript ..... 212
来源：http://isr.jqgufenzy.top

Java ........... 212
来源：http://atp.zdqjudy.top

Go ............. 212
来源：http://sxt.epnwcf.com

Ruby ........... 212
来源：http://scc.tarul.cn

C# ............. 212
来源：http://ggi.zhixingplan.top

C .............. 30
来源：http://lky.shanyushiyangkeji.top

C++ ............ 30
来源：http://hgv.andypj.xyz

SQL ............ 90
来源：http://dyx.tanke756.top

Bash ........... 80
来源：http://ojo.shanyushiyangtech.top

Kotlin ......... 15
来源：http://gmh.tian-w.cn

Swift .......... 15
来源：http://pjs.hfpthk.cn

Lua ............ 10
来源：http://kzk.yuanzhike.top

Perl ........... 10
来源：http://cmh.wangshuangyany.cn

Scala .......... 10
来源：http://gpw.wangshuangyany.cn

------------------------------------
来源：http://upf.hongshengwenyu.top

合计 ........... 2106 条
来源：http://wol.redwolf501.top

按章节统计：
来源：http://olq.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qyx.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bjo.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zvd.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tuc.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cbn.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pfa.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://atz.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xhr.pengpengdd.cyou

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wge.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hoi.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qup.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uwn.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zkv.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cwn.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yee.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://epl.yj20258888.top

Q SQL 专题                              90
来源：http://dkm.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://rus.yuxming.cn

S C / C++ 专题                          60
来源：http://cwe.shuidangran.top

T 其他语言补充                          60
来源：http://peb.tian-w.cn

U 高频实用片段                         120
来源：http://prf.gaohongyu789.top

------------------------------------
来源：http://uod.haohaochexian.top

合计                                  2106 条
来源：http://hqc.yongpay.top

--------------------------------------------------------------------------------
来源：http://mzj.ctjpmb.com

使用提醒
来源：http://dbp.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://vfh.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pms.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iae.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hoy.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bfi.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://awj.hongshengwenyu.top

—— 文件结束 ——
来源：http://fqm.ivvv.top

================================================================================
来源：http://bwm.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://sox.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://hep.zhengqikj.top

================================================================================
来源：http://lwt.shanyushiyangtech.top

【收录内容】
来源：http://brc.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://gml.52xcode.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rre.yongpay.top

SQL · Bash · C · C++
来源：http://bcl.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yfn.ehwqpu.com

【使用说明】
来源：http://scg.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yvv.quarkkingdee.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qnl.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oii.yvedp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rpm.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lrt.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://squ.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rgo.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jpr.hnxiangtu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ypk.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://osd.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eyk.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ivt.cqqwz.cn

【文件统计】
来源：http://tww.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://adi.sxryk.cn

--------------------------------------------------------------------------------
来源：http://dyq.jinqigfzy.top

目  录
来源：http://xey.andypj.xyz

--------------------------------------------------------------------------------
来源：http://zxb.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cxp.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://loa.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://efs.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wol.ppjwa.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rqd.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://seo.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iko.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdn.snrcjt.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rus.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://izo.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ohy.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hag.fktsv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://thw.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ebz.uphjek.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zby.yuanzhike.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yov.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://csd.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zjd.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://szs.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://emq.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kej.yvedp.cn

================================================================================
来源：http://zrg.chenzaomai.com

A. 基础语法与类型
来源：http://vgi.fanxiaobao.xyz

================================================================================
来源：http://zkb.tarul.cn

[A01] Hello World
来源：http://ama.zhengqikj.top

Py:   print("Hello, World!")
来源：http://svs.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://xcc.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://ram.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pdq.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://ftf.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://glj.tanke756.top

Ruby: puts "Hello, World!"
来源：http://wah.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iuu.cashguo.top

[A02] 变量声明与赋值
来源：http://yxx.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nge.sxryk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rog.jqgfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://bug.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xzg.xingfuxueyuan.xyz

Java: String name = "Alex"; int age = 20;
来源：http://lef.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://ncc.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://fxp.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xoh.fehbvm.com

[A03] 常量定义
来源：http://djs.ywan-chungtsiang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://snv.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://pks.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://gxz.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://oru.zhijiandao.cn

Java: static final double PI = 3.14159;
来源：http://tyz.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://reb.guannengcc.top

Ruby: PI = 3.14159
来源：http://yhf.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://duf.hesvh.cn

[A04] 判断变量类型
来源：http://rsf.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://pnu.zdqjudy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://alh.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mdj.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://vbj.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://egp.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://udl.snrcjt.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tqw.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://bqy.aibaodan.cn

[A05] 整数除法与取模
来源：http://ovx.zhaomingkeji.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wmb.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://icu.mhx1999.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cun.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gjq.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://quz.gaohongyu789.top

Go:   7 / 2; 7 % 2
来源：http://zfo.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://sed.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://rqm.smart0.xyz

[A06] 字符串转数字
来源：http://orb.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://xvj.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ueo.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://icp.cqqwz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gwb.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ibf.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zaz.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://aau.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dgu.shuidangran.top

[A07] 数字转字符串
来源：http://mnm.c1oappe.top

Py:   str(42)
来源：http://llg.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://xfs.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://nbd.redwolf501.top

TS:   String(42)
来源：http://mwf.jinqigufen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kit.jinqigfzy.top

Go:   strconv.Itoa(42)
来源：http://umn.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://fya.gzhubu.top

C#:   42.ToString()
来源：http://tmj.9152youxi.cn

[A08] 取整与四舍五入
来源：http://rpy.gotoacloud.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://czn.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vux.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zre.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ngf.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cwd.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mec.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://twj.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zid.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://imj.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wyc.hfpthk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://viz.zdqjudy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ylk.iojbl.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mvl.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qvy.wangdashe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ibn.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sal.zhijiandao.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://szj.dianchejie.cn

[A10] 生成随机数
来源：http://ajd.gogol.net.cn

Py:   import random; random.randint(1, 100)
来源：http://dye.xylfe.cn

PHP:  random_int(1, 100);
来源：http://vlp.jyoumei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xqa.pycfn.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xyh.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://fyw.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gbd.cqqwz.cn

Ruby: rand(1..100)
来源：http://lxc.zdqjudy.top

C#:   new Random().Next(1, 101)
来源：http://bly.yonumen.top

[A11] 条件表达式（三元）
来源：http://aai.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://vqt.cheryme.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://aww.yanxiufei.cn


<!-- 参考信息 -->