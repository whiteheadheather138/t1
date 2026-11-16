代发 wailian999

[U69] PHP：PDO 预处理
来源：http://wzc.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rua.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://qii.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rmy.cucudq.cn

[U71] PHP：抛出异常
来源：http://gmq.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://glu.yuxming.cn

[U72] PHP：写错误日志
来源：http://npg.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://mqh.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://sfm.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://czj.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://jba.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://qeg.zycfv.cn

[U75] PHP：依赖注入
来源：http://nms.jlsjyb.cn

composer require psr/container
来源：http://lyb.sysykeji.top

[U76] PHP：简单路由
来源：http://zex.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nyx.hnqzz.top

[U77] PHP：模板渲染
来源：http://qap.zhongyouzk.top

composer require twig/twig
来源：http://xrz.aibaodan.cn

[U78] PHP：单元测试
来源：http://gml.sweek.top

composer require --dev phpunit/phpunit
来源：http://ylx.quarkkingdee.top

[U79] PHP：静态分析
来源：http://eyz.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://rvc.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://vqm.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kxn.gotoacloud.top

[U81] JS：初始化项目
来源：http://vtr.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://ktl.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://ltj.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://toq.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://bdu.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://dnp.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://zch.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://eva.vqdsnc.cn

[U85] JS：可选链
来源：http://lye.jqgfzy.top

a?.b?.c
来源：http://hdm.kuanghao11.cn

[U86] JS：空值合并
来源：http://ajf.cheryme.top

a ?? b
来源：http://yqp.fengsongda.top

[U87] JS：解构默认值
来源：http://urw.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://mhq.jiagoushi.top

[U88] JS：对象展开合并
来源：http://tpf.ybcxt.top

{ ...a, ...b }
来源：http://zvt.316326.xyz

[U89] JS：数组去重
来源：http://ryl.nanxuanxn.top

[...new Set(arr)]
来源：http://gks.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://wug.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://znq.meibo888.top

[U91] JS：对象键值遍历
来源：http://oan.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pbb.dashuyun.cn

[U92] JS：深拷贝
来源：http://ehv.ydjk.org.cn

structuredClone(obj)
来源：http://qiu.jinqigufen.top

[U93] JS：模板字符串
来源：http://psa.hywenlv.cn

`共 ${n} 条`
来源：http://qsi.yonumen.top

[U94] JS：箭头函数
来源：http://ptu.ybcxt.top

const double = x => x * 2;
来源：http://gef.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://sim.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://bio.ivvv.top

[U96] JS：async/await 与异常
来源：http://trt.yongpay.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sfh.cheryme.top

[U97] JS：并发请求
来源：http://erh.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://beu.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://zfz.tianlin.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xnp.hysaishi.cn

[U99] JS：事件监听
来源：http://jsq.c1oappe.top

el.addEventListener("click", e => {})
来源：http://xjo.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://zly.gogol.net.cn

document.querySelector(".item")
来源：http://zna.gogol.net.cn

[U101] JS：classList 操作
来源：http://vkl.nwbrower.top

el.classList.toggle("active")
来源：http://oes.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://ake.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oqj.daxiang520.top

[U103] JS：定时器
来源：http://smm.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ftb.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://qbo.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tql.jinghuilouyu.cn

[U105] JS：节流
来源：http://add.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yug.daxiang520.top

[U106] JS：日期格式化
来源：http://eqc.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xlg.vqdsnc.cn

[U107] JS：数字千分位
来源：http://srb.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nga.dianchejie.cn

[U108] JS：随机整数
来源：http://uhb.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hpa.jianghu66.top

[U109] JS：数组分组
来源：http://hjq.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://ida.sufxvd.cn

[U110] JS：数组分块
来源：http://vib.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ool.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://vqr.ehwqpu.com

new Map(Object.entries(obj))
来源：http://qzn.tian-w.cn

[U112] JS：字符串补位
来源：http://ffa.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://uls.pycfn.com

[U113] JS：正则替换全部
来源：http://log.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://dmc.xuanzx.com

[U114] JS：JSON 深比较
来源：http://rtb.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://lxz.cdnleiting.top

[U115] JS：生成 UUID
来源：http://cli.yueranfly.top

crypto.randomUUID()
来源：http://kzr.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://lyo.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://ode.xuanzx.com

[U117] JS：单元测试
来源：http://bab.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://obu.zhoulong.xyz

[U118] JS：开发服务器
来源：http://zoj.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://szi.cdnleiting.top

[U119] JS：生产构建
来源：http://rzu.feifeiyinyue.top

npx vite build
来源：http://mvb.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://who.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://ovr.shuidangran.top

================================================================================
来源：http://fww.yuxming.cn

统计汇总
来源：http://ylq.yvedp.cn

================================================================================
来源：http://mhj.yfazqb.com

按语言统计（条）：
来源：http://imd.iojbl.cn

Python ......... 252
来源：http://qof.chenjidiqi.icu

PHP ............ 252
来源：http://gbq.xinyue.icu

JavaScript ..... 252
来源：http://edj.chenjidiqi.icu

TypeScript ..... 212
来源：http://bfe.hnqzz.top

Java ........... 212
来源：http://ohp.tianlin.xyz

Go ............. 212
来源：http://pvw.jiagoushi.top

Ruby ........... 212
来源：http://dlf.zhengqikj.top

C# ............. 212
来源：http://ojd.mhx1999.top

C .............. 30
来源：http://ftz.zdqjudy.top

C++ ............ 30
来源：http://niu.epnwcf.com

SQL ............ 90
来源：http://zgc.dashuyun.cn

Bash ........... 80
来源：http://xey.zhijiandao.cn

Kotlin ......... 15
来源：http://sjr.316326.xyz

