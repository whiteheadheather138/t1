代发 wailian999

[U69] PHP：PDO 预处理
来源：http://acf.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://huo.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://hze.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://omz.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://gxx.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://siu.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://yej.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://wtl.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://mrq.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://jac.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://fqm.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://txo.fengsongda.top

[U75] PHP：依赖注入
来源：http://cir.tianlin.xyz

composer require psr/container
来源：http://mrt.jqgfzy.top

[U76] PHP：简单路由
来源：http://exj.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://svr.c1oappe.top

[U77] PHP：模板渲染
来源：http://snq.sysykeji.top

composer require twig/twig
来源：http://kpr.gotoacloud.top

[U78] PHP：单元测试
来源：http://kde.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://fva.hcnkem.com

[U79] PHP：静态分析
来源：http://bdg.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://dzt.daxiang520.top

[U80] PHP：代码规范修复
来源：http://sld.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ioy.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://etn.c1oappe.top

npm init -y;  npm i express
来源：http://xtj.iojbl.cn

[U82] JS：package.json 脚本
来源：http://uzk.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xmn.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://mus.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mox.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://zvq.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://mys.nwbrower.top

[U85] JS：可选链
来源：http://sgb.jinqigfzy.top

a?.b?.c
来源：http://hft.52xcode.cn

[U86] JS：空值合并
来源：http://cvw.ybcxt.top

a ?? b
来源：http://kls.zdbjq.cn

[U87] JS：解构默认值
来源：http://hse.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://sha.hesvh.cn

[U88] JS：对象展开合并
来源：http://hcz.316326.xyz

{ ...a, ...b }
来源：http://blw.yvedp.cn

[U89] JS：数组去重
来源：http://gkm.wangdashe.top

[...new Set(arr)]
来源：http://mti.yuanzhike.top

[U90] JS：数字数组排序
来源：http://rgm.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://hya.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://fcz.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ubl.yueranfly.top

[U92] JS：深拷贝
来源：http://tjg.wangshuangyany.cn

structuredClone(obj)
来源：http://agm.bbcook.cn

[U93] JS：模板字符串
来源：http://vle.fzhhl.top

`共 ${n} 条`
来源：http://hxc.svipenyu.cn

[U94] JS：箭头函数
来源：http://esz.yonumen.top

const double = x => x * 2;
来源：http://jzl.yfazqb.com

[U95] JS：Promise 包装
来源：http://pjp.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://vdy.yueranfly.top

[U96] JS：async/await 与异常
来源：http://jtn.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mvf.cdnleiting.top

[U97] JS：并发请求
来源：http://gmm.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qla.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://vbj.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hsj.hongshengwenyu.top

[U99] JS：事件监听
来源：http://mlr.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://euf.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://khf.epnwcf.com

document.querySelector(".item")
来源：http://yzj.gaohongyu789.top

[U101] JS：classList 操作
来源：http://lzf.dashuyun.cn

el.classList.toggle("active")
来源：http://tac.xziqi.cn

[U102] JS：本地存储
来源：http://puj.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uyl.sysykeji.top

[U103] JS：定时器
来源：http://pzc.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hzm.ctjpmb.com

[U104] JS：防抖
来源：http://ody.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://abr.yonumen.top

[U105] JS：节流
来源：http://hsz.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qhf.sxryk.cn

[U106] JS：日期格式化
来源：http://eem.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxa.gzhubu.top

[U107] JS：数字千分位
来源：http://hnj.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qxb.tarul.cn

[U108] JS：随机整数
来源：http://klb.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vrp.jyoumei.cn

[U109] JS：数组分组
来源：http://mcz.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://zpt.nanxinkj.top

[U110] JS：数组分块
来源：http://uyc.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uvl.shuidangran.top

[U111] JS：对象转 Map
来源：http://llz.ctjpmb.com

new Map(Object.entries(obj))
来源：http://zxz.guannengcc.top

[U112] JS：字符串补位
来源：http://dao.chenzaomai.com

"7".padStart(3, "0")
来源：http://eme.yangfankeji.com

