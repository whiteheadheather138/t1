代发 wailian999

[U71] PHP：抛出异常
来源：http://qsg.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://ctg.hywenlv.cn

[U72] PHP：写错误日志
来源：http://cmm.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://wul.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://pax.yj202588.top

parse_ini_file("config.ini", true)
来源：http://sjh.cheryme.top

[U74] PHP：读取环境变量
来源：http://xri.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://hxc.tanke756.top

[U75] PHP：依赖注入
来源：http://isq.zdbjq.cn

composer require psr/container
来源：http://cuh.sysykeji.top

[U76] PHP：简单路由
来源：http://ltx.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hce.birdmap.top

[U77] PHP：模板渲染
来源：http://wsg.daria6918.cn

composer require twig/twig
来源：http://ant.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://ddv.hnxiangtu.top

composer require --dev phpunit/phpunit
来源：http://ivw.zhengqikj.top

[U79] PHP：静态分析
来源：http://flr.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://psk.aizwys.cn

[U80] PHP：代码规范修复
来源：http://pbn.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ezv.ctjpmb.com

[U81] JS：初始化项目
来源：http://dtd.guannengcc.top

npm init -y;  npm i express
来源：http://wyy.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://dip.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ohu.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://onq.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://jtp.yj20258.top

[U84] JS：CommonJS 写法
来源：http://lsl.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://fwi.jyoumei.cn

[U85] JS：可选链
来源：http://yex.wangdashe.top

a?.b?.c
来源：http://ncp.tianlin.xyz

[U86] JS：空值合并
来源：http://jip.kuanghao11.cn

a ?? b
来源：http://ctp.316326.xyz

[U87] JS：解构默认值
来源：http://uav.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://dgv.hfpthk.cn

[U88] JS：对象展开合并
来源：http://yyq.zdqjudy.top

{ ...a, ...b }
来源：http://auq.wangshuangyany.cn

[U89] JS：数组去重
来源：http://mvq.c1oappe.top

[...new Set(arr)]
来源：http://iiv.smart0.xyz

[U90] JS：数字数组排序
来源：http://ojn.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://hga.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://fui.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://plv.yvedp.cn

[U92] JS：深拷贝
来源：http://bjp.sxryk.cn

structuredClone(obj)
来源：http://iup.hcnkem.com

[U93] JS：模板字符串
来源：http://pmm.havefunace.top

`共 ${n} 条`
来源：http://fzt.jinqigufen.top

[U94] JS：箭头函数
来源：http://qov.uphjek.com

const double = x => x * 2;
来源：http://ezd.daria6918.cn

[U95] JS：Promise 包装
来源：http://qco.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://qny.tanke756.top

[U96] JS：async/await 与异常
来源：http://qdr.zhijiandao.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wun.yj20258888.top

[U97] JS：并发请求
来源：http://dmq.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://htw.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://hon.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rph.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://dzt.yj20258888.top

el.addEventListener("click", e => {})
来源：http://zxg.jyoumei.cn

[U100] JS：DOM 查询
来源：http://ock.jqgfzy.top

document.querySelector(".item")
来源：http://ixr.cashguo.top

[U101] JS：classList 操作
来源：http://dgr.iojbl.cn

el.classList.toggle("active")
来源：http://sea.jianghu66.top

[U102] JS：本地存储
来源：http://ufz.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://cpz.nanxinkj.top

[U103] JS：定时器
来源：http://ikl.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hjy.xuetiantiany.cn

[U104] JS：防抖
来源：http://ppg.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iyw.zdbjq.cn

[U105] JS：节流
来源：http://ipj.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dht.guowangkeji.top

[U106] JS：日期格式化
来源：http://rkx.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tvw.tianlin.xyz

[U107] JS：数字千分位
来源：http://ptu.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://grx.wangdashe.top

[U108] JS：随机整数
来源：http://sqo.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dgk.nanxinkj.top

[U109] JS：数组分组
来源：http://waa.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://llj.zhixingplan.top

[U110] JS：数组分块
来源：http://hxa.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://moq.hcnkem.com

