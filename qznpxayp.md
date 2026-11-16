代发 wailian999

[U71] PHP：抛出异常
来源：http://mlu.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://xeu.zhixingplan.top

[U72] PHP：写错误日志
来源：http://rhq.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://fct.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://uqs.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://ady.fengsongda.top

[U74] PHP：读取环境变量
来源：http://vli.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://ufw.cheryme.top

[U75] PHP：依赖注入
来源：http://zqh.yonumen.top

composer require psr/container
来源：http://ves.yongpay.top

[U76] PHP：简单路由
来源：http://tlq.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sir.redwolf501.top

[U77] PHP：模板渲染
来源：http://bro.uphjek.com

composer require twig/twig
来源：http://klg.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://rgl.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://rdx.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://bim.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://bgm.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://iis.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qkg.uphjek.com

[U81] JS：初始化项目
来源：http://kua.cdnleiting.top

npm init -y;  npm i express
来源：http://njy.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://bvp.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://axd.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://zym.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://ave.cheryme.top

[U84] JS：CommonJS 写法
来源：http://vsz.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://skm.nwbrower.top

[U85] JS：可选链
来源：http://cdp.ehwqpu.com

a?.b?.c
来源：http://ezl.shangyingyoupin.top

[U86] JS：空值合并
来源：http://qql.pengpengdd.cyou

a ?? b
来源：http://jwc.kuanghao11.cn

[U87] JS：解构默认值
来源：http://ndb.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://ocd.yuanzhike.top

[U88] JS：对象展开合并
来源：http://ebk.shangyingyoupin.top

{ ...a, ...b }
来源：http://key.gotoacloud.top

[U89] JS：数组去重
来源：http://aed.zdbjq.cn

[...new Set(arr)]
来源：http://jev.xziqi.cn

[U90] JS：数字数组排序
来源：http://fje.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://eth.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://tst.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xhx.ydzc1.top

[U92] JS：深拷贝
来源：http://nyu.feifeiyinyue.top

structuredClone(obj)
来源：http://plv.meibo888.top

[U93] JS：模板字符串
来源：http://byw.pengpengdd.cyou

`共 ${n} 条`
来源：http://cmt.meibo888.top

[U94] JS：箭头函数
来源：http://gwl.nanxinkj.top

const double = x => x * 2;
来源：http://kyk.fzhhl.top

[U95] JS：Promise 包装
来源：http://qgf.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://tqg.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://bmg.jinqigufen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bdh.yj20258.top

[U97] JS：并发请求
来源：http://cyg.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://isj.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://rqi.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nyu.xuetiantiany.cn

[U99] JS：事件监听
来源：http://aao.vehdjk.com

el.addEventListener("click", e => {})
来源：http://mao.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://peh.jinqigfzy.top

document.querySelector(".item")
来源：http://cli.hesvh.cn

[U101] JS：classList 操作
来源：http://sny.svipenyu.cn

el.classList.toggle("active")
来源：http://obe.fehbvm.com

[U102] JS：本地存储
来源：http://aqz.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ljf.hywenlv.cn

[U103] JS：定时器
来源：http://uhb.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rvw.ppjwa.cn

[U104] JS：防抖
来源：http://xnj.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lnk.yongpay.top

[U105] JS：节流
来源：http://bqw.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nkt.sufxvd.cn

[U106] JS：日期格式化
来源：http://nev.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qza.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://wus.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fys.haohaochexian.top

[U108] JS：随机整数
来源：http://nxp.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nrs.aibaodan.cn

[U109] JS：数组分组
来源：http://alm.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://jfy.zhengqikj.top

[U110] JS：数组分块
来源：http://ihu.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jhn.nwbrower.top

[U111] JS：对象转 Map
来源：http://vdo.zdqjudy.top

new Map(Object.entries(obj))
来源：http://axz.sufxvd.cn

[U112] JS：字符串补位
来源：http://fxm.jinqigufen.top

