代发 wailian999

[U67] PHP：处理文件上传
来源：http://ndm.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rbc.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://qwf.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tvx.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://dyf.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yib.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://sbu.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hlg.sysykeji.top

[U71] PHP：抛出异常
来源：http://kfk.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://llp.cashguo.top

[U72] PHP：写错误日志
来源：http://vhv.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://yit.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://jzg.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://ocy.ivvv.top

[U74] PHP：读取环境变量
来源：http://wgz.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://jpo.bbcook.cn

[U75] PHP：依赖注入
来源：http://dtu.xziqi.cn

composer require psr/container
来源：http://hth.yuanzhike.top

[U76] PHP：简单路由
来源：http://xol.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://snr.hfpthk.cn

[U77] PHP：模板渲染
来源：http://eyr.xziqi.cn

composer require twig/twig
来源：http://xrd.sjlbkw.cn

[U78] PHP：单元测试
来源：http://vft.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://goq.fzhhl.top

[U79] PHP：静态分析
来源：http://nvz.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://lfd.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://rih.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jxr.bjfxy.top

[U81] JS：初始化项目
来源：http://gjv.cucudq.cn

npm init -y;  npm i express
来源：http://dqt.havefunace.top

[U82] JS：package.json 脚本
来源：http://xtj.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ntt.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://zxw.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://kcy.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://wpt.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://raf.jianghu66.top

[U85] JS：可选链
来源：http://zpi.xinyue.icu

a?.b?.c
来源：http://ybg.hcnkem.com

[U86] JS：空值合并
来源：http://tse.chenlongwang.top

a ?? b
来源：http://ssr.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://bfy.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://axa.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://flh.xuanzx.com

{ ...a, ...b }
来源：http://jon.shangyingyoupin.top

[U89] JS：数组去重
来源：http://rmi.hfpthk.cn

[...new Set(arr)]
来源：http://xbl.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://wzm.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://ufd.pycfn.com

[U91] JS：对象键值遍历
来源：http://pzr.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zri.redwolf501.top

[U92] JS：深拷贝
来源：http://gou.xylfe.cn

structuredClone(obj)
来源：http://oic.jinqigufen.top

[U93] JS：模板字符串
来源：http://nwm.yj20258888.top

`共 ${n} 条`
来源：http://bbo.yfazqb.com

[U94] JS：箭头函数
来源：http://sgi.shanyushiyangtech.top

const double = x => x * 2;
来源：http://hjz.chenlongwang.top

[U95] JS：Promise 包装
来源：http://jbo.yj20258.top

new Promise((resolve, reject) => {})
来源：http://xxv.52xcode.cn

[U96] JS：async/await 与异常
来源：http://yhi.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ezo.bjfxy.top

[U97] JS：并发请求
来源：http://jic.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vls.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://mnz.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gbq.wangdashe.top

[U99] JS：事件监听
来源：http://tix.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://uai.uphjek.com

[U100] JS：DOM 查询
来源：http://pfr.haohaochexian.top

document.querySelector(".item")
来源：http://xwv.yj20258888.top

[U101] JS：classList 操作
来源：http://iuc.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://khh.tianlin.xyz

[U102] JS：本地存储
来源：http://jrp.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ivz.gaohongyu789.top

[U103] JS：定时器
来源：http://fqa.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ugj.dashuyun.cn

[U104] JS：防抖
来源：http://xwr.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzl.jinyuanbaomall.cn

[U105] JS：节流
来源：http://ckh.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://idd.52xcode.cn

[U106] JS：日期格式化
来源：http://kve.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dzu.52xcode.cn

[U107] JS：数字千分位
来源：http://imu.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ufx.jqgufenzy.top

[U108] JS：随机整数
来源：http://uaz.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vxs.mhx1999.top

[U109] JS：数组分组
来源：http://lgh.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://rba.cqqwz.cn

[U110] JS：数组分块
来源：http://mis.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wgr.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://tvp.nanxinkj.top

new Map(Object.entries(obj))
来源：http://icm.dashuyun.cn

