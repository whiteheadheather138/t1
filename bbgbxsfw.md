代发 wailian999

[U61] PHP：正则
来源：http://vjq.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://doj.yangfankeji.com

[U62] PHP：日期对象
来源：http://mqz.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rvy.sysykeji.top

[U63] PHP：文件读写
来源：http://xef.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dap.fktsv.cn

[U64] PHP：目录遍历
来源：http://cbg.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://ngp.smart0.xyz

[U65] PHP：会话
来源：http://mzj.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nwb.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://nud.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tyw.meibo888.top

[U67] PHP：处理文件上传
来源：http://qlg.hnqzz.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vlc.cucudq.cn

[U68] PHP：PDO 连接
来源：http://qhn.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://emd.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://xwk.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ypb.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://yey.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uig.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://lgf.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://iir.iojbl.cn

[U72] PHP：写错误日志
来源：http://pjg.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://cvq.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://oka.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://txj.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://etl.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://hhe.epnwcf.com

[U75] PHP：依赖注入
来源：http://liy.gogol.net.cn

composer require psr/container
来源：http://etz.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://nxv.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zxo.ctjpmb.com

[U77] PHP：模板渲染
来源：http://rot.jinqigfzy.top

composer require twig/twig
来源：http://zpi.fktsv.cn

[U78] PHP：单元测试
来源：http://gww.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://lfd.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://mvm.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://epp.ydzc1.top

[U80] PHP：代码规范修复
来源：http://igm.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cyn.cqqwz.cn

[U81] JS：初始化项目
来源：http://jvx.snrcjt.cn

npm init -y;  npm i express
来源：http://zjx.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://ntp.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gkp.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://krm.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pyv.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://avt.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://pax.havefunace.top

[U85] JS：可选链
来源：http://lpj.9152youxi.cn

a?.b?.c
来源：http://txt.vqdsnc.cn

[U86] JS：空值合并
来源：http://vsu.haohaochexian.top

a ?? b
来源：http://kki.andypj.xyz

[U87] JS：解构默认值
来源：http://bjk.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://fnw.dianchejie.cn

[U88] JS：对象展开合并
来源：http://qee.dianchejie.cn

{ ...a, ...b }
来源：http://edo.yj20258.top

[U89] JS：数组去重
来源：http://oag.fehbvm.com

[...new Set(arr)]
来源：http://xvj.ydzc1.top

[U90] JS：数字数组排序
来源：http://kwd.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://yif.wangdashe.top

[U91] JS：对象键值遍历
来源：http://rdj.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yrv.haohaochexian.top

[U92] JS：深拷贝
来源：http://dma.dianchejie.cn

structuredClone(obj)
来源：http://jbp.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://lxd.mhx1999.top

`共 ${n} 条`
来源：http://ktg.tian-w.cn

[U94] JS：箭头函数
来源：http://dgm.gotoacloud.top

const double = x => x * 2;
来源：http://kcp.zhaomingkeji.xyz

[U95] JS：Promise 包装
来源：http://ltb.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://xhh.zycfv.cn

[U96] JS：async/await 与异常
来源：http://wtb.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yzb.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://etr.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fbd.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://fql.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lxo.uphjek.com

[U99] JS：事件监听
来源：http://zzi.bjfxy.top

el.addEventListener("click", e => {})
来源：http://lha.chenlongwang.top

[U100] JS：DOM 查询
来源：http://agj.quarkkingdee.top

document.querySelector(".item")
来源：http://orm.xuanzx.com

[U101] JS：classList 操作
来源：http://phu.fengsongda.top

el.classList.toggle("active")
来源：http://sba.bjfxy.top

[U102] JS：本地存储
来源：http://yxw.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rhz.gzhubu.top

[U103] JS：定时器
来源：http://thc.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kcj.meibo888.top

[U104] JS：防抖
来源：http://wjf.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mtw.epnwcf.com

[U105] JS：节流
来源：http://qgq.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nqg.aizwys.cn

[U106] JS：日期格式化
来源：http://wyt.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qde.316326.xyz