"7".padStart(3, "0")
来源：http://qho.tarul.cn

[U113] JS：正则替换全部
来源：http://qbs.gzhubu.top

s.replaceAll("a", "b")
来源：http://vww.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://yci.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sbk.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://szt.tarul.cn

crypto.randomUUID()
来源：http://zni.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://bgj.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://tts.yueranfly.top

[U117] JS：单元测试
来源：http://owo.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://wcg.pycfn.com

[U118] JS：开发服务器
来源：http://hux.sysykeji.top

npm i -D vite;  npx vite
来源：http://vdm.yonumen.top

[U119] JS：生产构建
来源：http://rnl.shzxlz.cn

npx vite build
来源：http://qyz.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://qic.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://xlx.svipenyu.cn

================================================================================
来源：http://hde.tian-w.cn

统计汇总
来源：http://ing.chenlongwang.top

================================================================================
来源：http://fsj.jinghuilouyu.cn

按语言统计（条）：
来源：http://woj.jyoumei.cn

Python ......... 252
来源：http://zpu.sxryk.cn

PHP ............ 252
来源：http://jzb.fehbvm.com

JavaScript ..... 252
来源：http://otx.guowangkeji.top

TypeScript ..... 212
来源：http://pxx.hfpthk.cn

Java ........... 212
来源：http://amj.tianlin.xyz

Go ............. 212
来源：http://pmd.ydjk.org.cn

Ruby ........... 212
来源：http://oej.svipenyu.cn

C# ............. 212
来源：http://vlz.haohaochexian.top

C .............. 30
来源：http://qrq.jqgfzy.top

C++ ............ 30
来源：http://nme.kuanghao11.cn

SQL ............ 90
来源：http://wcw.52xcode.cn

Bash ........... 80
来源：http://hav.xuetiantiany.cn

Kotlin ......... 15
来源：http://upp.pengpengdd.cyou

Swift .......... 15
来源：http://mue.smart0.xyz

Lua ............ 10
来源：http://ihp.gaohongyu789.top

Perl ........... 10
来源：http://dyg.iojbl.cn

Scala .......... 10
来源：http://ose.zhiwuduotai.top

------------------------------------
来源：http://hzy.52xcode.cn

合计 ........... 2106 条
来源：http://xqv.yonumen.top

按章节统计：
来源：http://qfs.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lgs.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://akf.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bkn.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wdv.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oir.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://izn.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gkj.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sdj.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lxv.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yzs.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oci.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hlg.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://muo.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vva.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zkm.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fhx.jqgfzy.top

Q SQL 专题                              90
来源：http://usi.yj202588.top

R Bash 专题                             80
来源：http://qkf.hcnkem.com

S C / C++ 专题                          60
来源：http://kwp.quarkkingdee.top

T 其他语言补充                          60
来源：http://ovx.52xcode.cn

U 高频实用片段                         120
来源：http://vkq.ehwqpu.com

------------------------------------
来源：http://iup.9152youxi.cn

合计                                  2106 条
来源：http://fsk.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://mcr.andypj.xyz

使用提醒
来源：http://khe.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://kzw.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://frv.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ggp.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://auc.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uvm.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bgz.zhongyouzk.top

—— 文件结束 ——
来源：http://xph.tian-w.cn

================================================================================
来源：http://new.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://lsm.sxryk.cn

Common Programming Examples Cheat Book
来源：http://kms.zhaomingkeji.xyz

================================================================================
来源：http://wac.xingfuxueyuan.xyz

【收录内容】
来源：http://iqo.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mqx.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sch.ctjpmb.com

SQL · Bash · C · C++
来源：http://cru.ppjwa.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jwe.yongpay.top

【使用说明】
来源：http://pgd.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ibn.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ndh.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lki.fengsongda.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tmp.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://bjo.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jxt.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zso.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dmj.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fte.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://adk.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bgq.aizwys.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wfr.aizwys.cn

