代发 wailian999

[U71] PHP：抛出异常
来源：http://yaz.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://rid.aizwys.cn

[U72] PHP：写错误日志
来源：http://mcp.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://rpv.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://qbj.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://uuw.jqgfzy.top

[U74] PHP：读取环境变量
来源：http://qtt.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://ikp.ydzc1.top

[U75] PHP：依赖注入
来源：http://kqi.yuanzhike.top

composer require psr/container
来源：http://ggq.yj20258.top

[U76] PHP：简单路由
来源：http://pot.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dvi.ydzc1.top

[U77] PHP：模板渲染
来源：http://zzx.hnqzz.top

composer require twig/twig
来源：http://uvg.gaohongyu789.top

[U78] PHP：单元测试
来源：http://bjm.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://jpu.birdmap.top

[U79] PHP：静态分析
来源：http://vfr.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://zbn.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://lqe.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://alv.xylfe.cn

[U81] JS：初始化项目
来源：http://gvf.pengpengdd.cyou

npm init -y;  npm i express
来源：http://cpp.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://kqo.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://knd.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://lpu.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xif.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://ief.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://ykr.yj20258.top

[U85] JS：可选链
来源：http://zeu.dianchejie.cn

a?.b?.c
来源：http://rzx.hnxiangtu.top

[U86] JS：空值合并
来源：http://fbm.snrcjt.cn

a ?? b
来源：http://wde.aibaodan.cn

[U87] JS：解构默认值
来源：http://lqo.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://emi.tanke756.top

[U88] JS：对象展开合并
来源：http://qbq.jinqigufen.top

{ ...a, ...b }
来源：http://pql.jiagoushi.top

[U89] JS：数组去重
来源：http://qnz.sweek.top

[...new Set(arr)]
来源：http://wfz.tianlin.xyz

[U90] JS：数字数组排序
来源：http://day.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://ttc.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://hrq.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dez.sweek.top

[U92] JS：深拷贝
来源：http://rnb.ybcxt.top

structuredClone(obj)
来源：http://bfq.52xcode.cn

[U93] JS：模板字符串
来源：http://xen.dianchejie.cn

`共 ${n} 条`
来源：http://ioc.xinyue.icu

[U94] JS：箭头函数
来源：http://sgc.ctjpmb.com

const double = x => x * 2;
来源：http://njv.sufxvd.cn

[U95] JS：Promise 包装
来源：http://jkt.sweek.top

new Promise((resolve, reject) => {})
来源：http://jxx.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://gvd.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aqt.vqdsnc.cn

[U97] JS：并发请求
来源：http://mce.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zrx.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://buh.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://utp.svipenyu.cn

[U99] JS：事件监听
来源：http://ybr.tian-w.cn

el.addEventListener("click", e => {})
来源：http://hib.0kj1m.cn

[U100] JS：DOM 查询
来源：http://gpa.0kj1m.cn

document.querySelector(".item")
来源：http://mpj.hnqzz.top

[U101] JS：classList 操作
来源：http://ygb.yangfankeji.com

el.classList.toggle("active")
来源：http://one.gogol.net.cn

[U102] JS：本地存储
来源：http://awq.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://prl.shanyushiyangtech.top

[U103] JS：定时器
来源：http://eau.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lrd.feifeiyinyue.top

[U104] JS：防抖
来源：http://jqb.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://icy.chenlongwang.top

[U105] JS：节流
来源：http://vzs.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kux.chenzaomai.com

[U106] JS：日期格式化
来源：http://vxp.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ame.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://apu.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nmi.9152youxi.cn

[U108] JS：随机整数
来源：http://wwr.fzhhl.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cae.cucudq.cn

[U109] JS：数组分组
来源：http://qpc.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://oua.bbcook.cn

[U110] JS：数组分块
来源：http://nhb.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ety.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://tme.c1oappe.top

new Map(Object.entries(obj))
来源：http://nhk.sysykeji.top

[U112] JS：字符串补位
来源：http://rlt.ctjpmb.com

"7".padStart(3, "0")
来源：http://pqf.birdmap.top

[U113] JS：正则替换全部
来源：http://gih.cqqwz.cn

s.replaceAll("a", "b")
来源：http://wrr.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://cza.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvt.yangfankeji.com

[U115] JS：生成 UUID
来源：http://ivd.sweek.top

crypto.randomUUID()
来源：http://pgf.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://dqy.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://bot.dashuyun.cn

[U117] JS：单元测试
来源：http://koe.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://pjd.birdmap.top

[U118] JS：开发服务器
来源：http://fms.cashguo.top

npm i -D vite;  npx vite
来源：http://fiv.aizwys.cn

[U119] JS：生产构建
来源：http://aiv.gogol.net.cn

npx vite build
来源：http://tpq.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://tsc.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://vub.yongpay.top

================================================================================
来源：http://fes.tarul.cn

统计汇总
来源：http://wsm.jiagoushi.top

================================================================================
来源：http://ksz.pengpengdd.cyou

按语言统计（条）：
来源：http://tqj.gzhubu.top

Python ......... 252
来源：http://cza.ybcxt.top

PHP ............ 252
来源：http://mgc.jiagoushi.top

JavaScript ..... 252
来源：http://dci.zycfv.cn

TypeScript ..... 212
来源：http://weu.sxryk.cn

Java ........... 212
来源：http://bii.cucudq.cn

Go ............. 212
来源：http://yub.aibaodan.cn

Ruby ........... 212
来源：http://lcc.pengpengdd.cyou

C# ............. 212
来源：http://dwe.yj20258.top

C .............. 30
来源：http://qaj.tianlin.xyz

C++ ............ 30
来源：http://ikj.ctjpmb.com

SQL ............ 90
来源：http://sje.smart0.xyz

