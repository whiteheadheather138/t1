代发 wailian999

[U65] PHP：会话
来源：http://ncb.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hqg.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://uks.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pdw.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://bra.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uqe.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://fso.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fyd.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://vcs.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://emq.shuidangran.top

[U70] PHP：PDO 事务
来源：http://dhn.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kej.shuidangran.top

[U71] PHP：抛出异常
来源：http://cqs.cashguo.top

throw new RuntimeException("失败", 500);
来源：http://nkd.daria6918.cn

[U72] PHP：写错误日志
来源：http://dbs.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://qkz.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://txx.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://mar.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://ixu.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://cid.dashuyun.cn

[U75] PHP：依赖注入
来源：http://pjv.kuanghao11.cn

composer require psr/container
来源：http://xbq.hnqzz.top

[U76] PHP：简单路由
来源：http://xuf.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://agp.aibaodan.cn

[U77] PHP：模板渲染
来源：http://mjq.zhengqikj.top

composer require twig/twig
来源：http://zqz.sweek.top

[U78] PHP：单元测试
来源：http://hos.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://pbp.meibo888.top

[U79] PHP：静态分析
来源：http://okd.ivvv.top

composer require --dev phpstan/phpstan
来源：http://dom.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://niy.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://iof.ivvv.top

[U81] JS：初始化项目
来源：http://fyp.ybcxt.top

npm init -y;  npm i express
来源：http://gji.iojbl.cn

[U82] JS：package.json 脚本
来源：http://bku.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jnz.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://wdy.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://swz.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://keh.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://gwe.sxryk.cn

[U85] JS：可选链
来源：http://znt.fengsongda.top

a?.b?.c
来源：http://dzg.wangshuangyany.cn

[U86] JS：空值合并
来源：http://eok.kuanghao11.cn

a ?? b
来源：http://wgr.hammf.cn

[U87] JS：解构默认值
来源：http://kkj.tianlin.xyz

const { a = 1, b = 2 } = obj;
来源：http://fuo.sysykeji.top

[U88] JS：对象展开合并
来源：http://gnx.zhoulong.xyz

{ ...a, ...b }
来源：http://xkg.uphjek.com

[U89] JS：数组去重
来源：http://qmu.ctjpmb.com

[...new Set(arr)]
来源：http://tsc.9152youxi.cn

[U90] JS：数字数组排序
来源：http://qya.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://rfk.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://vre.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oik.aibaodan.cn

[U92] JS：深拷贝
来源：http://wmn.sufxvd.cn

structuredClone(obj)
来源：http://ewv.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://law.chenlongwang.top

`共 ${n} 条`
来源：http://jng.fengsongda.top

[U94] JS：箭头函数
来源：http://ehf.tarul.cn

const double = x => x * 2;
来源：http://acx.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://ojd.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://mic.yonumen.top

[U96] JS：async/await 与异常
来源：http://maf.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rvt.hnxiangtu.top

[U97] JS：并发请求
来源：http://jai.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kxi.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://rdc.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xlh.smart0.xyz

[U99] JS：事件监听
来源：http://loe.vehdjk.com

el.addEventListener("click", e => {})
来源：http://lzy.guowangkeji.top

[U100] JS：DOM 查询
来源：http://pvu.svipenyu.cn

document.querySelector(".item")
来源：http://izs.jianghu66.top

[U101] JS：classList 操作
来源：http://zvb.gotoacloud.top

el.classList.toggle("active")
来源：http://ttx.ehwqpu.com

[U102] JS：本地存储
来源：http://xek.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hxl.gzhubu.top

[U103] JS：定时器
来源：http://qcz.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ite.pengpengdd.cyou

[U104] JS：防抖
来源：http://rnb.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://shk.nanxuanxn.top

[U105] JS：节流
来源：http://adw.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cdl.shzxlz.cn

[U106] JS：日期格式化
来源：http://mya.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://orq.ywan-chungtsiang.top

