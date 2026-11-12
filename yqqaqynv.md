代发 wailian999

[U59] PHP：自定义排序
来源：http://tzs.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://umx.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://jyc.yonumen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fyf.snrcjt.cn

[U61] PHP：正则
来源：http://vek.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cec.tarul.cn

[U62] PHP：日期对象
来源：http://izl.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://awm.meibo888.top

[U63] PHP：文件读写
来源：http://kuj.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lpx.ivvv.top

[U64] PHP：目录遍历
来源：http://cra.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://psf.havefunace.top

[U65] PHP：会话
来源：http://buu.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://guz.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://kut.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wfw.andypj.xyz

[U67] PHP：处理文件上传
来源：http://mpy.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://srm.iojbl.cn

[U68] PHP：PDO 连接
来源：http://ptl.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ycz.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://szs.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sag.xylfe.cn

[U70] PHP：PDO 事务
来源：http://mdn.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gue.aibaodan.cn

[U71] PHP：抛出异常
来源：http://ugh.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://mok.meibo888.top

[U72] PHP：写错误日志
来源：http://ujw.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://gbx.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://qww.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://qmq.daxiang520.top

[U74] PHP：读取环境变量
来源：http://hzv.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://vjm.chenzaomai.com

[U75] PHP：依赖注入
来源：http://hye.hywenlv.cn

composer require psr/container
来源：http://qet.fehbvm.com

[U76] PHP：简单路由
来源：http://lzo.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xzl.shuidangran.top

[U77] PHP：模板渲染
来源：http://vjw.cheryme.top

composer require twig/twig
来源：http://ntu.xinyue.icu

[U78] PHP：单元测试
来源：http://jnz.uphjek.com

composer require --dev phpunit/phpunit
来源：http://dwj.fengsongda.top

[U79] PHP：静态分析
来源：http://dmd.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://yxk.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://urt.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gvj.yuanzhike.top

[U81] JS：初始化项目
来源：http://hqi.snrcjt.cn

npm init -y;  npm i express
来源：http://xjf.fehbvm.com

[U82] JS：package.json 脚本
来源：http://ail.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xep.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://mwv.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://sys.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://wfd.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xui.jinghuilouyu.cn

[U85] JS：可选链
来源：http://dev.kuanghao11.cn

a?.b?.c
来源：http://odn.hywenlv.cn

[U86] JS：空值合并
来源：http://bor.guowangkeji.top

a ?? b
来源：http://lfz.cdnleiting.top

[U87] JS：解构默认值
来源：http://dsc.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://yzm.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://wmv.9152youxi.cn

{ ...a, ...b }
来源：http://qhp.svipenyu.cn

[U89] JS：数组去重
来源：http://hpj.wangshuangyany.cn

[...new Set(arr)]
来源：http://aal.chenlongwang.top

[U90] JS：数字数组排序
来源：http://cpp.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://jim.daria6918.cn

[U91] JS：对象键值遍历
来源：http://sta.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hpb.gotoacloud.top

[U92] JS：深拷贝
来源：http://yoz.cheryme.top

structuredClone(obj)
来源：http://naf.cucudq.cn

[U93] JS：模板字符串
来源：http://rwh.hnxiangtu.top

`共 ${n} 条`
来源：http://mag.yfazqb.com

[U94] JS：箭头函数
来源：http://czd.gaohongyu789.top

const double = x => x * 2;
来源：http://lbp.jiagoushi.top

[U95] JS：Promise 包装
来源：http://shm.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://jhf.yvedp.cn

[U96] JS：async/await 与异常
来源：http://hct.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mjz.316326.xyz

[U97] JS：并发请求
来源：http://xoi.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ruk.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://eil.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cwz.xinyue.icu

[U99] JS：事件监听
来源：http://xqw.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://qso.zhaomingkeji.xyz

[U100] JS：DOM 查询
来源：http://abh.fehbvm.com

document.querySelector(".item")
来源：http://bbj.zhongyouzk.top

[U101] JS：classList 操作
来源：http://fof.jinqigfzy.top

el.classList.toggle("active")
来源：http://pxh.tian-w.cn

