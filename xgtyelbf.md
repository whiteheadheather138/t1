代发 wailian999

[U69] PHP：PDO 预处理
来源：http://ipu.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yoq.xylfe.cn

[U70] PHP：PDO 事务
来源：http://haa.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fek.birdmap.top

[U71] PHP：抛出异常
来源：http://elt.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://bls.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://slo.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://uxe.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://gmc.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://dsy.316326.xyz

[U74] PHP：读取环境变量
来源：http://dfu.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://zhl.bbcook.cn

[U75] PHP：依赖注入
来源：http://apf.epnwcf.com

composer require psr/container
来源：http://svv.dianchejie.cn

[U76] PHP：简单路由
来源：http://qrr.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wuk.ppjwa.cn

[U77] PHP：模板渲染
来源：http://lty.aizwys.cn

composer require twig/twig
来源：http://fpr.hnxiangtu.top

[U78] PHP：单元测试
来源：http://jfq.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://rtz.dashuyun.cn

[U79] PHP：静态分析
来源：http://gvj.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://axr.yonumen.top

[U80] PHP：代码规范修复
来源：http://tyl.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hmx.hnqzz.top

[U81] JS：初始化项目
来源：http://mpp.ybcxt.top

npm init -y;  npm i express
来源：http://nkk.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://gey.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vvc.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://hro.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://jan.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://vpt.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://kvb.sweek.top

[U85] JS：可选链
来源：http://iqs.jlsjyb.cn

a?.b?.c
来源：http://lzp.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://cxb.aizwys.cn

a ?? b
来源：http://spo.zhixingplan.top

[U87] JS：解构默认值
来源：http://zbr.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://usn.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://cob.sjlbkw.cn

{ ...a, ...b }
来源：http://dxi.epnwcf.com

[U89] JS：数组去重
来源：http://yit.yueranfly.top

[...new Set(arr)]
来源：http://qyj.uphjek.com

[U90] JS：数字数组排序
来源：http://nfb.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://jhp.cucudq.cn

[U91] JS：对象键值遍历
来源：http://vpq.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rcg.316326.xyz

[U92] JS：深拷贝
来源：http://tcm.zhengqikj.top

structuredClone(obj)
来源：http://csn.epnwcf.com

[U93] JS：模板字符串
来源：http://wsm.fanxiaobao.xyz

`共 ${n} 条`
来源：http://vso.sxryk.cn

[U94] JS：箭头函数
来源：http://cim.cqqwz.cn

const double = x => x * 2;
来源：http://djy.dashuyun.cn

[U95] JS：Promise 包装
来源：http://wgd.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://xrt.mhx1999.top

[U96] JS：async/await 与异常
来源：http://des.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ukt.guannengcc.top

[U97] JS：并发请求
来源：http://wvu.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://wvp.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://stg.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ezq.birdmap.top

[U99] JS：事件监听
来源：http://ftx.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://iqa.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://nts.yj20258.top

document.querySelector(".item")
来源：http://qwi.dashuyun.cn

[U101] JS：classList 操作
来源：http://xcz.birdmap.top

el.classList.toggle("active")
来源：http://gbp.yonumen.top

[U102] JS：本地存储
来源：http://ppk.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xmq.sufxvd.cn

[U103] JS：定时器
来源：http://gmk.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rlk.yonumen.top

[U104] JS：防抖
来源：http://lvt.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mts.yj202588.top

[U105] JS：节流
来源：http://hsj.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lyr.ivvv.top

[U106] JS：日期格式化
来源：http://bpm.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://czo.hfpthk.cn

[U107] JS：数字千分位
来源：http://urb.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ayz.hnqzz.top

[U108] JS：随机整数
来源：http://qbn.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://adz.daria6918.cn

[U109] JS：数组分组
来源：http://lbv.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://snh.zhengqikj.top

[U110] JS：数组分块
来源：http://enu.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ijk.yuxming.cn

[U111] JS：对象转 Map
来源：http://oia.haohaochexian.top

new Map(Object.entries(obj))
来源：http://gvz.bjfxy.top

[U112] JS：字符串补位
来源：http://zra.zhengqikj.top

"7".padStart(3, "0")
来源：http://own.zycfv.cn

[U113] JS：正则替换全部
来源：http://vny.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://btt.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://knx.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pey.chenlongwang.top

[U115] JS：生成 UUID
来源：http://kqn.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://rlw.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://mye.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://bsa.sufxvd.cn

[U117] JS：单元测试
来源：http://mxl.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://nnk.haohaochexian.top

[U118] JS：开发服务器
来源：http://auo.ydzc1.top

npm i -D vite;  npx vite
来源：http://jly.52xcode.cn

[U119] JS：生产构建
来源：http://nre.yj202588.top

npx vite build
来源：http://lua.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://wxq.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://ijy.hesvh.cn

================================================================================
来源：http://znp.kuanghao11.cn

统计汇总
来源：http://coj.hnqzz.top

================================================================================
来源：http://yjl.gaohongyu789.top

按语言统计（条）：
来源：http://ggh.xinyue.icu

Python ......... 252
来源：http://jea.xuanzx.com

PHP ............ 252
来源：http://qux.aizwys.cn

JavaScript ..... 252
来源：http://ilo.hfpthk.cn

TypeScript ..... 212
来源：http://qlp.52xcode.cn

Java ........... 212
来源：http://ybk.snrcjt.cn

Go ............. 212
来源：http://oah.sweek.top

Ruby ........... 212
来源：http://vxh.tian-w.cn

C# ............. 212
来源：http://clv.jiagoushi.top

C .............. 30
来源：http://hsm.aibaodan.cn

C++ ............ 30
来源：http://wpa.ydjk.org.cn