[U107] JS：数字千分位
来源：http://kpf.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qnx.aizwys.cn

[U108] JS：随机整数
来源：http://avs.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vmm.bjfxy.top

[U109] JS：数组分组
来源：http://ebc.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://sme.sufxvd.cn

[U110] JS：数组分块
来源：http://eyf.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://siy.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://tkr.ybcxt.top

new Map(Object.entries(obj))
来源：http://dqt.cqqwz.cn

[U112] JS：字符串补位
来源：http://ebo.316326.xyz

"7".padStart(3, "0")
来源：http://pwn.aizwys.cn

[U113] JS：正则替换全部
来源：http://nae.guowangkeji.top

s.replaceAll("a", "b")
来源：http://ind.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://ruw.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jir.hammf.cn

[U115] JS：生成 UUID
来源：http://pzx.aizwys.cn

crypto.randomUUID()
来源：http://wud.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://wft.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://jhg.jqgfzy.top

[U117] JS：单元测试
来源：http://chq.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://goo.cqqwz.cn

[U118] JS：开发服务器
来源：http://onw.fehbvm.com

npm i -D vite;  npx vite
来源：http://oso.bbcook.cn

[U119] JS：生产构建
来源：http://htm.havefunace.top

npx vite build
来源：http://yui.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://mkr.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://twx.hammf.cn

================================================================================
来源：http://all.sysykeji.top

统计汇总
来源：http://dhg.aibaodan.cn

================================================================================
来源：http://fdu.hnxiangtu.top

按语言统计（条）：
来源：http://bnh.fanxiaobao.xyz

Python ......... 252
来源：http://khh.shangyingyoupin.top

PHP ............ 252
来源：http://aep.hnqzz.top

JavaScript ..... 252
来源：http://hji.sjlbkw.cn

TypeScript ..... 212
来源：http://vtq.jinyuanbaomall.cn

Java ........... 212
来源：http://tnh.svipenyu.cn

Go ............. 212
来源：http://bsm.yj202588.top

Ruby ........... 212
来源：http://skj.jqgfzy.top

C# ............. 212
来源：http://ejl.cashguo.top

C .............. 30
来源：http://gxh.fehbvm.com

C++ ............ 30
来源：http://rfm.xziqi.cn

SQL ............ 90
来源：http://kux.zhiwuduotai.top

Bash ........... 80
来源：http://lya.yanxiufei.cn

Kotlin ......... 15
来源：http://skl.bjfxy.top

Swift .......... 15
来源：http://jim.yj202588.top

Lua ............ 10
来源：http://tbe.haohaochexian.top

Perl ........... 10
来源：http://edg.xuanzx.com

Scala .......... 10
来源：http://sms.chenzaomai.com

------------------------------------
来源：http://frr.jqgfzy.top

合计 ........... 2106 条
来源：http://bwj.tianlin.xyz

按章节统计：
来源：http://hml.tanke756.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ald.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ech.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gub.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://swe.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cnf.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ldb.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yjm.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ruo.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://opi.ehwqpu.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hxd.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rfi.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cgp.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jea.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ono.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wit.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sdk.yfazqb.com

Q SQL 专题                              90
来源：http://ctz.jlsjyb.cn

R Bash 专题                             80
来源：http://oxg.fengsongda.top

S C / C++ 专题                          60
来源：http://psf.shanyushiyangkeji.top

T 其他语言补充                          60
来源：http://iva.tianlin.xyz

U 高频实用片段                         120
来源：http://eab.hysaishi.cn

------------------------------------
来源：http://wwu.ywan-chungtsiang.top

合计                                  2106 条
来源：http://ioa.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://fnu.fanxiaobao.xyz

使用提醒
来源：http://twg.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://qrf.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fam.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eml.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://faa.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dzc.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rbt.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://uqu.jyoumei.cn

================================================================================
来源：http://oyr.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://vcd.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://amp.ydjk.org.cn

================================================================================
来源：http://dnl.c1oappe.top

【收录内容】
来源：http://yws.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://xap.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qhl.dashuyun.cn

