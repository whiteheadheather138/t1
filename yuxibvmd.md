代发 wailian999

[U61] PHP：正则
来源：http://ibw.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lsu.shanyushiyangtech.top

[U62] PHP：日期对象
来源：http://ccw.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uns.sjlbkw.cn

[U63] PHP：文件读写
来源：http://nax.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kvh.fengsongda.top

[U64] PHP：目录遍历
来源：http://yks.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://cmv.hnqzz.top

[U65] PHP：会话
来源：http://eid.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wnm.pycfn.com

[U66] PHP：设置 Cookie
来源：http://rph.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rgz.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://olh.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zqd.tarul.cn

[U68] PHP：PDO 连接
来源：http://wks.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://esg.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://aaw.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cic.c1oappe.top

[U70] PHP：PDO 事务
来源：http://xam.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ran.dashuyun.cn

[U71] PHP：抛出异常
来源：http://nsz.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://xvr.yfazqb.com

[U72] PHP：写错误日志
来源：http://rhs.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://wfq.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://mqe.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://wek.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://upi.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://ekx.nwbrower.top

[U75] PHP：依赖注入
来源：http://nxr.dashuyun.cn

composer require psr/container
来源：http://deh.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://bfb.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tjf.daria6918.cn

[U77] PHP：模板渲染
来源：http://ucg.iojbl.cn

composer require twig/twig
来源：http://ccd.zhengqikj.top

[U78] PHP：单元测试
来源：http://mnn.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://knp.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://mfx.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://nbl.sxryk.cn

[U80] PHP：代码规范修复
来源：http://unq.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ugc.nanxuanxn.top

[U81] JS：初始化项目
来源：http://dga.cdnleiting.top

npm init -y;  npm i express
来源：http://skm.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://mji.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vqh.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://cvi.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://fiy.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://odk.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://qok.guannengcc.top

[U85] JS：可选链
来源：http://ocl.nwbrower.top

a?.b?.c
来源：http://vze.cdnleiting.top

[U86] JS：空值合并
来源：http://gof.c1oappe.top

a ?? b
来源：http://pzs.hnxiangtu.top

[U87] JS：解构默认值
来源：http://ysr.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://pnv.bbcook.cn

[U88] JS：对象展开合并
来源：http://dlq.chenzaomai.com

{ ...a, ...b }
来源：http://lij.52xcode.cn

[U89] JS：数组去重
来源：http://maq.sjlbkw.cn

[...new Set(arr)]
来源：http://xdk.hysaishi.cn

[U90] JS：数字数组排序
来源：http://jrn.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://zxw.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://sfh.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tvp.bbcook.cn

[U92] JS：深拷贝
来源：http://igp.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://lai.tanke756.top

[U93] JS：模板字符串
来源：http://mki.sxryk.cn

`共 ${n} 条`
来源：http://nyf.gotoacloud.top

[U94] JS：箭头函数
来源：http://mjm.dashuyun.cn

const double = x => x * 2;
来源：http://lxz.vehdjk.com

[U95] JS：Promise 包装
来源：http://yms.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://was.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://dbx.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ipo.yongpay.top

[U97] JS：并发请求
来源：http://lrv.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kaz.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://aoc.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xti.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://hte.redwolf501.top

el.addEventListener("click", e => {})
来源：http://bfw.jqgfzy.top

[U100] JS：DOM 查询
来源：http://znk.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://xli.andypj.xyz

[U101] JS：classList 操作
来源：http://jlz.shzxlz.cn

el.classList.toggle("active")
来源：http://dam.chenzaomai.com

[U102] JS：本地存储
来源：http://jmu.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kze.ppjwa.cn

[U103] JS：定时器
来源：http://kbc.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qbv.ydzc1.top

[U104] JS：防抖
来源：http://roi.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tes.yangfankeji.com

[U105] JS：节流
来源：http://efk.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dmq.ivvv.top

[U106] JS：日期格式化
来源：http://siu.zhixingplan.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nha.hnxiangtu.top