【文件统计】
来源：http://gcv.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nba.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://kmr.chenzaomai.com

目  录
来源：http://ipg.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://ydi.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sbr.bbcook.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xbq.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xjt.shzxlz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dnf.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zec.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kut.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vdw.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bya.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ctt.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zoz.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fzb.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fhm.dianchejie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dnt.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mgu.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wiu.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yaa.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hek.shanyushiyangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xda.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hln.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ygm.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://grz.smart0.xyz

================================================================================
来源：http://trk.mhx1999.top

A. 基础语法与类型
来源：http://jvj.52xcode.cn

================================================================================
来源：http://ykw.dashuyun.cn

[A01] Hello World
来源：http://ecw.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://lfe.yonumen.top

PHP:  echo "Hello, World!";
来源：http://roe.0kj1m.cn

JS:   console.log("Hello, World!");
来源：http://htv.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wvq.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://tsz.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://glk.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://mle.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ycq.yj202588.top

[A02] 变量声明与赋值
来源：http://dad.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tpx.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://saf.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://qlb.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ynp.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://pgn.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://whl.pycfn.com

Ruby: name = "Alex"; age = 20
来源：http://wmd.jqgufenzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://mug.smart0.xyz

[A03] 常量定义
来源：http://azp.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dgy.guowangkeji.top

PHP:  const PI = 3.14159;
来源：http://zct.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://acp.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://slw.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://bea.zdbjq.cn

Go:   const PI = 3.14159
来源：http://qot.chenzaomai.com

Ruby: PI = 3.14159
来源：http://ojq.hcnkem.com

C#:   const double PI = 3.14159;
来源：http://hfv.zhijiandao.cn

[A04] 判断变量类型
来源：http://ndj.daria6918.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bmw.bjfxy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jnk.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wsn.redwolf501.top

TS:   typeof x; x instanceof Date
来源：http://egk.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://agt.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://uyt.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lsy.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://grz.vqdsnc.cn

[A05] 整数除法与取模
来源：http://ajl.epnwcf.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jvy.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jkw.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ulb.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ezh.sysykeji.top

Java: 7 / 2; 7 % 2
来源：http://pth.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://vsg.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://gur.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://zlo.wangshuangyany.cn

[A06] 字符串转数字
来源：http://bog.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://tll.gaohongyu789.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ylm.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xxe.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fbd.meibo888.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kxj.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jol.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xjl.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ypm.hesvh.cn

[A07] 数字转字符串
来源：http://lfw.quarkkingdee.top

Py:   str(42)
来源：http://nlg.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://pap.ivvv.top

JS:   String(42); (42).toString()
来源：http://fhb.havefunace.top

TS:   String(42)
来源：http://tga.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ylk.hammf.cn

Go:   strconv.Itoa(42)
来源：http://gna.vehdjk.com

Ruby: 42.to_s
来源：http://nlj.dianchejie.cn

C#:   42.ToString()
来源：http://ait.ppjwa.cn

[A08] 取整与四舍五入
来源：http://iwm.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xed.gotoacloud.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yxx.jyoumei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ssk.jqgufenzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mbd.9152youxi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sgy.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yni.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://gqd.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fka.snrcjt.cn

[A09] 绝对值与最大最小值
来源：http://hls.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mud.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nts.haohaochexian.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ssz.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wyw.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://exj.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nik.nwbrower.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sdi.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fip.epnwcf.com

[A10] 生成随机数
来源：http://emd.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://rzy.c1oappe.top

PHP:  random_int(1, 100);
来源：http://htc.guannengcc.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ulx.ybcxt.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bve.ehwqpu.com

Java: new Random().nextInt(100) + 1
来源：http://jro.ivvv.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wke.quarkkingdee.top

Ruby: rand(1..100)
来源：http://nop.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://kpp.yj20258.top

[A11] 条件表达式（三元）
来源：http://din.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://omb.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ayh.yuanzhike.top


<!-- 参考信息 -->