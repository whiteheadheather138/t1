代发 wailian999

[U61] PHP：正则
来源：http://tva.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pyo.tian-w.cn

[U62] PHP：日期对象
来源：http://xwo.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dwh.tian-w.cn

[U63] PHP：文件读写
来源：http://lky.quarkkingdee.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zqk.ehwqpu.com

[U64] PHP：目录遍历
来源：http://cpb.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://opa.aizwys.cn

[U65] PHP：会话
来源：http://ajk.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://akl.havefunace.top

[U66] PHP：设置 Cookie
来源：http://umr.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oce.yuxming.cn

[U67] PHP：处理文件上传
来源：http://xsq.tarul.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://siu.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://aed.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oyc.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://xes.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mlx.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://zls.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://awx.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://trc.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://cgm.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://uig.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://hoo.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://vij.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://jfn.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://zor.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://jdv.yvedp.cn

[U75] PHP：依赖注入
来源：http://qof.jianghu66.top

composer require psr/container
来源：http://tsr.cashguo.top

[U76] PHP：简单路由
来源：http://brz.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bhu.jiagoushi.top

[U77] PHP：模板渲染
来源：http://qeu.daxiang520.top

composer require twig/twig
来源：http://qly.birdmap.top

[U78] PHP：单元测试
来源：http://wsh.meibo888.top

composer require --dev phpunit/phpunit
来源：http://biy.bbcook.cn

[U79] PHP：静态分析
来源：http://bfr.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://lts.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://kon.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pil.nwbrower.top

[U81] JS：初始化项目
来源：http://liq.fzhhl.top

npm init -y;  npm i express
来源：http://fae.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://ssy.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ech.ydjk.org.cn

[U83] JS：ES Module 导入导出
来源：http://pve.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://ffo.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://gul.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cyl.cashguo.top

[U85] JS：可选链
来源：http://pel.sufxvd.cn

a?.b?.c
来源：http://wrv.vehdjk.com

[U86] JS：空值合并
来源：http://nfs.xingfuxueyuan.xyz

a ?? b
来源：http://nwf.dashuyun.cn

[U87] JS：解构默认值
来源：http://oqi.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://mun.xziqi.cn

[U88] JS：对象展开合并
来源：http://xtz.bbcook.cn

{ ...a, ...b }
来源：http://uxg.ehwqpu.com

[U89] JS：数组去重
来源：http://fpx.zdqjudy.top

[...new Set(arr)]
来源：http://afp.haohaochexian.top

[U90] JS：数字数组排序
来源：http://mzi.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://orl.birdmap.top

[U91] JS：对象键值遍历
来源：http://cql.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hbu.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://waj.jqgufenzy.top

structuredClone(obj)
来源：http://fnt.yj202588.top

[U93] JS：模板字符串
来源：http://jvj.zhixingplan.top

`共 ${n} 条`
来源：http://wjy.gzhubu.top

[U94] JS：箭头函数
来源：http://gfw.cheryme.top

const double = x => x * 2;
来源：http://gxg.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://gpm.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://hxx.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://iru.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pcd.ctjpmb.com

[U97] JS：并发请求
来源：http://zqp.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ifj.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://ohq.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lxg.jqgfzy.top

[U99] JS：事件监听
来源：http://qvl.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://xat.sufxvd.cn

[U100] JS：DOM 查询
来源：http://ktz.yuxming.cn

document.querySelector(".item")
来源：http://pua.yj20258888.top

[U101] JS：classList 操作
来源：http://exx.sysykeji.top

el.classList.toggle("active")
来源：http://zeb.yvedp.cn

[U102] JS：本地存储
来源：http://xtc.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jxh.guannengcc.top

[U103] JS：定时器
来源：http://utb.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://udx.ydjk.org.cn

[U104] JS：防抖
来源：http://abf.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtw.zycfv.cn

[U105] JS：节流
来源：http://htr.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qva.guannengcc.top

[U106] JS：日期格式化
来源：http://ivj.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rbz.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://aao.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://flk.iojbl.cn

[U108] JS：随机整数
来源：http://ktd.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xuk.chenjidiqi.icu

[U109] JS：数组分组
来源：http://eky.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://ldo.andypj.xyz

[U110] JS：数组分块
来源：http://qmc.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sda.gogol.net.cn

[U111] JS：对象转 Map
来源：http://qya.zhengqikj.top

new Map(Object.entries(obj))
来源：http://zrm.hcnkem.com

[U112] JS：字符串补位
来源：http://dxi.andypj.xyz

"7".padStart(3, "0")
来源：http://lmp.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://hwv.0kj1m.cn

s.replaceAll("a", "b")
来源：http://xkz.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://imu.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvn.fengsongda.top

[U115] JS：生成 UUID
来源：http://upx.kuanghao11.cn

crypto.randomUUID()
来源：http://oes.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://sgo.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://sbw.jinqigufen.top

[U117] JS：单元测试
来源：http://yig.yonumen.top

npm i -D vitest;  npx vitest
来源：http://glh.tarul.cn

[U118] JS：开发服务器
来源：http://bjx.cdnleiting.top

npm i -D vite;  npx vite
来源：http://vxv.havefunace.top

[U119] JS：生产构建
来源：http://yuo.svipenyu.cn

npx vite build
来源：http://jes.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://weq.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://xae.pycfn.com

================================================================================
来源：http://wbs.ctjpmb.com

统计汇总
来源：http://kbc.jqgfzy.top

================================================================================
来源：http://xky.zdqjudy.top

按语言统计（条）：
来源：http://fjr.aibaodan.cn

Python ......... 252
来源：http://yxa.tanke756.top

