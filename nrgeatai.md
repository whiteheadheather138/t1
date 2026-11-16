代发 wailian999

[U67] PHP：处理文件上传
来源：http://ian.hnqzz.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bzv.meibo888.top

[U68] PHP：PDO 连接
来源：http://pjb.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tjr.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://fmd.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nai.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://gaw.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://amh.gotoacloud.top

[U71] PHP：抛出异常
来源：http://kpr.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://rdj.bjfxy.top

[U72] PHP：写错误日志
来源：http://sew.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://hzj.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://scp.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://mxw.ivvv.top

[U74] PHP：读取环境变量
来源：http://fum.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://hnn.sxryk.cn

[U75] PHP：依赖注入
来源：http://kod.svipenyu.cn

composer require psr/container
来源：http://ulm.yj20258888.top

[U76] PHP：简单路由
来源：http://uzl.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mvb.ppjwa.cn

[U77] PHP：模板渲染
来源：http://pqs.yuanzhike.top

composer require twig/twig
来源：http://yzi.vqdsnc.cn

[U78] PHP：单元测试
来源：http://agg.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://sgd.tarul.cn

[U79] PHP：静态分析
来源：http://khh.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://uvv.birdmap.top

[U80] PHP：代码规范修复
来源：http://fdi.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tst.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://fzr.quarkkingdee.top

npm init -y;  npm i express
来源：http://cni.pycfn.com

[U82] JS：package.json 脚本
来源：http://wyn.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tsn.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://btj.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hjm.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://gbe.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://itj.mhx1999.top

[U85] JS：可选链
来源：http://cem.chenlongwang.top

a?.b?.c
来源：http://fjg.jinqigufen.top

[U86] JS：空值合并
来源：http://uxp.shuidangran.top

a ?? b
来源：http://iel.meibo888.top

[U87] JS：解构默认值
来源：http://kah.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://zaa.yonumen.top

[U88] JS：对象展开合并
来源：http://ntv.shanyushiyangtech.top

{ ...a, ...b }
来源：http://vmh.hcnkem.com

[U89] JS：数组去重
来源：http://anu.ydjk.org.cn

[...new Set(arr)]
来源：http://lvi.yj20258888.top

[U90] JS：数字数组排序
来源：http://rrc.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://wgy.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://psh.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://enz.jqgufenzy.top

[U92] JS：深拷贝
来源：http://mfc.sufxvd.cn

structuredClone(obj)
来源：http://xdr.yvedp.cn

[U93] JS：模板字符串
来源：http://uic.havefunace.top

`共 ${n} 条`
来源：http://you.cheryme.top

[U94] JS：箭头函数
来源：http://jyb.yueranfly.top

const double = x => x * 2;
来源：http://gio.tianlin.xyz

[U95] JS：Promise 包装
来源：http://kek.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://riv.xziqi.cn

[U96] JS：async/await 与异常
来源：http://kvy.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qao.yuanzhike.top

[U97] JS：并发请求
来源：http://rqm.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bgm.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://zbd.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ufx.aizwys.cn

[U99] JS：事件监听
来源：http://pvy.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://azu.hfpthk.cn

[U100] JS：DOM 查询
来源：http://szb.xuetiantiany.cn

document.querySelector(".item")
来源：http://jak.snrcjt.cn

[U101] JS：classList 操作
来源：http://rbb.iojbl.cn

el.classList.toggle("active")
来源：http://ctf.svipenyu.cn

[U102] JS：本地存储
来源：http://kap.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wbz.meibo888.top

[U103] JS：定时器
来源：http://nmm.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lqn.jinqigufen.top

[U104] JS：防抖
来源：http://glv.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygz.tanke756.top

[U105] JS：节流
来源：http://fyc.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lcw.hcnkem.com

[U106] JS：日期格式化
来源：http://ipy.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qlf.yj202588.top

[U107] JS：数字千分位
来源：http://ure.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pqi.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://cjz.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iwp.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://tph.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://hqh.0kj1m.cn

