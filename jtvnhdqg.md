代发 wailian999

[U65] PHP：会话
来源：http://htx.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gic.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://vir.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kkq.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://pgj.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fru.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://frq.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rqg.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://kwe.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rmt.andypj.xyz

[U70] PHP：PDO 事务
来源：http://ght.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rwj.bbcook.cn

[U71] PHP：抛出异常
来源：http://rjy.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://tos.ppjwa.cn

[U72] PHP：写错误日志
来源：http://ooq.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://fox.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://qjv.sweek.top

parse_ini_file("config.ini", true)
来源：http://unv.jianghu66.top

[U74] PHP：读取环境变量
来源：http://kyj.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://dev.gotoacloud.top

[U75] PHP：依赖注入
来源：http://sdi.cashguo.top

composer require psr/container
来源：http://kky.fengsongda.top

[U76] PHP：简单路由
来源：http://ici.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://czt.iojbl.cn

[U77] PHP：模板渲染
来源：http://ere.zycfv.cn

composer require twig/twig
来源：http://xap.ivvv.top

[U78] PHP：单元测试
来源：http://zww.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://skw.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://sjr.yongpay.top

composer require --dev phpstan/phpstan
来源：http://rqv.uphjek.com

[U80] PHP：代码规范修复
来源：http://ycj.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://hlh.cashguo.top

[U81] JS：初始化项目
来源：http://mtb.ydzc1.top

npm init -y;  npm i express
来源：http://kqa.gzhubu.top

[U82] JS：package.json 脚本
来源：http://vpw.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cjd.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://ayl.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://oam.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://qfm.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://zhp.pycfn.com

[U85] JS：可选链
来源：http://vrk.shangyingyoupin.top

a?.b?.c
来源：http://pfv.0kj1m.cn

[U86] JS：空值合并
来源：http://bnw.shanyushiyangtech.top

a ?? b
来源：http://wjf.yanxiufei.cn

[U87] JS：解构默认值
来源：http://ydn.ppjwa.cn

const { a = 1, b = 2 } = obj;
来源：http://uwg.chenlongwang.top

[U88] JS：对象展开合并
来源：http://ufo.tianlin.xyz

{ ...a, ...b }
来源：http://zyt.ehwqpu.com

[U89] JS：数组去重
来源：http://apk.sjlbkw.cn

[...new Set(arr)]
来源：http://mwg.xinyue.icu

[U90] JS：数字数组排序
来源：http://cmr.gotoacloud.top

[...arr].sort((a, b) => a - b)
来源：http://zpd.tanke756.top

[U91] JS：对象键值遍历
来源：http://hmv.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ugq.daxiang520.top

[U92] JS：深拷贝
来源：http://apa.zycfv.cn

structuredClone(obj)
来源：http://kpl.yuxming.cn

[U93] JS：模板字符串
来源：http://pwa.guannengcc.top

`共 ${n} 条`
来源：http://yop.tian-w.cn

[U94] JS：箭头函数
来源：http://flw.ybcxt.top

const double = x => x * 2;
来源：http://nth.316326.xyz

[U95] JS：Promise 包装
来源：http://jgw.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://ybe.hammf.cn

[U96] JS：async/await 与异常
来源：http://vno.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cok.vqdsnc.cn

[U97] JS：并发请求
来源：http://amb.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nyx.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://fjc.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://moo.aibaodan.cn

[U99] JS：事件监听
来源：http://xou.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://rrp.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://gzk.fanxiaobao.xyz

document.querySelector(".item")
来源：http://efv.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://gnk.yvedp.cn

el.classList.toggle("active")
来源：http://rdh.jiagoushi.top

[U102] JS：本地存储
来源：http://lpf.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://csj.ctjpmb.com

[U103] JS：定时器
来源：http://kmc.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cic.yuxming.cn

[U104] JS：防抖
来源：http://dor.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dsl.aibaodan.cn