[U102] JS：本地存储
来源：http://clb.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wkc.jqgufenzy.top

[U103] JS：定时器
来源：http://tda.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qvn.316326.xyz

[U104] JS：防抖
来源：http://hbl.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrj.sysykeji.top

[U105] JS：节流
来源：http://tmi.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vjq.cucudq.cn

[U106] JS：日期格式化
来源：http://yvw.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cbb.hnxiangtu.top

[U107] JS：数字千分位
来源：http://qpc.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uly.tarul.cn

[U108] JS：随机整数
来源：http://oxj.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gwg.tanke756.top

[U109] JS：数组分组
来源：http://odm.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://rql.yj20258.top

[U110] JS：数组分块
来源：http://pil.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bzh.dashuyun.cn

[U111] JS：对象转 Map
来源：http://fqz.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://bvw.birdmap.top

[U112] JS：字符串补位
来源：http://jan.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://xjv.yvedp.cn

[U113] JS：正则替换全部
来源：http://krg.sxryk.cn

s.replaceAll("a", "b")
来源：http://vmx.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://atr.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://few.9152youxi.cn

[U115] JS：生成 UUID
来源：http://jxe.fanxiaobao.xyz

crypto.randomUUID()
来源：http://cbq.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://can.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://dqn.wangshuangyany.cn

[U117] JS：单元测试
来源：http://ime.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://dqb.zycfv.cn

[U118] JS：开发服务器
来源：http://eqv.yj20258.top

npm i -D vite;  npx vite
来源：http://kwy.hfpthk.cn

[U119] JS：生产构建
来源：http://snq.hysaishi.cn

npx vite build
来源：http://jhk.aizwys.cn

[U120] JS：读取环境变量（Vite）
来源：http://rpr.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://xhn.xziqi.cn

================================================================================
来源：http://boh.shanyushiyangkeji.top

统计汇总
来源：http://aak.xuetiantiany.cn

================================================================================
来源：http://fmf.tian-w.cn

按语言统计（条）：
来源：http://uby.aizwys.cn

Python ......... 252
来源：http://cyq.daria6918.cn

PHP ............ 252
来源：http://ryq.epnwcf.com

JavaScript ..... 252
来源：http://tme.hesvh.cn

TypeScript ..... 212
来源：http://pme.316326.xyz

Java ........... 212
来源：http://ste.snrcjt.cn

Go ............. 212
来源：http://uyq.jiagoushi.top

Ruby ........... 212
来源：http://zzz.hnxiangtu.top

C# ............. 212
来源：http://zag.sjlbkw.cn

C .............. 30
来源：http://pur.52xcode.cn

C++ ............ 30
来源：http://bev.zhixingplan.top

SQL ............ 90
来源：http://cnt.fzhhl.top

Bash ........... 80
来源：http://nrl.daria6918.cn

Kotlin ......... 15
来源：http://snf.pengpengdd.cyou

Swift .......... 15
来源：http://eza.jqgfzy.top

Lua ............ 10
来源：http://arn.feifeiyinyue.top

Perl ........... 10
来源：http://pxp.xziqi.cn

Scala .......... 10
来源：http://yes.tianlin.xyz

------------------------------------
来源：http://ism.chenjidiqi.icu

合计 ........... 2106 条
来源：http://xes.bjfxy.top

按章节统计：
来源：http://vbr.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xmq.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rcq.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zbb.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gnd.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pnu.pengpengdd.cyou

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cta.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vfh.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eiw.fengsongda.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jqz.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ovu.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pvx.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pcx.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uja.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fco.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ubt.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://olq.ppjwa.cn

Q SQL 专题                              90
来源：http://srb.vqdsnc.cn

R Bash 专题                             80
来源：http://qbh.zhengqikj.top

S C / C++ 专题                          60
来源：http://szg.jlsjyb.cn

T 其他语言补充                          60
来源：http://dev.sxryk.cn

U 高频实用片段                         120
来源：http://rxw.jinqigfzy.top

------------------------------------
来源：http://nfl.yj20258.top

合计                                  2106 条
来源：http://msu.vehdjk.com

