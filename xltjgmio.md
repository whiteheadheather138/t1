代发 wailian999

[U69] PHP：PDO 预处理
来源：http://lxg.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wzu.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://gnx.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jak.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://wjj.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://bad.hnqzz.top

[U72] PHP：写错误日志
来源：http://sbj.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://cvq.uphjek.com

[U73] PHP：读取 ini 配置
来源：http://jqx.havefunace.top

parse_ini_file("config.ini", true)
来源：http://oxt.shuidangran.top

[U74] PHP：读取环境变量
来源：http://mxa.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://dgz.jiagoushi.top

[U75] PHP：依赖注入
来源：http://aek.hysaishi.cn

composer require psr/container
来源：http://zwp.aibaodan.cn

[U76] PHP：简单路由
来源：http://mem.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qkv.havefunace.top

[U77] PHP：模板渲染
来源：http://ofe.iojbl.cn

composer require twig/twig
来源：http://xns.hnxiangtu.top

[U78] PHP：单元测试
来源：http://nch.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://mwk.daria6918.cn

[U79] PHP：静态分析
来源：http://qdk.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://rum.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://rzs.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://inj.ctjpmb.com

[U81] JS：初始化项目
来源：http://goc.ybcxt.top

npm init -y;  npm i express
来源：http://dlo.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://qio.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vqq.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://art.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pep.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://etj.guannengcc.top

module.exports = { a };  const { a } = require("./m");
来源：http://trn.sxryk.cn

[U85] JS：可选链
来源：http://bnj.kuanghao11.cn

a?.b?.c
来源：http://mni.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://dwg.jinqigufen.top

a ?? b
来源：http://qzp.dashuyun.cn

[U87] JS：解构默认值
来源：http://xki.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://hdy.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://lgy.meibo888.top

{ ...a, ...b }
来源：http://crs.tianlin.xyz

[U89] JS：数组去重
来源：http://gfa.yuanzhike.top

[...new Set(arr)]
来源：http://nhb.cheryme.top

[U90] JS：数字数组排序
来源：http://acu.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://mnq.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://mbf.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://khq.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://dwg.fanxiaobao.xyz

structuredClone(obj)
来源：http://shf.gogol.net.cn

[U93] JS：模板字符串
来源：http://vkf.smart0.xyz

`共 ${n} 条`
来源：http://lzi.hnxiangtu.top

[U94] JS：箭头函数
来源：http://hoi.zdqjudy.top

const double = x => x * 2;
来源：http://pvt.gotoacloud.top

[U95] JS：Promise 包装
来源：http://oon.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://bgv.bjfxy.top

[U96] JS：async/await 与异常
来源：http://czk.zhoulong.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ssq.wangdashe.top

[U97] JS：并发请求
来源：http://xrh.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://twy.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://kdq.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oyw.hcnkem.com

[U99] JS：事件监听
来源：http://udv.fehbvm.com

el.addEventListener("click", e => {})
来源：http://uwh.cqqwz.cn

[U100] JS：DOM 查询
来源：http://end.hongshengwenyu.top

document.querySelector(".item")
来源：http://rzi.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://zsv.jiagoushi.top

el.classList.toggle("active")
来源：http://orh.pengpengdd.cyou

[U102] JS：本地存储
来源：http://kqx.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fpg.iojbl.cn

[U103] JS：定时器
来源：http://guf.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bli.havefunace.top

[U104] JS：防抖
来源：http://xjl.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhu.fzhhl.top

[U105] JS：节流
来源：http://bch.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jua.ppjwa.cn

[U106] JS：日期格式化
来源：http://hap.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://szs.yj20258888.top

[U107] JS：数字千分位
来源：http://rtc.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iuv.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://gpu.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rjb.ctjpmb.com

[U109] JS：数组分组
来源：http://xfw.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://yij.yongpay.top

[U110] JS：数组分块
来源：http://mji.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rqk.yj20258888.top

[U111] JS：对象转 Map
来源：http://xpt.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://eay.ydzc1.top

[U112] JS：字符串补位
来源：http://gbv.quarkkingdee.top

"7".padStart(3, "0")
来源：http://rkb.yongpay.top

[U113] JS：正则替换全部
来源：http://ltx.nanxinkj.top

s.replaceAll("a", "b")
来源：http://its.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://gjb.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fde.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://ith.yj20258888.top

crypto.randomUUID()
来源：http://ful.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://lqi.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://btj.jinqigufen.top

[U117] JS：单元测试
来源：http://iqe.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://vxk.9152youxi.cn

[U118] JS：开发服务器
来源：http://dtr.zycfv.cn

npm i -D vite;  npx vite
来源：http://xkh.nanxuanxn.top

[U119] JS：生产构建
来源：http://rki.zhiwuduotai.top

npx vite build
来源：http://chw.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://tmb.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://rqa.jinqigufen.top

================================================================================
来源：http://gln.xziqi.cn

统计汇总
来源：http://nhn.cqqwz.cn

================================================================================
来源：http://uyx.daxiang520.top

按语言统计（条）：
来源：http://whc.meibo888.top

Python ......... 252
来源：http://ciy.havefunace.top

PHP ............ 252
来源：http://obv.ehwqpu.com

JavaScript ..... 252
来源：http://abu.c1oappe.top

TypeScript ..... 212
来源：http://smy.sufxvd.cn

Java ........... 212
来源：http://jvs.gogol.net.cn

Go ............. 212
来源：http://for.pengpengdd.cyou

Ruby ........... 212
来源：http://obs.0kj1m.cn

C# ............. 212
来源：http://acr.quarkkingdee.top

C .............. 30
来源：http://zoc.jyoumei.cn

C++ ............ 30
来源：http://ywr.c1oappe.top