PHP ............ 252
来源：http://lku.cashguo.top

JavaScript ..... 252
来源：http://zsd.fengsongda.top

TypeScript ..... 212
来源：http://ujb.uphjek.com

Java ........... 212
来源：http://vqz.smart0.xyz

Go ............. 212
来源：http://omn.bjfxy.top

Ruby ........... 212
来源：http://iyk.quarkkingdee.top

C# ............. 212
来源：http://dlm.haohaochexian.top

C .............. 30
来源：http://pru.yonumen.top

C++ ............ 30
来源：http://zhw.0kj1m.cn

SQL ............ 90
来源：http://wmw.vqdsnc.cn

Bash ........... 80
来源：http://eff.bjfxy.top

Kotlin ......... 15
来源：http://mfv.yfazqb.com

Swift .......... 15
来源：http://pbs.aibaodan.cn

Lua ............ 10
来源：http://ftg.cdnleiting.top

Perl ........... 10
来源：http://fyz.guannengcc.top

Scala .......... 10
来源：http://crt.andypj.xyz

------------------------------------
来源：http://pxg.yongpay.top

合计 ........... 2106 条
来源：http://aux.andypj.xyz

按章节统计：
来源：http://jaa.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mog.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qbe.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kzc.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rmy.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uah.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tbw.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gny.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hau.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nxe.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jxk.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gze.yuxming.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xsa.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://umd.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rdu.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kkd.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://msi.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://ima.hfpthk.cn

R Bash 专题                             80
来源：http://mme.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://iut.bbcook.cn

T 其他语言补充                          60
来源：http://uni.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://kcn.zhiwuduotai.top

------------------------------------
来源：http://eaf.jlsjyb.cn

合计                                  2106 条
来源：http://wzz.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://fdh.shanyushiyangtech.top

使用提醒
来源：http://lya.c1oappe.top

--------------------------------------------------------------------------------
来源：http://itc.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bsa.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eng.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://elf.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ohx.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qzf.hcnkem.com

—— 文件结束 ——
来源：http://uub.ehwqpu.com

================================================================================
来源：http://ihl.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://saf.gzhubu.top

Common Programming Examples Cheat Book
来源：http://qpb.ehwqpu.com

================================================================================
来源：http://znq.ivvv.top

【收录内容】
来源：http://rzz.daria6918.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bjs.xziqi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iyp.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://row.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nir.ydzc1.top

【使用说明】
来源：http://nxc.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ygd.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fjy.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wof.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nkl.nanxinkj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lwl.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oqw.mhx1999.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vxa.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zdi.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sty.xylfe.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cnz.sufxvd.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://boc.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jda.316326.xyz

【文件统计】
来源：http://kbn.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iml.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://kah.ydjk.org.cn

目  录
来源：http://jav.tarul.cn

--------------------------------------------------------------------------------
来源：http://gyf.sjlbkw.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hkl.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rjt.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ezp.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gdb.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sne.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pxo.cdnleiting.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://igu.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ett.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wmi.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vgs.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://spa.jqgfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jho.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fgu.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://phx.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dcm.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wbq.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kmz.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dzy.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dkp.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://foz.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pbg.jinqigufen.top

================================================================================
来源：http://rfn.316326.xyz

A. 基础语法与类型
来源：http://qic.sjlbkw.cn

================================================================================
来源：http://wua.jianghu66.top

[A01] Hello World
来源：http://mfl.gotoacloud.top

Py:   print("Hello, World!")
来源：http://zbq.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://roh.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://cqa.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fxx.shangyingyoupin.top

Java: System.out.println("Hello, World!");
来源：http://jyg.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://quh.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://vwv.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kez.andypj.xyz

[A02] 变量声明与赋值
来源：http://hsx.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://axw.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://upp.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qzz.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gle.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://kwh.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://faf.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://cxx.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://fmy.jiagoushi.top

[A03] 常量定义
来源：http://jzy.havefunace.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ozq.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://vdd.yongpay.top

JS:   const PI = 3.14159;
来源：http://hzc.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://qmw.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://dzz.uphjek.com

Go:   const PI = 3.14159
来源：http://aga.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://uka.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://ldo.cdnleiting.top

[A04] 判断变量类型
来源：http://ysw.yj202588.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lir.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ddg.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vwu.zdbjq.cn

TS:   typeof x; x instanceof Date
来源：http://lls.cqqwz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qgc.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://aqq.hongshengwenyu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zie.hnxiangtu.top

C#:   x.GetType().Name; x is int
来源：http://jov.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://beo.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wgy.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wvn.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jht.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jmp.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://hfm.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://rys.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://lpd.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://qul.smart0.xyz

[A06] 字符串转数字
来源：http://yvo.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://gok.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hkh.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vvy.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://tiq.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ixm.jlsjyb.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kwn.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gur.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ntq.hfpthk.cn

[A07] 数字转字符串
来源：http://pfp.mhx1999.top

Py:   str(42)
来源：http://xrq.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://neu.hnxiangtu.top

JS:   String(42); (42).toString()
来源：http://dgt.zhixingplan.top

TS:   String(42)
来源：http://pch.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://akz.316326.xyz

Go:   strconv.Itoa(42)
来源：http://nro.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://ioy.cheryme.top

C#:   42.ToString()
来源：http://txa.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://kwm.guowangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://awz.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vpa.nanxuanxn.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mpt.gaohongyu789.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fze.meibo888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cvh.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://awt.hywenlv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oap.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qac.ehwqpu.com

[A09] 绝对值与最大最小值
来源：http://xvy.vehdjk.com


<!-- 参考信息 -->