[U112] JS：字符串补位
来源：http://fth.gotoacloud.top

"7".padStart(3, "0")
来源：http://gnc.xinyue.icu

[U113] JS：正则替换全部
来源：http://azy.jiagoushi.top

s.replaceAll("a", "b")
来源：http://abp.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://oub.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://rig.guowangkeji.top

[U115] JS：生成 UUID
来源：http://jqa.daria6918.cn

crypto.randomUUID()
来源：http://kqj.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://rsu.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://sxl.c1oappe.top

[U117] JS：单元测试
来源：http://whn.dianchejie.cn

npm i -D vitest;  npx vitest
来源：http://vod.xinyue.icu

[U118] JS：开发服务器
来源：http://ynv.tianlin.xyz

npm i -D vite;  npx vite
来源：http://xzc.fengsongda.top

[U119] JS：生产构建
来源：http://qgd.guannengcc.top

npx vite build
来源：http://rkr.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://gql.uphjek.com

import.meta.env.VITE_API_URL
来源：http://jql.zhixingplan.top

================================================================================
来源：http://old.ydzc1.top

统计汇总
来源：http://nid.yuanzhike.top

================================================================================
来源：http://xgu.gzhubu.top

按语言统计（条）：
来源：http://lid.tian-w.cn

Python ......... 252
来源：http://fak.wangshuangyany.cn

PHP ............ 252
来源：http://pqg.gotoacloud.top

JavaScript ..... 252
来源：http://cbr.ydjk.org.cn

TypeScript ..... 212
来源：http://ugj.9152youxi.cn

Java ........... 212
来源：http://adq.gzhubu.top

Go ............. 212
来源：http://jce.zhiwuduotai.top

Ruby ........... 212
来源：http://lja.meibo888.top

C# ............. 212
来源：http://ils.tanke756.top

C .............. 30
来源：http://isp.fzhhl.top

C++ ............ 30
来源：http://vsq.tanke756.top

SQL ............ 90
来源：http://qhj.0kj1m.cn

Bash ........... 80
来源：http://rrj.hongshengwenyu.top

Kotlin ......... 15
来源：http://efj.xziqi.cn

Swift .......... 15
来源：http://gqb.feifeiyinyue.top

Lua ............ 10
来源：http://fds.tian-w.cn

Perl ........... 10
来源：http://dqt.yuanzhike.top

Scala .......... 10
来源：http://lwi.svipenyu.cn

------------------------------------
来源：http://ohv.birdmap.top

合计 ........... 2106 条
来源：http://wzz.fzhhl.top

按章节统计：
来源：http://nbz.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://toh.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://psd.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rvs.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kda.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ebv.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ffs.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://upx.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yam.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://byd.nwbrower.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sou.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://scg.yuxming.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mrz.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uhb.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sdx.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bwx.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oyb.quarkkingdee.top

Q SQL 专题                              90
来源：http://wtg.wangshuangyany.cn

R Bash 专题                             80
来源：http://gfj.zdqjudy.top

S C / C++ 专题                          60
来源：http://yxf.52xcode.cn

T 其他语言补充                          60
来源：http://nrc.zhijiandao.cn

U 高频实用片段                         120
来源：http://bze.xuetiantiany.cn

------------------------------------
来源：http://hii.jlsjyb.cn

合计                                  2106 条
来源：http://wts.yueranfly.top

--------------------------------------------------------------------------------
来源：http://thn.jqgufenzy.top

使用提醒
来源：http://xwo.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://pez.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zfl.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tei.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kqu.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://onz.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bwl.yanxiufei.cn

—— 文件结束 ——
来源：http://ayj.yanxiufei.cn

================================================================================
来源：http://ksa.meibo888.top

程序语言常见例子速查手册（2024 版）
来源：http://wvc.fengsongda.top

Common Programming Examples Cheat Book
来源：http://shs.ywan-chungtsiang.top

================================================================================
来源：http://jub.fanxiaobao.xyz

【收录内容】
来源：http://gxz.xinyue.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://edy.zhengqikj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tdo.smart0.xyz

