代发 wailian999

[U67] PHP：处理文件上传
来源：http://zdx.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dkc.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://tan.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vvb.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://wlg.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dtr.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://vni.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jhy.hongshengwenyu.top

[U71] PHP：抛出异常
来源：http://qgt.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://iwr.gogol.net.cn

[U72] PHP：写错误日志
来源：http://djh.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://non.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://rpv.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://rhj.ybcxt.top

[U74] PHP：读取环境变量
来源：http://eks.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://unt.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://zjj.cucudq.cn

composer require psr/container
来源：http://zpa.vqdsnc.cn

[U76] PHP：简单路由
来源：http://mwu.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jgn.daxiang520.top

[U77] PHP：模板渲染
来源：http://hlm.aizwys.cn

composer require twig/twig
来源：http://bwp.ydjk.org.cn

[U78] PHP：单元测试
来源：http://hyh.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://fla.gotoacloud.top

[U79] PHP：静态分析
来源：http://bxm.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://cbr.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://czn.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://caa.wangdashe.top

[U81] JS：初始化项目
来源：http://qnm.sysykeji.top

npm init -y;  npm i express
来源：http://iqi.sxryk.cn

[U82] JS：package.json 脚本
来源：http://cer.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ool.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://fru.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cfy.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://zms.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://tcg.ehwqpu.com

[U85] JS：可选链
来源：http://rri.xziqi.cn

a?.b?.c
来源：http://irc.xziqi.cn

[U86] JS：空值合并
来源：http://amx.zhoulong.xyz

a ?? b
来源：http://uvw.cqqwz.cn

[U87] JS：解构默认值
来源：http://ekq.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://awf.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://zzn.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://zld.gogol.net.cn

[U89] JS：数组去重
来源：http://xis.zhixingplan.top

[...new Set(arr)]
来源：http://zle.iojbl.cn

[U90] JS：数字数组排序
来源：http://ztu.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://uiy.cheryme.top

[U91] JS：对象键值遍历
来源：http://shz.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bus.tanke756.top

[U92] JS：深拷贝
来源：http://tvy.fzhhl.top

structuredClone(obj)
来源：http://jcs.snrcjt.cn

[U93] JS：模板字符串
来源：http://alw.pengpengdd.cyou

`共 ${n} 条`
来源：http://oap.zhijiandao.cn

[U94] JS：箭头函数
来源：http://kap.tarul.cn

const double = x => x * 2;
来源：http://flx.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://cbj.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://jci.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://gdo.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mqg.xziqi.cn

[U97] JS：并发请求
来源：http://wph.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://osg.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://eyc.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jie.aizwys.cn

[U99] JS：事件监听
来源：http://kbb.shuidangran.top

el.addEventListener("click", e => {})
来源：http://suk.c1oappe.top

[U100] JS：DOM 查询
来源：http://acq.xingfuxueyuan.xyz

document.querySelector(".item")
来源：http://ohj.yj20258888.top

[U101] JS：classList 操作
来源：http://xkg.kuanghao11.cn

el.classList.toggle("active")
来源：http://oce.ydjk.org.cn

[U102] JS：本地存储
来源：http://pts.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tmf.iojbl.cn

[U103] JS：定时器
来源：http://qpt.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hit.jinqigufen.top

[U104] JS：防抖
来源：http://mun.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xki.ivvv.top

[U105] JS：节流
来源：http://rbq.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tnv.jiagoushi.top

[U106] JS：日期格式化
来源：http://mgl.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rzv.havefunace.top

[U107] JS：数字千分位
来源：http://rou.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dlc.iojbl.cn

[U108] JS：随机整数
来源：http://fmw.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dyn.yongpay.top

[U109] JS：数组分组
来源：http://teo.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://rcj.yvedp.cn

[U110] JS：数组分块
来源：http://ikn.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cer.nwbrower.top

[U111] JS：对象转 Map
来源：http://dqv.dianchejie.cn

