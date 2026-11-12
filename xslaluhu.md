代发 wailian999

[U69] PHP：PDO 预处理
来源：http://wvb.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://igp.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://yup.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://toz.tianlin.xyz

[U71] PHP：抛出异常
来源：http://drw.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://fbw.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://oan.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://xox.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://rsb.yj20258.top

parse_ini_file("config.ini", true)
来源：http://xby.guannengcc.top

[U74] PHP：读取环境变量
来源：http://ohl.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://pqz.c1oappe.top

[U75] PHP：依赖注入
来源：http://igu.guowangkeji.top

composer require psr/container
来源：http://xuk.ivvv.top

[U76] PHP：简单路由
来源：http://lem.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zgx.jqgfzy.top

[U77] PHP：模板渲染
来源：http://ztq.xziqi.cn

composer require twig/twig
来源：http://the.yj20258.top

[U78] PHP：单元测试
来源：http://ris.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://aiw.ivvv.top

[U79] PHP：静态分析
来源：http://pmz.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://bdr.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://bzf.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vas.zycfv.cn

[U81] JS：初始化项目
来源：http://elv.daxiang520.top

npm init -y;  npm i express
来源：http://tef.guannengcc.top

[U82] JS：package.json 脚本
来源：http://tre.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hem.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://adn.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qqf.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://rba.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cwg.andypj.xyz

[U85] JS：可选链
来源：http://bvk.cashguo.top

a?.b?.c
来源：http://yaq.zhiwuduotai.top

[U86] JS：空值合并
来源：http://pyd.cdnleiting.top

a ?? b
来源：http://wtm.sweek.top

[U87] JS：解构默认值
来源：http://qvx.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://art.haohaochexian.top

[U88] JS：对象展开合并
来源：http://nve.zhiwuduotai.top

{ ...a, ...b }
来源：http://jsn.gzhubu.top

[U89] JS：数组去重
来源：http://lta.cucudq.cn

[...new Set(arr)]
来源：http://jni.xuanzx.com

[U90] JS：数字数组排序
来源：http://seq.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://swi.gzhubu.top

[U91] JS：对象键值遍历
来源：http://hpd.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cmu.zhengqikj.top

[U92] JS：深拷贝
来源：http://yel.pengpengdd.cyou

structuredClone(obj)
来源：http://qep.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://ovo.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://qxc.cdnleiting.top

[U94] JS：箭头函数
来源：http://hux.jyoumei.cn

const double = x => x * 2;
来源：http://fxh.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://iwt.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://yfe.tanke756.top

[U96] JS：async/await 与异常
来源：http://xzo.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://psd.chenjidiqi.icu

[U97] JS：并发请求
来源：http://yvg.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xdx.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://poe.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xcm.jinqigufen.top

[U99] JS：事件监听
来源：http://osp.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://cwe.cqqwz.cn

[U100] JS：DOM 查询
来源：http://san.jlsjyb.cn

document.querySelector(".item")
来源：http://atb.dashuyun.cn

[U101] JS：classList 操作
来源：http://zkl.guannengcc.top

el.classList.toggle("active")
来源：http://vil.fzhhl.top

[U102] JS：本地存储
来源：http://jss.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tlp.haohaochexian.top

[U103] JS：定时器
来源：http://rfa.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cvb.9152youxi.cn

[U104] JS：防抖
来源：http://whu.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ect.ivvv.top

[U105] JS：节流
来源：http://bve.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fgu.snrcjt.cn

[U106] JS：日期格式化
来源：http://ymm.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://epu.sufxvd.cn

[U107] JS：数字千分位
来源：http://ygr.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lyx.wangdashe.top

[U108] JS：随机整数
来源：http://fyz.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vpn.aizwys.cn

[U109] JS：数组分组
来源：http://sqi.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://zcr.cdnleiting.top

[U110] JS：数组分块
来源：http://kwt.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://anu.316326.xyz

[U111] JS：对象转 Map
来源：http://hdl.yj20258888.top