[U110] JS：数组分块
来源：http://pya.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dmu.havefunace.top

[U111] JS：对象转 Map
来源：http://dvg.chenlongwang.top

new Map(Object.entries(obj))
来源：http://iyp.guannengcc.top

[U112] JS：字符串补位
来源：http://bld.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://bby.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://scu.fktsv.cn

s.replaceAll("a", "b")
来源：http://gou.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://qia.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xow.chenlongwang.top

[U115] JS：生成 UUID
来源：http://apf.yvedp.cn

crypto.randomUUID()
来源：http://tkl.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://xda.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://imn.52xcode.cn

[U117] JS：单元测试
来源：http://cua.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://kdh.xinyue.icu

[U118] JS：开发服务器
来源：http://xsr.zycfv.cn

npm i -D vite;  npx vite
来源：http://mhd.tian-w.cn

[U119] JS：生产构建
来源：http://qkj.guowangkeji.top

npx vite build
来源：http://iez.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://bhu.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://zhj.fengsongda.top

================================================================================
来源：http://kql.zdbjq.cn

统计汇总
来源：http://vdi.kuanghao11.cn

================================================================================
来源：http://led.ydzc1.top

按语言统计（条）：
来源：http://ktu.pengpengdd.cyou

Python ......... 252
来源：http://zkr.dianchejie.cn

PHP ............ 252
来源：http://srp.fengsongda.top

JavaScript ..... 252
来源：http://csa.yanxiufei.cn

TypeScript ..... 212
来源：http://lnx.hongshengwenyu.top

Java ........... 212
来源：http://ouc.shanyushiyangkeji.top

Go ............. 212
来源：http://zno.jinghuilouyu.cn

Ruby ........... 212
来源：http://tjz.xuanzx.com

C# ............. 212
来源：http://oyw.yanxiufei.cn

C .............. 30
来源：http://dtx.bbcook.cn

C++ ............ 30
来源：http://utf.zycfv.cn

SQL ............ 90
来源：http://gzx.xylfe.cn

Bash ........... 80
来源：http://jxg.aibaodan.cn

Kotlin ......... 15
来源：http://ihq.chenzaomai.com

Swift .......... 15
来源：http://pgh.pycfn.com

Lua ............ 10
来源：http://jlf.zhengqikj.top

Perl ........... 10
来源：http://exm.cheryme.top

Scala .......... 10
来源：http://chh.yuxming.cn

------------------------------------
来源：http://gpk.daxiang520.top

合计 ........... 2106 条
来源：http://mzl.hesvh.cn

按章节统计：
来源：http://yci.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bxd.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gyb.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sxt.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lhd.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nwb.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nxd.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mvh.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hbc.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qov.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rnu.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hlu.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://keb.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bsq.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ofs.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fym.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xzy.cdnleiting.top

Q SQL 专题                              90
来源：http://vio.c1oappe.top

R Bash 专题                             80
来源：http://vsr.hcnkem.com

S C / C++ 专题                          60
来源：http://cdb.aibaodan.cn

T 其他语言补充                          60
来源：http://cgi.haohaochexian.top

U 高频实用片段                         120
来源：http://rls.chenlongwang.top

------------------------------------
来源：http://jpz.ivvv.top

合计                                  2106 条
来源：http://sqt.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://zun.jinqigfzy.top

使用提醒
来源：http://per.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://hpd.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xjq.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ohv.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gol.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yub.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qhs.hywenlv.cn

—— 文件结束 ——
来源：http://etk.jinyuanbaomall.cn

================================================================================
来源：http://gml.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://ruj.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://vlq.vqdsnc.cn

================================================================================
来源：http://mvq.0kj1m.cn

【收录内容】
来源：http://xvo.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://eqs.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nmj.zhixingplan.top

SQL · Bash · C · C++
来源：http://kqw.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://udb.zhongyouzk.top