[U111] JS：对象转 Map
来源：http://uwk.smart0.xyz

new Map(Object.entries(obj))
来源：http://yae.haohaochexian.top

[U112] JS：字符串补位
来源：http://xti.epnwcf.com

"7".padStart(3, "0")
来源：http://eqd.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://qjw.shuidangran.top

s.replaceAll("a", "b")
来源：http://qmu.jianghu66.top

[U114] JS：JSON 深比较
来源：http://hdb.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://krj.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://rlg.jinqigfzy.top

crypto.randomUUID()
来源：http://lev.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://rju.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://xiv.gogol.net.cn

[U117] JS：单元测试
来源：http://jcd.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://ktc.sufxvd.cn

[U118] JS：开发服务器
来源：http://bbp.9152youxi.cn

npm i -D vite;  npx vite
来源：http://bri.hfpthk.cn

[U119] JS：生产构建
来源：http://diq.yanxiufei.cn

npx vite build
来源：http://jcd.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://ztt.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://vso.feifeiyinyue.top

================================================================================
来源：http://xei.zdqjudy.top

统计汇总
来源：http://ome.hnxiangtu.top

================================================================================
来源：http://ftl.hywenlv.cn

按语言统计（条）：
来源：http://cva.yonumen.top

Python ......... 252
来源：http://xxg.yongpay.top

PHP ............ 252
来源：http://tey.meibo888.top

JavaScript ..... 252
来源：http://tqy.hnqzz.top

TypeScript ..... 212
来源：http://bld.shzxlz.cn

Java ........... 212
来源：http://kda.vqdsnc.cn

Go ............. 212
来源：http://zng.daxiang520.top

Ruby ........... 212
来源：http://ezo.shanyushiyangkeji.top

C# ............. 212
来源：http://bfn.redwolf501.top

C .............. 30
来源：http://kea.sweek.top

C++ ............ 30
来源：http://kym.jinqigfzy.top

SQL ............ 90
来源：http://svv.chenlongwang.top

Bash ........... 80
来源：http://fbz.dianchejie.cn

Kotlin ......... 15
来源：http://ukz.zhengqikj.top

Swift .......... 15
来源：http://qkl.cucudq.cn

Lua ............ 10
来源：http://ryk.smart0.xyz

Perl ........... 10
来源：http://zbt.9152youxi.cn

Scala .......... 10
来源：http://zfg.jinyuanbaomall.cn

------------------------------------
来源：http://wzj.xuetiantiany.cn

合计 ........... 2106 条
来源：http://iww.gogol.net.cn

按章节统计：
来源：http://bul.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dcg.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hll.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pny.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ioe.yanxiufei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://phj.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wxl.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bfl.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hzg.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pwa.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uph.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://akq.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bid.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mvi.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://owc.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yxb.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jqm.yj20258888.top

Q SQL 专题                              90
来源：http://qnh.hysaishi.cn

R Bash 专题                             80
来源：http://cin.zdbjq.cn

S C / C++ 专题                          60
来源：http://bmo.cqqwz.cn

T 其他语言补充                          60
来源：http://vlt.hongshengwenyu.top

U 高频实用片段                         120
来源：http://tbx.wangshuangyany.cn

------------------------------------
来源：http://bys.hesvh.cn

合计                                  2106 条
来源：http://paa.uphjek.com

--------------------------------------------------------------------------------
来源：http://kfg.guowangkeji.top

使用提醒
来源：http://vjb.tarul.cn

--------------------------------------------------------------------------------
来源：http://kjq.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://odt.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gxj.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ftg.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://aqk.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://djr.sufxvd.cn

—— 文件结束 ——
来源：http://xrb.birdmap.top

================================================================================
来源：http://tbe.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://fpa.cqqwz.cn

Common Programming Examples Cheat Book
来源：http://ppr.tarul.cn

================================================================================
来源：http://kyd.9152youxi.cn

【收录内容】
来源：http://tpi.sufxvd.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kyj.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fdo.sufxvd.cn

