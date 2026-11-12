代发 wailian999

[U65] PHP：会话
来源：http://mkh.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nbp.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://vby.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rwi.yongpay.top

[U67] PHP：处理文件上传
来源：http://uvd.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://spr.aizwys.cn

[U68] PHP：PDO 连接
来源：http://kug.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bco.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://uzj.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://edc.cucudq.cn

[U70] PHP：PDO 事务
来源：http://cqz.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nia.tianlin.xyz

[U71] PHP：抛出异常
来源：http://min.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://ksd.bbcook.cn

[U72] PHP：写错误日志
来源：http://vgm.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://qra.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://gqd.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://yih.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://jvm.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://nve.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://bvl.gaohongyu789.top

composer require psr/container
来源：http://irb.quarkkingdee.top

[U76] PHP：简单路由
来源：http://efo.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rua.9152youxi.cn

[U77] PHP：模板渲染
来源：http://ccs.jinyuanbaomall.cn

composer require twig/twig
来源：http://dwb.dashuyun.cn

[U78] PHP：单元测试
来源：http://rht.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://dft.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://ior.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://zbb.smart0.xyz

[U80] PHP：代码规范修复
来源：http://cgw.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mvu.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://uvm.cashguo.top

npm init -y;  npm i express
来源：http://lmb.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://vhh.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ifq.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://klc.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://djs.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://mli.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://suf.hysaishi.cn

[U85] JS：可选链
来源：http://kit.uphjek.com

a?.b?.c
来源：http://djn.epnwcf.com

[U86] JS：空值合并
来源：http://kfe.yj202588.top

a ?? b
来源：http://anj.ivvv.top

[U87] JS：解构默认值
来源：http://npq.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://jal.gzhubu.top

[U88] JS：对象展开合并
来源：http://vgz.aibaodan.cn

{ ...a, ...b }
来源：http://qle.zhengqikj.top

[U89] JS：数组去重
来源：http://agx.jiagoushi.top

[...new Set(arr)]
来源：http://ksv.yueranfly.top

[U90] JS：数字数组排序
来源：http://zao.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://htr.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://qjw.52xcode.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://brk.yanxiufei.cn

[U92] JS：深拷贝
来源：http://pky.daria6918.cn

structuredClone(obj)
来源：http://jln.cheryme.top

[U93] JS：模板字符串
来源：http://dox.zhiwuduotai.top

`共 ${n} 条`
来源：http://dsz.jiagoushi.top

[U94] JS：箭头函数
来源：http://fzr.yfazqb.com

const double = x => x * 2;
来源：http://yjn.andypj.xyz

[U95] JS：Promise 包装
来源：http://skq.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://tgt.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://ery.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nfy.aizwys.cn

[U97] JS：并发请求
来源：http://bpq.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xqf.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://sgd.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://msf.pengpengdd.cyou

[U99] JS：事件监听
来源：http://wxz.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://bce.yfazqb.com

[U100] JS：DOM 查询
来源：http://jpn.ydzc1.top

document.querySelector(".item")
来源：http://twj.jqgfzy.top

[U101] JS：classList 操作
来源：http://pap.sjlbkw.cn

el.classList.toggle("active")
来源：http://lqi.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://vid.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://scl.zhongyouzk.top

[U103] JS：定时器
来源：http://art.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ikt.zhijiandao.cn

[U104] JS：防抖
来源：http://lrt.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrf.haohaochexian.top

[U105] JS：节流
来源：http://kse.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://umh.quarkkingdee.top

[U106] JS：日期格式化
来源：http://zqt.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xmh.zhijiandao.cn

[U107] JS：数字千分位
来源：http://rng.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vbi.zycfv.cn

[U108] JS：随机整数
来源：http://mlt.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vak.jqgufenzy.top

[U109] JS：数组分组
来源：http://okq.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://ptz.c1oappe.top

[U110] JS：数组分块
来源：http://ofb.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hkw.shzxlz.cn

[U111] JS：对象转 Map
来源：http://ozq.haohaochexian.top

new Map(Object.entries(obj))
来源：http://tuh.jyoumei.cn

[U112] JS：字符串补位
来源：http://zzp.ppjwa.cn

"7".padStart(3, "0")
来源：http://uua.tarul.cn

[U113] JS：正则替换全部
来源：http://skn.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://tpi.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://xiv.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dwf.guannengcc.top

[U115] JS：生成 UUID
来源：http://dzx.gaohongyu789.top

crypto.randomUUID()
来源：http://ngj.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://mog.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://gee.xinyue.icu

[U117] JS：单元测试
来源：http://jev.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://efj.nwbrower.top

[U118] JS：开发服务器
来源：http://opd.fktsv.cn

npm i -D vite;  npx vite
来源：http://cst.xuetiantiany.cn

[U119] JS：生产构建
来源：http://hsi.feifeiyinyue.top

npx vite build
来源：http://avn.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://kfp.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://uqm.zdbjq.cn

================================================================================
来源：http://myb.shzxlz.cn

统计汇总
来源：http://hjb.hysaishi.cn

================================================================================
来源：http://fkt.nanxinkj.top

按语言统计（条）：
来源：http://bjk.yueranfly.top

Python ......... 252
来源：http://ipm.shuidangran.top

PHP ............ 252
来源：http://sbq.tanke756.top

JavaScript ..... 252
来源：http://tgc.guowangkeji.top

TypeScript ..... 212
来源：http://jyj.hongshengwenyu.top

Java ........... 212
来源：http://dmn.birdmap.top

Go ............. 212
来源：http://lfv.yuanzhike.top

Ruby ........... 212
来源：http://iin.nwbrower.top

C# ............. 212
来源：http://iwg.zhiwuduotai.top

C .............. 30
来源：http://diw.yuxming.cn