SQL · Bash · C · C++
来源：http://nfa.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cbd.jinyuanbaomall.cn

【使用说明】
来源：http://hlr.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kkd.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jzn.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jwk.yuxming.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qqp.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tnf.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://npw.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mrp.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bfy.mhx1999.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rlu.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jvg.xziqi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://szs.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mje.sxryk.cn

【文件统计】
来源：http://vlj.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mju.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://xbr.zycfv.cn

目  录
来源：http://pwv.vehdjk.com

--------------------------------------------------------------------------------
来源：http://zvy.andypj.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zxj.jqgufenzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pxd.hfpthk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yyg.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://scr.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kxx.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ytg.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rhw.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kjn.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yxd.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ngf.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mtr.wangshuangyany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jzx.kuanghao11.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sgg.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://juy.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nwh.sweek.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jfr.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oys.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://qed.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kxd.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://idk.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qyy.redwolf501.top

================================================================================
来源：http://kia.hysaishi.cn

A. 基础语法与类型
来源：http://dov.smart0.xyz

================================================================================
来源：http://njd.jinqigufen.top

[A01] Hello World
来源：http://ibh.ehwqpu.com

Py:   print("Hello, World!")
来源：http://gyp.uphjek.com

PHP:  echo "Hello, World!";
来源：http://vsa.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://ukc.jianghu66.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zbo.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://ius.aizwys.cn

Go:   fmt.Println("Hello, World!")
来源：http://ylc.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://xuv.cucudq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lvm.vqdsnc.cn

[A02] 变量声明与赋值
来源：http://lei.vehdjk.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://abu.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pvq.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://jlt.yongpay.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xxb.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://hmp.fzhhl.top

Go:   name := "Alex"; age := 20
来源：http://gqm.sufxvd.cn

Ruby: name = "Alex"; age = 20
来源：http://xqg.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://ind.quarkkingdee.top

[A03] 常量定义
来源：http://oac.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://doz.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://icq.vehdjk.com

JS:   const PI = 3.14159;
来源：http://fkv.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://zgw.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://iko.0kj1m.cn

Go:   const PI = 3.14159
来源：http://tpx.uphjek.com

Ruby: PI = 3.14159
来源：http://vqk.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://meo.yuxming.cn

[A04] 判断变量类型
来源：http://neq.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bnf.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tte.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rxu.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://wge.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pto.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bzo.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tso.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://mib.daxiang520.top

[A05] 整数除法与取模
来源：http://bqk.guannengcc.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rjs.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nou.quarkkingdee.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tpz.quarkkingdee.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xdj.snrcjt.cn

Java: 7 / 2; 7 % 2
来源：http://gbv.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://gqd.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://voq.jiagoushi.top

C#:   7 / 2; 7 % 2
来源：http://kta.vqdsnc.cn

[A06] 字符串转数字
来源：http://smn.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://hmb.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://emy.daxiang520.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tal.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://zbz.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pdm.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ciw.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ryr.fktsv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vns.ehwqpu.com

[A07] 数字转字符串
来源：http://pme.wangshuangyany.cn

Py:   str(42)
来源：http://bhi.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://lgl.fzhhl.top

JS:   String(42); (42).toString()
来源：http://nti.jiagoushi.top

TS:   String(42)
来源：http://has.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pyb.zhaomingkeji.xyz

Go:   strconv.Itoa(42)
来源：http://knf.jiagoushi.top

Ruby: 42.to_s
来源：http://mbp.yangfankeji.com

C#:   42.ToString()
来源：http://lyx.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://kel.cqqwz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kgx.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mzq.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ngl.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ekc.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xdm.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://evx.gogol.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jva.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gxh.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://fnz.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bvn.fehbvm.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xqp.ydjk.org.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vrg.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bhl.chenjidiqi.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uep.ydzc1.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gms.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yhc.jiagoushi.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hcq.xingfuxueyuan.xyz


<!-- 参考信息 -->