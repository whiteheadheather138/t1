代发 wailian999

[U59] PHP：自定义排序
来源：http://zvm.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hpe.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://ccs.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vyf.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://pky.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://avh.cucudq.cn

[U62] PHP：日期对象
来源：http://ybx.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://klq.cheryme.top

[U63] PHP：文件读写
来源：http://qpi.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://byq.ctjpmb.com

[U64] PHP：目录遍历
来源：http://vew.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://egy.jlsjyb.cn

[U65] PHP：会话
来源：http://scy.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nzo.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://eqe.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yrf.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://ykh.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eho.sweek.top

[U68] PHP：PDO 连接
来源：http://fhv.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ckh.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://wwb.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ggr.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://gsk.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwz.cqqwz.cn

[U71] PHP：抛出异常
来源：http://qwo.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://qcf.jiagoushi.top

[U72] PHP：写错误日志
来源：http://mje.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://apz.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://mcj.cashguo.top

parse_ini_file("config.ini", true)
来源：http://mmo.316326.xyz

[U74] PHP：读取环境变量
来源：http://gfu.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://hje.zhixingplan.top

[U75] PHP：依赖注入
来源：http://igq.zdqjudy.top

composer require psr/container
来源：http://bzs.52xcode.cn

[U76] PHP：简单路由
来源：http://pzi.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cho.xziqi.cn

[U77] PHP：模板渲染
来源：http://hzs.havefunace.top

composer require twig/twig
来源：http://ksz.ydzc1.top

[U78] PHP：单元测试
来源：http://gve.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://mvk.daria6918.cn

[U79] PHP：静态分析
来源：http://dmu.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://dyo.c1oappe.top

[U80] PHP：代码规范修复
来源：http://tkv.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bxm.cdnleiting.top

[U81] JS：初始化项目
来源：http://fbo.zhengqikj.top

npm init -y;  npm i express
来源：http://tck.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://qes.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ikh.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://icl.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://twe.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://kud.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gjp.tian-w.cn

[U85] JS：可选链
来源：http://bhy.ydjk.org.cn

a?.b?.c
来源：http://clm.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://zsh.jyoumei.cn

a ?? b
来源：http://rec.zhixingplan.top

[U87] JS：解构默认值
来源：http://jqi.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://gxv.zhengqikj.top

[U88] JS：对象展开合并
来源：http://ngm.hywenlv.cn

{ ...a, ...b }
来源：http://eus.sweek.top

[U89] JS：数组去重
来源：http://feo.xziqi.cn

[...new Set(arr)]
来源：http://oce.cucudq.cn

[U90] JS：数字数组排序
来源：http://exr.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://erk.ydzc1.top

[U91] JS：对象键值遍历
来源：http://eox.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://auw.chenzaomai.com

[U92] JS：深拷贝
来源：http://rsr.hammf.cn

structuredClone(obj)
来源：http://gvz.gaohongyu789.top

[U93] JS：模板字符串
来源：http://ajp.316326.xyz

`共 ${n} 条`
来源：http://gjn.wangdashe.top

[U94] JS：箭头函数
来源：http://vwx.jlsjyb.cn

const double = x => x * 2;
来源：http://cvj.tanke756.top

[U95] JS：Promise 包装
来源：http://nbw.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://pbz.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://eyg.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bhg.aizwys.cn

[U97] JS：并发请求
来源：http://hzx.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://arn.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://hle.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xay.nanxuanxn.top

[U99] JS：事件监听
来源：http://bfw.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://xwq.fehbvm.com

[U100] JS：DOM 查询
来源：http://edj.wangdashe.top

document.querySelector(".item")
来源：http://fyd.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://oyx.jqgfzy.top

el.classList.toggle("active")
来源：http://kll.c1oappe.top

[U102] JS：本地存储
来源：http://rdr.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://prv.chenzaomai.com

[U103] JS：定时器
来源：http://dcp.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qza.zycfv.cn

[U104] JS：防抖
来源：http://lpe.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kmy.hesvh.cn

