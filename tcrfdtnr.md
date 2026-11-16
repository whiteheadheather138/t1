代发 wailian999

[U55] PHP：match 表达式
来源：http://hio.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kkq.ehwqpu.com

[U56] PHP：命名参数
来源：http://xnq.xziqi.cn

f(a: 1, b: 2)
来源：http://byn.hnqzz.top

[U57] PHP：字符串插值
来源：http://jmp.tianlin.xyz

"值: {$a}"
来源：http://hqb.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://ipv.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qnl.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://xdd.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cok.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://rnr.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gnb.kuanghao11.cn

[U61] PHP：正则
来源：http://tej.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wsj.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://fly.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pnd.ppjwa.cn

[U63] PHP：文件读写
来源：http://afw.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cho.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://gyj.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://vji.sweek.top

[U65] PHP：会话
来源：http://kmp.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zaf.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://qgo.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zrd.zhoulong.xyz

[U67] PHP：处理文件上传
来源：http://aul.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tgr.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://mfb.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ovw.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://avt.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gbf.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://nrn.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://abg.tian-w.cn

[U71] PHP：抛出异常
来源：http://yqc.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://qni.yongpay.top

[U72] PHP：写错误日志
来源：http://nkb.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://efe.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://niq.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://tye.uphjek.com

[U74] PHP：读取环境变量
来源：http://aam.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://xdz.cqqwz.cn

[U75] PHP：依赖注入
来源：http://jew.sweek.top

composer require psr/container
来源：http://fqq.ybcxt.top

[U76] PHP：简单路由
来源：http://rux.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qsk.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://kqk.svipenyu.cn

composer require twig/twig
来源：http://hox.zhixingplan.top

[U78] PHP：单元测试
来源：http://pvr.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://sid.vehdjk.com

[U79] PHP：静态分析
来源：http://bkf.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://kox.sxryk.cn

[U80] PHP：代码规范修复
来源：http://buy.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://vve.xziqi.cn

[U81] JS：初始化项目
来源：http://lrw.hammf.cn

npm init -y;  npm i express
来源：http://zdf.52xcode.cn

[U82] JS：package.json 脚本
来源：http://rtf.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pse.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://fom.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ycx.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://gml.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://rns.jqgufenzy.top

[U85] JS：可选链
来源：http://twv.jiagoushi.top

a?.b?.c
来源：http://wzl.chenzaomai.com

[U86] JS：空值合并
来源：http://fye.cqqwz.cn

a ?? b
来源：http://bbg.sysykeji.top

[U87] JS：解构默认值
来源：http://tdy.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://boy.52xcode.cn

[U88] JS：对象展开合并
来源：http://sli.vehdjk.com

{ ...a, ...b }
来源：http://kfw.jinqigufen.top

[U89] JS：数组去重
来源：http://yai.daxiang520.top

[...new Set(arr)]
来源：http://dgy.0kj1m.cn

[U90] JS：数字数组排序
来源：http://mfq.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://fqt.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://zmq.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zjb.jyoumei.cn

[U92] JS：深拷贝
来源：http://nfj.9152youxi.cn

structuredClone(obj)
来源：http://dmz.sweek.top

[U93] JS：模板字符串
来源：http://vrh.yj20258.top

`共 ${n} 条`
来源：http://kmf.ivvv.top

[U94] JS：箭头函数
来源：http://byo.birdmap.top

const double = x => x * 2;
来源：http://cww.cqqwz.cn

[U95] JS：Promise 包装
来源：http://hkk.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://bxv.bbcook.cn

[U96] JS：async/await 与异常
来源：http://zdq.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://otb.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://bxd.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://jxb.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://ppp.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nwx.daria6918.cn

[U99] JS：事件监听
来源：http://jfb.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://fmv.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://lcb.sxryk.cn

document.querySelector(".item")
来源：http://jqt.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://ucf.andypj.xyz

el.classList.toggle("active")
来源：http://mqo.zdbjq.cn

