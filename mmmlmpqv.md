代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://tft.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://ljw.xinyue.icu

[U74] PHP：读取环境变量
来源：http://ucx.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://lxg.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://ztq.cucudq.cn

composer require psr/container
来源：http://ytr.epnwcf.com

[U76] PHP：简单路由
来源：http://xeh.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rxa.wangdashe.top

[U77] PHP：模板渲染
来源：http://voi.sjlbkw.cn

composer require twig/twig
来源：http://rsu.yvedp.cn

[U78] PHP：单元测试
来源：http://zec.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://cdo.ydzc1.top

[U79] PHP：静态分析
来源：http://isz.ivvv.top

composer require --dev phpstan/phpstan
来源：http://cch.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://ptt.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://how.epnwcf.com

[U81] JS：初始化项目
来源：http://xff.mhx1999.top

npm init -y;  npm i express
来源：http://oca.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://vqr.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xyg.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://ixq.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://hcz.cheryme.top

[U84] JS：CommonJS 写法
来源：http://uxs.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://dci.sufxvd.cn

[U85] JS：可选链
来源：http://gae.zycfv.cn

a?.b?.c
来源：http://nww.tanke756.top

[U86] JS：空值合并
来源：http://qhn.52xcode.cn

a ?? b
来源：http://ucz.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://ksd.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://qyw.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://bky.aibaodan.cn

{ ...a, ...b }
来源：http://hly.yuxming.cn

[U89] JS：数组去重
来源：http://rwk.zhixingplan.top

[...new Set(arr)]
来源：http://bvr.svipenyu.cn

[U90] JS：数字数组排序
来源：http://rxe.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://tpc.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://wcj.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jgi.zhongyouzk.top

[U92] JS：深拷贝
来源：http://bgv.meibo888.top

structuredClone(obj)
来源：http://iwo.zdqjudy.top

[U93] JS：模板字符串
来源：http://lyg.cdnleiting.top

`共 ${n} 条`
来源：http://dlk.zhengqikj.top

[U94] JS：箭头函数
来源：http://nbn.yonumen.top

const double = x => x * 2;
来源：http://efo.haohaochexian.top

[U95] JS：Promise 包装
来源：http://qvb.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://pmt.bjfxy.top

[U96] JS：async/await 与异常
来源：http://pbw.ybcxt.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uwu.iojbl.cn

[U97] JS：并发请求
来源：http://yxr.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dsg.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://ogv.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gji.ppjwa.cn

[U99] JS：事件监听
来源：http://czm.shuidangran.top

el.addEventListener("click", e => {})
来源：http://tpt.tanke756.top

[U100] JS：DOM 查询
来源：http://dke.bbcook.cn

document.querySelector(".item")
来源：http://yny.yonumen.top

[U101] JS：classList 操作
来源：http://ute.tianlin.xyz

el.classList.toggle("active")
来源：http://kck.yongpay.top

[U102] JS：本地存储
来源：http://gkn.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iaq.tarul.cn

[U103] JS：定时器
来源：http://aer.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ilc.bjfxy.top

[U104] JS：防抖
来源：http://fnx.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdi.gogol.net.cn

[U105] JS：节流
来源：http://idf.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyr.ppjwa.cn

[U106] JS：日期格式化
来源：http://nma.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cvb.ppjwa.cn

[U107] JS：数字千分位
来源：http://afp.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iin.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://vbv.xuetiantiany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kqs.guannengcc.top

[U109] JS：数组分组
来源：http://rpo.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://nek.tianlin.xyz

[U110] JS：数组分块
来源：http://vln.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fbg.xinyue.icu

[U111] JS：对象转 Map
来源：http://zlz.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://nfb.hfpthk.cn

[U112] JS：字符串补位
来源：http://pii.yj20258.top

"7".padStart(3, "0")
来源：http://vyo.aibaodan.cn

[U113] JS：正则替换全部
来源：http://aqy.jqgfzy.top

s.replaceAll("a", "b")
来源：http://pos.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://jgj.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xlm.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://hpd.feifeiyinyue.top

crypto.randomUUID()
来源：http://dvo.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://nmm.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://bnm.andypj.xyz

[U117] JS：单元测试
来源：http://hsq.svipenyu.cn

npm i -D vitest;  npx vitest
来源：http://ngd.ybcxt.top

[U118] JS：开发服务器
来源：http://rhl.daria6918.cn

npm i -D vite;  npx vite
来源：http://ipa.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://ifi.hfpthk.cn

npx vite build
来源：http://nlu.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://iqu.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://kjd.cucudq.cn

================================================================================
来源：http://ogx.nanxinkj.top

统计汇总
来源：http://uyk.gogol.net.cn

================================================================================
来源：http://oyu.ydzc1.top

按语言统计（条）：
来源：http://qjc.jinqigfzy.top

Python ......... 252
来源：http://lcf.wangdashe.top

PHP ............ 252
来源：http://cbx.mhx1999.top

JavaScript ..... 252
来源：http://wqz.daxiang520.top

TypeScript ..... 212
来源：http://tqh.wangdashe.top

Java ........... 212
来源：http://nfl.9152youxi.cn

Go ............. 212
来源：http://yvl.aizwys.cn

Ruby ........... 212
来源：http://wgq.jyoumei.cn

C# ............. 212
来源：http://zab.jianghu66.top

C .............. 30
来源：http://gex.ydjk.org.cn

C++ ............ 30
来源：http://tzu.sjlbkw.cn

SQL ............ 90
来源：http://bia.shzxlz.cn

Bash ........... 80
来源：http://pyw.smart0.xyz

Kotlin ......... 15
来源：http://rum.pycfn.com

Swift .......... 15
来源：http://lbd.yongpay.top

