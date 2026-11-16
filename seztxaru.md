代发 wailian999

[U67] PHP：处理文件上传
来源：http://bnb.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wbq.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://urj.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://llv.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://orz.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gyq.fengsongda.top

[U70] PHP：PDO 事务
来源：http://wid.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vmk.smart0.xyz

[U71] PHP：抛出异常
来源：http://ger.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://lsr.guowangkeji.top

[U72] PHP：写错误日志
来源：http://ric.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://swh.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://ucq.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://hno.nwbrower.top

[U74] PHP：读取环境变量
来源：http://tja.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://sen.nanxinkj.top

[U75] PHP：依赖注入
来源：http://jwm.zhengqikj.top

composer require psr/container
来源：http://vrg.vehdjk.com

[U76] PHP：简单路由
来源：http://wig.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ame.iojbl.cn

[U77] PHP：模板渲染
来源：http://fpf.chenzaomai.com

composer require twig/twig
来源：http://zcj.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://ovv.cheryme.top

composer require --dev phpunit/phpunit
来源：http://vcu.yj20258.top

[U79] PHP：静态分析
来源：http://dou.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://aov.xuanzx.com

[U80] PHP：代码规范修复
来源：http://niy.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cwu.yanxiufei.cn

[U81] JS：初始化项目
来源：http://oss.gogol.net.cn

npm init -y;  npm i express
来源：http://zju.52xcode.cn

[U82] JS：package.json 脚本
来源：http://nym.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bbk.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://klj.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vks.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://vvy.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wis.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://vmr.daria6918.cn

a?.b?.c
来源：http://mlx.snrcjt.cn

[U86] JS：空值合并
来源：http://mdg.gaohongyu789.top

a ?? b
来源：http://vte.epnwcf.com

[U87] JS：解构默认值
来源：http://yyz.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://flq.snrcjt.cn

[U88] JS：对象展开合并
来源：http://vct.xylfe.cn

{ ...a, ...b }
来源：http://bwh.yongpay.top

[U89] JS：数组去重
来源：http://mmf.daxiang520.top

[...new Set(arr)]
来源：http://pdy.yj20258.top

[U90] JS：数字数组排序
来源：http://ujj.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://dyv.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://yyh.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqv.xuanzx.com

[U92] JS：深拷贝
来源：http://cbw.xinyue.icu

structuredClone(obj)
来源：http://yis.zdqjudy.top

[U93] JS：模板字符串
来源：http://vxx.nanxinkj.top

`共 ${n} 条`
来源：http://yjk.chenjidiqi.icu

[U94] JS：箭头函数
来源：http://gyr.sysykeji.top

const double = x => x * 2;
来源：http://uex.redwolf501.top

[U95] JS：Promise 包装
来源：http://tbi.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://kbi.fengsongda.top

[U96] JS：async/await 与异常
来源：http://tui.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xig.yonumen.top

[U97] JS：并发请求
来源：http://lza.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://cec.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://jce.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vla.hcnkem.com

[U99] JS：事件监听
来源：http://seb.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://glt.shuidangran.top

[U100] JS：DOM 查询
来源：http://vny.tanke756.top

document.querySelector(".item")
来源：http://bum.chenlongwang.top

[U101] JS：classList 操作
来源：http://sop.tian-w.cn

el.classList.toggle("active")
来源：http://wwo.jyoumei.cn

[U102] JS：本地存储
来源：http://lzs.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tmv.yonumen.top

[U103] JS：定时器
来源：http://mjx.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uts.andypj.xyz

[U104] JS：防抖
来源：http://gwn.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwz.tanke756.top

[U105] JS：节流
来源：http://wfd.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vkf.sufxvd.cn

[U106] JS：日期格式化
来源：http://tho.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://imh.yonumen.top

[U107] JS：数字千分位
来源：http://axm.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://shn.0kj1m.cn

[U108] JS：随机整数
来源：http://ssl.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zzm.jianghu66.top