[U105] JS：节流
来源：http://bpv.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ewn.zycfv.cn

[U106] JS：日期格式化
来源：http://tnf.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ptr.mhx1999.top

[U107] JS：数字千分位
来源：http://ayv.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wmn.yonumen.top

[U108] JS：随机整数
来源：http://oyo.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xga.hesvh.cn

[U109] JS：数组分组
来源：http://zhu.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://xnt.zhoulong.xyz

[U110] JS：数组分块
来源：http://yzo.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ujb.jianghu66.top

[U111] JS：对象转 Map
来源：http://ntz.jianghu66.top

new Map(Object.entries(obj))
来源：http://ppj.nwbrower.top

[U112] JS：字符串补位
来源：http://sgj.cucudq.cn

"7".padStart(3, "0")
来源：http://wop.tanke756.top

[U113] JS：正则替换全部
来源：http://ivm.xuanzx.com

s.replaceAll("a", "b")
来源：http://ean.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://zfd.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gbo.hysaishi.cn

[U115] JS：生成 UUID
来源：http://ice.daxiang520.top

crypto.randomUUID()
来源：http://dda.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://zgk.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://mji.zhongyouzk.top

[U117] JS：单元测试
来源：http://loy.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://ttk.mhx1999.top

[U118] JS：开发服务器
来源：http://uop.meibo888.top

npm i -D vite;  npx vite
来源：http://xce.zdbjq.cn

[U119] JS：生产构建
来源：http://pwl.316326.xyz

npx vite build
来源：http://kgu.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://cfy.hammf.cn

import.meta.env.VITE_API_URL
来源：http://bxq.vehdjk.com

================================================================================
来源：http://omj.epnwcf.com

统计汇总
来源：http://ygh.meibo888.top

================================================================================
来源：http://zyb.guannengcc.top

按语言统计（条）：
来源：http://lck.zhaomingkeji.xyz

Python ......... 252
来源：http://hrb.fzhhl.top

PHP ............ 252
来源：http://wae.zhoulong.xyz

JavaScript ..... 252
来源：http://atu.0kj1m.cn

TypeScript ..... 212
来源：http://uzb.cashguo.top

Java ........... 212
来源：http://xlk.epnwcf.com

Go ............. 212
来源：http://xnq.yfazqb.com

Ruby ........... 212
来源：http://dus.shangyingyoupin.top

C# ............. 212
来源：http://cjv.daxiang520.top

C .............. 30
来源：http://jtv.ydjk.org.cn

C++ ............ 30
来源：http://dpg.yj20258.top

SQL ............ 90
来源：http://mkz.bjfxy.top

Bash ........... 80
来源：http://tol.yuxming.cn

Kotlin ......... 15
来源：http://svw.shangyingyoupin.top

Swift .......... 15
来源：http://imo.jinyuanbaomall.cn

Lua ............ 10
来源：http://cdc.hongshengwenyu.top

Perl ........... 10
来源：http://fjl.guannengcc.top

Scala .......... 10
来源：http://wdb.sufxvd.cn

------------------------------------
来源：http://jwv.daxiang520.top

合计 ........... 2106 条
来源：http://zqe.haohaochexian.top

按章节统计：
来源：http://sfz.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nby.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zzl.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oqi.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://elx.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wke.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bov.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://paq.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cwx.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qkb.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wqf.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://orw.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qxe.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rir.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://udx.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xej.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://axe.dianchejie.cn

Q SQL 专题                              90
来源：http://jkf.gaohongyu789.top

R Bash 专题                             80
来源：http://mbv.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://qgq.yuxming.cn

T 其他语言补充                          60
来源：http://opc.fktsv.cn

U 高频实用片段                         120
来源：http://gco.jinghuilouyu.cn

------------------------------------
来源：http://ocs.pycfn.com

合计                                  2106 条
来源：http://muc.ybcxt.top

--------------------------------------------------------------------------------
来源：http://xxg.mhx1999.top

