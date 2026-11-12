代发 wailian999

[U63] PHP：文件读写
来源：http://ikm.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://spm.guannengcc.top

[U64] PHP：目录遍历
来源：http://iev.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://gam.yangfankeji.com

[U65] PHP：会话
来源：http://hob.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://tya.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://ndy.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ieq.sweek.top

[U67] PHP：处理文件上传
来源：http://fkz.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mtu.uphjek.com

[U68] PHP：PDO 连接
来源：http://kyl.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xik.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://zqj.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pfm.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://ejq.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://umi.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://zuw.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://zwt.cheryme.top

[U72] PHP：写错误日志
来源：http://lxy.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://yqt.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://rjr.birdmap.top

parse_ini_file("config.ini", true)
来源：http://bex.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://eym.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://cyw.haohaochexian.top

[U75] PHP：依赖注入
来源：http://mli.jinghuilouyu.cn

composer require psr/container
来源：http://dxw.yj20258.top

[U76] PHP：简单路由
来源：http://gzc.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://udt.ivvv.top

[U77] PHP：模板渲染
来源：http://epa.meibo888.top

composer require twig/twig
来源：http://cyy.yj20258888.top

[U78] PHP：单元测试
来源：http://fbx.tanke756.top

composer require --dev phpunit/phpunit
来源：http://tht.tianlin.xyz

[U79] PHP：静态分析
来源：http://fvs.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://ror.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://dtp.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://jvc.dianchejie.cn

[U81] JS：初始化项目
来源：http://nis.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://kwr.fengsongda.top

[U82] JS：package.json 脚本
来源：http://gdd.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ryk.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://dbt.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kbs.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://mni.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://csk.mhx1999.top

[U85] JS：可选链
来源：http://ezx.sufxvd.cn

a?.b?.c
来源：http://gbi.fktsv.cn

[U86] JS：空值合并
来源：http://wys.jinqigfzy.top

a ?? b
来源：http://pmo.cheryme.top

[U87] JS：解构默认值
来源：http://xrv.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://cja.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://brt.zycfv.cn

{ ...a, ...b }
来源：http://hiu.yj20258.top

[U89] JS：数组去重
来源：http://dkz.cucudq.cn

[...new Set(arr)]
来源：http://scb.jinqigufen.top

[U90] JS：数字数组排序
来源：http://vnc.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://ubb.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://xmh.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cum.yangfankeji.com

[U92] JS：深拷贝
来源：http://ifp.cdnleiting.top

structuredClone(obj)
来源：http://yth.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://kmr.xuanzx.com

`共 ${n} 条`
来源：http://khl.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://xjo.pycfn.com

const double = x => x * 2;
来源：http://hsn.9152youxi.cn

[U95] JS：Promise 包装
来源：http://wjo.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://wrn.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://osj.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://waw.cucudq.cn

[U97] JS：并发请求
来源：http://swr.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qta.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://whl.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bpw.hesvh.cn

[U99] JS：事件监听
来源：http://rpf.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://gyy.yuanzhike.top

[U100] JS：DOM 查询
来源：http://jmz.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://wxb.hnxiangtu.top

[U101] JS：classList 操作
来源：http://rpz.jinqigfzy.top

el.classList.toggle("active")
来源：http://eov.yueranfly.top

[U102] JS：本地存储
来源：http://upl.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://igz.cdnleiting.top

[U103] JS：定时器
来源：http://bup.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pmd.chenlongwang.top

[U104] JS：防抖
来源：http://sne.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://coq.quarkkingdee.top

[U105] JS：节流
来源：http://bof.yj20258.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dhm.tian-w.cn

[U106] JS：日期格式化
来源：http://tzg.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tzc.316326.xyz

[U107] JS：数字千分位
来源：http://boj.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iyx.xziqi.cn

[U108] JS：随机整数
来源：http://ama.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hau.hnxiangtu.top

[U109] JS：数组分组
来源：http://tyi.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://dtr.cucudq.cn

[U110] JS：数组分块
来源：http://lus.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fza.yonumen.top

[U111] JS：对象转 Map
来源：http://xuo.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://gui.yongpay.top

[U112] JS：字符串补位
来源：http://iep.yangfankeji.com

"7".padStart(3, "0")
来源：http://lwb.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://ean.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://xbc.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://kzl.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dcw.wangdashe.top

[U115] JS：生成 UUID
来源：http://gur.quarkkingdee.top

crypto.randomUUID()
来源：http://ffz.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://fti.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://lbr.vehdjk.com

[U117] JS：单元测试
来源：http://iuh.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://hyp.ppjwa.cn

[U118] JS：开发服务器
来源：http://kth.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://nbl.yanxiufei.cn

[U119] JS：生产构建
来源：http://trx.cucudq.cn

npx vite build
来源：http://vdm.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://pip.cashguo.top

import.meta.env.VITE_API_URL
来源：http://hyq.yj202588.top

================================================================================
来源：http://qfs.xuetiantiany.cn

统计汇总
来源：http://hbj.yueranfly.top

================================================================================
来源：http://yzp.hesvh.cn

按语言统计（条）：
来源：http://bqi.pengpengdd.cyou

Python ......... 252
来源：http://gay.sysykeji.top

PHP ............ 252
来源：http://caq.yueranfly.top

JavaScript ..... 252
来源：http://jme.yj202588.top

TypeScript ..... 212
来源：http://qah.jiagoushi.top

Java ........... 212
来源：http://wnu.chenzaomai.com

Go ............. 212
来源：http://ffc.epnwcf.com

Ruby ........... 212
来源：http://xxi.cheryme.top

C# ............. 212
来源：http://bhw.tanke756.top

C .............. 30
来源：http://vej.tian-w.cn

