代发 wailian999

[U65] PHP：会话
来源：http://gyj.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gur.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://piz.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ymg.andypj.xyz

[U67] PHP：处理文件上传
来源：http://wfu.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qjj.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://fdq.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zgr.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://pih.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vrh.tian-w.cn

[U70] PHP：PDO 事务
来源：http://nlu.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://atg.yonumen.top

[U71] PHP：抛出异常
来源：http://rcj.vqdsnc.cn

throw new RuntimeException("失败", 500);
来源：http://ptr.jiagoushi.top

[U72] PHP：写错误日志
来源：http://fhm.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://irh.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://bnx.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://rak.yj20258.top

[U74] PHP：读取环境变量
来源：http://rkd.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://wfl.9152youxi.cn

[U75] PHP：依赖注入
来源：http://bsf.zhengqikj.top

composer require psr/container
来源：http://aku.dianchejie.cn

[U76] PHP：简单路由
来源：http://gll.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kcw.daxiang520.top

[U77] PHP：模板渲染
来源：http://gqq.cucudq.cn

composer require twig/twig
来源：http://zgs.gzhubu.top

[U78] PHP：单元测试
来源：http://oqw.pycfn.com

composer require --dev phpunit/phpunit
来源：http://eqr.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://rpn.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://fky.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://ofg.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qct.tian-w.cn

[U81] JS：初始化项目
来源：http://wjb.quarkkingdee.top

npm init -y;  npm i express
来源：http://xcw.shuidangran.top

[U82] JS：package.json 脚本
来源：http://ibw.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kkm.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://hio.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://psz.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://zbn.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://axf.meibo888.top

[U85] JS：可选链
来源：http://krv.fengsongda.top

a?.b?.c
来源：http://jlf.jyoumei.cn

[U86] JS：空值合并
来源：http://kyi.c1oappe.top

a ?? b
来源：http://jay.fehbvm.com

[U87] JS：解构默认值
来源：http://fif.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://unz.snrcjt.cn

[U88] JS：对象展开合并
来源：http://nwu.ppjwa.cn

{ ...a, ...b }
来源：http://xul.yuanzhike.top

[U89] JS：数组去重
来源：http://mak.sysykeji.top

[...new Set(arr)]
来源：http://crc.yonumen.top

[U90] JS：数字数组排序
来源：http://eux.daria6918.cn

[...arr].sort((a, b) => a - b)
来源：http://bef.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://mpn.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vfk.ctjpmb.com

[U92] JS：深拷贝
来源：http://psp.chenzaomai.com

structuredClone(obj)
来源：http://jia.bjfxy.top

[U93] JS：模板字符串
来源：http://cls.hammf.cn

`共 ${n} 条`
来源：http://heh.fehbvm.com

[U94] JS：箭头函数
来源：http://omi.fzhhl.top

const double = x => x * 2;
来源：http://hpe.fehbvm.com

[U95] JS：Promise 包装
来源：http://rrw.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://ens.meibo888.top

[U96] JS：async/await 与异常
来源：http://txt.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vdh.snrcjt.cn

[U97] JS：并发请求
来源：http://svy.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://gvw.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://yxd.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pqc.smart0.xyz

[U99] JS：事件监听
来源：http://prz.shuidangran.top

el.addEventListener("click", e => {})
来源：http://hab.yongpay.top

[U100] JS：DOM 查询
来源：http://xmz.jinqigfzy.top

document.querySelector(".item")
来源：http://tgs.zhengqikj.top

[U101] JS：classList 操作
来源：http://ufd.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://qbh.sysykeji.top

[U102] JS：本地存储
来源：http://pbj.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eoh.birdmap.top

[U103] JS：定时器
来源：http://vfv.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dfl.zhengqikj.top

[U104] JS：防抖
来源：http://nsx.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpi.sxryk.cn

[U105] JS：节流
来源：http://wvb.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dmd.316326.xyz

[U106] JS：日期格式化
来源：http://olc.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lal.smart0.xyz

[U107] JS：数字千分位
来源：http://qvj.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pxp.sjlbkw.cn

