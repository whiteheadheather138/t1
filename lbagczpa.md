代发 wailian999

[U61] PHP：正则
来源：http://iql.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sbp.yj20258888.top

[U62] PHP：日期对象
来源：http://gbn.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fca.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://grp.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nmy.xinyue.icu

[U64] PHP：目录遍历
来源：http://hky.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://vyb.sysykeji.top

[U65] PHP：会话
来源：http://niu.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://woz.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://gwk.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gcy.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://siq.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://efz.yfazqb.com

[U68] PHP：PDO 连接
来源：http://ixz.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hua.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://mju.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gse.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://xwf.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gif.yuxming.cn

[U71] PHP：抛出异常
来源：http://ocp.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://ojo.bbcook.cn

[U72] PHP：写错误日志
来源：http://oid.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://tnv.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://gkk.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://plp.andypj.xyz

[U74] PHP：读取环境变量
来源：http://pwn.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://ayv.mhx1999.top

[U75] PHP：依赖注入
来源：http://oix.tarul.cn

composer require psr/container
来源：http://wbp.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://euk.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zfm.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://ull.dashuyun.cn

composer require twig/twig
来源：http://soq.yuanzhike.top

[U78] PHP：单元测试
来源：http://fpl.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://brk.zhoulong.xyz

[U79] PHP：静态分析
来源：http://qvt.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://qrl.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://iih.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bzm.yj202588.top

[U81] JS：初始化项目
来源：http://lmc.tarul.cn

npm init -y;  npm i express
来源：http://moy.ybcxt.top

[U82] JS：package.json 脚本
来源：http://dvj.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qcd.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://wmt.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://zpj.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://htg.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jfs.dashuyun.cn

[U85] JS：可选链
来源：http://vxz.zdbjq.cn

a?.b?.c
来源：http://adt.jqgufenzy.top

[U86] JS：空值合并
来源：http://dmu.gotoacloud.top

a ?? b
来源：http://vtw.aizwys.cn

[U87] JS：解构默认值
来源：http://hmu.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://qss.cucudq.cn

[U88] JS：对象展开合并
来源：http://dyn.yj20258888.top

{ ...a, ...b }
来源：http://smv.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://fjf.andypj.xyz

[...new Set(arr)]
来源：http://kpo.c1oappe.top

[U90] JS：数字数组排序
来源：http://ogp.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://xag.pycfn.com

[U91] JS：对象键值遍历
来源：http://kbb.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dek.ybcxt.top

[U92] JS：深拷贝
来源：http://wdp.jinyuanbaomall.cn

structuredClone(obj)
来源：http://hsa.ydjk.org.cn

[U93] JS：模板字符串
来源：http://xkd.pengpengdd.cyou

`共 ${n} 条`
来源：http://qdn.sweek.top

[U94] JS：箭头函数
来源：http://uyy.ppjwa.cn

const double = x => x * 2;
来源：http://mmw.316326.xyz

[U95] JS：Promise 包装
来源：http://gkg.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://ojy.gzhubu.top

[U96] JS：async/await 与异常
来源：http://rod.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://upy.pycfn.com

[U97] JS：并发请求
来源：http://vkt.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wst.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://lqm.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tfj.9152youxi.cn

[U99] JS：事件监听
来源：http://vtw.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://xnj.jianghu66.top

[U100] JS：DOM 查询
来源：http://jwl.fanxiaobao.xyz

document.querySelector(".item")
来源：http://lns.cucudq.cn

[U101] JS：classList 操作
来源：http://gtk.birdmap.top

el.classList.toggle("active")
来源：http://dbn.xziqi.cn

[U102] JS：本地存储
来源：http://nzg.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://aig.bjfxy.top

[U103] JS：定时器
来源：http://uob.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ttf.fzhhl.top

[U104] JS：防抖
来源：http://eox.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uwu.wangshuangyany.cn

[U105] JS：节流
来源：http://axq.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://afv.epnwcf.com

[U106] JS：日期格式化
来源：http://jyo.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ugo.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://vgt.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bni.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://utr.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tlp.daria6918.cn

[U109] JS：数组分组
来源：http://lpx.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://rrx.zhixingplan.top

[U110] JS：数组分块
来源：http://qon.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cjz.aizwys.cn

[U111] JS：对象转 Map
来源：http://aaz.yueranfly.top

new Map(Object.entries(obj))
来源：http://mti.jianghu66.top

[U112] JS：字符串补位
来源：http://agk.hysaishi.cn

"7".padStart(3, "0")
来源：http://bnd.shuidangran.top

[U113] JS：正则替换全部
来源：http://hcq.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://phm.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://tnm.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://ron.fehbvm.com

[U115] JS：生成 UUID
来源：http://wvj.xziqi.cn

crypto.randomUUID()
来源：http://qdy.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://kta.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://dgn.jinqigfzy.top

[U117] JS：单元测试
来源：http://iuo.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://tzy.jinqigufen.top

[U118] JS：开发服务器
来源：http://awp.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://lfc.0kj1m.cn

[U119] JS：生产构建
来源：http://edf.daria6918.cn

npx vite build
来源：http://xja.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://rjq.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://fjr.xinyue.icu

================================================================================
来源：http://dtp.ywan-chungtsiang.top

统计汇总
来源：http://cti.wangshuangyany.cn

================================================================================
来源：http://ggx.shanyushiyangkeji.top

按语言统计（条）：
来源：http://wcx.guowangkeji.top

Python ......... 252
来源：http://yxj.xinyue.icu

PHP ............ 252
来源：http://vxu.meibo888.top

JavaScript ..... 252
来源：http://xlr.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://tut.jinqigfzy.top