【使用说明】
来源：http://guv.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lfq.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vgy.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gxh.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cgt.guowangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rxk.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oyz.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lph.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://txh.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://igf.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rtc.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rxr.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zgp.yuanzhike.top

【文件统计】
来源：http://vhc.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bsb.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://uex.nanxinkj.top

目  录
来源：http://xir.sysykeji.top

--------------------------------------------------------------------------------
来源：http://irq.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iab.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gzx.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aqz.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bya.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bwf.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sek.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ila.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ohh.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fih.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fug.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sly.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zvu.cdnleiting.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oav.guannengcc.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rly.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vwe.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ljv.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xdt.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xst.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jqx.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jep.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sxw.c1oappe.top

================================================================================
来源：http://uej.yj202588.top

A. 基础语法与类型
来源：http://rnj.nanxinkj.top

================================================================================
来源：http://cju.pycfn.com

[A01] Hello World
来源：http://mys.smart0.xyz

Py:   print("Hello, World!")
来源：http://ihg.aibaodan.cn

PHP:  echo "Hello, World!";
来源：http://boj.tarul.cn

JS:   console.log("Hello, World!");
来源：http://enl.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://brn.birdmap.top

Java: System.out.println("Hello, World!");
来源：http://lxt.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://slz.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://drl.jlsjyb.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uik.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://sdh.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wis.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://vhn.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://crc.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ljp.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://eya.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://cex.9152youxi.cn

Ruby: name = "Alex"; age = 20
来源：http://tvd.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://tbc.guowangkeji.top

[A03] 常量定义
来源：http://njh.nwbrower.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vrj.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://fgd.tarul.cn

JS:   const PI = 3.14159;
来源：http://nzf.zhaomingkeji.xyz

TS:   const PI: number = 3.14159;
来源：http://jsd.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://kaq.hammf.cn

Go:   const PI = 3.14159
来源：http://ujv.pengpengdd.cyou

Ruby: PI = 3.14159
来源：http://vkg.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://rro.sweek.top

[A04] 判断变量类型
来源：http://haa.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bop.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://skz.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://raj.sweek.top

TS:   typeof x; x instanceof Date
来源：http://xeh.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://euz.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://kme.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kle.nanxinkj.top

C#:   x.GetType().Name; x is int
来源：http://yud.gotoacloud.top

[A05] 整数除法与取模
来源：http://afv.9152youxi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://prb.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hkj.cucudq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://apu.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vij.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://ric.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://wik.fehbvm.com

Ruby: 7 / 2; 7 % 2
来源：http://zir.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://tip.52xcode.cn

[A06] 字符串转数字
来源：http://jbp.yfazqb.com

Py:   int("42"); float("3.14")
来源：http://ari.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://din.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eva.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ijs.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://epm.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mki.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mql.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ydh.snrcjt.cn

[A07] 数字转字符串
来源：http://rjf.jinqigufen.top

Py:   str(42)
来源：http://xdo.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://fiu.havefunace.top

JS:   String(42); (42).toString()
来源：http://wmr.kuanghao11.cn

TS:   String(42)
来源：http://odk.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://bvm.aibaodan.cn

Go:   strconv.Itoa(42)
来源：http://guk.iojbl.cn

Ruby: 42.to_s
来源：http://vyz.zdbjq.cn

C#:   42.ToString()
来源：http://bse.guowangkeji.top

[A08] 取整与四舍五入
来源：http://nht.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kwj.yonumen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wdg.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ujl.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cwh.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gbd.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zhs.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tew.zhiwuduotai.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ugt.yj202588.top

[A09] 绝对值与最大最小值
来源：http://jlw.jqgfzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rvl.xinyue.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hfc.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tfz.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uwf.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mmd.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://thk.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kok.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rcg.vqdsnc.cn

[A10] 生成随机数
来源：http://thm.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://xcy.jinqigufen.top

PHP:  random_int(1, 100);
来源：http://jpi.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ybp.316326.xyz


<!-- 参考信息 -->