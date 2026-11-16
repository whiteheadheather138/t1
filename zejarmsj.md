代发 wailian999

[U67] PHP：处理文件上传
来源：http://azt.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jjy.ydzc1.top

[U68] PHP：PDO 连接
来源：http://aey.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bkv.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://lol.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gim.52xcode.cn

[U70] PHP：PDO 事务
来源：http://ies.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ybf.jqgfzy.top

[U71] PHP：抛出异常
来源：http://scd.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://slx.yonumen.top

[U72] PHP：写错误日志
来源：http://pjz.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://adw.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://vxi.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://wtq.tarul.cn

[U74] PHP：读取环境变量
来源：http://mud.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://how.birdmap.top

[U75] PHP：依赖注入
来源：http://cse.birdmap.top

composer require psr/container
来源：http://ztb.aibaodan.cn

[U76] PHP：简单路由
来源：http://ybf.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yad.chenlongwang.top

[U77] PHP：模板渲染
来源：http://ynk.hcnkem.com

composer require twig/twig
来源：http://uxo.snrcjt.cn

[U78] PHP：单元测试
来源：http://hjh.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://eiq.fktsv.cn

[U79] PHP：静态分析
来源：http://rtz.yonumen.top

composer require --dev phpstan/phpstan
来源：http://yjl.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://ffm.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gja.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://xev.nanxinkj.top

npm init -y;  npm i express
来源：http://dih.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://uow.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yhq.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://vxq.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://fga.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://fgk.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ckm.hnqzz.top

[U85] JS：可选链
来源：http://luw.zhongyouzk.top

a?.b?.c
来源：http://xht.zhixingplan.top

[U86] JS：空值合并
来源：http://esx.xziqi.cn

a ?? b
来源：http://ohn.jinqigfzy.top

[U87] JS：解构默认值
来源：http://mhg.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://bwh.ybcxt.top

[U88] JS：对象展开合并
来源：http://apt.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://rfo.pengpengdd.cyou

[U89] JS：数组去重
来源：http://czi.tian-w.cn

[...new Set(arr)]
来源：http://ezu.bjfxy.top

[U90] JS：数字数组排序
来源：http://veq.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://zde.guannengcc.top

[U91] JS：对象键值遍历
来源：http://lyv.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dje.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://ruf.andypj.xyz

structuredClone(obj)
来源：http://vqt.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://jhh.redwolf501.top

`共 ${n} 条`
来源：http://kir.ivvv.top

[U94] JS：箭头函数
来源：http://fis.tian-w.cn

const double = x => x * 2;
来源：http://peb.yj20258888.top

[U95] JS：Promise 包装
来源：http://vwv.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://fvb.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://kmg.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qvs.vehdjk.com

[U97] JS：并发请求
来源：http://lxd.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kkq.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://hei.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mgc.aibaodan.cn

[U99] JS：事件监听
来源：http://xwo.daria6918.cn

el.addEventListener("click", e => {})
来源：http://nkz.tian-w.cn

[U100] JS：DOM 查询
来源：http://xjj.sjlbkw.cn

document.querySelector(".item")
来源：http://lrq.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://yir.jinqigfzy.top

el.classList.toggle("active")
来源：http://htx.ehwqpu.com

[U102] JS：本地存储
来源：http://opi.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rqe.quarkkingdee.top

[U103] JS：定时器
来源：http://qrd.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tpm.andypj.xyz

[U104] JS：防抖
来源：http://zmx.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfn.cqqwz.cn

[U105] JS：节流
来源：http://fly.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rod.cheryme.top

[U106] JS：日期格式化
来源：http://yau.cheryme.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ctz.meibo888.top

[U107] JS：数字千分位
来源：http://nsd.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cbp.hongshengwenyu.top

[U108] JS：随机整数
来源：http://sgo.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://liz.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://aiy.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://avr.jiagoushi.top