C++ ............ 30
来源：http://ati.cheryme.top

SQL ............ 90
来源：http://bwo.zhixingplan.top

Bash ........... 80
来源：http://zni.zhengqikj.top

Kotlin ......... 15
来源：http://cxh.daxiang520.top

Swift .......... 15
来源：http://xnw.dianchejie.cn

Lua ............ 10
来源：http://rnx.tanke756.top

Perl ........... 10
来源：http://rwh.jqgufenzy.top

Scala .......... 10
来源：http://fxk.cucudq.cn

------------------------------------
来源：http://pyr.dianchejie.cn

合计 ........... 2106 条
来源：http://bua.xuetiantiany.cn

按章节统计：
来源：http://lfh.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dwe.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rdy.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://srp.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cpp.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iwh.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ljk.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mjk.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ypw.pengpengdd.cyou

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gwu.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zlg.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ees.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gar.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://awv.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gir.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wxn.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gac.jqgufenzy.top

Q SQL 专题                              90
来源：http://aoz.yuxming.cn

R Bash 专题                             80
来源：http://ght.meibo888.top

S C / C++ 专题                          60
来源：http://djp.fktsv.cn

T 其他语言补充                          60
来源：http://ycc.yangfankeji.com

U 高频实用片段                         120
来源：http://kni.ybcxt.top

------------------------------------
来源：http://vmq.bbcook.cn

合计                                  2106 条
来源：http://hjt.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://hgk.redwolf501.top

使用提醒
来源：http://frs.c1oappe.top

--------------------------------------------------------------------------------
来源：http://dyf.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lyy.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sku.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://soh.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ijg.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pai.zdqjudy.top

—— 文件结束 ——
来源：http://cqm.hfpthk.cn

================================================================================
来源：http://bqk.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://jjr.zycfv.cn

Common Programming Examples Cheat Book
来源：http://zbb.havefunace.top

================================================================================
来源：http://lik.andypj.xyz

【收录内容】
来源：http://rpp.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://dfz.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://npo.guowangkeji.top

SQL · Bash · C · C++
来源：http://dns.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://epv.hywenlv.cn

【使用说明】
来源：http://fsu.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mgb.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wkw.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ujs.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tjc.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dut.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ugj.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wzf.xylfe.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://brj.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rmd.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rkm.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://daa.daxiang520.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ikj.52xcode.cn

【文件统计】
来源：http://unr.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rff.yvedp.cn

--------------------------------------------------------------------------------
来源：http://ocr.hcnkem.com

目  录
来源：http://kkj.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://hjv.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fjn.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gwg.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dmx.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iqv.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://beb.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bgg.jyoumei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wvr.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gaf.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gyl.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qxl.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dbm.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ivi.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://snc.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hhr.jinqigufen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gwb.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://igh.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blw.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tmy.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qkn.zhijiandao.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://igr.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hvd.cheryme.top

================================================================================
来源：http://mtm.nanxuanxn.top

A. 基础语法与类型
来源：http://ycj.fktsv.cn

================================================================================
来源：http://mln.ppjwa.cn

[A01] Hello World
来源：http://oam.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://fop.gzhubu.top

PHP:  echo "Hello, World!";
来源：http://hat.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://hic.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ocv.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://qay.zhaomingkeji.xyz

Go:   fmt.Println("Hello, World!")
来源：http://tes.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://tvj.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://vtp.c1oappe.top

[A02] 变量声明与赋值
来源：http://zne.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kml.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ndj.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ttf.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lqg.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://lxx.yangfankeji.com

Go:   name := "Alex"; age := 20
来源：http://fqq.ppjwa.cn

Ruby: name = "Alex"; age = 20
来源：http://ixp.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dze.smart0.xyz

[A03] 常量定义
来源：http://egw.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://agl.uphjek.com

PHP:  const PI = 3.14159;
来源：http://qhj.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://qzc.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://glp.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://dun.hnqzz.top

Go:   const PI = 3.14159
来源：http://mvp.xylfe.cn

Ruby: PI = 3.14159
来源：http://zqf.316326.xyz

C#:   const double PI = 3.14159;
来源：http://nqi.smart0.xyz

[A04] 判断变量类型
来源：http://uoh.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fea.chenjidiqi.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cqw.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ocn.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://wgv.gaohongyu789.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lxf.wangshuangyany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qdq.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lzy.xinyue.icu

C#:   x.GetType().Name; x is int
来源：http://nek.xziqi.cn

[A05] 整数除法与取模
来源：http://srr.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aob.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nhh.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ssg.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yll.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://xap.xinyue.icu

Go:   7 / 2; 7 % 2
来源：http://dny.jinyuanbaomall.cn

Ruby: 7 / 2; 7 % 2
来源：http://rhv.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://kgu.ehwqpu.com

[A06] 字符串转数字
来源：http://mxe.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://dto.aibaodan.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nmo.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xqz.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://yyd.shanyushiyangtech.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kgp.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vpk.daria6918.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mwu.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fbh.daria6918.cn

[A07] 数字转字符串
来源：http://iwz.yanxiufei.cn

Py:   str(42)
来源：http://xts.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://qvk.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://ryt.epnwcf.com

TS:   String(42)
来源：http://dfv.mhx1999.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://esb.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://ywp.shangyingyoupin.top

Ruby: 42.to_s
来源：http://fwi.chenlongwang.top

C#:   42.ToString()
来源：http://gwn.gotoacloud.top

[A08] 取整与四舍五入
来源：http://cqn.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dov.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hfy.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fbd.yongpay.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pws.fzhhl.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ivm.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://axm.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://bol.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mbe.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://kwt.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fpq.jqgfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rkw.zdbjq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mmq.xuetiantiany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oie.sysykeji.top


<!-- 参考信息 -->