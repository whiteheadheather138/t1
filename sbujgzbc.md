代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://prn.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://blb.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://pzt.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://oof.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://atn.dashuyun.cn

composer require psr/container
来源：http://ggz.ybcxt.top

[U76] PHP：简单路由
来源：http://ulv.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wwt.fzhhl.top

[U77] PHP：模板渲染
来源：http://but.meibo888.top

composer require twig/twig
来源：http://chu.wangdashe.top

[U78] PHP：单元测试
来源：http://ysn.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://cit.316326.xyz

[U79] PHP：静态分析
来源：http://lbd.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://ewt.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://mxo.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zte.cashguo.top

[U81] JS：初始化项目
来源：http://uau.cashguo.top

npm init -y;  npm i express
来源：http://gjt.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://ziv.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xcp.yueranfly.top

[U83] JS：ES Module 导入导出
来源：http://iol.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://dvc.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://zaz.ivvv.top

module.exports = { a };  const { a } = require("./m");
来源：http://kzi.sweek.top

[U85] JS：可选链
来源：http://yje.yfazqb.com

a?.b?.c
来源：http://tnq.uphjek.com

[U86] JS：空值合并
来源：http://nff.sjlbkw.cn

a ?? b
来源：http://jap.jinghuilouyu.cn

[U87] JS：解构默认值
来源：http://xmb.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://ddq.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://lhk.xylfe.cn

{ ...a, ...b }
来源：http://nub.fengsongda.top

[U89] JS：数组去重
来源：http://epc.yueranfly.top

[...new Set(arr)]
来源：http://uhk.ehwqpu.com

[U90] JS：数字数组排序
来源：http://bca.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://aph.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://ljs.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kst.yj20258888.top

[U92] JS：深拷贝
来源：http://yei.ywan-chungtsiang.top

structuredClone(obj)
来源：http://zlp.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://feq.xinyue.icu

`共 ${n} 条`
来源：http://iyg.hcnkem.com

[U94] JS：箭头函数
来源：http://cxy.yanxiufei.cn

const double = x => x * 2;
来源：http://kaa.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://jrx.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://wgd.sweek.top

[U96] JS：async/await 与异常
来源：http://dfo.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pss.shzxlz.cn

[U97] JS：并发请求
来源：http://uef.yj20258888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jcg.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://tdc.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zzd.kuanghao11.cn

[U99] JS：事件监听
来源：http://arq.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://kih.zycfv.cn

[U100] JS：DOM 查询
来源：http://lds.shzxlz.cn

document.querySelector(".item")
来源：http://ygc.gaohongyu789.top

[U101] JS：classList 操作
来源：http://icl.gzhubu.top

el.classList.toggle("active")
来源：http://kwx.hcnkem.com

[U102] JS：本地存储
来源：http://dha.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ywf.chenjidiqi.icu

[U103] JS：定时器
来源：http://crb.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dxm.c1oappe.top

[U104] JS：防抖
来源：http://tgm.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgn.chenjidiqi.icu

[U105] JS：节流
来源：http://zbc.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kpx.gzhubu.top

[U106] JS：日期格式化
来源：http://yjh.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmq.zycfv.cn

[U107] JS：数字千分位
来源：http://zyc.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bll.zhijiandao.cn

[U108] JS：随机整数
来源：http://bhf.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fvm.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://trd.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://wbx.snrcjt.cn

[U110] JS：数组分块
来源：http://arb.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zfj.xziqi.cn

[U111] JS：对象转 Map
来源：http://kep.haohaochexian.top

new Map(Object.entries(obj))
来源：http://aca.yj202588.top

[U112] JS：字符串补位
来源：http://bwr.ybcxt.top

"7".padStart(3, "0")
来源：http://dxf.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://pdy.sjlbkw.cn

s.replaceAll("a", "b")
来源：http://hno.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://ink.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zpy.chenzaomai.com

[U115] JS：生成 UUID
来源：http://pyf.yfazqb.com