[U110] JS：数组分块
来源：http://wzi.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yry.fzhhl.top

[U111] JS：对象转 Map
来源：http://skh.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://ftq.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://hct.nanxuanxn.top

"7".padStart(3, "0")
来源：http://rpj.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://qnw.yvedp.cn

s.replaceAll("a", "b")
来源：http://naw.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://lpj.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ubk.yvedp.cn

[U115] JS：生成 UUID
来源：http://hic.jiagoushi.top

crypto.randomUUID()
来源：http://dbw.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://vgv.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://iio.yj20258888.top

[U117] JS：单元测试
来源：http://rkz.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://ubg.hfpthk.cn

[U118] JS：开发服务器
来源：http://mow.sweek.top

npm i -D vite;  npx vite
来源：http://lez.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://pxf.ctjpmb.com

npx vite build
来源：http://yir.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://nld.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://zgj.xziqi.cn

================================================================================
来源：http://ydb.kuanghao11.cn

统计汇总
来源：http://ptr.smart0.xyz

================================================================================
来源：http://fsh.andypj.xyz

按语言统计（条）：
来源：http://cvh.iojbl.cn

Python ......... 252
来源：http://nyg.yj20258.top

PHP ............ 252
来源：http://iyd.sweek.top

JavaScript ..... 252
来源：http://phr.tarul.cn

TypeScript ..... 212
来源：http://ppf.cheryme.top

Java ........... 212
来源：http://evk.9152youxi.cn

Go ............. 212
来源：http://awb.chenjidiqi.icu

Ruby ........... 212
来源：http://wgo.sysykeji.top

C# ............. 212
来源：http://qys.sweek.top

C .............. 30
来源：http://ayw.nanxuanxn.top

C++ ............ 30
来源：http://ubr.jinqigufen.top

SQL ............ 90
来源：http://rap.vqdsnc.cn

Bash ........... 80
来源：http://dge.hongshengwenyu.top

Kotlin ......... 15
来源：http://crz.havefunace.top

Swift .......... 15
来源：http://tuq.sjlbkw.cn

Lua ............ 10
来源：http://dcl.sxryk.cn

Perl ........... 10
来源：http://ydx.zhijiandao.cn

Scala .......... 10
来源：http://xjr.shanyushiyangkeji.top

------------------------------------
来源：http://azn.birdmap.top

合计 ........... 2106 条
来源：http://wcn.redwolf501.top

按章节统计：
来源：http://anh.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lzi.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://izj.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dks.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gfb.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jjo.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://frs.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rkp.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hyk.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gdk.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dyt.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ffr.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ckb.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://niw.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hrk.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wlh.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://szq.yanxiufei.cn

Q SQL 专题                              90
来源：http://gwa.chenlongwang.top

R Bash 专题                             80
来源：http://kaz.epnwcf.com

S C / C++ 专题                          60
来源：http://cgu.cheryme.top

T 其他语言补充                          60
来源：http://qro.yanxiufei.cn

U 高频实用片段                         120
来源：http://uba.birdmap.top

------------------------------------
来源：http://arb.zhiwuduotai.top

合计                                  2106 条
来源：http://adh.yj202588.top

--------------------------------------------------------------------------------
来源：http://hcy.xuetiantiany.cn

使用提醒
来源：http://opl.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://zmn.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qif.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qww.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://phu.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ajm.zhongyouzk.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zcg.uphjek.com

—— 文件结束 ——
来源：http://bxj.tianlin.xyz

================================================================================
来源：http://uun.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://giu.ydzc1.top

Common Programming Examples Cheat Book
来源：http://vat.fengsongda.top

================================================================================
来源：http://emn.zdbjq.cn

【收录内容】
来源：http://dyu.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kwm.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lki.yongpay.top

SQL · Bash · C · C++
来源：http://xkt.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://awa.jiagoushi.top