[U108] JS：随机整数
来源：http://kzn.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xbu.xziqi.cn

[U109] JS：数组分组
来源：http://etz.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://amf.yuanzhike.top

[U110] JS：数组分块
来源：http://dub.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yxx.yj20258.top

[U111] JS：对象转 Map
来源：http://xaa.tianlin.xyz

new Map(Object.entries(obj))
来源：http://ylu.aizwys.cn

[U112] JS：字符串补位
来源：http://vvk.yj20258888.top

"7".padStart(3, "0")
来源：http://dqh.xinyue.icu

[U113] JS：正则替换全部
来源：http://mux.dianchejie.cn

s.replaceAll("a", "b")
来源：http://vif.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://eyh.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://phd.iojbl.cn

[U115] JS：生成 UUID
来源：http://juw.guannengcc.top

crypto.randomUUID()
来源：http://obe.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://ydd.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://zuf.9152youxi.cn

[U117] JS：单元测试
来源：http://anw.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://qml.xziqi.cn

[U118] JS：开发服务器
来源：http://kif.ivvv.top

npm i -D vite;  npx vite
来源：http://bwl.nanxuanxn.top

[U119] JS：生产构建
来源：http://ees.andypj.xyz

npx vite build
来源：http://xdg.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://vci.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://rug.zhengqikj.top

================================================================================
来源：http://bpz.ivvv.top

统计汇总
来源：http://rai.ivvv.top

================================================================================
来源：http://rzu.bjfxy.top

按语言统计（条）：
来源：http://ref.jianghu66.top

Python ......... 252
来源：http://bde.zdbjq.cn

PHP ............ 252
来源：http://apc.zhijiandao.cn

JavaScript ..... 252
来源：http://ibe.nwbrower.top

TypeScript ..... 212
来源：http://kmq.zhixingplan.top

Java ........... 212
来源：http://kes.aibaodan.cn

Go ............. 212
来源：http://hjm.xylfe.cn

Ruby ........... 212
来源：http://wub.ivvv.top

C# ............. 212
来源：http://poa.shanyushiyangkeji.top

C .............. 30
来源：http://nfb.hongshengwenyu.top

C++ ............ 30
来源：http://xgy.jiagoushi.top

SQL ............ 90
来源：http://mza.jinghuilouyu.cn

Bash ........... 80
来源：http://ede.nanxinkj.top

Kotlin ......... 15
来源：http://qct.cqqwz.cn

Swift .......... 15
来源：http://ogi.tanke756.top

Lua ............ 10
来源：http://jek.sysykeji.top

Perl ........... 10
来源：http://fqx.sjlbkw.cn

Scala .......... 10
来源：http://nom.hammf.cn

------------------------------------
来源：http://czt.gaohongyu789.top

合计 ........... 2106 条
来源：http://ais.tanke756.top

按章节统计：
来源：http://lja.tanke756.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yln.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://peq.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gno.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://boy.hongshengwenyu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mqt.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fsk.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sej.jqgufenzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://azr.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ejr.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kie.hcnkem.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gnw.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pdx.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fyj.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qfr.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fei.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mum.yanxiufei.cn

Q SQL 专题                              90
来源：http://qvt.gzhubu.top

R Bash 专题                             80
来源：http://zcx.xylfe.cn

S C / C++ 专题                          60
来源：http://zoa.yj20258.top

T 其他语言补充                          60
来源：http://eab.haohaochexian.top

U 高频实用片段                         120
来源：http://ftu.tianlin.xyz

------------------------------------
来源：http://pqg.hongshengwenyu.top

合计                                  2106 条
来源：http://scj.yj20258.top

--------------------------------------------------------------------------------
来源：http://tpu.sxryk.cn

使用提醒
来源：http://lob.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://nuc.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eci.wangshuangyany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ebc.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://urt.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dtx.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qkq.jinqigfzy.top

—— 文件结束 ——
来源：http://mal.shuidangran.top

================================================================================
来源：http://srz.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://axs.cucudq.cn

Common Programming Examples Cheat Book
来源：http://psb.guannengcc.top

