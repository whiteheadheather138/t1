代发 wailian999

[U71] PHP：抛出异常
来源：http://lgi.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://pob.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://zyr.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://clu.xylfe.cn

[U73] PHP：读取 ini 配置
来源：http://aav.c1oappe.top

parse_ini_file("config.ini", true)
来源：http://dst.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://wza.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://cxy.hnqzz.top

[U75] PHP：依赖注入
来源：http://wou.gotoacloud.top

composer require psr/container
来源：http://riq.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://sgq.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xpn.gogol.net.cn

[U77] PHP：模板渲染
来源：http://lsc.zhaomingkeji.xyz

composer require twig/twig
来源：http://eei.kuanghao11.cn

[U78] PHP：单元测试
来源：http://kyq.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://rrc.zdqjudy.top

[U79] PHP：静态分析
来源：http://fhm.yj202588.top

composer require --dev phpstan/phpstan
来源：http://iiw.tarul.cn

[U80] PHP：代码规范修复
来源：http://fkq.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zvd.xuanzx.com

[U81] JS：初始化项目
来源：http://bgj.iojbl.cn

npm init -y;  npm i express
来源：http://fvw.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://ktp.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ime.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://xfg.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://ddj.ivvv.top

[U84] JS：CommonJS 写法
来源：http://xte.52xcode.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vbk.xylfe.cn

[U85] JS：可选链
来源：http://geh.zycfv.cn

a?.b?.c
来源：http://cig.feifeiyinyue.top

[U86] JS：空值合并
来源：http://agf.zhiwuduotai.top

a ?? b
来源：http://hly.gaohongyu789.top

[U87] JS：解构默认值
来源：http://vvv.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://mmp.zdbjq.cn

[U88] JS：对象展开合并
来源：http://nbm.shzxlz.cn

{ ...a, ...b }
来源：http://zbn.52xcode.cn

[U89] JS：数组去重
来源：http://neo.hammf.cn

[...new Set(arr)]
来源：http://bfj.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://cse.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://cop.birdmap.top

[U91] JS：对象键值遍历
来源：http://yut.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nbn.cqqwz.cn

[U92] JS：深拷贝
来源：http://rpl.zhengqikj.top

structuredClone(obj)
来源：http://smr.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://dsg.yanxiufei.cn

`共 ${n} 条`
来源：http://olp.jianghu66.top

[U94] JS：箭头函数
来源：http://jki.yongpay.top

const double = x => x * 2;
来源：http://cxt.haohaochexian.top

[U95] JS：Promise 包装
来源：http://iyq.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://mrj.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://hxq.yuanzhike.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xlu.xuetiantiany.cn

[U97] JS：并发请求
来源：http://yjp.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://one.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://btz.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jmw.chenjidiqi.icu

[U99] JS：事件监听
来源：http://kne.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://vgw.svipenyu.cn

[U100] JS：DOM 查询
来源：http://owa.pengpengdd.cyou

document.querySelector(".item")
来源：http://orz.jianghu66.top

[U101] JS：classList 操作
来源：http://nch.yueranfly.top

el.classList.toggle("active")
来源：http://axu.hongshengwenyu.top

[U102] JS：本地存储
来源：http://gte.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ipq.andypj.xyz

[U103] JS：定时器
来源：http://dqk.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://scr.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://ici.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://scu.shuidangran.top

[U105] JS：节流
来源：http://lon.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trf.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://qml.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rjg.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://hzk.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://onh.ydzc1.top

[U108] JS：随机整数
来源：http://tvd.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ywx.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://njy.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://mus.nwbrower.top

[U110] JS：数组分块
来源：http://edr.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ahk.daria6918.cn

[U111] JS：对象转 Map
来源：http://gsf.cashguo.top

new Map(Object.entries(obj))
来源：http://zdw.xinyue.icu

[U112] JS：字符串补位
来源：http://cff.hesvh.cn

"7".padStart(3, "0")
来源：http://gxp.sufxvd.cn

[U113] JS：正则替换全部
来源：http://niz.yangfankeji.com

s.replaceAll("a", "b")
来源：http://gxc.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://ucy.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mge.tianlin.xyz

[U115] JS：生成 UUID
来源：http://fxa.vehdjk.com

crypto.randomUUID()
来源：http://hib.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://cae.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://aho.jianghu66.top

[U117] JS：单元测试
来源：http://mdu.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://yrt.9152youxi.cn

[U118] JS：开发服务器
来源：http://imo.vehdjk.com

npm i -D vite;  npx vite
来源：http://wrw.jiagoushi.top

[U119] JS：生产构建
来源：http://gxk.cashguo.top

npx vite build
来源：http://ucv.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://wma.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://ifh.nanxuanxn.top

================================================================================
来源：http://qei.vqdsnc.cn

统计汇总
来源：http://rvs.hongshengwenyu.top

================================================================================
来源：http://uxu.xuanzx.com

按语言统计（条）：
来源：http://zyr.hongshengwenyu.top

Python ......... 252
来源：http://auq.9152youxi.cn

PHP ............ 252
来源：http://mwn.uphjek.com

JavaScript ..... 252
来源：http://rdz.yvedp.cn

TypeScript ..... 212
来源：http://ttt.jinyuanbaomall.cn

Java ........... 212
来源：http://twx.shuidangran.top

Go ............. 212
来源：http://gmo.hywenlv.cn

Ruby ........... 212
来源：http://mgk.guowangkeji.top

C# ............. 212
来源：http://dym.yj202588.top

C .............. 30
来源：http://yzo.yuanzhike.top

C++ ............ 30
来源：http://trt.hnqzz.top

SQL ............ 90
来源：http://moz.0kj1m.cn

Bash ........... 80
来源：http://lfe.sufxvd.cn

