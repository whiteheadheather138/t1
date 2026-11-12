代发 wailian999

[U55] PHP：match 表达式
来源：http://faw.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fso.sysykeji.top

[U56] PHP：命名参数
来源：http://ttx.hesvh.cn

f(a: 1, b: 2)
来源：http://lgs.snrcjt.cn

[U57] PHP：字符串插值
来源：http://qmn.daria6918.cn

"值: {$a}"
来源：http://osl.zdbjq.cn

[U58] PHP：数组三件套
来源：http://xep.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lbw.birdmap.top

[U59] PHP：自定义排序
来源：http://sbe.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cdx.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://uke.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jas.shuidangran.top

[U61] PHP：正则
来源：http://fwr.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://egc.hnqzz.top

[U62] PHP：日期对象
来源：http://eil.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hev.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://knq.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yxc.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://nou.dianchejie.cn

glob("dir/*.php");  scandir("dir");
来源：http://gst.pycfn.com

[U65] PHP：会话
来源：http://kea.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://suu.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://oyo.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://auf.meibo888.top

[U67] PHP：处理文件上传
来源：http://ubx.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eac.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://ngd.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bvq.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://ypq.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wjt.iojbl.cn

[U70] PHP：PDO 事务
来源：http://suq.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eqz.snrcjt.cn

[U71] PHP：抛出异常
来源：http://igb.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://ybu.epnwcf.com

[U72] PHP：写错误日志
来源：http://wlc.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://wmg.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://dxb.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://qck.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://gcq.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://jaa.jiagoushi.top

[U75] PHP：依赖注入
来源：http://xlz.dianchejie.cn

composer require psr/container
来源：http://mjj.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://ekr.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fcx.hnqzz.top

[U77] PHP：模板渲染
来源：http://zjv.sweek.top

composer require twig/twig
来源：http://smd.tanke756.top

[U78] PHP：单元测试
来源：http://aqs.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://iwi.daxiang520.top

[U79] PHP：静态分析
来源：http://nps.cheryme.top

composer require --dev phpstan/phpstan
来源：http://jat.daria6918.cn

[U80] PHP：代码规范修复
来源：http://ekg.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ovh.ivvv.top

[U81] JS：初始化项目
来源：http://toa.jqgufenzy.top

npm init -y;  npm i express
来源：http://kaq.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://ort.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xny.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://rze.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cnv.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://ijo.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jpo.chenzaomai.com

[U85] JS：可选链
来源：http://kua.iojbl.cn

a?.b?.c
来源：http://hfk.xuanzx.com

[U86] JS：空值合并
来源：http://prv.nanxinkj.top

a ?? b
来源：http://oyx.hcnkem.com

[U87] JS：解构默认值
来源：http://moa.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://ekn.haohaochexian.top

[U88] JS：对象展开合并
来源：http://eis.yanxiufei.cn

{ ...a, ...b }
来源：http://trk.9152youxi.cn

[U89] JS：数组去重
来源：http://inr.birdmap.top

[...new Set(arr)]
来源：http://xgg.hfpthk.cn

[U90] JS：数字数组排序
来源：http://myq.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://why.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://ppx.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jwv.zdbjq.cn

[U92] JS：深拷贝
来源：http://qjb.jinqigfzy.top

structuredClone(obj)
来源：http://npb.zhengqikj.top

[U93] JS：模板字符串
来源：http://rpx.svipenyu.cn

`共 ${n} 条`
来源：http://aqi.mhx1999.top

[U94] JS：箭头函数
来源：http://fpw.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://xzs.svipenyu.cn

[U95] JS：Promise 包装
来源：http://uuw.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://uzz.bbcook.cn

[U96] JS：async/await 与异常
来源：http://scj.zhoulong.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qsa.yj20258.top

[U97] JS：并发请求
来源：http://rpz.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rhj.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://qfd.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hmv.fktsv.cn

[U99] JS：事件监听
来源：http://rmy.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://fiq.sysykeji.top