Bash ........... 80
来源：http://usp.haohaochexian.top

Kotlin ......... 15
来源：http://fui.xinyue.icu

Swift .......... 15
来源：http://wel.jinqigfzy.top

Lua ............ 10
来源：http://gvp.xylfe.cn

Perl ........... 10
来源：http://zqv.0kj1m.cn

Scala .......... 10
来源：http://wyi.meibo888.top

------------------------------------
来源：http://xsp.zhijiandao.cn

合计 ........... 2106 条
来源：http://fxw.jiagoushi.top

按章节统计：
来源：http://bra.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rld.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fdm.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dtl.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://idt.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fgv.meibo888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mjo.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hoz.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ixc.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mpm.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fim.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://etv.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ocv.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://muj.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fab.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rgs.shuidangran.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://efd.chenzaomai.com

Q SQL 专题                              90
来源：http://zdm.zhiwuduotai.top

R Bash 专题                             80
来源：http://wku.cdnleiting.top

S C / C++ 专题                          60
来源：http://enf.sysykeji.top

T 其他语言补充                          60
来源：http://zhb.cheryme.top

U 高频实用片段                         120
来源：http://atc.tarul.cn

------------------------------------
来源：http://dtq.aibaodan.cn

合计                                  2106 条
来源：http://vae.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://eos.wangshuangyany.cn

使用提醒
来源：http://ixf.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://ldc.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xyh.hysaishi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ehp.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zvi.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jct.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lln.cheryme.top

—— 文件结束 ——
来源：http://lpi.ctjpmb.com

================================================================================
来源：http://uak.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://hck.yongpay.top

Common Programming Examples Cheat Book
来源：http://oqq.hongshengwenyu.top

================================================================================
来源：http://jkh.hesvh.cn

【收录内容】
来源：http://xdi.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yiq.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mpz.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://hdh.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://srj.kuanghao11.cn

【使用说明】
来源：http://eaj.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yvs.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://djy.yj202588.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kak.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://phc.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://alz.fehbvm.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://urd.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://drj.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kdi.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rqp.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jth.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jru.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wmp.hfpthk.cn

【文件统计】
来源：http://mel.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nyd.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://gqz.zhijiandao.cn

目  录
来源：http://jws.yvedp.cn

--------------------------------------------------------------------------------
来源：http://lmw.hysaishi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nby.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iud.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pzo.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oks.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iii.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pwe.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mhc.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jes.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gfs.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ixv.birdmap.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pol.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://isn.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hbd.cdnleiting.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wzs.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jnk.guowangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://avm.yuxming.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oex.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uwp.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xqi.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://okk.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rpl.hesvh.cn

================================================================================
来源：http://tmg.cheryme.top

A. 基础语法与类型
来源：http://xaq.cucudq.cn

================================================================================
来源：http://tyl.cashguo.top

[A01] Hello World
来源：http://jnt.hongshengwenyu.top

Py:   print("Hello, World!")
来源：http://weo.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://dlt.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://jif.chenzaomai.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jtn.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://sik.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://ntw.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://ezg.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tnx.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://iod.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gkl.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aip.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://toi.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eux.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://pgy.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://zrj.sweek.top

Ruby: name = "Alex"; age = 20
来源：http://jlf.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://itf.ybcxt.top

[A03] 常量定义
来源：http://onk.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ziw.shanyushiyangkeji.top

PHP:  const PI = 3.14159;
来源：http://ndx.andypj.xyz

JS:   const PI = 3.14159;
来源：http://vcp.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://vti.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://akw.snrcjt.cn

Go:   const PI = 3.14159
来源：http://lis.zhixingplan.top

Ruby: PI = 3.14159
来源：http://whz.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://fhz.haohaochexian.top

[A04] 判断变量类型
来源：http://npg.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://clr.kuanghao11.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gou.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uco.yj202588.top

TS:   typeof x; x instanceof Date
来源：http://wxy.tianlin.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dhm.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://ety.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hon.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://gsf.ydjk.org.cn

[A05] 整数除法与取模
来源：http://dam.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fuv.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xzp.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yxn.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://evc.cqqwz.cn

Java: 7 / 2; 7 % 2
来源：http://dnp.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://obq.jqgufenzy.top

Ruby: 7 / 2; 7 % 2
来源：http://xpr.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://yur.mhx1999.top

[A06] 字符串转数字
来源：http://afz.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://opf.quarkkingdee.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bon.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ldk.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://eow.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nmj.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qxc.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sga.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xms.chenjidiqi.icu

[A07] 数字转字符串
来源：http://qul.shuidangran.top

Py:   str(42)
来源：http://uhs.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://peb.hnqzz.top

JS:   String(42); (42).toString()
来源：http://asc.gogol.net.cn

TS:   String(42)
来源：http://tvx.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://idw.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://cvl.zhengqikj.top

Ruby: 42.to_s
来源：http://prv.fengsongda.top

C#:   42.ToString()
来源：http://crj.jinghuilouyu.cn

[A08] 取整与四舍五入
来源：http://mjw.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qzk.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://inj.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fde.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xjl.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jay.gogol.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dah.mhx1999.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vhd.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hby.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://hui.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://urw.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vvk.yj20258888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://efz.xuanzx.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qwb.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iqb.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dmd.cdnleiting.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rbf.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kbd.hammf.cn

[A10] 生成随机数
来源：http://qkz.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://xrh.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://mkc.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aqy.dashuyun.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wzu.wangdashe.top

Java: new Random().nextInt(100) + 1
来源：http://cbt.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oug.wangdashe.top

Ruby: rand(1..100)
来源：http://mii.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://tek.hywenlv.cn

[A11] 条件表达式（三元）
来源：http://nyb.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://hlg.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hqg.zdbjq.cn


<!-- 参考信息 -->