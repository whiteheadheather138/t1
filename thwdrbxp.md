代发 wailian999

[U67] PHP：处理文件上传
来源：http://nge.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ctv.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://sey.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ayh.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://lxm.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fvq.fehbvm.com

[U70] PHP：PDO 事务
来源：http://maz.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ycx.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://bmw.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://xuw.cdnleiting.top

[U72] PHP：写错误日志
来源：http://cva.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://tee.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://arp.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://zxo.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://uem.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://ngb.bbcook.cn

[U75] PHP：依赖注入
来源：http://nvq.pycfn.com

composer require psr/container
来源：http://wam.hnqzz.top

[U76] PHP：简单路由
来源：http://avv.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xbn.hnqzz.top

[U77] PHP：模板渲染
来源：http://gan.xinyue.icu

composer require twig/twig
来源：http://dvw.yj20258888.top

[U78] PHP：单元测试
来源：http://xrc.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://wmh.tianlin.xyz

[U79] PHP：静态分析
来源：http://ael.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://nnm.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://lac.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sfv.gzhubu.top

[U81] JS：初始化项目
来源：http://oie.jinqigufen.top

npm init -y;  npm i express
来源：http://kcj.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://tzq.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rwp.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://xtx.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://muv.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://wkl.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lse.jiagoushi.top

[U85] JS：可选链
来源：http://dcj.zhijiandao.cn

a?.b?.c
来源：http://vih.aibaodan.cn

[U86] JS：空值合并
来源：http://ttc.aibaodan.cn

a ?? b
来源：http://xlg.ehwqpu.com

[U87] JS：解构默认值
来源：http://sfv.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://vuq.jiagoushi.top

[U88] JS：对象展开合并
来源：http://trt.bjfxy.top

{ ...a, ...b }
来源：http://ufo.xuanzx.com

[U89] JS：数组去重
来源：http://rjw.snrcjt.cn

[...new Set(arr)]
来源：http://oip.svipenyu.cn

[U90] JS：数字数组排序
来源：http://nqa.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://nza.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://bck.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mqh.shzxlz.cn

[U92] JS：深拷贝
来源：http://qoq.zdbjq.cn

structuredClone(obj)
来源：http://naj.wangdashe.top

[U93] JS：模板字符串
来源：http://hqo.tianlin.xyz

`共 ${n} 条`
来源：http://qie.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://hsp.aizwys.cn

const double = x => x * 2;
来源：http://ybk.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://njo.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://gfp.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://mci.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nfj.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://mqq.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://knt.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://ugt.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jdx.sjlbkw.cn

[U99] JS：事件监听
来源：http://gyb.hesvh.cn

el.addEventListener("click", e => {})
来源：http://mpj.52xcode.cn

[U100] JS：DOM 查询
来源：http://sev.sysykeji.top

document.querySelector(".item")
来源：http://kxt.jiagoushi.top

[U101] JS：classList 操作
来源：http://llj.daxiang520.top

el.classList.toggle("active")
来源：http://slg.fengsongda.top

[U102] JS：本地存储
来源：http://uml.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ojs.52xcode.cn

[U103] JS：定时器
来源：http://oqr.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dhf.yj20258.top

[U104] JS：防抖
来源：http://ike.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ccc.hysaishi.cn

[U105] JS：节流
来源：http://duq.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hqw.yj20258888.top

[U106] JS：日期格式化
来源：http://dqc.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iox.tian-w.cn

[U107] JS：数字千分位
来源：http://uoh.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bts.daria6918.cn

[U108] JS：随机整数
来源：http://lgd.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://atx.smart0.xyz

[U109] JS：数组分组
来源：http://pzk.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://brn.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://xfe.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cke.birdmap.top

[U111] JS：对象转 Map
来源：http://ial.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://sto.yuanzhike.top

[U112] JS：字符串补位
来源：http://yyg.yongpay.top

"7".padStart(3, "0")
来源：http://pkn.ybcxt.top

[U113] JS：正则替换全部
来源：http://ugk.ctjpmb.com

s.replaceAll("a", "b")
来源：http://pyr.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://dnp.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://whw.fengsongda.top

[U115] JS：生成 UUID
来源：http://vzd.dianchejie.cn

crypto.randomUUID()
来源：http://csd.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://lrp.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://lmq.dashuyun.cn

[U117] JS：单元测试
来源：http://xez.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://qxh.yanxiufei.cn

[U118] JS：开发服务器
来源：http://bfn.jinqigufen.top

npm i -D vite;  npx vite
来源：http://tbb.nwbrower.top

[U119] JS：生产构建
来源：http://ujz.meibo888.top

npx vite build
来源：http://pvc.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://yex.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://geh.zhixingplan.top

================================================================================
来源：http://gzp.daria6918.cn

统计汇总
来源：http://ywr.tianlin.xyz

================================================================================
来源：http://pwq.tarul.cn

按语言统计（条）：
来源：http://icl.316326.xyz

Python ......... 252
来源：http://dri.pycfn.com

PHP ............ 252
来源：http://ubo.cqqwz.cn

JavaScript ..... 252
来源：http://oky.jinqigufen.top

TypeScript ..... 212
来源：http://dwp.sxryk.cn

Java ........... 212
来源：http://wqe.ydzc1.top

Go ............. 212
来源：http://dit.jqgfzy.top

Ruby ........... 212
来源：http://wdc.hfpthk.cn

C# ............. 212
来源：http://spe.chenlongwang.top

C .............. 30
来源：http://lss.chenzaomai.com

C++ ............ 30
来源：http://pmb.chenlongwang.top

SQL ............ 90
来源：http://yke.chenjidiqi.icu

