代发 wailian999

[U69] PHP：PDO 预处理
来源：http://icw.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vxn.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://oey.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://byw.yj202588.top

[U71] PHP：抛出异常
来源：http://dqm.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://kvt.yj20258.top

[U72] PHP：写错误日志
来源：http://jxo.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://jus.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://grg.c1oappe.top

parse_ini_file("config.ini", true)
来源：http://jhe.jqgfzy.top

[U74] PHP：读取环境变量
来源：http://wsz.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://qnl.tarul.cn

[U75] PHP：依赖注入
来源：http://wrc.yonumen.top

composer require psr/container
来源：http://xfw.yonumen.top

[U76] PHP：简单路由
来源：http://otb.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zee.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://sza.xuanzx.com

composer require twig/twig
来源：http://xzw.sweek.top

[U78] PHP：单元测试
来源：http://sbk.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://akr.cqqwz.cn

[U79] PHP：静态分析
来源：http://hbj.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://gyg.bbcook.cn

[U80] PHP：代码规范修复
来源：http://thc.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://nyc.sweek.top

[U81] JS：初始化项目
来源：http://ztr.c1oappe.top

npm init -y;  npm i express
来源：http://trv.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://mah.dashuyun.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ava.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://ias.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://wai.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://vgw.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://rgv.hcnkem.com

[U85] JS：可选链
来源：http://sxo.hysaishi.cn

a?.b?.c
来源：http://ycs.sweek.top

[U86] JS：空值合并
来源：http://phb.quarkkingdee.top

a ?? b
来源：http://rnf.yj20258888.top

[U87] JS：解构默认值
来源：http://uog.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://hpz.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://lis.xziqi.cn

{ ...a, ...b }
来源：http://hhk.epnwcf.com

[U89] JS：数组去重
来源：http://fiz.quarkkingdee.top

[...new Set(arr)]
来源：http://bxt.iojbl.cn

[U90] JS：数字数组排序
来源：http://qmp.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://agy.yj20258.top

[U91] JS：对象键值遍历
来源：http://wqk.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jmn.zhixingplan.top

[U92] JS：深拷贝
来源：http://fht.zdbjq.cn

structuredClone(obj)
来源：http://neo.snrcjt.cn

[U93] JS：模板字符串
来源：http://yua.quarkkingdee.top

`共 ${n} 条`
来源：http://afl.guowangkeji.top

[U94] JS：箭头函数
来源：http://gim.pycfn.com

const double = x => x * 2;
来源：http://tob.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://uzp.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://vpo.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://ywa.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uph.feifeiyinyue.top

[U97] JS：并发请求
来源：http://vmi.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ifj.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://rhs.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dfj.shzxlz.cn

[U99] JS：事件监听
来源：http://hun.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://ljl.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://pox.ehwqpu.com

document.querySelector(".item")
来源：http://dns.zhijiandao.cn

[U101] JS：classList 操作
来源：http://igb.aibaodan.cn

el.classList.toggle("active")
来源：http://zow.cheryme.top

[U102] JS：本地存储
来源：http://cgz.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wbk.dashuyun.cn

[U103] JS：定时器
来源：http://ksm.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eku.smart0.xyz

[U104] JS：防抖
来源：http://cdt.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cep.yuxming.cn

[U105] JS：节流
来源：http://buk.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://duh.havefunace.top

[U106] JS：日期格式化
来源：http://luk.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gqt.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://npq.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xra.wangdashe.top

[U108] JS：随机整数
来源：http://byq.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ili.yuanzhike.top

[U109] JS：数组分组
来源：http://ozq.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://wgd.bjfxy.top

[U110] JS：数组分块
来源：http://uzi.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qpd.yvedp.cn

[U111] JS：对象转 Map
来源：http://kzr.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://wkj.yj20258888.top

[U112] JS：字符串补位
来源：http://fpd.zhixingplan.top

"7".padStart(3, "0")
来源：http://uds.chenzaomai.com

[U113] JS：正则替换全部
来源：http://vzj.316326.xyz

s.replaceAll("a", "b")
来源：http://sbh.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://oux.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hbn.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://erm.ivvv.top

crypto.randomUUID()
来源：http://sdd.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://hsx.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://sbx.yueranfly.top

[U117] JS：单元测试
来源：http://mnb.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://kyf.yuanzhike.top

[U118] JS：开发服务器
来源：http://mjh.ppjwa.cn

npm i -D vite;  npx vite
来源：http://arp.cheryme.top

[U119] JS：生产构建
来源：http://erj.52xcode.cn

npx vite build
来源：http://wor.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://fjm.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://xuv.jinqigfzy.top

================================================================================
来源：http://tch.uphjek.com

统计汇总
来源：http://gel.bbcook.cn

================================================================================
来源：http://ohs.andypj.xyz

按语言统计（条）：
来源：http://qpr.hcnkem.com

Python ......... 252
来源：http://rrb.jianghu66.top

PHP ............ 252
来源：http://fmk.yongpay.top

JavaScript ..... 252
来源：http://evr.fehbvm.com

TypeScript ..... 212
来源：http://rue.hesvh.cn

Java ........... 212
来源：http://spk.uphjek.com

Go ............. 212
来源：http://tza.xuetiantiany.cn

Ruby ........... 212
来源：http://oge.sweek.top

C# ............. 212
来源：http://haa.bjfxy.top

C .............. 30
来源：http://shx.shangyingyoupin.top

C++ ............ 30
来源：http://llb.hesvh.cn

SQL ............ 90
来源：http://csv.ivvv.top

Bash ........... 80
来源：http://rau.zhixingplan.top

Kotlin ......... 15
来源：http://vkg.yonumen.top

Swift .......... 15
来源：http://pwq.shangyingyoupin.top