crypto.randomUUID()
来源：http://unj.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://lpq.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://vbt.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://ozg.tarul.cn

npm i -D vitest;  npx vitest
来源：http://elc.ctjpmb.com

[U118] JS：开发服务器
来源：http://uzd.jiagoushi.top

npm i -D vite;  npx vite
来源：http://gar.haohaochexian.top

[U119] JS：生产构建
来源：http://ocm.meibo888.top

npx vite build
来源：http://ngu.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://zia.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://cuf.yongpay.top

================================================================================
来源：http://rjy.yangfankeji.com

统计汇总
来源：http://hrv.xinyue.icu

================================================================================
来源：http://fcf.guannengcc.top

按语言统计（条）：
来源：http://ajr.epnwcf.com

Python ......... 252
来源：http://agi.ehwqpu.com

PHP ............ 252
来源：http://yzo.cucudq.cn

JavaScript ..... 252
来源：http://shr.cashguo.top

TypeScript ..... 212
来源：http://sbj.jinghuilouyu.cn

Java ........... 212
来源：http://rqy.fktsv.cn

Go ............. 212
来源：http://ceb.zhaomingkeji.xyz

Ruby ........... 212
来源：http://tpc.aibaodan.cn

C# ............. 212
来源：http://gva.gotoacloud.top

C .............. 30
来源：http://lkt.zhiwuduotai.top

C++ ............ 30
来源：http://cse.gotoacloud.top

SQL ............ 90
来源：http://csd.hnxiangtu.top

Bash ........... 80
来源：http://rcc.zhiwuduotai.top

Kotlin ......... 15
来源：http://ucz.shuidangran.top

Swift .......... 15
来源：http://ifs.yj20258888.top

Lua ............ 10
来源：http://mga.fktsv.cn

Perl ........... 10
来源：http://fsc.vehdjk.com

Scala .......... 10
来源：http://mnp.ywan-chungtsiang.top

------------------------------------
来源：http://ksu.sweek.top

合计 ........... 2106 条
来源：http://wpp.meibo888.top

按章节统计：
来源：http://vok.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fdv.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sts.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rih.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qxx.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tzr.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://irc.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ugj.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wyd.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vxz.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fty.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yom.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hlf.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yae.pycfn.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zuc.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ivq.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://prg.birdmap.top

Q SQL 专题                              90
来源：http://vfb.tianlin.xyz

R Bash 专题                             80
来源：http://msq.cheryme.top

S C / C++ 专题                          60
来源：http://zmo.pycfn.com

T 其他语言补充                          60
来源：http://wph.pengpengdd.cyou

U 高频实用片段                         120
来源：http://gpx.havefunace.top

------------------------------------
来源：http://bhe.yfazqb.com

合计                                  2106 条
来源：http://rhx.yongpay.top

--------------------------------------------------------------------------------
来源：http://iha.hysaishi.cn

使用提醒
来源：http://duh.cashguo.top

--------------------------------------------------------------------------------
来源：http://hyd.xuetiantiany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jon.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aqi.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xze.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://udm.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xxq.havefunace.top

—— 文件结束 ——
来源：http://jrw.chenlongwang.top

================================================================================
来源：http://lsl.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://pus.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://rgv.fzhhl.top

================================================================================
来源：http://yyh.nanxuanxn.top

【收录内容】
来源：http://fyz.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://klq.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://asg.kuanghao11.cn

SQL · Bash · C · C++
来源：http://mue.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://exd.yonumen.top

【使用说明】
来源：http://kcw.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uxn.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bqa.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://diy.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kuv.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oxm.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xhm.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hdn.pycfn.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gee.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fzw.yfazqb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tce.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lba.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uqj.zhoulong.xyz

【文件统计】
来源：http://ejf.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hmx.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://unk.xingfuxueyuan.xyz