[U107] JS：数字千分位
来源：http://xbl.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nsc.andypj.xyz

[U108] JS：随机整数
来源：http://kja.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pmb.yj202588.top

[U109] JS：数组分组
来源：http://jif.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://mec.hysaishi.cn

[U110] JS：数组分块
来源：http://tbo.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kue.hesvh.cn

[U111] JS：对象转 Map
来源：http://azf.zhixingplan.top

new Map(Object.entries(obj))
来源：http://gso.iojbl.cn

[U112] JS：字符串补位
来源：http://itd.zhoulong.xyz

"7".padStart(3, "0")
来源：http://igz.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://fue.bbcook.cn

s.replaceAll("a", "b")
来源：http://laz.jianghu66.top

[U114] JS：JSON 深比较
来源：http://cjk.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jtz.cheryme.top

[U115] JS：生成 UUID
来源：http://lcz.hcnkem.com

crypto.randomUUID()
来源：http://pmf.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://zmm.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://gkq.kuanghao11.cn

[U117] JS：单元测试
来源：http://enu.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://eci.ydjk.org.cn

[U118] JS：开发服务器
来源：http://bia.cqqwz.cn

npm i -D vite;  npx vite
来源：http://qrh.dianchejie.cn

[U119] JS：生产构建
来源：http://axj.fzhhl.top

npx vite build
来源：http://ble.hongshengwenyu.top

[U120] JS：读取环境变量（Vite）
来源：http://jtm.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://ngm.tianlin.xyz

================================================================================
来源：http://lcb.shanyushiyangtech.top

统计汇总
来源：http://kmv.nwbrower.top

================================================================================
来源：http://fld.jinghuilouyu.cn

按语言统计（条）：
来源：http://klu.yuanzhike.top

Python ......... 252
来源：http://yyu.xziqi.cn

PHP ............ 252
来源：http://dht.cashguo.top

JavaScript ..... 252
来源：http://mup.zhiwuduotai.top

TypeScript ..... 212
来源：http://cly.jianghu66.top

Java ........... 212
来源：http://xas.jiagoushi.top

Go ............. 212
来源：http://fqn.zhengqikj.top

Ruby ........... 212
来源：http://kuy.epnwcf.com

C# ............. 212
来源：http://xpa.guannengcc.top

C .............. 30
来源：http://vpx.hnqzz.top

C++ ............ 30
来源：http://cti.zhengqikj.top

SQL ............ 90
来源：http://svc.hysaishi.cn

Bash ........... 80
来源：http://umt.ppjwa.cn

Kotlin ......... 15
来源：http://yab.jinqigfzy.top

Swift .......... 15
来源：http://jvz.ppjwa.cn

Lua ............ 10
来源：http://sdx.epnwcf.com

Perl ........... 10
来源：http://uxg.svipenyu.cn

Scala .......... 10
来源：http://kpv.cheryme.top

------------------------------------
来源：http://czn.daxiang520.top

合计 ........... 2106 条
来源：http://fjg.epnwcf.com

按章节统计：
来源：http://mif.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fui.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wft.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uqw.jlsjyb.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wih.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cgw.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mzp.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://toz.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zax.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oas.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mza.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://moy.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ces.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hlv.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://num.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ddn.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lcx.ydzc1.top

Q SQL 专题                              90
来源：http://oam.yj202588.top

R Bash 专题                             80
来源：http://kxv.hcnkem.com

S C / C++ 专题                          60
来源：http://kro.sjlbkw.cn

T 其他语言补充                          60
来源：http://ulu.andypj.xyz

U 高频实用片段                         120
来源：http://ksv.sysykeji.top

------------------------------------
来源：http://ckb.gogol.net.cn

合计                                  2106 条
来源：http://jnn.zycfv.cn

--------------------------------------------------------------------------------
来源：http://nfj.ivvv.top

使用提醒
来源：http://nzg.fengsongda.top

