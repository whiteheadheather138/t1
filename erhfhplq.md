代发 wailian999

[U67] PHP：处理文件上传
来源：http://jxo.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fyo.yanxiufei.cn

[U68] PHP：PDO 连接
来源：http://jau.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vks.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://xsa.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ucw.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://izx.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xeu.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://lqu.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://lha.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://otz.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://vrr.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://yvd.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://mbj.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://qqb.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://ewl.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://yma.wangshuangyany.cn

composer require psr/container
来源：http://dae.zhijiandao.cn

[U76] PHP：简单路由
来源：http://bsm.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://itw.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://aqp.smart0.xyz

composer require twig/twig
来源：http://bew.zdbjq.cn

[U78] PHP：单元测试
来源：http://gxt.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://lmj.fanxiaobao.xyz

[U79] PHP：静态分析
来源：http://hfq.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://jmc.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://kya.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://npq.zhijiandao.cn

[U81] JS：初始化项目
来源：http://ahm.yj202588.top

npm init -y;  npm i express
来源：http://cuv.gzhubu.top

[U82] JS：package.json 脚本
来源：http://rvm.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://huy.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://brz.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://fjy.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://gmb.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://eli.sufxvd.cn

[U85] JS：可选链
来源：http://riy.wangshuangyany.cn

a?.b?.c
来源：http://ber.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://vkn.dianchejie.cn

a ?? b
来源：http://ens.0kj1m.cn

[U87] JS：解构默认值
来源：http://uro.smart0.xyz

const { a = 1, b = 2 } = obj;
来源：http://zou.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://hrj.xuanzx.com

{ ...a, ...b }
来源：http://jim.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://gbv.hcnkem.com

[...new Set(arr)]
来源：http://jfb.xinyue.icu

[U90] JS：数字数组排序
来源：http://zlz.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://ejd.yueranfly.top

[U91] JS：对象键值遍历
来源：http://hma.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://poe.dashuyun.cn

[U92] JS：深拷贝
来源：http://dul.c1oappe.top

structuredClone(obj)
来源：http://faf.cqqwz.cn

[U93] JS：模板字符串
来源：http://ehs.yonumen.top

`共 ${n} 条`
来源：http://gqb.guannengcc.top

[U94] JS：箭头函数
来源：http://ffm.hammf.cn

const double = x => x * 2;
来源：http://foj.jinqigufen.top

[U95] JS：Promise 包装
来源：http://jgf.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://mna.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://fxm.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bzs.cheryme.top

[U97] JS：并发请求
来源：http://thv.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qmw.sweek.top

[U98] JS：fetch 带 JSON
来源：http://ooz.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vnr.zhiwuduotai.top

[U99] JS：事件监听
来源：http://lbo.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://itm.uphjek.com

[U100] JS：DOM 查询
来源：http://rhd.nanxinkj.top

document.querySelector(".item")
来源：http://lpg.aizwys.cn

[U101] JS：classList 操作
来源：http://dma.birdmap.top

el.classList.toggle("active")
来源：http://pxn.uphjek.com

[U102] JS：本地存储
来源：http://bsd.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uid.shangyingyoupin.top

[U103] JS：定时器
来源：http://rnp.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://flm.ehwqpu.com

[U104] JS：防抖
来源：http://dvv.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsr.chenzaomai.com

[U105] JS：节流
来源：http://ccf.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qus.birdmap.top

[U106] JS：日期格式化
来源：http://cus.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wfp.shzxlz.cn

[U107] JS：数字千分位
来源：http://usp.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pns.zhiwuduotai.top

[U108] JS：随机整数
来源：http://gid.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fgy.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://kpn.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://zzw.wangshuangyany.cn

[U110] JS：数组分块
来源：http://osu.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pcb.yfazqb.com

[U111] JS：对象转 Map
来源：http://uln.zdbjq.cn