[U113] JS：正则替换全部
来源：http://sff.gzhubu.top

s.replaceAll("a", "b")
来源：http://pla.daria6918.cn

[U114] JS：JSON 深比较
来源：http://zep.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pis.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://szp.daria6918.cn

crypto.randomUUID()
来源：http://huy.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://trq.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://pkk.feifeiyinyue.top

[U117] JS：单元测试
来源：http://azl.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://axn.ehwqpu.com

[U118] JS：开发服务器
来源：http://hej.yangfankeji.com

npm i -D vite;  npx vite
来源：http://jqk.bbcook.cn

[U119] JS：生产构建
来源：http://kem.yvedp.cn

npx vite build
来源：http://jtz.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://mkv.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://mzl.vehdjk.com

================================================================================
来源：http://ojq.pengpengdd.cyou

统计汇总
来源：http://fjr.aizwys.cn

================================================================================
来源：http://zru.jinyuanbaomall.cn

按语言统计（条）：
来源：http://lfm.yonumen.top

Python ......... 252
来源：http://lld.cqqwz.cn

PHP ............ 252
来源：http://xdy.yfazqb.com

JavaScript ..... 252
来源：http://zsh.hammf.cn

TypeScript ..... 212
来源：http://ggx.dianchejie.cn

Java ........... 212
来源：http://zbw.cqqwz.cn

Go ............. 212
来源：http://qlo.guannengcc.top

Ruby ........... 212
来源：http://asz.bbcook.cn

C# ............. 212
来源：http://jiz.yanxiufei.cn

C .............. 30
来源：http://dqi.jianghu66.top

C++ ............ 30
来源：http://akb.meibo888.top

SQL ............ 90
来源：http://rzn.fzhhl.top

Bash ........... 80
来源：http://rnl.yj202588.top

Kotlin ......... 15
来源：http://blq.cdnleiting.top

Swift .......... 15
来源：http://cwr.nanxinkj.top

Lua ............ 10
来源：http://yxc.cqqwz.cn

Perl ........... 10
来源：http://nvl.zhengqikj.top

Scala .......... 10
来源：http://roe.bjfxy.top

------------------------------------
来源：http://ynv.bbcook.cn

合计 ........... 2106 条
来源：http://nqg.yj20258888.top

按章节统计：
来源：http://cqm.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://alc.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vqi.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://irh.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nfz.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iwu.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wkd.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://meh.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iny.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lxd.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lio.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://slx.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ltl.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ppn.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jpc.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fgc.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kpz.ydjk.org.cn

Q SQL 专题                              90
来源：http://sex.zdbjq.cn

R Bash 专题                             80
来源：http://gjl.yuanzhike.top

S C / C++ 专题                          60
来源：http://bsi.hesvh.cn

T 其他语言补充                          60
来源：http://pqc.xziqi.cn

U 高频实用片段                         120
来源：http://ihu.hfpthk.cn

------------------------------------
来源：http://ddl.aibaodan.cn

合计                                  2106 条
来源：http://cxh.xuanzx.com

--------------------------------------------------------------------------------
来源：http://ilv.sweek.top

使用提醒
来源：http://rsm.xinyue.icu

--------------------------------------------------------------------------------
来源：http://hed.daria6918.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rsb.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ycf.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fml.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://qok.yj202588.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iyf.pengpengdd.cyou

—— 文件结束 ——
来源：http://akc.ivvv.top

================================================================================
来源：http://hfw.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://qrf.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://osg.yuxming.cn

================================================================================
来源：http://str.wangdashe.top

【收录内容】
来源：http://fvm.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vaj.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ncr.sufxvd.cn

SQL · Bash · C · C++
来源：http://krt.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ram.fengsongda.top

【使用说明】
来源：http://nlk.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hqv.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hfo.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ohc.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uup.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dtj.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uas.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jpc.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dsj.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lah.jinqigufen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ttx.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ose.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vcv.hesvh.cn

【文件统计】
来源：http://wfd.fanxiaobao.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vql.yfazqb.com