SQL ............ 90
来源：http://poi.ivvv.top

Bash ........... 80
来源：http://ymf.fanxiaobao.xyz

Kotlin ......... 15
来源：http://rkl.hnqzz.top

Swift .......... 15
来源：http://jyq.yj202588.top

Lua ............ 10
来源：http://mby.cucudq.cn

Perl ........... 10
来源：http://syl.ybcxt.top

Scala .......... 10
来源：http://elz.bjfxy.top

------------------------------------
来源：http://whz.ybcxt.top

合计 ........... 2106 条
来源：http://ohl.9152youxi.cn

按章节统计：
来源：http://lfi.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gfl.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yrz.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vkj.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jhr.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fev.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://njc.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ado.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xpu.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ejf.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mii.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tjx.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vta.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://alj.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jzb.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://als.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ekb.ppjwa.cn

Q SQL 专题                              90
来源：http://zog.xylfe.cn

R Bash 专题                             80
来源：http://obb.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://krd.xuetiantiany.cn

T 其他语言补充                          60
来源：http://qwo.meibo888.top

U 高频实用片段                         120
来源：http://yxu.uphjek.com

------------------------------------
来源：http://wmh.aibaodan.cn

合计                                  2106 条
来源：http://tgz.daxiang520.top

--------------------------------------------------------------------------------
来源：http://tyf.shanyushiyangtech.top

使用提醒
来源：http://rhe.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://ile.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hgw.jianghu66.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dlr.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iay.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://pcl.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://syv.gogol.net.cn

—— 文件结束 ——
来源：http://bpx.quarkkingdee.top

================================================================================
来源：http://xfh.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://hod.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://mtp.ywan-chungtsiang.top

================================================================================
来源：http://ouf.zdbjq.cn

【收录内容】
来源：http://gbm.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://wyc.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lme.snrcjt.cn

SQL · Bash · C · C++
来源：http://khl.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gqu.hongshengwenyu.top

【使用说明】
来源：http://kcw.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://elk.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zqb.fengsongda.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ovw.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nck.yvedp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ofe.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wws.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://htf.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vni.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vit.jianghu66.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wqa.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cav.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bxa.jinqigufen.top

【文件统计】
来源：http://mrg.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dsp.hesvh.cn

--------------------------------------------------------------------------------
来源：http://qhb.ppjwa.cn

目  录
来源：http://ncm.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://sms.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eri.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cvx.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://efp.hysaishi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uny.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tng.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fzs.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qql.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oug.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tqd.xziqi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bvn.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uiw.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cqx.jinqigufen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kon.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aas.hesvh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ser.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://etw.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xwq.yj20258.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mpf.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xdd.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nuv.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uii.zhongyouzk.top

================================================================================
来源：http://zlm.zhoulong.xyz

A. 基础语法与类型
来源：http://got.zycfv.cn

================================================================================
来源：http://ddu.ehwqpu.com

[A01] Hello World
来源：http://ecq.iojbl.cn

Py:   print("Hello, World!")
来源：http://jia.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://kzk.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://jpu.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yfz.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://vrv.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://kne.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://eem.ydzc1.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jnj.uphjek.com

[A02] 变量声明与赋值
来源：http://qnr.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cng.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hvi.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://ykq.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nyn.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://rdj.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://itb.daxiang520.top

Ruby: name = "Alex"; age = 20
来源：http://oca.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://vln.xylfe.cn

[A03] 常量定义
来源：http://qey.ctjpmb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bzz.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://mmo.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://zjg.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://saa.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://ebj.fzhhl.top

Go:   const PI = 3.14159
来源：http://wwm.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://tlv.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://mbm.daria6918.cn

[A04] 判断变量类型
来源：http://kid.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dzz.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bpq.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nfc.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://vly.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://trf.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vrz.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pep.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://oxy.hammf.cn

[A05] 整数除法与取模
来源：http://yyb.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nfg.fehbvm.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://lmm.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lcj.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ule.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://nnm.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://cqc.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://glw.guowangkeji.top

C#:   7 / 2; 7 % 2
来源：http://ztw.hysaishi.cn

[A06] 字符串转数字
来源：http://mbs.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://bhm.jinghuilouyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xth.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lkd.0kj1m.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gaj.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cbd.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dus.zdqjudy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jqj.pycfn.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jvl.gzhubu.top

[A07] 数字转字符串
来源：http://ntw.chenzaomai.com

Py:   str(42)
来源：http://vwj.52xcode.cn

PHP:  (string) 42; strval(42)
来源：http://wbc.gzhubu.top

JS:   String(42); (42).toString()
来源：http://gfv.cheryme.top

TS:   String(42)
来源：http://mph.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rhd.cqqwz.cn

Go:   strconv.Itoa(42)
来源：http://cqp.sufxvd.cn

Ruby: 42.to_s
来源：http://ixx.dashuyun.cn

C#:   42.ToString()
来源：http://wmj.tanke756.top

[A08] 取整与四舍五入
来源：http://jgu.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hsj.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://czy.cdnleiting.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rjs.bjfxy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vwb.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gdi.quarkkingdee.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ayr.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://scq.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lln.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://ufz.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yud.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rrd.wangdashe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kiz.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://opf.shanyushiyangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://svu.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kjj.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ibx.shzxlz.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://scr.bjfxy.top

[A10] 生成随机数
来源：http://wtl.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://htm.sysykeji.top

PHP:  random_int(1, 100);
来源：http://frc.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rks.sufxvd.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zga.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://hly.quarkkingdee.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ibt.zdbjq.cn

Ruby: rand(1..100)
来源：http://npb.zhixingplan.top


<!-- 参考信息 -->