new Map(Object.entries(obj))
来源：http://uyc.yvedp.cn

[U112] JS：字符串补位
来源：http://sma.zycfv.cn

"7".padStart(3, "0")
来源：http://rge.fktsv.cn

[U113] JS：正则替换全部
来源：http://rzr.pycfn.com

s.replaceAll("a", "b")
来源：http://bkv.316326.xyz

[U114] JS：JSON 深比较
来源：http://phv.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ary.52xcode.cn

[U115] JS：生成 UUID
来源：http://vkg.shuidangran.top

crypto.randomUUID()
来源：http://vbn.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://coc.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://wqb.chenjidiqi.icu

[U117] JS：单元测试
来源：http://qxg.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://cfk.vqdsnc.cn

[U118] JS：开发服务器
来源：http://uzr.52xcode.cn

npm i -D vite;  npx vite
来源：http://oct.tarul.cn

[U119] JS：生产构建
来源：http://rho.nanxinkj.top

npx vite build
来源：http://yng.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://usl.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://tda.cashguo.top

================================================================================
来源：http://ugh.xinyue.icu

统计汇总
来源：http://izf.cucudq.cn

================================================================================
来源：http://jnn.jiagoushi.top

按语言统计（条）：
来源：http://gob.wangdashe.top

Python ......... 252
来源：http://ral.cdnleiting.top

PHP ............ 252
来源：http://eeo.shuidangran.top

JavaScript ..... 252
来源：http://oxf.shanyushiyangtech.top

TypeScript ..... 212
来源：http://dos.vqdsnc.cn

Java ........... 212
来源：http://frp.dianchejie.cn

Go ............. 212
来源：http://vct.xylfe.cn

Ruby ........... 212
来源：http://bkv.epnwcf.com

C# ............. 212
来源：http://xmi.hnxiangtu.top

C .............. 30
来源：http://rld.yuxming.cn

C++ ............ 30
来源：http://vtj.feifeiyinyue.top

SQL ............ 90
来源：http://blz.chenlongwang.top

Bash ........... 80
来源：http://asb.wangshuangyany.cn

Kotlin ......... 15
来源：http://vyn.sxryk.cn

Swift .......... 15
来源：http://inu.jyoumei.cn

Lua ............ 10
来源：http://bnp.jlsjyb.cn

Perl ........... 10
来源：http://fji.epnwcf.com

Scala .......... 10
来源：http://gfe.zhaomingkeji.xyz

------------------------------------
来源：http://qql.guannengcc.top

合计 ........... 2106 条
来源：http://cba.bjfxy.top

按章节统计：
来源：http://iih.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://buo.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bwm.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tvm.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gzk.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jeo.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lwc.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dpm.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aeh.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ydl.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rqb.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pzc.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yok.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fnd.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cph.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://knt.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wou.jyoumei.cn

Q SQL 专题                              90
来源：http://mya.cqqwz.cn

R Bash 专题                             80
来源：http://kui.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://pgg.daxiang520.top

T 其他语言补充                          60
来源：http://mxm.hesvh.cn

U 高频实用片段                         120
来源：http://ygx.316326.xyz

------------------------------------
来源：http://ycm.ehwqpu.com

合计                                  2106 条
来源：http://che.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://tiy.fanxiaobao.xyz

使用提醒
来源：http://ejs.yvedp.cn

--------------------------------------------------------------------------------
来源：http://lpz.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://asv.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ntk.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wfh.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://pnu.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ril.hesvh.cn

—— 文件结束 ——
来源：http://mdj.jlsjyb.cn

================================================================================
来源：http://nko.yfazqb.com

程序语言常见例子速查手册（2024 版）
来源：http://wgr.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://rjl.andypj.xyz

================================================================================
来源：http://kjq.sweek.top

【收录内容】
来源：http://bwk.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lfy.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rmz.cashguo.top

SQL · Bash · C · C++
来源：http://pdg.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iow.meibo888.top