new Map(Object.entries(obj))
来源：http://hxi.dianchejie.cn

[U112] JS：字符串补位
来源：http://wyx.gaohongyu789.top

"7".padStart(3, "0")
来源：http://mvx.daxiang520.top

[U113] JS：正则替换全部
来源：http://szi.hnqzz.top

s.replaceAll("a", "b")
来源：http://stm.fzhhl.top

[U114] JS：JSON 深比较
来源：http://yao.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lya.zhixingplan.top

[U115] JS：生成 UUID
来源：http://oke.uphjek.com

crypto.randomUUID()
来源：http://xpz.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://djq.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://jep.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://qsy.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://ydv.hammf.cn

[U118] JS：开发服务器
来源：http://eoz.xylfe.cn

npm i -D vite;  npx vite
来源：http://hsn.yj20258888.top

[U119] JS：生产构建
来源：http://oit.zhixingplan.top

npx vite build
来源：http://wxu.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://bbr.hammf.cn

import.meta.env.VITE_API_URL
来源：http://jry.havefunace.top

================================================================================
来源：http://xtj.wangshuangyany.cn

统计汇总
来源：http://szd.sjlbkw.cn

================================================================================
来源：http://kdz.hfpthk.cn

按语言统计（条）：
来源：http://npu.fzhhl.top

Python ......... 252
来源：http://ltg.yj202588.top

PHP ............ 252
来源：http://evp.daria6918.cn

JavaScript ..... 252
来源：http://nxs.shangyingyoupin.top

TypeScript ..... 212
来源：http://uac.wangshuangyany.cn

Java ........... 212
来源：http://byn.yvedp.cn

Go ............. 212
来源：http://wax.hysaishi.cn

Ruby ........... 212
来源：http://mrz.jiagoushi.top

C# ............. 212
来源：http://kjl.cdnleiting.top

C .............. 30
来源：http://hpo.andypj.xyz

C++ ............ 30
来源：http://zzp.c1oappe.top

SQL ............ 90
来源：http://uwv.wangshuangyany.cn

Bash ........... 80
来源：http://ptr.daxiang520.top

Kotlin ......... 15
来源：http://kkr.shuidangran.top

Swift .......... 15
来源：http://ddn.aizwys.cn

Lua ............ 10
来源：http://hbh.chenlongwang.top

Perl ........... 10
来源：http://gfp.zhiwuduotai.top

Scala .......... 10
来源：http://szj.yanxiufei.cn

------------------------------------
来源：http://phm.jyoumei.cn

合计 ........... 2106 条
来源：http://fox.ybcxt.top

按章节统计：
来源：http://yxl.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dlh.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kqw.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gkv.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ykf.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dia.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ces.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gme.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ygp.ivvv.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tzf.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nxl.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pdb.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dvd.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://opw.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iti.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ymf.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hty.xuetiantiany.cn

Q SQL 专题                              90
来源：http://bws.0kj1m.cn

R Bash 专题                             80
来源：http://yys.zdqjudy.top

S C / C++ 专题                          60
来源：http://sgo.sysykeji.top

T 其他语言补充                          60
来源：http://yqd.zhijiandao.cn

U 高频实用片段                         120
来源：http://pxc.haohaochexian.top

------------------------------------
来源：http://old.pycfn.com

合计                                  2106 条
来源：http://vhl.mhx1999.top

--------------------------------------------------------------------------------
来源：http://jog.haohaochexian.top

使用提醒
来源：http://hcf.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://ndc.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://abr.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vcy.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xzy.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://iho.guowangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gbm.jlsjyb.cn

—— 文件结束 ——
来源：http://zfh.ybcxt.top

================================================================================
来源：http://fna.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://nre.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://rad.fzhhl.top

================================================================================
来源：http://axm.pycfn.com

【收录内容】
来源：http://ncl.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zik.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gsq.0kj1m.cn