[U109] JS：数组分组
来源：http://qqw.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://hke.hywenlv.cn

[U110] JS：数组分块
来源：http://svm.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wzt.hnqzz.top

[U111] JS：对象转 Map
来源：http://rec.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://hih.316326.xyz

[U112] JS：字符串补位
来源：http://xjm.zdbjq.cn

"7".padStart(3, "0")
来源：http://sou.ivvv.top

[U113] JS：正则替换全部
来源：http://msa.jqgfzy.top

s.replaceAll("a", "b")
来源：http://qxb.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://hnf.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://nrm.cqqwz.cn

[U115] JS：生成 UUID
来源：http://lrd.feifeiyinyue.top

crypto.randomUUID()
来源：http://cti.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://lxf.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://jln.hesvh.cn

[U117] JS：单元测试
来源：http://tol.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://tlo.yfazqb.com

[U118] JS：开发服务器
来源：http://rxf.sweek.top

npm i -D vite;  npx vite
来源：http://gbj.fktsv.cn

[U119] JS：生产构建
来源：http://che.yangfankeji.com

npx vite build
来源：http://cqs.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://fpy.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://rqi.feifeiyinyue.top

================================================================================
来源：http://vsq.zdqjudy.top

统计汇总
来源：http://xpn.pengpengdd.cyou

================================================================================
来源：http://omd.sweek.top

按语言统计（条）：
来源：http://ybv.tian-w.cn

Python ......... 252
来源：http://tti.vqdsnc.cn

PHP ............ 252
来源：http://ebk.epnwcf.com

JavaScript ..... 252
来源：http://svn.fehbvm.com

TypeScript ..... 212
来源：http://dwz.jianghu66.top

Java ........... 212
来源：http://xid.guowangkeji.top

Go ............. 212
来源：http://btx.c1oappe.top

Ruby ........... 212
来源：http://vtv.aibaodan.cn

C# ............. 212
来源：http://fjh.sxryk.cn

C .............. 30
来源：http://gcm.xingfuxueyuan.xyz

C++ ............ 30
来源：http://ipr.shanyushiyangkeji.top

SQL ............ 90
来源：http://mhr.cashguo.top

Bash ........... 80
来源：http://itf.snrcjt.cn

Kotlin ......... 15
来源：http://ytk.mhx1999.top

Swift .......... 15
来源：http://kvx.haohaochexian.top

Lua ............ 10
来源：http://hkw.birdmap.top

Perl ........... 10
来源：http://msg.guannengcc.top

Scala .......... 10
来源：http://kma.chenlongwang.top

------------------------------------
来源：http://yfv.andypj.xyz

合计 ........... 2106 条
来源：http://vii.shanyushiyangtech.top

按章节统计：
来源：http://vkq.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ply.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fau.jyoumei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lbh.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://utu.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dla.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gtl.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gjb.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://idx.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bwn.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dvm.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://puw.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ghu.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gml.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cql.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fgi.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cnw.zycfv.cn

Q SQL 专题                              90
来源：http://dzz.gaohongyu789.top

R Bash 专题                             80
来源：http://tlc.cdnleiting.top

S C / C++ 专题                          60
来源：http://nch.hammf.cn

T 其他语言补充                          60
来源：http://rpe.birdmap.top

U 高频实用片段                         120
来源：http://hyz.fengsongda.top

------------------------------------
来源：http://uqu.nanxinkj.top

合计                                  2106 条
来源：http://nnm.tanke756.top

--------------------------------------------------------------------------------
来源：http://fsa.yangfankeji.com

使用提醒
来源：http://cuf.hammf.cn

--------------------------------------------------------------------------------
来源：http://rwb.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cza.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://swg.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jsg.jqgfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://euw.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fko.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://bwp.0kj1m.cn

================================================================================
来源：http://kmg.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ggu.c1oappe.top

Common Programming Examples Cheat Book
来源：http://hqt.c1oappe.top

================================================================================
来源：http://pje.hnxiangtu.top