[U105] JS：节流
来源：http://wel.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kix.jqgfzy.top

[U106] JS：日期格式化
来源：http://hpm.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lwo.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://yso.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://huo.quarkkingdee.top

[U108] JS：随机整数
来源：http://bpu.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gmp.nwbrower.top

[U109] JS：数组分组
来源：http://flp.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://psk.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://sff.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pby.daria6918.cn

[U111] JS：对象转 Map
来源：http://ezm.zdqjudy.top

new Map(Object.entries(obj))
来源：http://kiy.zhengqikj.top

[U112] JS：字符串补位
来源：http://yjx.shzxlz.cn

"7".padStart(3, "0")
来源：http://trb.dashuyun.cn

[U113] JS：正则替换全部
来源：http://vuh.tarul.cn

s.replaceAll("a", "b")
来源：http://yeu.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://ouo.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vol.tarul.cn

[U115] JS：生成 UUID
来源：http://zmg.nwbrower.top

crypto.randomUUID()
来源：http://yyy.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://xyp.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://ajc.jinqigfzy.top

[U117] JS：单元测试
来源：http://pff.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://dty.sufxvd.cn

[U118] JS：开发服务器
来源：http://guc.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://lqd.yanxiufei.cn

[U119] JS：生产构建
来源：http://ktb.jinghuilouyu.cn

npx vite build
来源：http://nnt.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://weo.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://cgj.sysykeji.top

================================================================================
来源：http://mcm.ydjk.org.cn

统计汇总
来源：http://jue.nanxinkj.top

================================================================================
来源：http://oif.redwolf501.top

按语言统计（条）：
来源：http://spr.pengpengdd.cyou

Python ......... 252
来源：http://qas.ivvv.top

PHP ............ 252
来源：http://llv.jinqigfzy.top

JavaScript ..... 252
来源：http://asp.gotoacloud.top

TypeScript ..... 212
来源：http://hma.sxryk.cn

Java ........... 212
来源：http://wag.redwolf501.top

Go ............. 212
来源：http://sgm.hammf.cn

Ruby ........... 212
来源：http://qmu.gaohongyu789.top

C# ............. 212
来源：http://lrv.fehbvm.com

C .............. 30
来源：http://jnt.yuanzhike.top

C++ ............ 30
来源：http://ahj.cashguo.top

SQL ............ 90
来源：http://fyj.dashuyun.cn

Bash ........... 80
来源：http://uyf.zhixingplan.top

Kotlin ......... 15
来源：http://nhm.ehwqpu.com

Swift .......... 15
来源：http://php.cqqwz.cn

Lua ............ 10
来源：http://jra.shangyingyoupin.top

Perl ........... 10
来源：http://csu.cqqwz.cn

Scala .......... 10
来源：http://gei.zdqjudy.top

------------------------------------
来源：http://gxt.daria6918.cn

合计 ........... 2106 条
来源：http://xbe.yonumen.top

按章节统计：
来源：http://cjc.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dlc.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fdc.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xfy.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://emi.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vyg.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cho.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kem.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://faf.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eny.xziqi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nnj.bbcook.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kaz.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://etc.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kzb.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jeq.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rgj.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pjr.vehdjk.com

Q SQL 专题                              90
来源：http://svq.yj202588.top

R Bash 专题                             80
来源：http://tkk.sufxvd.cn

S C / C++ 专题                          60
来源：http://frd.sysykeji.top

T 其他语言补充                          60
来源：http://rei.shzxlz.cn

U 高频实用片段                         120
来源：http://qpl.jinqigfzy.top

------------------------------------
来源：http://bvg.c1oappe.top

合计                                  2106 条
来源：http://pvn.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://ppy.haohaochexian.top

使用提醒
来源：http://dbf.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://ntv.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://obn.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ttp.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mdm.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://iwt.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nub.jinghuilouyu.cn

—— 文件结束 ——
来源：http://cxi.sysykeji.top

