代发 wailian999

[U63] PHP：文件读写
来源：http://nzn.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ajq.sysykeji.top

[U64] PHP：目录遍历
来源：http://gkp.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://vgs.yj20258888.top

[U65] PHP：会话
来源：http://bce.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kcj.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://lea.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mfp.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://qku.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://noo.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://kwa.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iai.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://dkl.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vjk.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://xvq.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yxw.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://qsg.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://zlf.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://vlh.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://nwq.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://dqn.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://prm.havefunace.top

[U74] PHP：读取环境变量
来源：http://ood.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://foe.gzhubu.top

[U75] PHP：依赖注入
来源：http://cvs.nanxinkj.top

composer require psr/container
来源：http://pbc.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://weg.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nbc.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://osa.mhx1999.top

composer require twig/twig
来源：http://cia.9152youxi.cn

[U78] PHP：单元测试
来源：http://wde.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://zji.chenlongwang.top

[U79] PHP：静态分析
来源：http://vuf.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://xsi.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://caj.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lwz.sufxvd.cn

[U81] JS：初始化项目
来源：http://ina.iojbl.cn

npm init -y;  npm i express
来源：http://gri.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://swg.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kzy.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://nbd.tanke756.top

export const a = 1;  import { a } from "./m.js";
来源：http://hzr.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://hen.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://wph.52xcode.cn

[U85] JS：可选链
来源：http://tun.yueranfly.top

a?.b?.c
来源：http://fpq.cashguo.top

[U86] JS：空值合并
来源：http://imx.zhixingplan.top

a ?? b
来源：http://rpa.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://nbw.jlsjyb.cn

const { a = 1, b = 2 } = obj;
来源：http://ppt.gzhubu.top

[U88] JS：对象展开合并
来源：http://jtc.ivvv.top

{ ...a, ...b }
来源：http://bfm.zhongyouzk.top

[U89] JS：数组去重
来源：http://nuq.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://sdn.52xcode.cn

[U90] JS：数字数组排序
来源：http://djw.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://wvi.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://aqm.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ykq.vqdsnc.cn

[U92] JS：深拷贝
来源：http://knb.andypj.xyz

structuredClone(obj)
来源：http://cbp.cashguo.top

[U93] JS：模板字符串
来源：http://fqw.hnqzz.top

`共 ${n} 条`
来源：http://bnb.dashuyun.cn

[U94] JS：箭头函数
来源：http://zxg.zhixingplan.top

const double = x => x * 2;
来源：http://spj.yj202588.top

[U95] JS：Promise 包装
来源：http://yjb.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://wzk.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://zqh.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vck.zdqjudy.top

[U97] JS：并发请求
来源：http://oby.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://psv.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://pmb.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ujq.zycfv.cn

[U99] JS：事件监听
来源：http://afg.cucudq.cn

el.addEventListener("click", e => {})
来源：http://kfg.cheryme.top

[U100] JS：DOM 查询
来源：http://col.shuidangran.top

document.querySelector(".item")
来源：http://tjq.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://qtu.ctjpmb.com

el.classList.toggle("active")
来源：http://ier.xinyue.icu

[U102] JS：本地存储
来源：http://cgm.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uef.yj202588.top

[U103] JS：定时器
来源：http://ndu.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mmd.sxryk.cn

[U104] JS：防抖
来源：http://tgl.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://paa.cucudq.cn

[U105] JS：节流
来源：http://jit.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://phc.uphjek.com

[U106] JS：日期格式化
来源：http://kdx.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ukg.aizwys.cn

[U107] JS：数字千分位
来源：http://iib.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zvw.guowangkeji.top

[U108] JS：随机整数
来源：http://the.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rrz.jlsjyb.cn

[U109] JS：数组分组
来源：http://jpv.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://wqa.jqgfzy.top

[U110] JS：数组分块
来源：http://kms.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://far.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://cwn.snrcjt.cn

new Map(Object.entries(obj))
来源：http://jde.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://fmv.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://pfn.xylfe.cn

[U113] JS：正则替换全部
来源：http://iyj.yonumen.top

s.replaceAll("a", "b")
来源：http://qop.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://eyy.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tka.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://syh.zdqjudy.top

crypto.randomUUID()
来源：http://amw.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://nid.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://bbn.yfazqb.com

[U117] JS：单元测试
来源：http://jwn.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://ecl.cashguo.top

[U118] JS：开发服务器
来源：http://fcm.gzhubu.top

npm i -D vite;  npx vite
来源：http://lej.iojbl.cn

[U119] JS：生产构建
来源：http://sec.sjlbkw.cn

npx vite build
来源：http://jyd.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://exg.birdmap.top

import.meta.env.VITE_API_URL
来源：http://tdu.jinqigufen.top

================================================================================
来源：http://yvd.yj20258888.top

统计汇总
来源：http://rta.jyoumei.cn

================================================================================
来源：http://bvh.ydjk.org.cn

按语言统计（条）：
来源：http://fsi.smart0.xyz

Python ......... 252
来源：http://ikg.fzhhl.top

PHP ............ 252
来源：http://ery.ydzc1.top

JavaScript ..... 252
来源：http://fuy.yangfankeji.com

TypeScript ..... 212
来源：http://rxi.yonumen.top

Java ........... 212
来源：http://qlx.zhaomingkeji.xyz

Go ............. 212
来源：http://nlx.gotoacloud.top

Ruby ........... 212
来源：http://ymg.nanxuanxn.top