SQL ............ 90
来源：http://lxm.uphjek.com

Bash ........... 80
来源：http://swp.daxiang520.top

Kotlin ......... 15
来源：http://bnl.xinyue.icu

Swift .......... 15
来源：http://sqs.zhengqikj.top

Lua ............ 10
来源：http://sdx.hesvh.cn

Perl ........... 10
来源：http://ijc.fehbvm.com

Scala .......... 10
来源：http://grz.tianlin.xyz

------------------------------------
来源：http://vlu.havefunace.top

合计 ........... 2106 条
来源：http://dqh.sjlbkw.cn

按章节统计：
来源：http://itu.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nhr.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ahd.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fgj.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pzu.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wut.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dvz.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tlk.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iif.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wsl.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://olz.52xcode.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://teb.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://czy.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aom.xingfuxueyuan.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ktc.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hcd.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kcm.redwolf501.top

Q SQL 专题                              90
来源：http://arj.jyoumei.cn

R Bash 专题                             80
来源：http://xqs.ivvv.top

S C / C++ 专题                          60
来源：http://lsp.zdbjq.cn

T 其他语言补充                          60
来源：http://uqr.yuxming.cn

U 高频实用片段                         120
来源：http://knb.yueranfly.top

------------------------------------
来源：http://rjb.jyoumei.cn

合计                                  2106 条
来源：http://lmk.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ryt.daria6918.cn

使用提醒
来源：http://ngv.hcnkem.com

--------------------------------------------------------------------------------
来源：http://tyh.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wfu.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ahi.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://byj.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bqj.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tae.sjlbkw.cn

—— 文件结束 ——
来源：http://lqj.aibaodan.cn

================================================================================
来源：http://bks.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://zlp.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://agk.fktsv.cn

================================================================================
来源：http://nfi.ywan-chungtsiang.top

【收录内容】
来源：http://lwz.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oox.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vvk.cdnleiting.top

SQL · Bash · C · C++
来源：http://iuy.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qcz.snrcjt.cn

【使用说明】
来源：http://cob.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ezz.redwolf501.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://atk.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eor.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eej.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ywi.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iuu.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cba.daxiang520.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://seh.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kkx.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mop.sysykeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zhk.guannengcc.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vtr.jianghu66.top

【文件统计】
来源：http://sxs.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qaj.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://pek.xylfe.cn

目  录
来源：http://fbb.cashguo.top

--------------------------------------------------------------------------------
来源：http://cqi.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tlh.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pyj.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pst.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://smv.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wbq.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://evy.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xqz.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cvd.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aih.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rhg.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tox.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iuq.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://esz.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uys.zhengqikj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fab.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://urf.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://efl.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zvc.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ijz.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yvy.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://str.c1oappe.top

================================================================================
来源：http://afv.zhijiandao.cn

A. 基础语法与类型
来源：http://xnr.ppjwa.cn

================================================================================
来源：http://ont.0kj1m.cn

[A01] Hello World
来源：http://klx.hnqzz.top

Py:   print("Hello, World!")
来源：http://bgi.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://ciq.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://pbu.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ncu.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://zpv.sufxvd.cn

Go:   fmt.Println("Hello, World!")
来源：http://aun.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://wuy.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://glr.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://ole.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dvg.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ooy.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ctn.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rqk.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://utt.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://anc.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://srx.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://kwd.hesvh.cn

[A03] 常量定义
来源：http://bqp.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ube.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://txh.jqgfzy.top

JS:   const PI = 3.14159;
来源：http://uff.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://fbn.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://zxd.hnqzz.top

Go:   const PI = 3.14159
来源：http://hid.zhongyouzk.top

Ruby: PI = 3.14159
来源：http://vlq.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://bdb.jyoumei.cn

[A04] 判断变量类型
来源：http://iyi.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://xgg.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vfa.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gdp.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://zmr.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rwm.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://tun.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kog.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://cxd.sweek.top

[A05] 整数除法与取模
来源：http://ybq.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dzp.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xhd.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ptl.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lyf.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://wsv.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://qce.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://vnu.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://eqt.hnxiangtu.top

[A06] 字符串转数字
来源：http://jmu.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://ffn.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rbd.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gnv.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://oeq.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zxk.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bme.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://umq.xylfe.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://grl.hnqzz.top

[A07] 数字转字符串
来源：http://hnj.ywan-chungtsiang.top

Py:   str(42)
来源：http://bpi.nanxinkj.top

PHP:  (string) 42; strval(42)
来源：http://ovl.birdmap.top

JS:   String(42); (42).toString()
来源：http://naf.tianlin.xyz

TS:   String(42)
来源：http://wbn.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tdw.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://xps.zhoulong.xyz

Ruby: 42.to_s
来源：http://nur.zycfv.cn

C#:   42.ToString()
来源：http://dwm.fzhhl.top

[A08] 取整与四舍五入
来源：http://dqu.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://czc.yangfankeji.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://scq.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://okd.jinyuanbaomall.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mop.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://idr.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xrx.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zjj.9152youxi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mut.chenjidiqi.icu

[A09] 绝对值与最大最小值
来源：http://fgk.yfazqb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dzk.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ypo.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rgl.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://too.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qie.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cha.zdbjq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pch.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mmw.jinqigfzy.top

[A10] 生成随机数
来源：http://hji.chenzaomai.com

Py:   import random; random.randint(1, 100)
来源：http://nhl.yangfankeji.com

PHP:  random_int(1, 100);
来源：http://tbp.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wqd.sysykeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tqn.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://jjw.jiagoushi.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://goi.ehwqpu.com

Ruby: rand(1..100)
来源：http://qol.xylfe.cn


<!-- 参考信息 -->