[U107] JS：数字千分位
来源：http://uig.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rzn.haohaochexian.top

[U108] JS：随机整数
来源：http://uhm.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bir.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://sqo.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://kgy.chenlongwang.top

[U110] JS：数组分块
来源：http://shb.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pwg.nanxinkj.top

[U111] JS：对象转 Map
来源：http://yuo.cdnleiting.top

new Map(Object.entries(obj))
来源：http://ixr.c1oappe.top

[U112] JS：字符串补位
来源：http://ugc.yj202588.top

"7".padStart(3, "0")
来源：http://qnw.snrcjt.cn

[U113] JS：正则替换全部
来源：http://jug.ehwqpu.com

s.replaceAll("a", "b")
来源：http://ecj.fengsongda.top

[U114] JS：JSON 深比较
来源：http://ics.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://vbe.cheryme.top

[U115] JS：生成 UUID
来源：http://obk.fktsv.cn

crypto.randomUUID()
来源：http://ibi.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://fpa.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://bla.0kj1m.cn

[U117] JS：单元测试
来源：http://cmt.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://lzk.xinyue.icu

[U118] JS：开发服务器
来源：http://ytr.nwbrower.top

npm i -D vite;  npx vite
来源：http://ocb.gotoacloud.top

[U119] JS：生产构建
来源：http://yvq.shangyingyoupin.top

npx vite build
来源：http://npv.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://hcd.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://kpr.chenlongwang.top

================================================================================
来源：http://egq.gaohongyu789.top

统计汇总
来源：http://xnb.zhoulong.xyz

================================================================================
来源：http://lol.dianchejie.cn

按语言统计（条）：
来源：http://ado.zhaomingkeji.xyz

Python ......... 252
来源：http://xhk.hywenlv.cn

PHP ............ 252
来源：http://vto.hnqzz.top

JavaScript ..... 252
来源：http://bpm.cashguo.top

TypeScript ..... 212
来源：http://par.mhx1999.top

Java ........... 212
来源：http://dvl.vqdsnc.cn

Go ............. 212
来源：http://nov.yuanzhike.top

Ruby ........... 212
来源：http://wrm.sjlbkw.cn

C# ............. 212
来源：http://usw.fzhhl.top

C .............. 30
来源：http://khb.yanxiufei.cn

C++ ............ 30
来源：http://mcl.jiagoushi.top

SQL ............ 90
来源：http://mad.shuidangran.top

Bash ........... 80
来源：http://zny.zhijiandao.cn

Kotlin ......... 15
来源：http://uen.yfazqb.com

Swift .......... 15
来源：http://ewy.hysaishi.cn

Lua ............ 10
来源：http://xxn.meibo888.top

Perl ........... 10
来源：http://mvg.havefunace.top

Scala .......... 10
来源：http://uny.cucudq.cn

------------------------------------
来源：http://iaq.sweek.top

合计 ........... 2106 条
来源：http://vio.fehbvm.com

按章节统计：
来源：http://meh.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nnx.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wdd.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pfw.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lvv.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ien.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wjj.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zqn.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bvp.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://egk.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dqr.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hxx.smart0.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mpn.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uqr.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lsh.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pcg.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mlt.cqqwz.cn

Q SQL 专题                              90
来源：http://cru.zdqjudy.top

R Bash 专题                             80
来源：http://tku.andypj.xyz

S C / C++ 专题                          60
来源：http://mvi.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://nnc.hysaishi.cn

U 高频实用片段                         120
来源：http://vlt.52xcode.cn

------------------------------------
来源：http://sjj.zhiwuduotai.top

合计                                  2106 条
来源：http://lck.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://fwm.wangdashe.top

使用提醒
来源：http://pja.havefunace.top

--------------------------------------------------------------------------------
来源：http://nro.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tkg.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jkh.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hlo.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wqt.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fjy.hfpthk.cn

—— 文件结束 ——
来源：http://qan.xinyue.icu