new Map(Object.entries(obj))
来源：http://iya.jlsjyb.cn

[U112] JS：字符串补位
来源：http://ofv.ppjwa.cn

"7".padStart(3, "0")
来源：http://cdz.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://qje.tian-w.cn

s.replaceAll("a", "b")
来源：http://luj.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://akg.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://bmm.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://wim.xuanzx.com

crypto.randomUUID()
来源：http://fim.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://sjm.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://rxc.birdmap.top

[U117] JS：单元测试
来源：http://hjp.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://ppx.ctjpmb.com

[U118] JS：开发服务器
来源：http://hir.zhixingplan.top

npm i -D vite;  npx vite
来源：http://ano.9152youxi.cn

[U119] JS：生产构建
来源：http://hge.chenjidiqi.icu

npx vite build
来源：http://paz.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://xmp.birdmap.top

import.meta.env.VITE_API_URL
来源：http://cji.aizwys.cn

================================================================================
来源：http://zkf.svipenyu.cn

统计汇总
来源：http://jxz.yfazqb.com

================================================================================
来源：http://gnb.chenzaomai.com

按语言统计（条）：
来源：http://qmu.sjlbkw.cn

Python ......... 252
来源：http://lqd.yfazqb.com

PHP ............ 252
来源：http://gvf.yongpay.top

JavaScript ..... 252
来源：http://cpa.bjfxy.top

TypeScript ..... 212
来源：http://mge.birdmap.top

Java ........... 212
来源：http://rww.ydjk.org.cn

Go ............. 212
来源：http://mzc.cdnleiting.top

Ruby ........... 212
来源：http://nwn.hongshengwenyu.top

C# ............. 212
来源：http://ytb.jlsjyb.cn

C .............. 30
来源：http://lbt.hcnkem.com

C++ ............ 30
来源：http://zxb.jyoumei.cn

SQL ............ 90
来源：http://yak.52xcode.cn

Bash ........... 80
来源：http://dtl.uphjek.com

Kotlin ......... 15
来源：http://pqo.yongpay.top

Swift .......... 15
来源：http://bra.pycfn.com

Lua ............ 10
来源：http://cai.yvedp.cn

Perl ........... 10
来源：http://qxk.jinyuanbaomall.cn

Scala .......... 10
来源：http://qiq.nanxuanxn.top

------------------------------------
来源：http://gov.vqdsnc.cn

合计 ........... 2106 条
来源：http://jwh.aibaodan.cn

按章节统计：
来源：http://gbo.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zbj.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://atz.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dfw.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sgk.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://agz.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mde.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://udt.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wck.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ydh.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://igx.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ygk.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gxi.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zdf.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ttj.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cmt.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nli.pycfn.com

Q SQL 专题                              90
来源：http://qhx.aibaodan.cn

R Bash 专题                             80
来源：http://srv.yuanzhike.top

S C / C++ 专题                          60
来源：http://idw.9152youxi.cn

T 其他语言补充                          60
来源：http://itl.9152youxi.cn

U 高频实用片段                         120
来源：http://dbb.svipenyu.cn

------------------------------------
来源：http://qpu.hammf.cn

合计                                  2106 条
来源：http://yut.yfazqb.com

--------------------------------------------------------------------------------
来源：http://zhm.sufxvd.cn

使用提醒
来源：http://zrj.andypj.xyz

--------------------------------------------------------------------------------
来源：http://xsq.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hyq.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zdq.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zhd.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lar.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rix.xziqi.cn

—— 文件结束 ——
来源：http://bdc.zdqjudy.top

================================================================================
来源：http://kus.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://tnh.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://qkl.yuxming.cn

================================================================================
来源：http://fdt.fktsv.cn

【收录内容】
来源：http://ryq.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lsf.ivvv.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hsc.jinqigfzy.top

SQL · Bash · C · C++
来源：http://yim.yuanzhike.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rjq.mhx1999.top