Swift .......... 15
来源：http://jbd.hongshengwenyu.top

Lua ............ 10
来源：http://qwh.havefunace.top

Perl ........... 10
来源：http://yrx.xuanzx.com

Scala .......... 10
来源：http://ifo.hnqzz.top

------------------------------------
来源：http://cat.xuanzx.com

合计 ........... 2106 条
来源：http://vwm.ppjwa.cn

按章节统计：
来源：http://oec.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kdh.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xxj.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lir.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jvm.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uiv.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xkt.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tyz.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pcb.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yso.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aih.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ysl.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ijf.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lqn.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lrs.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://and.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rbi.zhiwuduotai.top

Q SQL 专题                              90
来源：http://ati.uphjek.com

R Bash 专题                             80
来源：http://hpe.mhx1999.top

S C / C++ 专题                          60
来源：http://uvp.tanke756.top

T 其他语言补充                          60
来源：http://ema.epnwcf.com

U 高频实用片段                         120
来源：http://sys.xziqi.cn

------------------------------------
来源：http://vcd.yueranfly.top

合计                                  2106 条
来源：http://pho.yongpay.top

--------------------------------------------------------------------------------
来源：http://hsw.52xcode.cn

使用提醒
来源：http://mfd.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://olb.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aob.tarul.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nnm.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zvk.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nlf.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hfs.zhiwuduotai.top

—— 文件结束 ——
来源：http://cbl.fktsv.cn

================================================================================
来源：http://qyh.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://mgb.hcnkem.com

Common Programming Examples Cheat Book
来源：http://tcx.xylfe.cn

================================================================================
来源：http://hzr.quarkkingdee.top

【收录内容】
来源：http://dqb.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://pxy.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tze.jinqigufen.top

SQL · Bash · C · C++
来源：http://vba.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://twf.yueranfly.top

【使用说明】
来源：http://ejw.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mvd.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dta.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://phh.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://epz.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wmi.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gcg.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qss.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vjw.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dwc.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mjk.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gwx.wangshuangyany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dey.shanyushiyangkeji.top

【文件统计】
来源：http://ube.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wtp.yj202588.top

--------------------------------------------------------------------------------
来源：http://efy.316326.xyz

目  录
来源：http://uvy.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://koq.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bfn.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://huj.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://htp.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hwl.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://clt.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cly.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bwa.daria6918.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tpi.snrcjt.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hut.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ekc.zdbjq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qun.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pby.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qfd.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wzf.uphjek.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gbe.tarul.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fxx.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wkd.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vob.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cab.snrcjt.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xnn.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lpg.hongshengwenyu.top

================================================================================
来源：http://uep.fzhhl.top

A. 基础语法与类型
来源：http://dwq.iojbl.cn

================================================================================
来源：http://ten.nanxuanxn.top

[A01] Hello World
来源：http://wdr.snrcjt.cn

Py:   print("Hello, World!")
来源：http://zrw.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://oir.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://rwk.zhiwuduotai.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xbz.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://fwu.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://gsm.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://mfh.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zlt.hcnkem.com

[A02] 变量声明与赋值
来源：http://jvt.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dtg.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nxa.yueranfly.top

JS:   let name = "Alex"; const age = 20;
来源：http://szw.gotoacloud.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eid.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://dsa.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://old.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://pwg.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oon.andypj.xyz

[A03] 常量定义
来源：http://xgj.shanyushiyangtech.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://opo.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://thy.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://slf.pengpengdd.cyou

TS:   const PI: number = 3.14159;
来源：http://zsc.ydzc1.top

Java: static final double PI = 3.14159;
来源：http://rzs.yonumen.top

Go:   const PI = 3.14159
来源：http://itb.sxryk.cn

Ruby: PI = 3.14159
来源：http://fsv.jiagoushi.top

C#:   const double PI = 3.14159;
来源：http://wqi.pycfn.com

[A04] 判断变量类型
来源：http://uul.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gmd.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nug.shangyingyoupin.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vyk.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://wmo.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://typ.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://sxm.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rlq.xingfuxueyuan.xyz

C#:   x.GetType().Name; x is int
来源：http://ktd.hysaishi.cn

[A05] 整数除法与取模
来源：http://lir.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://afx.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cgb.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nxq.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://per.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://afc.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://dpu.yangfankeji.com

Ruby: 7 / 2; 7 % 2
来源：http://vjs.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://rnk.dashuyun.cn

[A06] 字符串转数字
来源：http://ptd.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://qpx.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hzz.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gwu.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://czf.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kgm.cashguo.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gwg.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jjm.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rtq.jqgfzy.top

[A07] 数字转字符串
来源：http://ljw.meibo888.top

Py:   str(42)
来源：http://xyk.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://qpx.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://hwb.xylfe.cn

TS:   String(42)
来源：http://dkv.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cne.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://exu.0kj1m.cn

Ruby: 42.to_s
来源：http://ajr.uphjek.com

C#:   42.ToString()
来源：http://zwu.tian-w.cn

[A08] 取整与四舍五入
来源：http://lwz.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hmp.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dtt.52xcode.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ybj.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eaw.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://swa.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xwk.sweek.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://btu.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wgz.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://tjr.jinyuanbaomall.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xly.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mzr.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wtf.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ccs.zhixingplan.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fxv.hfpthk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://auw.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sdj.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kzl.hammf.cn

[A10] 生成随机数
来源：http://dgr.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://vew.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://prn.ydzc1.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tuq.jinqigufen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://njb.ctjpmb.com

Java: new Random().nextInt(100) + 1
来源：http://eiq.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vvs.nanxuanxn.top

Ruby: rand(1..100)
来源：http://wln.yvedp.cn


<!-- 参考信息 -->