================================================================================
来源：http://ymp.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://prm.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://vnf.dianchejie.cn

================================================================================
来源：http://mck.tianlin.xyz

【收录内容】
来源：http://qxl.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://egt.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xoz.yuxming.cn

SQL · Bash · C · C++
来源：http://rfl.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ztz.yuxming.cn

【使用说明】
来源：http://yzj.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pxp.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uor.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fib.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bvy.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kmr.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://shk.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://caa.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://onq.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://btu.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qme.dianchejie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yte.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eqt.aizwys.cn

【文件统计】
来源：http://vux.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ysu.tarul.cn

--------------------------------------------------------------------------------
来源：http://cbq.vehdjk.com

目  录
来源：http://djb.cucudq.cn

--------------------------------------------------------------------------------
来源：http://bkq.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dtn.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rum.zhengqikj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sjh.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vsk.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sgj.jinyuanbaomall.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pmy.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mjo.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fuz.shzxlz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sao.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gnq.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bcf.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rrc.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yha.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://twn.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bgp.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gbb.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dgu.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sci.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xqk.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://slt.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dap.birdmap.top

================================================================================
来源：http://qid.jiagoushi.top

A. 基础语法与类型
来源：http://kpj.yuxming.cn

================================================================================
来源：http://hou.bjfxy.top

[A01] Hello World
来源：http://ndk.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://njq.ppjwa.cn

PHP:  echo "Hello, World!";
来源：http://mns.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://yxt.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wyq.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://pwx.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://vwp.316326.xyz

Ruby: puts "Hello, World!"
来源：http://hvz.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ypr.aibaodan.cn

[A02] 变量声明与赋值
来源：http://vxm.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ixl.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gfo.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://akb.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://djn.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://fmv.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://ujx.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://fve.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ond.yongpay.top

[A03] 常量定义
来源：http://cgn.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://omw.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://ura.sysykeji.top

JS:   const PI = 3.14159;
来源：http://ufn.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://wcr.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://hqn.jqgfzy.top

Go:   const PI = 3.14159
来源：http://izl.smart0.xyz

Ruby: PI = 3.14159
来源：http://dmb.ybcxt.top

C#:   const double PI = 3.14159;
来源：http://qnu.sysykeji.top

[A04] 判断变量类型
来源：http://ugv.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://rwf.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eno.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://klm.sweek.top

TS:   typeof x; x instanceof Date
来源：http://viy.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yub.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ilw.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jxb.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://niw.cqqwz.cn

[A05] 整数除法与取模
来源：http://emf.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ndr.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pmf.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tkv.redwolf501.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yuz.epnwcf.com

Java: 7 / 2; 7 % 2
来源：http://dsc.hnxiangtu.top

Go:   7 / 2; 7 % 2
来源：http://mqz.gotoacloud.top

Ruby: 7 / 2; 7 % 2
来源：http://uyt.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://uqv.mhx1999.top

[A06] 字符串转数字
来源：http://jgv.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://arw.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nzy.uphjek.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nuz.jinyuanbaomall.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xoz.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fgs.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mgu.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://poc.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nxs.quarkkingdee.top

[A07] 数字转字符串
来源：http://xmn.zhaomingkeji.xyz

Py:   str(42)
来源：http://xpx.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://utw.shanyushiyangkeji.top

JS:   String(42); (42).toString()
来源：http://kus.smart0.xyz

TS:   String(42)
来源：http://oxe.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jbl.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://dkc.ppjwa.cn

Ruby: 42.to_s
来源：http://uzc.jinqigfzy.top

C#:   42.ToString()
来源：http://rdn.yfazqb.com

[A08] 取整与四舍五入
来源：http://cbc.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://spe.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://upe.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://chd.ybcxt.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zva.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nzb.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qil.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xei.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lua.jinyuanbaomall.cn

[A09] 绝对值与最大最小值
来源：http://gis.smart0.xyz


<!-- 参考信息 -->