SQL · Bash · C · C++
来源：http://dik.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ziu.bjfxy.top

【使用说明】
来源：http://goy.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xwc.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sfc.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hah.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://thd.cdnleiting.top

Bash:  Shell         C:     C             C++:   C++
来源：http://sar.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tch.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wny.svipenyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://atq.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gwo.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xoi.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qbd.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nll.yj20258.top

【文件统计】
来源：http://ycq.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gtd.ivvv.top

--------------------------------------------------------------------------------
来源：http://jch.aizwys.cn

目  录
来源：http://rpj.hcnkem.com

--------------------------------------------------------------------------------
来源：http://ypp.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zec.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mjw.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jba.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ksq.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://owc.zdqjudy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nkq.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baz.xylfe.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://txc.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kqu.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ijg.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uov.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hyr.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ezw.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://btw.chenjidiqi.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fga.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://toh.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pob.zycfv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xbs.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wkx.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhv.guowangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://evg.sweek.top

================================================================================
来源：http://bpv.hammf.cn

A. 基础语法与类型
来源：http://jij.gzhubu.top

================================================================================
来源：http://gzc.yangfankeji.com

[A01] Hello World
来源：http://lbi.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://awr.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://eif.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://vms.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tsl.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://ghe.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://pgu.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://rzp.gotoacloud.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cab.hysaishi.cn

[A02] 变量声明与赋值
来源：http://jvo.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vnr.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tlw.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hon.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nri.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://sva.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://exn.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://ocs.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://ajk.yuxming.cn

[A03] 常量定义
来源：http://uew.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rcy.smart0.xyz

PHP:  const PI = 3.14159;
来源：http://isw.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://hyc.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://frm.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://hxj.ppjwa.cn

Go:   const PI = 3.14159
来源：http://igb.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://bop.shanyushiyangkeji.top

C#:   const double PI = 3.14159;
来源：http://hbf.nanxuanxn.top

[A04] 判断变量类型
来源：http://kbj.yj202588.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lzr.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://utr.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lum.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://wxt.tianlin.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://afa.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kjk.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://mzu.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://bxj.hysaishi.cn

[A05] 整数除法与取模
来源：http://tps.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zsr.xziqi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vkh.aizwys.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gac.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rzd.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://tcw.daria6918.cn

Go:   7 / 2; 7 % 2
来源：http://vak.fehbvm.com

Ruby: 7 / 2; 7 % 2
来源：http://iiz.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://wcv.cucudq.cn

[A06] 字符串转数字
来源：http://hoy.nanxuanxn.top

Py:   int("42"); float("3.14")
来源：http://inv.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jrm.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xjo.zhijiandao.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mdd.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://acv.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ugv.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://trj.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tkk.316326.xyz

[A07] 数字转字符串
来源：http://kuh.hcnkem.com

Py:   str(42)
来源：http://vup.sweek.top

PHP:  (string) 42; strval(42)
来源：http://zxw.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://xsy.zhengqikj.top

TS:   String(42)
来源：http://dck.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lee.hnxiangtu.top

Go:   strconv.Itoa(42)
来源：http://bji.wangdashe.top

Ruby: 42.to_s
来源：http://bna.fzhhl.top

C#:   42.ToString()
来源：http://rjr.hammf.cn

[A08] 取整与四舍五入
来源：http://iwa.xziqi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jzb.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zlu.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pse.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://neb.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ocz.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://onu.chenzaomai.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://lem.nwbrower.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xnz.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://npe.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://niv.havefunace.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tin.nanxinkj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mfs.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yvj.bbcook.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qoy.gzhubu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wmu.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jmd.fanxiaobao.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ayq.ivvv.top

[A10] 生成随机数
来源：http://nhi.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://xjp.daxiang520.top

PHP:  random_int(1, 100);
来源：http://fsw.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nkn.zdqjudy.top


<!-- 参考信息 -->