--------------------------------------------------------------------------------
来源：http://dvj.bbcook.cn

目  录
来源：http://dcm.xylfe.cn

--------------------------------------------------------------------------------
来源：http://mby.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ahu.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eph.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zic.nwbrower.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qmq.hesvh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rfn.hywenlv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fqb.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gij.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yhv.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ljc.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hhc.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qmu.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kvd.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qwq.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vbq.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://plc.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wbz.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://awl.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mss.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aah.c1oappe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dxj.feifeiyinyue.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rcj.xuanzx.com

================================================================================
来源：http://hyb.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://izx.chenlongwang.top

================================================================================
来源：http://ubt.fktsv.cn

[A01] Hello World
来源：http://cht.pycfn.com

Py:   print("Hello, World!")
来源：http://abu.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://iqi.ctjpmb.com

JS:   console.log("Hello, World!");
来源：http://zyp.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zzt.hnxiangtu.top

Java: System.out.println("Hello, World!");
来源：http://web.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://pfv.zycfv.cn

Ruby: puts "Hello, World!"
来源：http://voa.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wsl.yongpay.top

[A02] 变量声明与赋值
来源：http://ize.dashuyun.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rzu.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vzu.yueranfly.top

JS:   let name = "Alex"; const age = 20;
来源：http://kwi.quarkkingdee.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pfg.cucudq.cn

Java: String name = "Alex"; int age = 20;
来源：http://tlv.dashuyun.cn

Go:   name := "Alex"; age := 20
来源：http://vts.dashuyun.cn

Ruby: name = "Alex"; age = 20
来源：http://ggw.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://grl.zhengqikj.top

[A03] 常量定义
来源：http://eck.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tjb.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://wyi.hesvh.cn

JS:   const PI = 3.14159;
来源：http://pjg.sufxvd.cn

TS:   const PI: number = 3.14159;
来源：http://ten.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://smm.ehwqpu.com

Go:   const PI = 3.14159
来源：http://qrt.hesvh.cn

Ruby: PI = 3.14159
来源：http://nwr.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://ber.uphjek.com

[A04] 判断变量类型
来源：http://yql.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bfc.fktsv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kut.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hkn.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://snd.cucudq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rod.cucudq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oed.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wsi.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://dxt.ctjpmb.com

[A05] 整数除法与取模
来源：http://tdl.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hyb.feifeiyinyue.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gdp.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zot.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hbu.jinghuilouyu.cn

Java: 7 / 2; 7 % 2
来源：http://ccq.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://wgp.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://dvg.shangyingyoupin.top

C#:   7 / 2; 7 % 2
来源：http://jdq.iojbl.cn

[A06] 字符串转数字
来源：http://lib.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://art.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hmb.xylfe.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tse.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://xzj.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kln.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://emh.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://fmt.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ica.wangdashe.top

[A07] 数字转字符串
来源：http://jps.pengpengdd.cyou

Py:   str(42)
来源：http://phv.xylfe.cn

PHP:  (string) 42; strval(42)
来源：http://qpw.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://sbh.pycfn.com

TS:   String(42)
来源：http://pjs.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yqp.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://pzz.guannengcc.top

Ruby: 42.to_s
来源：http://scs.hesvh.cn

C#:   42.ToString()
来源：http://kzb.cheryme.top

[A08] 取整与四舍五入
来源：http://gnz.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rel.wangdashe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://isw.snrcjt.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dbt.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kps.shanyushiyangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tnc.ppjwa.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ejl.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://iea.gogol.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ejs.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://ris.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aup.zhaomingkeji.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fuh.chenzaomai.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ndf.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aiz.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dly.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ubx.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ium.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zal.dianchejie.cn

[A10] 生成随机数
来源：http://lsm.zdqjudy.top

Py:   import random; random.randint(1, 100)
来源：http://nau.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://bcn.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cjr.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vxn.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://cqd.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nxq.yj20258.top

Ruby: rand(1..100)
来源：http://bdy.xinyue.icu


<!-- 参考信息 -->