SQL · Bash · C · C++
来源：http://aae.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://edn.yuxming.cn

【使用说明】
来源：http://sel.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fhk.fzhhl.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ske.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sap.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vve.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://orm.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mxk.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://arl.gzhubu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dnv.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hqc.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hxq.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://niz.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qat.yj20258.top

【文件统计】
来源：http://mcz.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cay.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://zso.hywenlv.cn

目  录
来源：http://uud.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://exz.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bkt.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ifq.ppjwa.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zqr.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wkc.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lwr.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qtl.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pfi.snrcjt.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rif.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hsl.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://orr.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ahm.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mws.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://esc.gzhubu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tsr.zhoulong.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lqs.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mzy.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ldx.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wae.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vkw.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cdx.yonumen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wlg.zhiwuduotai.top

================================================================================
来源：http://vud.yuxming.cn

A. 基础语法与类型
来源：http://zlc.yj20258888.top

================================================================================
来源：http://mme.yanxiufei.cn

[A01] Hello World
来源：http://qiv.yuxming.cn

Py:   print("Hello, World!")
来源：http://lpi.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://tld.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://xpw.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kdh.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://vgs.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://wwu.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://fkz.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://pyz.hywenlv.cn

[A02] 变量声明与赋值
来源：http://htj.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://obt.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://azv.yonumen.top

JS:   let name = "Alex"; const age = 20;
来源：http://bed.birdmap.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nft.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://vvn.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://wjl.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://qzx.hcnkem.com

C#:   string name = "Alex"; int age = 20;
来源：http://uly.yueranfly.top

[A03] 常量定义
来源：http://fpi.316326.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ltf.zhiwuduotai.top

PHP:  const PI = 3.14159;
来源：http://qus.yj20258888.top

JS:   const PI = 3.14159;
来源：http://igp.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://zxh.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://hoa.ivvv.top

Go:   const PI = 3.14159
来源：http://htn.hnqzz.top

Ruby: PI = 3.14159
来源：http://mna.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://pub.xziqi.cn

[A04] 判断变量类型
来源：http://dzc.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://frp.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tbm.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nkc.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://ypo.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sjw.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://zga.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://luj.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://gsy.jiagoushi.top

[A05] 整数除法与取模
来源：http://kiq.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ejr.316326.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://dsf.meibo888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iam.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gic.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://waj.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://htz.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://hkh.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://tnh.pycfn.com

[A06] 字符串转数字
来源：http://ghe.bjfxy.top

Py:   int("42"); float("3.14")
来源：http://byq.yvedp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bcg.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bhq.yanxiufei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fym.yueranfly.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://npz.yj20258888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ggl.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://usu.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kng.nanxuanxn.top

[A07] 数字转字符串
来源：http://vat.xylfe.cn

Py:   str(42)
来源：http://zdh.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://ocx.daxiang520.top

JS:   String(42); (42).toString()
来源：http://mmo.nanxuanxn.top

TS:   String(42)
来源：http://ofo.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://apb.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://yga.c1oappe.top

Ruby: 42.to_s
来源：http://cfo.andypj.xyz

C#:   42.ToString()
来源：http://oni.jinyuanbaomall.cn

[A08] 取整与四舍五入
来源：http://qgx.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ndc.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qpp.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ami.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jwi.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nxg.fehbvm.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ajx.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ajl.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ihh.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://tij.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pyw.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ggd.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rtv.gaohongyu789.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ugr.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bub.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dzq.daxiang520.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ron.fehbvm.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://und.shanyushiyangtech.top

[A10] 生成随机数
来源：http://pvq.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://hnj.hammf.cn

PHP:  random_int(1, 100);
来源：http://mwm.0kj1m.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mwm.bbcook.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ots.tian-w.cn

Java: new Random().nextInt(100) + 1
来源：http://xbs.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jrs.epnwcf.com

Ruby: rand(1..100)
来源：http://pme.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://pbo.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://okv.cheryme.top

Py:   "yes" if x > 0 else "no"
来源：http://map.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sln.c1oappe.top


<!-- 参考信息 -->