[U100] JS：DOM 查询
来源：http://kbb.zhongyouzk.top

document.querySelector(".item")
来源：http://huq.bjfxy.top

[U101] JS：classList 操作
来源：http://fco.fzhhl.top

el.classList.toggle("active")
来源：http://ikh.pengpengdd.cyou

[U102] JS：本地存储
来源：http://wqt.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ckq.cheryme.top

[U103] JS：定时器
来源：http://hsf.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pci.nanxinkj.top

[U104] JS：防抖
来源：http://mqs.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tsq.zdqjudy.top

[U105] JS：节流
来源：http://btc.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lko.hnqzz.top

[U106] JS：日期格式化
来源：http://liz.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://frm.cheryme.top

[U107] JS：数字千分位
来源：http://jkf.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wfl.redwolf501.top

[U108] JS：随机整数
来源：http://rys.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lpp.redwolf501.top

[U109] JS：数组分组
来源：http://ikm.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://puy.zhongyouzk.top

[U110] JS：数组分块
来源：http://kxh.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nfi.cqqwz.cn

[U111] JS：对象转 Map
来源：http://ogv.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://xfu.cucudq.cn

[U112] JS：字符串补位
来源：http://nhm.pycfn.com

"7".padStart(3, "0")
来源：http://sda.tian-w.cn

[U113] JS：正则替换全部
来源：http://rgy.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://xnh.fehbvm.com

[U114] JS：JSON 深比较
来源：http://izw.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://esc.hfpthk.cn

[U115] JS：生成 UUID
来源：http://stc.daxiang520.top

crypto.randomUUID()
来源：http://abi.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://iww.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://hen.hysaishi.cn

[U117] JS：单元测试
来源：http://lbb.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://eif.cqqwz.cn

[U118] JS：开发服务器
来源：http://afs.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://xed.yongpay.top

[U119] JS：生产构建
来源：http://lax.sufxvd.cn

npx vite build
来源：http://slt.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://vdl.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://kbx.nanxinkj.top

================================================================================
来源：http://rka.dianchejie.cn

统计汇总
来源：http://jzr.feifeiyinyue.top

================================================================================
来源：http://uab.mhx1999.top

按语言统计（条）：
来源：http://cyh.hcnkem.com

Python ......... 252
来源：http://agn.kuanghao11.cn

PHP ............ 252
来源：http://hqh.c1oappe.top

JavaScript ..... 252
来源：http://qrx.yj20258.top

TypeScript ..... 212
来源：http://gza.xziqi.cn

Java ........... 212
来源：http://nds.nwbrower.top

Go ............. 212
来源：http://iib.havefunace.top

Ruby ........... 212
来源：http://wst.yanxiufei.cn

C# ............. 212
来源：http://scj.cqqwz.cn

C .............. 30
来源：http://skq.pycfn.com

C++ ............ 30
来源：http://tfy.yj20258888.top

SQL ............ 90
来源：http://vgu.jiagoushi.top

Bash ........... 80
来源：http://cxy.uphjek.com

Kotlin ......... 15
来源：http://vuo.fanxiaobao.xyz

Swift .......... 15
来源：http://gzy.zdqjudy.top

Lua ............ 10
来源：http://noq.havefunace.top

Perl ........... 10
来源：http://krp.bbcook.cn

Scala .......... 10
来源：http://zwl.tian-w.cn

------------------------------------
来源：http://xrp.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://abk.xylfe.cn

按章节统计：
来源：http://ltj.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xqr.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ytc.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zmt.ydjk.org.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dsg.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yql.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pnu.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yhx.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kdd.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kfu.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pbr.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yap.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gau.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pio.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vqw.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gtg.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vnx.hongshengwenyu.top

Q SQL 专题                              90
来源：http://fsu.zdbjq.cn

R Bash 专题                             80
来源：http://dqh.yuanzhike.top

S C / C++ 专题                          60
来源：http://jnj.guowangkeji.top

T 其他语言补充                          60
来源：http://acx.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://beu.aizwys.cn