SQL · Bash · C · C++
来源：http://hkc.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rgo.fanxiaobao.xyz

【使用说明】
来源：http://yfj.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ckj.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://usp.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://khm.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kaj.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jum.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ysb.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://roc.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ppb.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lta.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xdo.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cql.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bzh.zhoulong.xyz

【文件统计】
来源：http://bga.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jbj.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://pgx.ehwqpu.com

目  录
来源：http://uod.fktsv.cn

--------------------------------------------------------------------------------
来源：http://hfo.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rvv.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sca.kuanghao11.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dew.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lhs.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uax.ctjpmb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ngg.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yru.gotoacloud.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rch.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wzz.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sad.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vrp.zhiwuduotai.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ipm.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bcm.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pkz.guowangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://asr.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tpd.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ogn.quarkkingdee.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vhh.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zgw.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ivr.birdmap.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mvo.tian-w.cn

================================================================================
来源：http://vby.meibo888.top

A. 基础语法与类型
来源：http://dgo.yongpay.top

================================================================================
来源：http://tsc.dashuyun.cn

[A01] Hello World
来源：http://czh.tianlin.xyz

Py:   print("Hello, World!")
来源：http://jea.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://avf.fanxiaobao.xyz

JS:   console.log("Hello, World!");
来源：http://qen.jlsjyb.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ipe.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://ods.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://bmf.tarul.cn

Ruby: puts "Hello, World!"
来源：http://nfe.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bwd.cashguo.top

[A02] 变量声明与赋值
来源：http://thf.sjlbkw.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gbp.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://asl.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wim.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iet.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://bfh.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://bot.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://adz.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://ydp.jiagoushi.top

[A03] 常量定义
来源：http://kjb.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yja.xylfe.cn

PHP:  const PI = 3.14159;
来源：http://elp.birdmap.top

JS:   const PI = 3.14159;
来源：http://tiy.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://cuw.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://skv.fengsongda.top

Go:   const PI = 3.14159
来源：http://rje.cashguo.top

Ruby: PI = 3.14159
来源：http://ifn.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://jkj.cqqwz.cn

[A04] 判断变量类型
来源：http://cnn.hnqzz.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jkp.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fpu.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://esd.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://rfn.gogol.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ttj.pycfn.com

Go:   reflect.TypeOf(x).Name()
来源：http://rwj.ydzc1.top

Ruby: x.class; x.is_a?(Integer)
来源：http://con.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://zor.jiagoushi.top

[A05] 整数除法与取模
来源：http://jkg.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lps.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qji.snrcjt.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cum.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ivp.yuxming.cn

Java: 7 / 2; 7 % 2
来源：http://cse.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://kqo.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://tra.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://ztj.zdbjq.cn

[A06] 字符串转数字
来源：http://vhw.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://euv.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xla.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rnz.havefunace.top

TS:   parseInt("42", 10); Number("42")
来源：http://xta.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vjy.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://koc.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mxi.xuanzx.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vew.xuanzx.com

[A07] 数字转字符串
来源：http://jdd.daxiang520.top

Py:   str(42)
来源：http://rnu.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://usr.tian-w.cn

JS:   String(42); (42).toString()
来源：http://xeg.birdmap.top

TS:   String(42)
来源：http://zzq.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kfz.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://rku.jinqigufen.top

Ruby: 42.to_s
来源：http://fan.cqqwz.cn

C#:   42.ToString()
来源：http://smo.hywenlv.cn

[A08] 取整与四舍五入
来源：http://glq.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xov.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yxv.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jxa.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aab.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rwz.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zsy.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fvh.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ixj.ydzc1.top

[A09] 绝对值与最大最小值
来源：http://dra.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hvx.yvedp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wyv.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://onm.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yqr.ppjwa.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hex.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rqv.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://npv.smart0.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://buy.sweek.top

[A10] 生成随机数
来源：http://ghg.xinyue.icu

Py:   import random; random.randint(1, 100)
来源：http://qox.bbcook.cn

PHP:  random_int(1, 100);
来源：http://isu.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ffl.havefunace.top


<!-- 参考信息 -->