【使用说明】
来源：http://qvw.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yey.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fqp.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://znm.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xaq.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zvo.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ifk.sweek.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://urd.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eff.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xnd.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dju.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cuy.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dpk.fzhhl.top

【文件统计】
来源：http://lnb.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://twx.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://utz.quarkkingdee.top

目  录
来源：http://dkg.pycfn.com

--------------------------------------------------------------------------------
来源：http://ior.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yvg.andypj.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://urz.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qzj.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nht.c1oappe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iku.ctjpmb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ebq.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kwa.fktsv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uxc.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tui.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hdv.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tyq.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cgo.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vjn.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pzp.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hbv.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://beq.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mqf.tian-w.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eay.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ysd.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpk.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blk.zhiwuduotai.top

================================================================================
来源：http://hvz.epnwcf.com

A. 基础语法与类型
来源：http://lml.mhx1999.top

================================================================================
来源：http://zdu.yuxming.cn

[A01] Hello World
来源：http://hbf.andypj.xyz

Py:   print("Hello, World!")
来源：http://nyx.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://yfz.zhijiandao.cn

JS:   console.log("Hello, World!");
来源：http://zbo.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bix.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://euo.yfazqb.com

Go:   fmt.Println("Hello, World!")
来源：http://gmo.smart0.xyz

Ruby: puts "Hello, World!"
来源：http://kxj.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://twh.xylfe.cn

[A02] 变量声明与赋值
来源：http://ldg.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rmp.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xay.9152youxi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://czu.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vda.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://opc.jinghuilouyu.cn

Go:   name := "Alex"; age := 20
来源：http://npo.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://vzy.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://coz.zhixingplan.top

[A03] 常量定义
来源：http://olz.zycfv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nyh.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://tvo.52xcode.cn

JS:   const PI = 3.14159;
来源：http://ahk.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://vgw.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://iky.havefunace.top

Go:   const PI = 3.14159
来源：http://bxa.bjfxy.top

Ruby: PI = 3.14159
来源：http://qdt.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://nza.epnwcf.com

[A04] 判断变量类型
来源：http://gig.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yth.daria6918.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ddh.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uqq.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://crp.pengpengdd.cyou

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lhq.pengpengdd.cyou

Go:   reflect.TypeOf(x).Name()
来源：http://kdn.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yke.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://xtq.gzhubu.top

[A05] 整数除法与取模
来源：http://jje.fanxiaobao.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jco.sysykeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xsy.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dhv.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hmk.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://myk.hysaishi.cn

Go:   7 / 2; 7 % 2
来源：http://swd.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://ygv.52xcode.cn

C#:   7 / 2; 7 % 2
来源：http://ycs.redwolf501.top

[A06] 字符串转数字
来源：http://ckp.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://feh.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://exg.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xae.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jme.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://chb.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rue.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uue.cheryme.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://luf.bjfxy.top

[A07] 数字转字符串
来源：http://wfu.jiagoushi.top

Py:   str(42)
来源：http://dmd.meibo888.top

PHP:  (string) 42; strval(42)
来源：http://jbd.hesvh.cn

JS:   String(42); (42).toString()
来源：http://wna.svipenyu.cn

TS:   String(42)
来源：http://dsl.snrcjt.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://szl.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://dsb.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://odl.9152youxi.cn

C#:   42.ToString()
来源：http://vii.sweek.top

[A08] 取整与四舍五入
来源：http://iyo.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aqu.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mhc.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dlp.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dzb.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bul.zdbjq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yod.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://esa.kuanghao11.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bwv.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://ucr.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://glt.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qpa.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tbm.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vuc.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://swm.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rzu.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://per.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://epu.jqgufenzy.top

[A10] 生成随机数
来源：http://apx.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://tje.yonumen.top

PHP:  random_int(1, 100);
来源：http://bwj.xuanzx.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cwj.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pmd.0kj1m.cn

Java: new Random().nextInt(100) + 1
来源：http://qww.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sqt.hywenlv.cn

Ruby: rand(1..100)
来源：http://tzq.zycfv.cn


<!-- 参考信息 -->