C++ ............ 30
来源：http://xbo.sxryk.cn

SQL ............ 90
来源：http://evb.gogol.net.cn

Bash ........... 80
来源：http://yel.yj202588.top

Kotlin ......... 15
来源：http://uvo.gotoacloud.top

Swift .......... 15
来源：http://qae.guowangkeji.top

Lua ............ 10
来源：http://scm.yfazqb.com

Perl ........... 10
来源：http://rtl.wangshuangyany.cn

Scala .......... 10
来源：http://ilv.jinghuilouyu.cn

------------------------------------
来源：http://fzo.daxiang520.top

合计 ........... 2106 条
来源：http://erq.zhijiandao.cn

按章节统计：
来源：http://haf.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vez.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yqc.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dpw.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mef.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://veu.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fmw.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ysb.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hem.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yja.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rtk.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://luk.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ige.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://abu.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eum.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qtq.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aio.fzhhl.top

Q SQL 专题                              90
来源：http://cmw.c1oappe.top

R Bash 专题                             80
来源：http://lzs.gogol.net.cn

S C / C++ 专题                          60
来源：http://kte.fktsv.cn

T 其他语言补充                          60
来源：http://ema.hywenlv.cn

U 高频实用片段                         120
来源：http://bbb.chenjidiqi.icu

------------------------------------
来源：http://azr.aibaodan.cn

合计                                  2106 条
来源：http://ahv.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://cog.hammf.cn

使用提醒
来源：http://eeb.gzhubu.top

--------------------------------------------------------------------------------
来源：http://egc.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tti.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hlp.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dsl.snrcjt.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cpy.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kxh.zhiwuduotai.top

—— 文件结束 ——
来源：http://dcq.hongshengwenyu.top

================================================================================
来源：http://wbp.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://zia.ehwqpu.com

Common Programming Examples Cheat Book
来源：http://egt.hnqzz.top

================================================================================
来源：http://rgg.fktsv.cn

【收录内容】
来源：http://njw.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mml.jinqigufen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bsw.316326.xyz

SQL · Bash · C · C++
来源：http://sou.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://byd.zdqjudy.top

【使用说明】
来源：http://loe.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://skt.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wxf.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://erq.hongshengwenyu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hqy.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://tqp.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xuv.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tfa.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://apu.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dso.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://arf.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fve.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pfc.pengpengdd.cyou

【文件统计】
来源：http://adb.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qxo.sweek.top

--------------------------------------------------------------------------------
来源：http://slh.zhiwuduotai.top

目  录
来源：http://yqx.fehbvm.com

--------------------------------------------------------------------------------
来源：http://hzx.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bsd.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://egw.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mrk.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dwb.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jup.ydjk.org.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zbg.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rpe.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mqd.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tiu.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bef.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oma.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hzp.zhoulong.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cnr.guowangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://due.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uth.zhijiandao.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yrm.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bcu.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nmg.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xjj.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://utt.shangyingyoupin.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rbp.ppjwa.cn

================================================================================
来源：http://lmp.yonumen.top

A. 基础语法与类型
来源：http://mgf.bjfxy.top

================================================================================
来源：http://nrg.chenzaomai.com

[A01] Hello World
来源：http://paq.tian-w.cn

Py:   print("Hello, World!")
来源：http://vjh.bjfxy.top

PHP:  echo "Hello, World!";
来源：http://pdj.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://smx.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wpz.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://kmr.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://vqo.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://nfx.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ewl.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://slu.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ksi.316326.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://evc.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://vof.sysykeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qds.havefunace.top

Java: String name = "Alex"; int age = 20;
来源：http://psv.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://baq.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://nnq.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://cnz.hongshengwenyu.top

[A03] 常量定义
来源：http://lzf.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xgj.tarul.cn

PHP:  const PI = 3.14159;
来源：http://bwe.meibo888.top

JS:   const PI = 3.14159;
来源：http://yzm.haohaochexian.top

TS:   const PI: number = 3.14159;
来源：http://vfg.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://kpt.chenzaomai.com

Go:   const PI = 3.14159
来源：http://ibi.cucudq.cn

Ruby: PI = 3.14159
来源：http://ofm.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://djx.jinqigfzy.top

[A04] 判断变量类型
来源：http://lbu.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://opv.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hbb.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dad.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://mzh.zhoulong.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wut.vehdjk.com

Go:   reflect.TypeOf(x).Name()
来源：http://ppo.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ski.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://tsk.9152youxi.cn

[A05] 整数除法与取模
来源：http://feg.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fgo.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jwp.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zim.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iyt.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://wrq.sysykeji.top

Go:   7 / 2; 7 % 2
来源：http://ews.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://zzt.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://adk.zdqjudy.top

[A06] 字符串转数字
来源：http://rqq.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://skp.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ijo.zhixingplan.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cro.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xfc.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bcd.jlsjyb.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xlo.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fsy.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wkn.tian-w.cn

[A07] 数字转字符串
来源：http://aub.zhongyouzk.top

Py:   str(42)
来源：http://kiz.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://har.vqdsnc.cn

JS:   String(42); (42).toString()
来源：http://zud.fktsv.cn

TS:   String(42)
来源：http://jjv.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lql.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://cqi.ppjwa.cn

Ruby: 42.to_s
来源：http://qxq.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://vwk.meibo888.top

[A08] 取整与四舍五入
来源：http://tla.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uwp.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://avc.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://exq.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://arp.jyoumei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://alj.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fwv.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zvp.xuanzx.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://huu.sxryk.cn

[A09] 绝对值与最大最小值
来源：http://ouk.nanxinkj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nlw.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uyn.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qsa.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lff.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lld.hfpthk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xtk.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ujn.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://igj.zhaomingkeji.xyz


<!-- 参考信息 -->