Java ........... 212
来源：http://arb.zhengqikj.top

Go ............. 212
来源：http://kyd.jyoumei.cn

Ruby ........... 212
来源：http://blu.guowangkeji.top

C# ............. 212
来源：http://gnt.jqgufenzy.top

C .............. 30
来源：http://sji.jlsjyb.cn

C++ ............ 30
来源：http://rop.guannengcc.top

SQL ............ 90
来源：http://wzk.jyoumei.cn

Bash ........... 80
来源：http://jiq.ctjpmb.com

Kotlin ......... 15
来源：http://njh.zdqjudy.top

Swift .......... 15
来源：http://qca.yj20258.top

Lua ............ 10
来源：http://ozf.svipenyu.cn

Perl ........... 10
来源：http://vfd.jiagoushi.top

Scala .......... 10
来源：http://edq.xziqi.cn

------------------------------------
来源：http://iap.nanxuanxn.top

合计 ........... 2106 条
来源：http://drl.feifeiyinyue.top

按章节统计：
来源：http://vbr.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://crf.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yhy.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://duo.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ckb.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wlo.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vcu.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gaj.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nwt.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jkc.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xra.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ucp.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cly.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bid.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ftb.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wnv.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jlg.316326.xyz

Q SQL 专题                              90
来源：http://kbu.pycfn.com

R Bash 专题                             80
来源：http://tlp.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://gho.xziqi.cn

T 其他语言补充                          60
来源：http://sih.hysaishi.cn

U 高频实用片段                         120
来源：http://tlf.hesvh.cn

------------------------------------
来源：http://mwc.tian-w.cn

合计                                  2106 条
来源：http://cpx.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://quz.sweek.top

使用提醒
来源：http://xub.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://itw.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nxj.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xbn.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jse.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://olp.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rey.meibo888.top

—— 文件结束 ——
来源：http://fwt.hcnkem.com

================================================================================
来源：http://fby.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://wui.zhixingplan.top

Common Programming Examples Cheat Book
来源：http://sht.shanyushiyangkeji.top

================================================================================
来源：http://seb.yj20258.top

【收录内容】
来源：http://wxs.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hzi.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fvm.daxiang520.top

SQL · Bash · C · C++
来源：http://fdv.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yna.meibo888.top

【使用说明】
来源：http://xtw.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yne.xingfuxueyuan.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oec.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hum.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yge.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rev.snrcjt.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sei.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qpm.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://axc.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yzm.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uqg.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pkt.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nhu.andypj.xyz

【文件统计】
来源：http://bds.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hxp.aizwys.cn

--------------------------------------------------------------------------------
来源：http://dzh.yj202588.top

目  录
来源：http://gcb.fengsongda.top

--------------------------------------------------------------------------------
来源：http://mgk.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yyw.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wbg.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rof.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ptk.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nmc.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eeo.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://riy.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xta.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://paw.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://djo.daria6918.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ntk.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jdw.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ydo.iojbl.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nwd.zhengqikj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aog.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qhb.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gik.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://odr.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zlg.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hcp.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ehe.cqqwz.cn

================================================================================
来源：http://xbk.yongpay.top

A. 基础语法与类型
来源：http://cft.xuanzx.com

================================================================================
来源：http://xyb.9152youxi.cn

[A01] Hello World
来源：http://okk.zdqjudy.top

Py:   print("Hello, World!")
来源：http://hay.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://sus.kuanghao11.cn

JS:   console.log("Hello, World!");
来源：http://cki.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kur.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://zre.dashuyun.cn

Go:   fmt.Println("Hello, World!")
来源：http://ige.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://deo.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xtg.yj202588.top

[A02] 变量声明与赋值
来源：http://gqg.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fgh.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cxr.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://vho.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sil.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://elp.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://tvy.wangshuangyany.cn

Ruby: name = "Alex"; age = 20
来源：http://teo.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eyz.quarkkingdee.top

[A03] 常量定义
来源：http://csn.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vvc.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://gsr.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://hgp.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://ykp.havefunace.top

Java: static final double PI = 3.14159;
来源：http://myz.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://ely.fzhhl.top

Ruby: PI = 3.14159
来源：http://mnb.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://uhc.bbcook.cn

[A04] 判断变量类型
来源：http://ygd.yj202588.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jsc.birdmap.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rek.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tog.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://dsw.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qdj.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://mzh.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://emz.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://mkg.tianlin.xyz

[A05] 整数除法与取模
来源：http://adk.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yka.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zcz.hcnkem.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mjp.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qix.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://dde.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://phn.shanyushiyangtech.top

Ruby: 7 / 2; 7 % 2
来源：http://dfm.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://ewl.haohaochexian.top

[A06] 字符串转数字
来源：http://vcz.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://upm.jinqigufen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pbd.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fnl.jinyuanbaomall.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ruy.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dof.xingfuxueyuan.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://olx.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ggo.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ltc.zhoulong.xyz

[A07] 数字转字符串
来源：http://mch.fehbvm.com

Py:   str(42)
来源：http://ino.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://lyn.feifeiyinyue.top

JS:   String(42); (42).toString()
来源：http://oke.guannengcc.top

TS:   String(42)
来源：http://wte.sweek.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fbp.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://tzq.c1oappe.top

Ruby: 42.to_s
来源：http://siq.sysykeji.top

C#:   42.ToString()
来源：http://qcq.bjfxy.top

[A08] 取整与四舍五入
来源：http://qlm.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pti.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gsy.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zse.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cgo.jinqigufen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ezt.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ylt.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bak.yangfankeji.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://itv.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://mwv.ctjpmb.com


<!-- 参考信息 -->