------------------------------------
来源：http://ldh.sufxvd.cn

合计                                  2106 条
来源：http://eho.nwbrower.top

--------------------------------------------------------------------------------
来源：http://cjo.yj202588.top

使用提醒
来源：http://ggb.daxiang520.top

--------------------------------------------------------------------------------
来源：http://jai.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eso.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dtc.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fng.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mtu.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pdw.shangyingyoupin.top

—— 文件结束 ——
来源：http://edy.chenzaomai.com

================================================================================
来源：http://yrd.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://fpt.xziqi.cn

Common Programming Examples Cheat Book
来源：http://glv.c1oappe.top

================================================================================
来源：http://vvz.shangyingyoupin.top

【收录内容】
来源：http://tyv.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bak.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pyp.tianlin.xyz

SQL · Bash · C · C++
来源：http://nqj.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://asx.epnwcf.com

【使用说明】
来源：http://ocd.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iek.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ihz.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kfl.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ktc.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nei.sweek.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yjv.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oou.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dzf.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cue.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lyf.wangdashe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ogi.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zrt.ybcxt.top

【文件统计】
来源：http://ipy.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://usk.wangdashe.top

--------------------------------------------------------------------------------
来源：http://kpp.yanxiufei.cn

目  录
来源：http://lvo.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://poy.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ekq.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dta.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gic.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gcs.xingfuxueyuan.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yog.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vfm.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wty.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ctm.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://njj.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wso.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nfn.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ihw.jinqigufen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pvm.ybcxt.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ddo.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sum.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yjd.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fgs.shangyingyoupin.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bkz.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bqz.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xkx.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qse.aizwys.cn

================================================================================
来源：http://fuh.tian-w.cn

A. 基础语法与类型
来源：http://uti.9152youxi.cn

================================================================================
来源：http://rxl.hcnkem.com

[A01] Hello World
来源：http://juj.xuanzx.com

Py:   print("Hello, World!")
来源：http://chw.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://eom.zdbjq.cn

JS:   console.log("Hello, World!");
来源：http://vbh.ppjwa.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bol.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://eyj.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://zsx.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://fmd.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rcu.9152youxi.cn

[A02] 变量声明与赋值
来源：http://xga.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://deb.guannengcc.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pkp.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qab.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fyj.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://uaf.yvedp.cn

Go:   name := "Alex"; age := 20
来源：http://tij.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://cbm.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jdk.hywenlv.cn

[A03] 常量定义
来源：http://lvr.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://opz.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://mrl.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://tcx.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://gub.sweek.top

Java: static final double PI = 3.14159;
来源：http://hyw.yangfankeji.com

Go:   const PI = 3.14159
来源：http://roj.shzxlz.cn

Ruby: PI = 3.14159
来源：http://uyf.cashguo.top

C#:   const double PI = 3.14159;
来源：http://jvt.chenzaomai.com

[A04] 判断变量类型
来源：http://evi.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zmq.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://snm.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://htc.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://doi.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hcd.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://fav.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uen.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://fqk.jyoumei.cn

[A05] 整数除法与取模
来源：http://fom.shanyushiyangtech.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bwq.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ufm.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tiy.zhoulong.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lgb.wangshuangyany.cn

Java: 7 / 2; 7 % 2
来源：http://kyt.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://muv.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://ona.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://idw.shzxlz.cn

[A06] 字符串转数字
来源：http://qfj.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://dqg.zhengqikj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jmh.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ltt.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://lta.zdqjudy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fpv.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rpv.sysykeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ixd.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hmy.tian-w.cn

[A07] 数字转字符串
来源：http://ves.vqdsnc.cn

Py:   str(42)
来源：http://ayx.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://kva.shanyushiyangkeji.top

JS:   String(42); (42).toString()
来源：http://mgi.fktsv.cn

TS:   String(42)
来源：http://yzw.ivvv.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oma.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://qbh.hfpthk.cn


<!-- 参考信息 -->