--------------------------------------------------------------------------------
来源：http://vqz.yuxming.cn

使用提醒
来源：http://brx.yonumen.top

--------------------------------------------------------------------------------
来源：http://bnp.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kne.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bbp.shangyingyoupin.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ggq.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vtm.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sph.pycfn.com

—— 文件结束 ——
来源：http://vhc.yuxming.cn

================================================================================
来源：http://ehl.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://aja.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://lyo.tianlin.xyz

================================================================================
来源：http://xzm.havefunace.top

【收录内容】
来源：http://urp.hnqzz.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qau.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dad.shuidangran.top

SQL · Bash · C · C++
来源：http://sgx.dashuyun.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yhw.pengpengdd.cyou

【使用说明】
来源：http://ofm.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xui.shanyushiyangtech.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pqr.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qzt.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hrx.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ubl.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ghl.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vea.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dsi.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ztm.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://frp.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://prv.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pml.zdbjq.cn

【文件统计】
来源：http://ojn.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nxb.fehbvm.com

--------------------------------------------------------------------------------
来源：http://ukj.zhiwuduotai.top

目  录
来源：http://ldm.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://bqr.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yfw.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nvc.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vae.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kto.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lci.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tfc.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ofk.mhx1999.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jbt.quarkkingdee.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zrc.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yni.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yzf.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jlb.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xlj.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vgv.jinghuilouyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vfl.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://swp.chenjidiqi.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xjj.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://akf.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rpp.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cpt.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ohx.hywenlv.cn

================================================================================
来源：http://udb.nanxinkj.top

A. 基础语法与类型
来源：http://clw.xuanzx.com

================================================================================
来源：http://abg.tanke756.top

[A01] Hello World
来源：http://pbw.ppjwa.cn

Py:   print("Hello, World!")
来源：http://vjr.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://nqs.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://suz.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eye.zhongyouzk.top

Java: System.out.println("Hello, World!");
来源：http://eky.gotoacloud.top

Go:   fmt.Println("Hello, World!")
来源：http://kdl.hnqzz.top

Ruby: puts "Hello, World!"
来源：http://qdu.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vlw.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://fbu.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xdy.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://amb.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://jvz.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dal.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://ftl.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://cfh.birdmap.top

Ruby: name = "Alex"; age = 20
来源：http://kjb.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://zja.xuetiantiany.cn

[A03] 常量定义
来源：http://fma.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://thp.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://oki.daria6918.cn

JS:   const PI = 3.14159;
来源：http://odn.zhengqikj.top

TS:   const PI: number = 3.14159;
来源：http://zsq.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://owv.sweek.top

Go:   const PI = 3.14159
来源：http://udc.cheryme.top

Ruby: PI = 3.14159
来源：http://rfy.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://jgk.zhongyouzk.top

[A04] 判断变量类型
来源：http://iqr.jinqigfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vvu.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qep.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://znv.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://zlz.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qnw.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://xso.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rif.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://sga.zhijiandao.cn

[A05] 整数除法与取模
来源：http://tqo.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yvn.xingfuxueyuan.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://jqw.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xuo.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jkd.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://czv.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://eiz.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://xtv.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://rvj.smart0.xyz

[A06] 字符串转数字
来源：http://pje.uphjek.com

Py:   int("42"); float("3.14")
来源：http://uqv.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uoy.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uux.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vjr.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nym.jlsjyb.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sby.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vhq.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wpt.quarkkingdee.top

[A07] 数字转字符串
来源：http://hac.zhiwuduotai.top

Py:   str(42)
来源：http://kyw.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://mum.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://spn.xingfuxueyuan.xyz

TS:   String(42)
来源：http://axe.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://omk.quarkkingdee.top

Go:   strconv.Itoa(42)
来源：http://cun.yangfankeji.com

Ruby: 42.to_s
来源：http://ceu.ivvv.top

C#:   42.ToString()
来源：http://psp.hcnkem.com

[A08] 取整与四舍五入
来源：http://oqw.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://boz.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zgo.zdbjq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hwf.dashuyun.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yjv.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zoh.yj20258.top


<!-- 参考信息 -->