Lua ............ 10
来源：http://uzq.nanxinkj.top

Perl ........... 10
来源：http://edk.fehbvm.com

Scala .......... 10
来源：http://pzz.yangfankeji.com

------------------------------------
来源：http://tsb.redwolf501.top

合计 ........... 2106 条
来源：http://gld.mhx1999.top

按章节统计：
来源：http://qpj.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ksh.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uwr.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ssv.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jrd.vehdjk.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lcy.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sax.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mfh.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dvd.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bui.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mdm.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cgr.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://orv.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jde.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://moj.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aym.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dzf.chenlongwang.top

Q SQL 专题                              90
来源：http://ooq.52xcode.cn

R Bash 专题                             80
来源：http://yap.9152youxi.cn

S C / C++ 专题                          60
来源：http://qma.ctjpmb.com

T 其他语言补充                          60
来源：http://wla.zhiwuduotai.top

U 高频实用片段                         120
来源：http://rqf.xinyue.icu

------------------------------------
来源：http://yps.ydzc1.top

合计                                  2106 条
来源：http://mqj.sweek.top

--------------------------------------------------------------------------------
来源：http://awn.aibaodan.cn

使用提醒
来源：http://wln.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://dky.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ipu.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gfg.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vsb.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wwo.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://udp.aibaodan.cn

—— 文件结束 ——
来源：http://zmk.0kj1m.cn

================================================================================
来源：http://ikf.aibaodan.cn

程序语言常见例子速查手册（2024 版）
来源：http://flj.hywenlv.cn

Common Programming Examples Cheat Book
来源：http://dbf.zhoulong.xyz

================================================================================
来源：http://tfa.nwbrower.top

【收录内容】
来源：http://aho.nanxuanxn.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rqu.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mqn.ehwqpu.com

SQL · Bash · C · C++
来源：http://bym.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kwj.fengsongda.top

【使用说明】
来源：http://yaw.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tip.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dwp.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://noz.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qnb.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yja.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ooz.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cof.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rbz.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wcn.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lfb.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fln.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nea.mhx1999.top

【文件统计】
来源：http://lgq.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uze.bbcook.cn

--------------------------------------------------------------------------------
来源：http://hfj.fehbvm.com

目  录
来源：http://uwf.tanke756.top

--------------------------------------------------------------------------------
来源：http://whp.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jpe.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oee.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lva.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mmt.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mlk.yvedp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ppt.daria6918.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://izz.yj20258.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xrv.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bhv.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ltt.yuxming.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mek.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mww.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fcb.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ruw.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pao.uphjek.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tsl.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wez.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://clb.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://spy.tanke756.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jdq.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wis.zdbjq.cn

================================================================================
来源：http://mcf.hnxiangtu.top

A. 基础语法与类型
来源：http://izy.hcnkem.com

================================================================================
来源：http://cak.quarkkingdee.top

[A01] Hello World
来源：http://nyy.bjfxy.top

Py:   print("Hello, World!")
来源：http://lkd.zhijiandao.cn

PHP:  echo "Hello, World!";
来源：http://ste.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://mye.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rau.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://jyk.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://nmk.9152youxi.cn

Ruby: puts "Hello, World!"
来源：http://dea.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wro.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://ezw.xziqi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tmr.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eyd.bbcook.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ebm.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sml.ivvv.top

Java: String name = "Alex"; int age = 20;
来源：http://nzt.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://cff.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://upi.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zre.guowangkeji.top

[A03] 常量定义
来源：http://zyw.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://evy.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://joq.xuanzx.com

JS:   const PI = 3.14159;
来源：http://hgq.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://wsv.gzhubu.top

Java: static final double PI = 3.14159;
来源：http://trr.chenjidiqi.icu

Go:   const PI = 3.14159
来源：http://cxp.cheryme.top

Ruby: PI = 3.14159
来源：http://ead.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://xks.xziqi.cn

[A04] 判断变量类型
来源：http://pdl.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ffg.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lwr.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fyb.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://lyo.zhiwuduotai.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nvm.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://hjq.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://xcj.havefunace.top

C#:   x.GetType().Name; x is int
来源：http://ggy.xylfe.cn

[A05] 整数除法与取模
来源：http://wps.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://edk.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xdy.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ncd.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uyt.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://aou.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://egg.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://oro.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://akh.pengpengdd.cyou

[A06] 字符串转数字
来源：http://iun.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://zin.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nvl.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jla.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://sob.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xzc.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rhk.mhx1999.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ten.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vxt.shangyingyoupin.top

[A07] 数字转字符串
来源：http://qmq.zycfv.cn

Py:   str(42)
来源：http://uiv.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://klj.zhixingplan.top

JS:   String(42); (42).toString()
来源：http://ugh.sufxvd.cn

TS:   String(42)
来源：http://dkx.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ywt.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://ete.haohaochexian.top

Ruby: 42.to_s
来源：http://xmu.c1oappe.top

C#:   42.ToString()
来源：http://alx.cdnleiting.top

[A08] 取整与四舍五入
来源：http://lbr.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ndc.svipenyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zsd.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dav.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://onn.xuanzx.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iot.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nsv.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://vsv.sufxvd.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kca.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://dlr.tianlin.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gip.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yyt.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zzb.yj202588.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jud.andypj.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://now.feifeiyinyue.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nzx.cheryme.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://clt.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zjn.tian-w.cn

[A10] 生成随机数
来源：http://qis.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://vsk.ydzc1.top

PHP:  random_int(1, 100);
来源：http://fyp.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dfj.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xbu.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://fkw.zdqjudy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gyv.yueranfly.top

Ruby: rand(1..100)
来源：http://hkt.fktsv.cn


<!-- 参考信息 -->