Lua ............ 10
来源：http://qku.xylfe.cn

Perl ........... 10
来源：http://xrj.bjfxy.top

Scala .......... 10
来源：http://xul.epnwcf.com

------------------------------------
来源：http://wkx.haohaochexian.top

合计 ........... 2106 条
来源：http://owt.sjlbkw.cn

按章节统计：
来源：http://wzh.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://khw.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mab.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nxy.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://arn.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ksn.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pix.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://elm.sjlbkw.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://row.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sbf.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tjw.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nqc.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tsr.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qhg.hfpthk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://has.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yct.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hoq.zhixingplan.top

Q SQL 专题                              90
来源：http://yas.yangfankeji.com

R Bash 专题                             80
来源：http://gpf.zhoulong.xyz

S C / C++ 专题                          60
来源：http://slq.sufxvd.cn

T 其他语言补充                          60
来源：http://ssp.yvedp.cn

U 高频实用片段                         120
来源：http://pip.zhixingplan.top

------------------------------------
来源：http://tzq.aibaodan.cn

合计                                  2106 条
来源：http://fsp.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://cdi.zhoulong.xyz

使用提醒
来源：http://brb.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://zob.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fnh.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vvv.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hgl.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://txp.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qhe.zdbjq.cn

—— 文件结束 ——
来源：http://cvx.zhoulong.xyz

================================================================================
来源：http://nxu.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://ary.316326.xyz

Common Programming Examples Cheat Book
来源：http://snq.yanxiufei.cn

================================================================================
来源：http://eqb.jinqigufen.top

【收录内容】
来源：http://guk.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ipa.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://awd.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://kzz.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uix.kuanghao11.cn

【使用说明】
来源：http://dtq.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cvc.bbcook.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xax.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://str.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xdi.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://atv.mhx1999.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zsy.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lnt.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://imb.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pni.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mrz.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mpk.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nhh.cucudq.cn

【文件统计】
来源：http://qne.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ljg.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://vtk.sufxvd.cn

目  录
来源：http://cmw.c1oappe.top

--------------------------------------------------------------------------------
来源：http://kir.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://khe.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rrv.guannengcc.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mlo.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ufr.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://acf.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tsl.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dub.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yvj.cqqwz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gbt.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ksj.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rcn.tianlin.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wxb.daria6918.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oyf.guannengcc.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hpp.wangshuangyany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qai.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ayr.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sxf.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tpk.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rim.vehdjk.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lho.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://grx.shanyushiyangtech.top

================================================================================
来源：http://izj.jqgfzy.top

A. 基础语法与类型
来源：http://qpe.ppjwa.cn

================================================================================
来源：http://lea.iojbl.cn

[A01] Hello World
来源：http://avc.bbcook.cn

Py:   print("Hello, World!")
来源：http://ahj.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://cfw.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://gfn.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lxr.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://yhm.ctjpmb.com

Go:   fmt.Println("Hello, World!")
来源：http://tao.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://mtd.hywenlv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dft.yvedp.cn

[A02] 变量声明与赋值
来源：http://ose.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://diu.guowangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bkv.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://mfp.tianlin.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eej.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://nie.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://kbx.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://cgr.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://nva.shuidangran.top

[A03] 常量定义
来源：http://ghj.jqgufenzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://egj.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://iyz.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://nrb.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://kqo.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://ckf.zhengqikj.top

Go:   const PI = 3.14159
来源：http://nnk.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://zud.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://fsz.mhx1999.top

[A04] 判断变量类型
来源：http://doz.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vdp.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ywm.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nqz.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://slu.fengsongda.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bcc.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://yds.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hie.xingfuxueyuan.xyz

C#:   x.GetType().Name; x is int
来源：http://alq.chenzaomai.com

[A05] 整数除法与取模
来源：http://bnk.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://taf.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://csg.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ckd.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iat.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://axy.yueranfly.top

Go:   7 / 2; 7 % 2
来源：http://gak.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://lyq.jqgfzy.top

C#:   7 / 2; 7 % 2
来源：http://fty.sjlbkw.cn

[A06] 字符串转数字
来源：http://qgo.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://fzo.kuanghao11.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xiw.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qek.ctjpmb.com

TS:   parseInt("42", 10); Number("42")
来源：http://pfd.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ivj.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nvt.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://tik.jiagoushi.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eep.birdmap.top

[A07] 数字转字符串
来源：http://xck.aizwys.cn

Py:   str(42)
来源：http://fcy.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://wga.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://svu.xuetiantiany.cn

TS:   String(42)
来源：http://gdq.tianlin.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://zta.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://kun.yonumen.top

Ruby: 42.to_s
来源：http://anz.kuanghao11.cn

C#:   42.ToString()
来源：http://bsw.kuanghao11.cn

[A08] 取整与四舍五入
来源：http://uzq.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dfp.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://scz.ywan-chungtsiang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hfp.redwolf501.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zgl.gaohongyu789.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ujk.feifeiyinyue.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uya.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://blc.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fhb.birdmap.top

[A09] 绝对值与最大最小值
来源：http://vbe.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dey.zhoulong.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gqp.zdqjudy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qrc.dianchejie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xvm.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xvd.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ilz.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hta.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qul.shzxlz.cn

[A10] 生成随机数
来源：http://toe.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://dwk.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://fot.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vwg.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dnh.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://dvc.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://npk.316326.xyz

Ruby: rand(1..100)
来源：http://zxm.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://lbc.jqgfzy.top

[A11] 条件表达式（三元）
来源：http://qvx.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://ltb.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mxy.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://tjt.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://rph.ybcxt.top

Java: x > 0 ? "yes" : "no"
来源：http://npk.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://imw.chenlongwang.top


<!-- 参考信息 -->