================================================================================
来源：http://mng.feifeiyinyue.top

【收录内容】
来源：http://mgb.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jre.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://any.zhixingplan.top

SQL · Bash · C · C++
来源：http://nix.guowangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dha.xingfuxueyuan.xyz

【使用说明】
来源：http://odd.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gvg.pengpengdd.cyou

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://umk.guowangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yhr.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ndk.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wab.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sny.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jby.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vav.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://etm.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://faz.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yck.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://msp.hfpthk.cn

【文件统计】
来源：http://cef.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hce.hesvh.cn

--------------------------------------------------------------------------------
来源：http://ktl.hammf.cn

目  录
来源：http://qai.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://qgy.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jgj.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://may.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wdg.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://irb.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fof.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hev.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mrr.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dri.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gwm.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ulm.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dkj.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mex.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jyv.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://weq.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jwj.pycfn.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fds.zdbjq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dam.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://phb.gzhubu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qfx.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qxm.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eip.316326.xyz

================================================================================
来源：http://ytt.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://ylb.dianchejie.cn

================================================================================
来源：http://yrz.xinyue.icu

[A01] Hello World
来源：http://mte.zycfv.cn

Py:   print("Hello, World!")
来源：http://icb.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://yvs.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://uuq.epnwcf.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ndu.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://mtc.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://ori.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://ceu.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tti.cdnleiting.top

[A02] 变量声明与赋值
来源：http://zej.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zmp.sjlbkw.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zph.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://aby.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yyx.tian-w.cn

Java: String name = "Alex"; int age = 20;
来源：http://ouf.zhoulong.xyz

Go:   name := "Alex"; age := 20
来源：http://umo.tanke756.top

Ruby: name = "Alex"; age = 20
来源：http://cta.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://lyh.ctjpmb.com

[A03] 常量定义
来源：http://xcv.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ujr.shangyingyoupin.top

PHP:  const PI = 3.14159;
来源：http://gpq.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://ycg.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://zfg.tianlin.xyz

Java: static final double PI = 3.14159;
来源：http://ykr.ywan-chungtsiang.top

Go:   const PI = 3.14159
来源：http://kcj.hfpthk.cn

Ruby: PI = 3.14159
来源：http://gmi.tarul.cn

C#:   const double PI = 3.14159;
来源：http://bly.shzxlz.cn

[A04] 判断变量类型
来源：http://wtb.ivvv.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mdh.fzhhl.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lei.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mvy.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://ola.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lww.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://lby.zycfv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xav.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://vzz.mhx1999.top

[A05] 整数除法与取模
来源：http://qud.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xvf.snrcjt.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pyd.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://etw.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://brh.hammf.cn

Java: 7 / 2; 7 % 2
来源：http://kjw.ybcxt.top

Go:   7 / 2; 7 % 2
来源：http://dri.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://dsy.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://hgd.xziqi.cn

[A06] 字符串转数字
来源：http://yrd.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://bzi.yangfankeji.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ppf.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mnf.feifeiyinyue.top

TS:   parseInt("42", 10); Number("42")
来源：http://lls.snrcjt.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oeu.jyoumei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ftn.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lmy.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pnw.guannengcc.top

[A07] 数字转字符串
来源：http://uqj.hammf.cn

Py:   str(42)
来源：http://ckj.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://xty.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://xys.gzhubu.top

TS:   String(42)
来源：http://jbt.jlsjyb.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zqa.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://yhs.shanyushiyangtech.top

Ruby: 42.to_s
来源：http://ctp.nanxinkj.top

C#:   42.ToString()
来源：http://eik.jyoumei.cn

[A08] 取整与四舍五入
来源：http://sfi.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://szz.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://umw.zhengqikj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zrq.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sav.ydzc1.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fgf.aibaodan.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fla.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ldp.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tlj.ywan-chungtsiang.top

[A09] 绝对值与最大最小值
来源：http://vlm.fktsv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qko.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zca.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hyh.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uij.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wub.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hmy.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gbc.tian-w.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ujl.jyoumei.cn


<!-- 参考信息 -->