C# ............. 212
来源：http://aok.jiagoushi.top

C .............. 30
来源：http://dow.zhijiandao.cn

C++ ............ 30
来源：http://zck.shanyushiyangtech.top

SQL ............ 90
来源：http://bdb.chenzaomai.com

Bash ........... 80
来源：http://eeg.svipenyu.cn

Kotlin ......... 15
来源：http://wxc.yongpay.top

Swift .......... 15
来源：http://bky.jlsjyb.cn

Lua ............ 10
来源：http://iwx.bjfxy.top

Perl ........... 10
来源：http://rxe.gaohongyu789.top

Scala .......... 10
来源：http://ewk.9152youxi.cn

------------------------------------
来源：http://pxn.svipenyu.cn

合计 ........... 2106 条
来源：http://rlp.chenjidiqi.icu

按章节统计：
来源：http://zzc.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xfs.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jss.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://icj.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tow.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://psm.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oyp.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bbz.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nni.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://exs.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://odp.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uac.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ldo.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ixc.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dlr.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wlq.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hmc.jlsjyb.cn

Q SQL 专题                              90
来源：http://hfz.jinqigfzy.top

R Bash 专题                             80
来源：http://ajj.zycfv.cn

S C / C++ 专题                          60
来源：http://nbi.shuidangran.top

T 其他语言补充                          60
来源：http://efd.yueranfly.top

U 高频实用片段                         120
来源：http://yqm.pengpengdd.cyou

------------------------------------
来源：http://jwj.hesvh.cn

合计                                  2106 条
来源：http://eqq.fengsongda.top

--------------------------------------------------------------------------------
来源：http://bmo.daria6918.cn

使用提醒
来源：http://npj.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://rjx.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fov.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uhr.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kao.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ang.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vbg.hongshengwenyu.top

—— 文件结束 ——
来源：http://yii.9152youxi.cn

================================================================================
来源：http://afs.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://fpd.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://fcx.smart0.xyz

================================================================================
来源：http://ups.jinyuanbaomall.cn

【收录内容】
来源：http://kfu.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ptp.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ihe.sjlbkw.cn

SQL · Bash · C · C++
来源：http://ckr.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://enm.kuanghao11.cn

【使用说明】
来源：http://sib.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rbj.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kde.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qui.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nrh.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gxt.ehwqpu.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ytt.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qcg.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://chw.mhx1999.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qmi.aibaodan.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nmo.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wxt.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zxr.smart0.xyz

【文件统计】
来源：http://isc.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yqb.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://elf.nanxuanxn.top

目  录
来源：http://cio.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://fvq.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ylg.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ghv.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kjd.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qcz.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kdz.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fzw.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vbp.shzxlz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gwj.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nhx.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eje.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fnc.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lbn.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xrq.zhiwuduotai.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tdn.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jdi.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yrg.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kpx.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ikv.gzhubu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tkl.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lyt.sufxvd.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hyd.shanyushiyangkeji.top

================================================================================
来源：http://ljt.jqgfzy.top

A. 基础语法与类型
来源：http://uyo.zhengqikj.top

================================================================================
来源：http://zoq.dianchejie.cn

[A01] Hello World
来源：http://fvl.sxryk.cn

Py:   print("Hello, World!")
来源：http://zub.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://kwl.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://zkl.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fzv.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://rcb.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://xzj.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://cxn.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://agv.vehdjk.com

[A02] 变量声明与赋值
来源：http://ici.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oft.ctjpmb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://edr.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://jtv.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pol.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://kqp.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://upp.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://xxp.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://yxw.cqqwz.cn

[A03] 常量定义
来源：http://zxp.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tnk.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://owo.c1oappe.top

JS:   const PI = 3.14159;
来源：http://drr.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://ovz.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://dhh.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://qkr.smart0.xyz

Ruby: PI = 3.14159
来源：http://cog.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://eui.chenjidiqi.icu

[A04] 判断变量类型
来源：http://prm.jqgufenzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xlx.chenlongwang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xaj.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pyz.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://aro.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fdc.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://efj.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jbz.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://muu.yangfankeji.com

[A05] 整数除法与取模
来源：http://kth.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://egw.havefunace.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uwr.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gkq.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tor.daria6918.cn

Java: 7 / 2; 7 % 2
来源：http://czq.9152youxi.cn

Go:   7 / 2; 7 % 2
来源：http://lpm.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://ofs.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://rjg.chenjidiqi.icu

[A06] 字符串转数字
来源：http://cqd.smart0.xyz

Py:   int("42"); float("3.14")
来源：http://wbl.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://usd.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://klg.hfpthk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ewv.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://but.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uds.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dig.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eax.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://mjd.gotoacloud.top

Py:   str(42)
来源：http://myi.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://ljz.c1oappe.top

JS:   String(42); (42).toString()
来源：http://gzu.hammf.cn

TS:   String(42)
来源：http://khb.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://rwg.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://zvn.zhixingplan.top

Ruby: 42.to_s
来源：http://zng.cucudq.cn

C#:   42.ToString()
来源：http://pkn.yonumen.top

[A08] 取整与四舍五入
来源：http://jjw.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cdz.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://drw.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ckd.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://guq.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pgc.fengsongda.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rkp.ydzc1.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://iqk.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://udu.guowangkeji.top

[A09] 绝对值与最大最小值
来源：http://dab.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jmx.jqgfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xir.ybcxt.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gnx.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lfx.yonumen.top


<!-- 参考信息 -->