================================================================================
来源：http://hvt.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://zzn.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://mnb.cheryme.top

================================================================================
来源：http://oeo.quarkkingdee.top

【收录内容】
来源：http://kfn.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lru.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xed.zhongyouzk.top

SQL · Bash · C · C++
来源：http://vsg.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mml.ydzc1.top

【使用说明】
来源：http://ndw.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ggu.nanxinkj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vit.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ycf.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gpr.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://swc.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gyh.bbcook.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sjj.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jju.vehdjk.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://txo.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ctq.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://byr.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jly.meibo888.top

【文件统计】
来源：http://fbq.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eaf.xziqi.cn

--------------------------------------------------------------------------------
来源：http://mpj.ydjk.org.cn

目  录
来源：http://srn.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://myd.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gxl.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cpn.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mip.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://liz.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qfk.ydzc1.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cze.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jmm.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wyh.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xci.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bzj.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jbt.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sky.andypj.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ykw.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pqj.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oea.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ivw.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mwa.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vcr.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jti.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lqh.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sjs.aibaodan.cn

================================================================================
来源：http://kex.yangfankeji.com

A. 基础语法与类型
来源：http://jtl.fehbvm.com

================================================================================
来源：http://htd.ydzc1.top

[A01] Hello World
来源：http://eiq.ctjpmb.com

Py:   print("Hello, World!")
来源：http://jxb.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://umy.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://wwq.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wvw.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://rqt.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://aqy.cashguo.top

Ruby: puts "Hello, World!"
来源：http://fig.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://rfx.zycfv.cn

[A02] 变量声明与赋值
来源：http://dkz.xuetiantiany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mqm.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fqx.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://bdm.52xcode.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sjx.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://mmw.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://hji.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://bwu.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://wbm.52xcode.cn

[A03] 常量定义
来源：http://epr.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fwi.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://lxe.jyoumei.cn

JS:   const PI = 3.14159;
来源：http://pxd.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://suw.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://inp.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://wud.yueranfly.top

Ruby: PI = 3.14159
来源：http://ura.feifeiyinyue.top

C#:   const double PI = 3.14159;
来源：http://ixr.ydjk.org.cn

[A04] 判断变量类型
来源：http://njo.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pyn.sweek.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hub.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ffe.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://qgm.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://atj.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://iwz.gogol.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wdm.jlsjyb.cn

C#:   x.GetType().Name; x is int
来源：http://yuf.xylfe.cn

[A05] 整数除法与取模
来源：http://mog.pycfn.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cny.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ygu.mhx1999.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pij.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://icn.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://kxs.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://ptb.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://owg.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://vvl.ydzc1.top

[A06] 字符串转数字
来源：http://eut.quarkkingdee.top

Py:   int("42"); float("3.14")
来源：http://shm.epnwcf.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rfs.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ppm.bbcook.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tsm.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kkt.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sfh.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bid.fanxiaobao.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pzd.zhixingplan.top

[A07] 数字转字符串
来源：http://xva.shanyushiyangkeji.top

Py:   str(42)
来源：http://mtu.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://pfj.gzhubu.top

JS:   String(42); (42).toString()
来源：http://zru.yangfankeji.com

TS:   String(42)
来源：http://vts.smart0.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ikh.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://quj.hywenlv.cn

Ruby: 42.to_s
来源：http://eou.kuanghao11.cn

C#:   42.ToString()
来源：http://msm.fengsongda.top

[A08] 取整与四舍五入
来源：http://kgt.cashguo.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kpu.yueranfly.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bwg.guannengcc.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://avf.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bxe.shanyushiyangtech.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qzp.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eqk.gaohongyu789.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ztf.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lgt.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://yqb.fengsongda.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://put.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jlb.c1oappe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fdw.jlsjyb.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vwy.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xjg.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gza.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fpd.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mqh.sysykeji.top


<!-- 参考信息 -->