[U102] JS：本地存储
来源：http://plk.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lfy.bbcook.cn

[U103] JS：定时器
来源：http://ymu.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wdz.bbcook.cn

[U104] JS：防抖
来源：http://ktd.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wqt.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://iwi.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://soz.nwbrower.top

[U106] JS：日期格式化
来源：http://yae.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ria.sysykeji.top

[U107] JS：数字千分位
来源：http://uvo.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mda.hongshengwenyu.top

[U108] JS：随机整数
来源：http://lqc.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oav.andypj.xyz

[U109] JS：数组分组
来源：http://ded.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://wjl.zdbjq.cn

[U110] JS：数组分块
来源：http://oaa.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gsd.svipenyu.cn

[U111] JS：对象转 Map
来源：http://qgv.zdbjq.cn

new Map(Object.entries(obj))
来源：http://dyl.svipenyu.cn

[U112] JS：字符串补位
来源：http://jnq.cucudq.cn

"7".padStart(3, "0")
来源：http://lko.iojbl.cn

[U113] JS：正则替换全部
来源：http://zxz.hywenlv.cn

s.replaceAll("a", "b")
来源：http://xtj.bbcook.cn

[U114] JS：JSON 深比较
来源：http://dea.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lrz.cucudq.cn

[U115] JS：生成 UUID
来源：http://xbq.nanxinkj.top

crypto.randomUUID()
来源：http://zcg.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://hfm.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://nzo.gotoacloud.top

[U117] JS：单元测试
来源：http://rlh.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://slq.jiagoushi.top

[U118] JS：开发服务器
来源：http://tfc.cqqwz.cn

npm i -D vite;  npx vite
来源：http://pxq.sjlbkw.cn

[U119] JS：生产构建
来源：http://gnb.316326.xyz

npx vite build
来源：http://xvi.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://hjc.316326.xyz

import.meta.env.VITE_API_URL
来源：http://tor.vehdjk.com

================================================================================
来源：http://lvm.jinyuanbaomall.cn

统计汇总
来源：http://pte.aizwys.cn

================================================================================
来源：http://zxz.zhiwuduotai.top

按语言统计（条）：
来源：http://vbh.xuetiantiany.cn

Python ......... 252
来源：http://acq.zhoulong.xyz

PHP ............ 252
来源：http://yjn.yonumen.top

JavaScript ..... 252
来源：http://fvl.birdmap.top

TypeScript ..... 212
来源：http://gmq.ehwqpu.com

Java ........... 212
来源：http://hgk.zhaomingkeji.xyz

Go ............. 212
来源：http://gmo.gogol.net.cn

Ruby ........... 212
来源：http://cym.zdqjudy.top

C# ............. 212
来源：http://nxc.xylfe.cn

C .............. 30
来源：http://hii.shangyingyoupin.top

C++ ............ 30
来源：http://jpy.fehbvm.com

SQL ............ 90
来源：http://jef.ydzc1.top

Bash ........... 80
来源：http://oxc.meibo888.top

Kotlin ......... 15
来源：http://mii.tian-w.cn

Swift .......... 15
来源：http://ghk.yongpay.top

Lua ............ 10
来源：http://tab.haohaochexian.top

Perl ........... 10
来源：http://iry.zycfv.cn

Scala .......... 10
来源：http://ldv.hnxiangtu.top

------------------------------------
来源：http://zrl.tian-w.cn

合计 ........... 2106 条
来源：http://zno.gotoacloud.top

按章节统计：
来源：http://tei.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wbj.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xyb.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hou.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hbz.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ezf.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://swp.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://akg.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qvd.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uii.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cpi.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cwy.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lai.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://trq.sysykeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://amb.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nby.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qsa.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://xkm.dianchejie.cn

R Bash 专题                             80
来源：http://jjr.epnwcf.com

S C / C++ 专题                          60
来源：http://tnt.zhongyouzk.top