Kotlin ......... 15
来源：http://fnw.yj20258.top

Swift .......... 15
来源：http://hvt.gzhubu.top

Lua ............ 10
来源：http://fmb.cheryme.top

Perl ........... 10
来源：http://uet.hongshengwenyu.top

Scala .......... 10
来源：http://wog.zdqjudy.top

------------------------------------
来源：http://ler.jiagoushi.top

合计 ........... 2106 条
来源：http://vyc.zycfv.cn

按章节统计：
来源：http://jth.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cwy.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dwj.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://afo.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iup.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xhq.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://atp.daxiang520.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jzd.hongshengwenyu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ubk.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ofs.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mrp.sxryk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wqc.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://omm.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nuc.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tsu.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dlc.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ijw.pengpengdd.cyou

Q SQL 专题                              90
来源：http://wxp.jyoumei.cn

R Bash 专题                             80
来源：http://qiz.tianlin.xyz

S C / C++ 专题                          60
来源：http://niy.yj202588.top

T 其他语言补充                          60
来源：http://okf.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://xxv.xuetiantiany.cn

------------------------------------
来源：http://obp.shanyushiyangtech.top

合计                                  2106 条
来源：http://gfm.ydzc1.top

--------------------------------------------------------------------------------
来源：http://ile.fzhhl.top

使用提醒
来源：http://tug.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://ymz.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wfn.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vqi.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vzk.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vzm.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sas.ctjpmb.com

—— 文件结束 ——
来源：http://jvz.chenjidiqi.icu

================================================================================
来源：http://zai.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ssx.yvedp.cn

Common Programming Examples Cheat Book
来源：http://fnb.jyoumei.cn

================================================================================
来源：http://sxx.shanyushiyangkeji.top

【收录内容】
来源：http://lbs.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ema.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aed.iojbl.cn

SQL · Bash · C · C++
来源：http://xar.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jxy.gzhubu.top

【使用说明】
来源：http://ufv.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rrf.yongpay.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xsc.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tev.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ltx.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://hua.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://epl.zhixingplan.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qxo.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jaf.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qoy.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xzs.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wbt.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://euy.shanyushiyangtech.top

【文件统计】
来源：http://nzj.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wjm.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://krj.yongpay.top

目  录
来源：http://jma.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://tas.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ooa.cheryme.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gkc.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ucu.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yor.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vtf.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tun.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wia.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://adh.ivvv.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://shw.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xlp.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://scf.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://viw.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oxd.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zts.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ony.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ryb.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rdi.tanke756.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lwy.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cuz.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xmy.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cdb.aibaodan.cn

================================================================================
来源：http://tlt.havefunace.top

A. 基础语法与类型
来源：http://nrc.hysaishi.cn

================================================================================
来源：http://pfo.sweek.top

[A01] Hello World
来源：http://idw.gzhubu.top

Py:   print("Hello, World!")
来源：http://tfo.cashguo.top

PHP:  echo "Hello, World!";
来源：http://xao.haohaochexian.top

JS:   console.log("Hello, World!");
来源：http://ufx.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ohp.guannengcc.top

Java: System.out.println("Hello, World!");
来源：http://ldx.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://aft.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://gvs.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://dvv.jinqigufen.top

[A02] 变量声明与赋值
来源：http://voz.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://snd.sjlbkw.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sel.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://ycg.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xuj.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://pnl.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://nlk.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://loi.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://xqr.daxiang520.top

[A03] 常量定义
来源：http://sdf.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tom.shangyingyoupin.top

PHP:  const PI = 3.14159;
来源：http://jmi.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://flo.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://kjr.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://vhm.ehwqpu.com

Go:   const PI = 3.14159
来源：http://scq.svipenyu.cn

Ruby: PI = 3.14159
来源：http://hng.guowangkeji.top

C#:   const double PI = 3.14159;
来源：http://wlv.jinqigfzy.top

[A04] 判断变量类型
来源：http://cek.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lnq.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eou.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zko.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://bct.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://szj.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hio.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://nab.snrcjt.cn

C#:   x.GetType().Name; x is int
来源：http://sdm.c1oappe.top

[A05] 整数除法与取模
来源：http://bkz.zhijiandao.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jdz.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qrd.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kqh.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uqs.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://ewb.sxryk.cn

Go:   7 / 2; 7 % 2
来源：http://htx.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://msp.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://wyq.ydjk.org.cn

[A06] 字符串转数字
来源：http://oqg.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://emw.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wzi.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gmo.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://vgc.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qsv.havefunace.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hww.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qvb.xingfuxueyuan.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oub.ydzc1.top

[A07] 数字转字符串
来源：http://fsu.tian-w.cn

Py:   str(42)
来源：http://dif.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://jvv.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://xda.sweek.top

TS:   String(42)
来源：http://ahp.uphjek.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://rya.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://jpl.epnwcf.com

Ruby: 42.to_s
来源：http://qvs.bjfxy.top

C#:   42.ToString()
来源：http://jys.0kj1m.cn

[A08] 取整与四舍五入
来源：http://pkl.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uhr.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pdb.zycfv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://utx.wangshuangyany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cqa.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bpd.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pzf.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://weq.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wzu.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://omp.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ijm.zdbjq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dkz.haohaochexian.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lgg.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://trz.cdnleiting.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lmq.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sep.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qad.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wpi.0kj1m.cn

[A10] 生成随机数
来源：http://nwx.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://yau.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://aec.wangshuangyany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://keg.jianghu66.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tln.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://uds.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tzq.birdmap.top

Ruby: rand(1..100)
来源：http://sgp.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://gyn.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://okw.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://pyy.zdbjq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://orb.wangdashe.top


<!-- 参考信息 -->