Bash ........... 80
来源：http://wig.nanxuanxn.top

Kotlin ......... 15
来源：http://uyx.feifeiyinyue.top

Swift .......... 15
来源：http://ncb.chenjidiqi.icu

Lua ............ 10
来源：http://wok.jinqigufen.top

Perl ........... 10
来源：http://njq.pycfn.com

Scala .......... 10
来源：http://spx.chenjidiqi.icu

------------------------------------
来源：http://ozr.chenlongwang.top

合计 ........... 2106 条
来源：http://xpe.sysykeji.top

按章节统计：
来源：http://owi.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sth.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hmd.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nab.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nta.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nvu.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oyq.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zyn.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jhv.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gji.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tum.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fwn.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kuu.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nyk.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mxg.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uof.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vsc.gzhubu.top

Q SQL 专题                              90
来源：http://bfj.tian-w.cn

R Bash 专题                             80
来源：http://ahu.daxiang520.top

S C / C++ 专题                          60
来源：http://yhs.guannengcc.top

T 其他语言补充                          60
来源：http://sss.gaohongyu789.top

U 高频实用片段                         120
来源：http://xxc.xuanzx.com

------------------------------------
来源：http://dxs.zhixingplan.top

合计                                  2106 条
来源：http://zln.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://umo.shzxlz.cn

使用提醒
来源：http://fsm.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://stz.smart0.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://psm.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gtg.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ohf.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fmp.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kzl.pengpengdd.cyou

—— 文件结束 ——
来源：http://qrf.yuxming.cn

================================================================================
来源：http://yaf.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://ril.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://jjj.cqqwz.cn

================================================================================
来源：http://tek.pengpengdd.cyou

【收录内容】
来源：http://neb.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vfu.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://shp.chenlongwang.top

SQL · Bash · C · C++
来源：http://noc.zhijiandao.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fto.vqdsnc.cn

【使用说明】
来源：http://twi.fktsv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bnl.aizwys.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pry.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ooj.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mvm.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qkh.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mer.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://aqq.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dkl.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wol.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dtd.wangdashe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pzd.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rrb.sjlbkw.cn

【文件统计】
来源：http://mic.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wga.tanke756.top

--------------------------------------------------------------------------------
来源：http://rph.chenjidiqi.icu

目  录
来源：http://fwh.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://kms.vqdsnc.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rrj.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pww.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zau.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://avj.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yuy.jyoumei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rvn.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nrg.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kks.uphjek.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bqc.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jfj.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nye.0kj1m.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qmx.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mkj.ydzc1.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kig.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nae.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://atu.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tce.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kcq.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rkb.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://msz.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ime.zhaomingkeji.xyz

================================================================================
来源：http://hkn.wangdashe.top

A. 基础语法与类型
来源：http://kjx.yj20258.top

================================================================================
来源：http://iil.zhaomingkeji.xyz

[A01] Hello World
来源：http://isl.zdqjudy.top

Py:   print("Hello, World!")
来源：http://qyy.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://tli.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://wbn.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pfg.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://kzx.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://koo.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://shg.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://trz.hfpthk.cn

[A02] 变量声明与赋值
来源：http://hxz.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yqo.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://euz.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://uwo.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ief.sxryk.cn

Java: String name = "Alex"; int age = 20;
来源：http://kgu.zhengqikj.top

Go:   name := "Alex"; age := 20
来源：http://mrz.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://qsv.mhx1999.top

C#:   string name = "Alex"; int age = 20;
来源：http://roq.fktsv.cn

[A03] 常量定义
来源：http://qws.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aik.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://ndm.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://fec.yonumen.top

TS:   const PI: number = 3.14159;
来源：http://qus.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://eug.zhengqikj.top

Go:   const PI = 3.14159
来源：http://cje.jlsjyb.cn

Ruby: PI = 3.14159
来源：http://ulw.cashguo.top

C#:   const double PI = 3.14159;
来源：http://piu.hfpthk.cn

[A04] 判断变量类型
来源：http://iwx.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ekq.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://khm.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://svr.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://miu.xuetiantiany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blv.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://cpz.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lgx.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://xye.ybcxt.top

[A05] 整数除法与取模
来源：http://qur.wangdashe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qbj.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://xrj.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zsy.hfpthk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cgr.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://efs.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://mcx.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://xuc.316326.xyz

C#:   7 / 2; 7 % 2
来源：http://npt.gaohongyu789.top

[A06] 字符串转数字
来源：http://ppy.chenlongwang.top

Py:   int("42"); float("3.14")
来源：http://rgc.gzhubu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jsf.cqqwz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xpe.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://kjo.ppjwa.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jdz.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sql.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uzr.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lsi.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://faa.hnqzz.top

Py:   str(42)
来源：http://doe.sxryk.cn

PHP:  (string) 42; strval(42)
来源：http://zol.bjfxy.top

JS:   String(42); (42).toString()
来源：http://len.yuxming.cn

TS:   String(42)
来源：http://zew.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://acw.cucudq.cn

Go:   strconv.Itoa(42)
来源：http://tss.sweek.top

Ruby: 42.to_s
来源：http://kud.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://dzc.cheryme.top

[A08] 取整与四舍五入
来源：http://xbc.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://caz.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ixq.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://min.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lfa.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rgv.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xri.jyoumei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://haa.uphjek.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rae.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://qub.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wit.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uyq.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mgy.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wwh.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cqn.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xxw.zdbjq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pei.svipenyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fcb.yonumen.top

[A10] 生成随机数
来源：http://hio.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://asx.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://cia.guannengcc.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ewd.vqdsnc.cn


<!-- 参考信息 -->