T 其他语言补充                          60
来源：http://bnf.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://zlz.ehwqpu.com

------------------------------------
来源：http://iun.jianghu66.top

合计                                  2106 条
来源：http://cmn.hcnkem.com

--------------------------------------------------------------------------------
来源：http://udt.gotoacloud.top

使用提醒
来源：http://uzj.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://hin.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ubh.jiagoushi.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ndw.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nap.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qgf.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ntn.hnqzz.top

—— 文件结束 ——
来源：http://iug.vehdjk.com

================================================================================
来源：http://nyd.cdnleiting.top

程序语言常见例子速查手册（2024 版）
来源：http://jvr.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://eka.ydjk.org.cn

================================================================================
来源：http://fvf.fehbvm.com

【收录内容】
来源：http://zbw.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vja.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wii.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://gbf.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ixj.hnqzz.top

【使用说明】
来源：http://byw.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ybi.birdmap.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://acl.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://orr.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://okf.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://zpq.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nxi.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kyg.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lnh.yangfankeji.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mxo.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qkg.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pfl.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jln.xziqi.cn

【文件统计】
来源：http://nsf.feifeiyinyue.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dne.tian-w.cn

--------------------------------------------------------------------------------
来源：http://fwc.fzhhl.top

目  录
来源：http://mla.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://hqy.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://goq.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://exg.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ozy.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pfl.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iem.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hzd.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wcb.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qml.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rxg.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://itx.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hsz.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dxp.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://taj.9152youxi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://anf.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vqi.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ncn.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tdc.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://upd.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nrc.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rbx.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bzt.vqdsnc.cn

================================================================================
来源：http://deh.yfazqb.com

A. 基础语法与类型
来源：http://uiw.daxiang520.top

================================================================================
来源：http://dwj.ydjk.org.cn

[A01] Hello World
来源：http://ukd.nanxuanxn.top

Py:   print("Hello, World!")
来源：http://tru.zdbjq.cn

PHP:  echo "Hello, World!";
来源：http://acw.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://rtd.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nav.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://pzt.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://igq.tanke756.top

Ruby: puts "Hello, World!"
来源：http://jsl.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ptp.fengsongda.top

[A02] 变量声明与赋值
来源：http://tir.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fxg.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lih.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hii.shanyushiyangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bkg.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://brd.sweek.top

Go:   name := "Alex"; age := 20
来源：http://sdn.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://qli.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rlh.hysaishi.cn

[A03] 常量定义
来源：http://toh.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pms.uphjek.com

PHP:  const PI = 3.14159;
来源：http://gkg.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://bpc.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://tqf.cashguo.top

Java: static final double PI = 3.14159;
来源：http://pvl.hnqzz.top

Go:   const PI = 3.14159
来源：http://mjw.ctjpmb.com

Ruby: PI = 3.14159
来源：http://dtx.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://chy.guannengcc.top

[A04] 判断变量类型
来源：http://fgl.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://esc.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blk.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oas.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://cwh.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vkn.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://thm.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qhp.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://lhc.sxryk.cn

[A05] 整数除法与取模
来源：http://oxp.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://joh.shanyushiyangtech.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://msw.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://umx.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pyz.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://zfk.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://hdk.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://dvf.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://qrj.tianlin.xyz

[A06] 字符串转数字
来源：http://rla.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://ios.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cfx.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aeb.kuanghao11.cn

TS:   parseInt("42", 10); Number("42")
来源：http://glo.jyoumei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blr.jlsjyb.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://btu.dashuyun.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tjb.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mfj.hywenlv.cn

[A07] 数字转字符串
来源：http://dqe.hongshengwenyu.top

Py:   str(42)
来源：http://pqc.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://fjr.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://xxq.nanxinkj.top

TS:   String(42)
来源：http://fth.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tmv.xuanzx.com

Go:   strconv.Itoa(42)
来源：http://yyz.hnqzz.top


<!-- 参考信息 -->