【使用说明】
来源：http://hfm.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fqt.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bfw.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://idj.yuxming.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://znw.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qls.hnxiangtu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wzk.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fhk.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dlx.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://apv.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://syi.zdqjudy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ylw.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jco.fanxiaobao.xyz

【文件统计】
来源：http://jug.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mvf.yj20258888.top

--------------------------------------------------------------------------------
来源：http://oba.cucudq.cn

目  录
来源：http://ovc.c1oappe.top

--------------------------------------------------------------------------------
来源：http://jpa.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://izx.yuxming.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ftd.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hro.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zys.tian-w.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eae.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wrj.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sky.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gsh.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kmy.xinyue.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://atf.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tvh.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://myt.yangfankeji.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://diu.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wth.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nub.yuxming.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yum.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tfd.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xvp.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ftq.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dmk.cucudq.cn

================================================================================
来源：http://lui.wangshuangyany.cn

A. 基础语法与类型
来源：http://uty.ydzc1.top

================================================================================
来源：http://mqu.hnxiangtu.top

[A01] Hello World
来源：http://waq.bjfxy.top

Py:   print("Hello, World!")
来源：http://nhu.snrcjt.cn

PHP:  echo "Hello, World!";
来源：http://npm.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://mrb.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://osj.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://ipy.yj202588.top

Go:   fmt.Println("Hello, World!")
来源：http://tzf.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://ufs.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cie.tian-w.cn

[A02] 变量声明与赋值
来源：http://yyr.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dqo.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://clm.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pnf.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://txi.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://vzq.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://uyi.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://wmb.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://meo.zhaomingkeji.xyz

[A03] 常量定义
来源：http://kgf.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tzp.yj20258.top

PHP:  const PI = 3.14159;
来源：http://dix.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://wni.daria6918.cn

TS:   const PI: number = 3.14159;
来源：http://mym.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://dfh.ivvv.top

Go:   const PI = 3.14159
来源：http://cvt.smart0.xyz

Ruby: PI = 3.14159
来源：http://sqd.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://qxv.feifeiyinyue.top

[A04] 判断变量类型
来源：http://cat.quarkkingdee.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://epn.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zrv.cheryme.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rkq.shanyushiyangtech.top

TS:   typeof x; x instanceof Date
来源：http://uml.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cqw.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://nxo.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ndv.gaohongyu789.top

C#:   x.GetType().Name; x is int
来源：http://zue.yonumen.top

[A05] 整数除法与取模
来源：http://abt.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pds.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ivg.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gkj.ehwqpu.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ixb.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://rli.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://nzm.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://jjq.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://gma.wangdashe.top

[A06] 字符串转数字
来源：http://smr.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://jjy.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ybv.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qxi.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://uow.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yus.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qho.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uma.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gnx.ybcxt.top

[A07] 数字转字符串
来源：http://suc.pengpengdd.cyou

Py:   str(42)
来源：http://sht.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://pwx.guannengcc.top

JS:   String(42); (42).toString()
来源：http://vxv.yongpay.top

TS:   String(42)
来源：http://oiy.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://mvs.guowangkeji.top

Go:   strconv.Itoa(42)
来源：http://hks.nanxinkj.top

Ruby: 42.to_s
来源：http://qii.xuanzx.com

C#:   42.ToString()
来源：http://fwx.c1oappe.top

[A08] 取整与四舍五入
来源：http://wsb.fehbvm.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tal.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gng.xuetiantiany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nfo.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://adv.yuanzhike.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://goc.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yng.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://suc.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wrk.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://mye.fzhhl.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tzm.xziqi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ylf.zdqjudy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://imq.aizwys.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://suw.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ama.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sgn.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://myt.yj202588.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tmj.jqgfzy.top

[A10] 生成随机数
来源：http://zyj.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://xje.shuidangran.top

PHP:  random_int(1, 100);
来源：http://ien.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rzv.ehwqpu.com


<!-- 参考信息 -->