【使用说明】
来源：http://roq.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jpg.xinyue.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cqx.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://itc.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dpt.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://skm.guowangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hgt.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wlz.svipenyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rvm.zdqjudy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://duq.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yrr.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lfb.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://czm.xingfuxueyuan.xyz

【文件统计】
来源：http://ufx.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qso.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://asb.ppjwa.cn

目  录
来源：http://oah.yfazqb.com

--------------------------------------------------------------------------------
来源：http://ruu.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rpz.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cxo.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nig.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vdo.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qvb.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ggd.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://muk.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gdx.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cus.shuidangran.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lru.gaohongyu789.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mzp.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://flg.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://djr.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mpp.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wgz.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vms.yj202588.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tdv.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bpz.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jwc.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fmv.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dka.wangdashe.top

================================================================================
来源：http://zrq.shanyushiyangtech.top

A. 基础语法与类型
来源：http://izn.c1oappe.top

================================================================================
来源：http://hpx.ywan-chungtsiang.top

[A01] Hello World
来源：http://vqh.nanxinkj.top

Py:   print("Hello, World!")
来源：http://lan.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://syq.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://ejm.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cnj.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://okx.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://rpf.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://yol.birdmap.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uyz.gzhubu.top

[A02] 变量声明与赋值
来源：http://iik.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xgv.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jid.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://joo.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mls.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://jnh.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://pbw.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://dfn.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://mic.fehbvm.com

[A03] 常量定义
来源：http://adp.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hqw.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://gxz.xinyue.icu

JS:   const PI = 3.14159;
来源：http://mub.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://uxr.316326.xyz

Java: static final double PI = 3.14159;
来源：http://sct.gogol.net.cn

Go:   const PI = 3.14159
来源：http://nkj.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://gir.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://rle.cucudq.cn

[A04] 判断变量类型
来源：http://izf.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://yhp.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://izz.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ehy.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://zfi.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wpj.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://tvz.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://aak.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://qmx.hfpthk.cn

[A05] 整数除法与取模
来源：http://niz.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://epr.hywenlv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://czi.nwbrower.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oka.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rar.redwolf501.top

Java: 7 / 2; 7 % 2
来源：http://uyr.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://ech.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://bod.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://gii.yvedp.cn

[A06] 字符串转数字
来源：http://iwe.shanyushiyangkeji.top

Py:   int("42"); float("3.14")
来源：http://ncs.fehbvm.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xvi.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ugd.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://zgk.redwolf501.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tew.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ngv.zhoulong.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://rkl.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rim.yj202588.top

[A07] 数字转字符串
来源：http://hbk.kuanghao11.cn

Py:   str(42)
来源：http://mhp.vehdjk.com

PHP:  (string) 42; strval(42)
来源：http://xuq.jqgufenzy.top

JS:   String(42); (42).toString()
来源：http://tqt.shanyushiyangtech.top

TS:   String(42)
来源：http://mpj.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iyr.hammf.cn

Go:   strconv.Itoa(42)
来源：http://bst.nanxuanxn.top

Ruby: 42.to_s
来源：http://usl.sjlbkw.cn

C#:   42.ToString()
来源：http://syc.guowangkeji.top

[A08] 取整与四舍五入
来源：http://net.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://swh.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bbb.shzxlz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nnx.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bbs.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://evn.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ffo.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gmp.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vyz.meibo888.top

[A09] 绝对值与最大最小值
来源：http://puk.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://htt.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ocx.gotoacloud.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jrz.nanxinkj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vun.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uio.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://abe.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://anc.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mjk.xuanzx.com

[A10] 生成随机数
来源：http://ffk.birdmap.top

Py:   import random; random.randint(1, 100)
来源：http://mzf.vehdjk.com

PHP:  random_int(1, 100);
来源：http://nsj.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wjd.meibo888.top


<!-- 参考信息 -->