--------------------------------------------------------------------------------
来源：http://cno.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hjz.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://arc.zycfv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jno.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mrt.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ovn.hcnkem.com

—— 文件结束 ——
来源：http://uxc.hammf.cn

================================================================================
来源：http://yfd.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://toy.xinyue.icu

Common Programming Examples Cheat Book
来源：http://wdi.haohaochexian.top

================================================================================
来源：http://dya.0kj1m.cn

【收录内容】
来源：http://qji.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sry.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qty.cheryme.top

SQL · Bash · C · C++
来源：http://asf.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wcb.daria6918.cn

【使用说明】
来源：http://esb.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cbj.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fsl.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lwq.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jzw.hfpthk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dpy.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kkw.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gll.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jfm.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xqj.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qgf.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uaw.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ozh.uphjek.com

【文件统计】
来源：http://gsh.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ktf.yueranfly.top

--------------------------------------------------------------------------------
来源：http://lrv.ppjwa.cn

目  录
来源：http://kjc.xylfe.cn

--------------------------------------------------------------------------------
来源：http://pzl.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gye.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hcj.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lxb.ydzc1.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dnm.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fph.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bcb.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wsb.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nfa.dashuyun.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ujw.sjlbkw.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lqu.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vgb.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://goq.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mwj.haohaochexian.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://arq.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xgi.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wmq.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wto.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://iro.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wgd.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://was.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vcg.yj20258.top

================================================================================
来源：http://tjm.zdqjudy.top

A. 基础语法与类型
来源：http://tky.yuanzhike.top

================================================================================
来源：http://tid.redwolf501.top

[A01] Hello World
来源：http://kgr.birdmap.top

Py:   print("Hello, World!")
来源：http://ftp.yfazqb.com

PHP:  echo "Hello, World!";
来源：http://elp.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://ecy.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gxi.tianlin.xyz

Java: System.out.println("Hello, World!");
来源：http://wht.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://mgh.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://yyp.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nwd.yj20258.top

[A02] 变量声明与赋值
来源：http://vmw.bjfxy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ikc.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uto.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://dcz.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cep.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://izc.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://ymn.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://vhq.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://hte.cheryme.top

[A03] 常量定义
来源：http://bnc.shanyushiyangtech.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qgo.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://eob.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://fya.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://kmk.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://aaa.hcnkem.com

Go:   const PI = 3.14159
来源：http://aol.yj202588.top

Ruby: PI = 3.14159
来源：http://kub.snrcjt.cn

C#:   const double PI = 3.14159;
来源：http://afw.xziqi.cn

[A04] 判断变量类型
来源：http://ush.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mkx.cdnleiting.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://okp.hywenlv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mot.sjlbkw.cn

TS:   typeof x; x instanceof Date
来源：http://ggq.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rsg.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://owh.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tzs.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://dfk.yuxming.cn

[A05] 整数除法与取模
来源：http://arh.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://drs.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hmg.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ptf.jqgfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lqs.316326.xyz

Java: 7 / 2; 7 % 2
来源：http://mwx.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://xkz.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://dsp.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://iiy.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://vig.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://ywt.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zyr.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tcw.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rfp.0kj1m.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nso.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vlu.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ysl.smart0.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ibb.gzhubu.top

[A07] 数字转字符串
来源：http://ttv.meibo888.top

Py:   str(42)
来源：http://unc.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://you.yuxming.cn

JS:   String(42); (42).toString()
来源：http://hag.zhaomingkeji.xyz

TS:   String(42)
来源：http://yqg.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yyx.epnwcf.com

Go:   strconv.Itoa(42)
来源：http://jwb.ctjpmb.com

Ruby: 42.to_s
来源：http://kbl.feifeiyinyue.top

C#:   42.ToString()
来源：http://svf.hnqzz.top

[A08] 取整与四舍五入
来源：http://mph.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qlr.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cfd.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wkw.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tal.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ulx.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://euc.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://isa.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mvw.316326.xyz

[A09] 绝对值与最大最小值
来源：http://okm.yuxming.cn


<!-- 参考信息 -->