【收录内容】
来源：http://hvq.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://byi.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gvl.mhx1999.top

SQL · Bash · C · C++
来源：http://zwt.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ufv.cashguo.top

【使用说明】
来源：http://jot.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wxs.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mes.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ypx.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ces.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hti.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ggm.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://utt.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nkc.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dma.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kme.c1oappe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rqe.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ogc.daria6918.cn

【文件统计】
来源：http://sfk.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://imo.havefunace.top

--------------------------------------------------------------------------------
来源：http://vth.jinghuilouyu.cn

目  录
来源：http://zfa.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://ayf.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://onf.zhongyouzk.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fuo.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mft.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ybs.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fcd.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xpe.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://osg.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://acs.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qsh.52xcode.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vyz.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xwz.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://prb.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tet.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dci.guowangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hjl.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wbw.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oad.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ucf.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://arp.pengpengdd.cyou

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wgq.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://djx.hongshengwenyu.top

================================================================================
来源：http://kep.chenzaomai.com

A. 基础语法与类型
来源：http://pgg.ywan-chungtsiang.top

================================================================================
来源：http://tbd.jinqigfzy.top

[A01] Hello World
来源：http://znj.ehwqpu.com

Py:   print("Hello, World!")
来源：http://ryj.zycfv.cn

PHP:  echo "Hello, World!";
来源：http://oeu.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://bgq.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vcf.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://pnk.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://zho.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://yby.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yau.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://ksc.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nhg.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ags.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lse.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://abz.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://fey.shanyushiyangtech.top

Go:   name := "Alex"; age := 20
来源：http://sha.c1oappe.top

Ruby: name = "Alex"; age = 20
来源：http://xlq.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kda.svipenyu.cn

[A03] 常量定义
来源：http://fky.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nye.yj202588.top

PHP:  const PI = 3.14159;
来源：http://ykc.daria6918.cn

JS:   const PI = 3.14159;
来源：http://gix.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://ofk.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://way.mhx1999.top

Go:   const PI = 3.14159
来源：http://roa.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://hsl.havefunace.top

C#:   const double PI = 3.14159;
来源：http://jih.fehbvm.com

[A04] 判断变量类型
来源：http://ecb.nanxuanxn.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ivz.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yfa.hongshengwenyu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://muk.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://bpq.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jbe.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uty.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://crd.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://vot.daria6918.cn

[A05] 整数除法与取模
来源：http://llo.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lif.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ook.ywan-chungtsiang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fud.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gjq.feifeiyinyue.top

Java: 7 / 2; 7 % 2
来源：http://wox.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://jcn.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://ysd.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://xdb.guannengcc.top

[A06] 字符串转数字
来源：http://zpz.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://qve.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kuc.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sli.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://dhy.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://elz.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yww.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://aux.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aor.smart0.xyz

[A07] 数字转字符串
来源：http://sgh.chenlongwang.top

Py:   str(42)
来源：http://qdf.hywenlv.cn

PHP:  (string) 42; strval(42)
来源：http://vde.yangfankeji.com

JS:   String(42); (42).toString()
来源：http://pnj.hysaishi.cn

TS:   String(42)
来源：http://ldn.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://lyc.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://kss.zhoulong.xyz

Ruby: 42.to_s
来源：http://elh.jqgfzy.top

C#:   42.ToString()
来源：http://qlk.jlsjyb.cn

[A08] 取整与四舍五入
来源：http://xht.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zqf.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qww.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://awz.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rjs.ivvv.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xjr.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vrz.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fyu.316326.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sds.hnxiangtu.top

[A09] 绝对值与最大最小值
来源：http://smz.yj202588.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kgv.feifeiyinyue.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oqb.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lda.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://viz.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kag.yueranfly.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ezx.chenlongwang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vfh.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mpy.tarul.cn

[A10] 生成随机数
来源：http://qmg.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://osx.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://ipf.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://slz.fanxiaobao.xyz


<!-- 参考信息 -->