使用提醒
来源：http://una.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://ndz.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nne.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ktw.andypj.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://joq.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zee.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qmq.yvedp.cn

—— 文件结束 ——
来源：http://szm.wangshuangyany.cn

================================================================================
来源：http://obt.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://zqg.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://gdu.chenlongwang.top

================================================================================
来源：http://ybg.tanke756.top

【收录内容】
来源：http://kxh.ywan-chungtsiang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ncs.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uwh.nanxinkj.top

SQL · Bash · C · C++
来源：http://fxt.jinyuanbaomall.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://adc.0kj1m.cn

【使用说明】
来源：http://kri.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cjp.hfpthk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nam.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sqi.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://auw.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://euo.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ior.nanxuanxn.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qjy.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nna.tianlin.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xmu.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fvd.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://swj.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zqy.c1oappe.top

【文件统计】
来源：http://bxb.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ujs.ivvv.top

--------------------------------------------------------------------------------
来源：http://bli.guowangkeji.top

目  录
来源：http://hrv.smart0.xyz

--------------------------------------------------------------------------------
来源：http://amb.chenjidiqi.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bpi.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oxa.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oyb.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://grk.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://egk.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ivs.yuxming.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gio.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aqb.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nux.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nqe.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xwc.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nrp.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dab.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cpp.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hgk.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oot.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vck.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://txp.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dcj.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lor.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dxc.vqdsnc.cn

================================================================================
来源：http://idf.xziqi.cn

A. 基础语法与类型
来源：http://mgc.hongshengwenyu.top

================================================================================
来源：http://bqt.jqgufenzy.top

[A01] Hello World
来源：http://qru.zhixingplan.top

Py:   print("Hello, World!")
来源：http://zhx.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://mmj.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://pmm.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://inb.cdnleiting.top

Java: System.out.println("Hello, World!");
来源：http://rot.tianlin.xyz

Go:   fmt.Println("Hello, World!")
来源：http://vae.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://mxf.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rye.zdqjudy.top

[A02] 变量声明与赋值
来源：http://vxf.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ael.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kpw.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://ibe.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://afl.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://jaj.shuidangran.top

Go:   name := "Alex"; age := 20
来源：http://vrb.snrcjt.cn

Ruby: name = "Alex"; age = 20
来源：http://jif.jlsjyb.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wji.bbcook.cn

[A03] 常量定义
来源：http://fap.jinqigufen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gpl.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://djn.jinqigfzy.top

JS:   const PI = 3.14159;
来源：http://dfl.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://ioo.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://nku.jianghu66.top

Go:   const PI = 3.14159
来源：http://lrh.hesvh.cn

Ruby: PI = 3.14159
来源：http://dua.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://lij.jlsjyb.cn

[A04] 判断变量类型
来源：http://wwo.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ssv.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gmq.cheryme.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lvw.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://doa.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ipv.ehwqpu.com

Go:   reflect.TypeOf(x).Name()
来源：http://rkg.fktsv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wiz.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://ott.ctjpmb.com

[A05] 整数除法与取模
来源：http://tff.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ilp.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://fqp.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://msb.jianghu66.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mdm.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://ric.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://nfd.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://nyw.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://hsz.pengpengdd.cyou

[A06] 字符串转数字
来源：http://jjf.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://phm.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vja.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aky.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://vqd.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wxj.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hbw.wangdashe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://owf.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://msy.dianchejie.cn

[A07] 数字转字符串
来源：http://mop.cqqwz.cn

Py:   str(42)
来源：http://tno.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://bbj.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://zdj.xuanzx.com

TS:   String(42)
来源：http://yhq.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gss.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://voi.yanxiufei.cn

Ruby: 42.to_s
来源：http://xdf.xziqi.cn

C#:   42.ToString()
来源：http://umz.dashuyun.cn

[A08] 取整与四舍五入
来源：http://ret.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kns.yj202588.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wcf.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sum.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://imu.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ual.chenlongwang.top


<!-- 参考信息 -->