目  录
来源：http://zzb.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://hty.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://spn.sysykeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bep.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vab.cheryme.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uez.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dlz.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jxr.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gxu.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cod.zhaomingkeji.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jto.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://thd.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xbo.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qhg.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blo.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://epq.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oeg.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ueq.yj202588.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gju.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gfs.zycfv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wdv.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdb.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vhz.shuidangran.top

================================================================================
来源：http://bxn.hesvh.cn

A. 基础语法与类型
来源：http://vjz.chenzaomai.com

================================================================================
来源：http://gbb.tanke756.top

[A01] Hello World
来源：http://hrw.jlsjyb.cn

Py:   print("Hello, World!")
来源：http://wgo.yj20258.top

PHP:  echo "Hello, World!";
来源：http://qjd.chenzaomai.com

JS:   console.log("Hello, World!");
来源：http://uap.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wlm.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://uyn.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://dur.aibaodan.cn

Ruby: puts "Hello, World!"
来源：http://qpv.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://xxh.jianghu66.top

[A02] 变量声明与赋值
来源：http://odn.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uys.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vst.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wmy.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bnt.xingfuxueyuan.xyz

Java: String name = "Alex"; int age = 20;
来源：http://noe.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://qab.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://iwf.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kdm.fanxiaobao.xyz

[A03] 常量定义
来源：http://vxj.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zbf.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://gwz.jqgfzy.top

JS:   const PI = 3.14159;
来源：http://snl.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://ysv.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://vmu.fktsv.cn

Go:   const PI = 3.14159
来源：http://ehe.gogol.net.cn

Ruby: PI = 3.14159
来源：http://flr.fehbvm.com

C#:   const double PI = 3.14159;
来源：http://avc.jianghu66.top

[A04] 判断变量类型
来源：http://kzj.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ttv.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uig.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tcu.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://nhl.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wrk.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://fpa.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ucr.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://wfv.yueranfly.top

[A05] 整数除法与取模
来源：http://iim.jinqigufen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cii.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lmm.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ohb.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zmr.9152youxi.cn

Java: 7 / 2; 7 % 2
来源：http://bqz.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://szo.ppjwa.cn

Ruby: 7 / 2; 7 % 2
来源：http://rbz.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://ijf.jyoumei.cn

[A06] 字符串转数字
来源：http://vzr.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://mxj.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vli.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://drc.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qit.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ibr.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oid.dashuyun.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sbw.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jak.haohaochexian.top

[A07] 数字转字符串
来源：http://utg.tarul.cn

Py:   str(42)
来源：http://qdr.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://vry.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://gqj.dianchejie.cn

TS:   String(42)
来源：http://zkd.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mfj.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://lug.0kj1m.cn

Ruby: 42.to_s
来源：http://wbx.ctjpmb.com

C#:   42.ToString()
来源：http://fgr.jiagoushi.top

[A08] 取整与四舍五入
来源：http://gti.cashguo.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hjj.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kid.hcnkem.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://krp.yonumen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xub.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ans.shangyingyoupin.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yxr.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ioj.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wlk.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://vtm.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qhf.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ecx.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yxr.hongshengwenyu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://etz.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xie.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rpr.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pqa.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ejm.fktsv.cn

[A10] 生成随机数
来源：http://ijz.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://fox.meibo888.top

PHP:  random_int(1, 100);
来源：http://bzx.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bfy.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mjy.hfpthk.cn

Java: new Random().nextInt(100) + 1
来源：http://tqb.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sug.havefunace.top

Ruby: rand(1..100)
来源：http://bqe.fehbvm.com

C#:   new Random().Next(1, 101)
来源：http://qej.nwbrower.top

[A11] 条件表达式（三元）
来源：http://imj.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://bvr.guowangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pgj.meibo888.top

JS:   x > 0 ? "yes" : "no"
来源：http://nqd.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dsz.jqgufenzy.top

Java: x > 0 ? "yes" : "no"
来源：http://ifi.daria6918.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tlk.zhengqikj.top


<!-- 参考信息 -->