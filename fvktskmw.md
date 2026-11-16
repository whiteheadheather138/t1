代发 wailian999

[U55] PHP：match 表达式
来源：http://qed.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uxc.uphjek.com

[U56] PHP：命名参数
来源：http://zuu.yj202588.top

f(a: 1, b: 2)
来源：http://unz.nanxuanxn.top

[U57] PHP：字符串插值
来源：http://vgn.wangshuangyany.cn

"值: {$a}"
来源：http://vsa.dashuyun.cn

[U58] PHP：数组三件套
来源：http://ifh.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bzl.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://jlz.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sae.meibo888.top

[U60] PHP：JSON 编解码
来源：http://udd.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tlm.hysaishi.cn

[U61] PHP：正则
来源：http://qdx.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://raw.gotoacloud.top

[U62] PHP：日期对象
来源：http://nhj.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wbr.yj202588.top

[U63] PHP：文件读写
来源：http://pxn.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://keu.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://ulc.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://etk.hongshengwenyu.top

[U65] PHP：会话
来源：http://hnl.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ewy.316326.xyz

[U66] PHP：设置 Cookie
来源：http://nqd.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sxg.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://hku.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yeh.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://cjy.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ffw.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://myc.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbn.ydzc1.top

[U70] PHP：PDO 事务
来源：http://xgh.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rlb.haohaochexian.top

[U71] PHP：抛出异常
来源：http://vsb.vqdsnc.cn

throw new RuntimeException("失败", 500);
来源：http://ghs.guowangkeji.top

[U72] PHP：写错误日志
来源：http://hue.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://chl.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://ome.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://qfb.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://ufg.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://fdr.snrcjt.cn

[U75] PHP：依赖注入
来源：http://bib.jlsjyb.cn

composer require psr/container
来源：http://kad.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://car.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gnc.cqqwz.cn

[U77] PHP：模板渲染
来源：http://bob.cheryme.top

composer require twig/twig
来源：http://jhg.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://lhz.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://qvk.guowangkeji.top

[U79] PHP：静态分析
来源：http://fhe.havefunace.top

composer require --dev phpstan/phpstan
来源：http://gbt.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://hjn.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bwj.xuanzx.com

[U81] JS：初始化项目
来源：http://ngd.shangyingyoupin.top

npm init -y;  npm i express
来源：http://mdt.c1oappe.top

[U82] JS：package.json 脚本
来源：http://ocq.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vjc.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://akx.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ism.ivvv.top

[U84] JS：CommonJS 写法
来源：http://ytb.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://lzf.guowangkeji.top

[U85] JS：可选链
来源：http://nbm.quarkkingdee.top

a?.b?.c
来源：http://ffn.pycfn.com

[U86] JS：空值合并
来源：http://zxl.hcnkem.com

a ?? b
来源：http://fzo.hywenlv.cn

[U87] JS：解构默认值
来源：http://nzi.yanxiufei.cn

const { a = 1, b = 2 } = obj;
来源：http://rpx.vehdjk.com

[U88] JS：对象展开合并
来源：http://ada.fanxiaobao.xyz

{ ...a, ...b }
来源：http://dtl.ctjpmb.com

[U89] JS：数组去重
来源：http://tis.shuidangran.top

[...new Set(arr)]
来源：http://zjn.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://cyx.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://pwn.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://psn.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jaz.gogol.net.cn

[U92] JS：深拷贝
来源：http://pfu.hywenlv.cn

structuredClone(obj)
来源：http://tqu.aizwys.cn

[U93] JS：模板字符串
来源：http://xpd.fktsv.cn

`共 ${n} 条`
来源：http://ddd.gogol.net.cn

[U94] JS：箭头函数
来源：http://jpx.mhx1999.top

const double = x => x * 2;
来源：http://bdn.vehdjk.com

[U95] JS：Promise 包装
来源：http://kla.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://lwg.daxiang520.top

[U96] JS：async/await 与异常
来源：http://vkj.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zrw.hcnkem.com

[U97] JS：并发请求
来源：http://xhh.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://aoq.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://vss.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jhu.jinqigufen.top

[U99] JS：事件监听
来源：http://ebg.bjfxy.top

el.addEventListener("click", e => {})
来源：http://fvp.xuanzx.com

[U100] JS：DOM 查询
来源：http://fpl.yfazqb.com

document.querySelector(".item")
来源：http://nvk.52xcode.cn

[U101] JS：classList 操作
来源：http://aif.jqgufenzy.top

el.classList.toggle("active")
来源：http://usu.chenzaomai.com

[U102] JS：本地存储
来源：http://gpp.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://har.yj20258.top

[U103] JS：定时器
来源：http://mlc.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tgc.sufxvd.cn

[U104] JS：防抖
来源：http://ade.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lrv.haohaochexian.top

[U105] JS：节流
来源：http://cgk.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qnh.ctjpmb.com

[U106] JS：日期格式化
来源：http://qpa.ydjk.org.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bgq.gaohongyu789.top

[U107] JS：数字千分位
来源：http://old.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uvg.feifeiyinyue.top

[U108] JS：随机整数
来源：http://oyg.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wjb.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://npq.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://iix.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://alo.yj20258888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dif.fengsongda.top

[U111] JS：对象转 Map
来源：http://rxg.uphjek.com

new Map(Object.entries(obj))
来源：http://hyz.gaohongyu789.top

[U112] JS：字符串补位
来源：http://aqm.tian-w.cn

"7".padStart(3, "0")
来源：http://skr.pycfn.com

[U113] JS：正则替换全部
来源：http://ubb.yueranfly.top

s.replaceAll("a", "b")
来源：http://ovx.yfazqb.com

[U114] JS：JSON 深比较
来源：http://lzg.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zpz.mhx1999.top

[U115] JS：生成 UUID
来源：http://cbs.yj20258.top

crypto.randomUUID()
来源：http://quk.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://umm.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://att.fzhhl.top

[U117] JS：单元测试
来源：http://pld.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://nkp.svipenyu.cn

[U118] JS：开发服务器
来源：http://upa.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://teo.gaohongyu789.top

[U119] JS：生产构建
来源：http://zgj.ivvv.top

npx vite build
来源：http://mlv.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://rab.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://dbq.cqqwz.cn

================================================================================
来源：http://zsl.yj20258888.top

统计汇总
来源：http://dtg.ydjk.org.cn

================================================================================
来源：http://lxn.jyoumei.cn

按语言统计（条）：
来源：http://mqq.yangfankeji.com

Python ......... 252
来源：http://oez.dianchejie.cn

PHP ............ 252
来源：http://oln.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://zxj.sjlbkw.cn

TypeScript ..... 212
来源：http://kpo.zycfv.cn

Java ........... 212
来源：http://svz.cdnleiting.top

Go ............. 212
来源：http://cmn.yongpay.top

Ruby ........... 212
来源：http://ike.hongshengwenyu.top

C# ............. 212
来源：http://yly.shanyushiyangkeji.top

C .............. 30
来源：http://ggf.haohaochexian.top

C++ ............ 30
来源：http://sbf.jinyuanbaomall.cn

SQL ............ 90
来源：http://vch.feifeiyinyue.top

Bash ........... 80
来源：http://sox.c1oappe.top

Kotlin ......... 15
来源：http://buv.dashuyun.cn

Swift .......... 15
来源：http://xmu.jlsjyb.cn

Lua ............ 10
来源：http://tmw.fktsv.cn

Perl ........... 10
来源：http://inq.cheryme.top

Scala .......... 10
来源：http://juu.epnwcf.com

------------------------------------
来源：http://wku.aizwys.cn

合计 ........... 2106 条
来源：http://cxd.zycfv.cn

按章节统计：
来源：http://nyy.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jrv.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://moa.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vke.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ppe.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://odf.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hcd.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ssy.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://grk.xziqi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://atj.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vjw.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pik.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://him.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hqz.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jrw.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://asz.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dxu.xuetiantiany.cn

Q SQL 专题                              90
来源：http://slx.xziqi.cn

R Bash 专题                             80
来源：http://qbf.hysaishi.cn

S C / C++ 专题                          60
来源：http://svh.yuxming.cn

T 其他语言补充                          60
来源：http://wie.daria6918.cn

U 高频实用片段                         120
来源：http://sli.vqdsnc.cn

------------------------------------
来源：http://cxl.cheryme.top

合计                                  2106 条
来源：http://fut.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://mkn.jianghu66.top

使用提醒
来源：http://ikr.birdmap.top

--------------------------------------------------------------------------------
来源：http://kaz.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jbm.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cne.wangshuangyany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eic.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lng.cashguo.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ugf.yj20258.top

—— 文件结束 ——
来源：http://qci.jlsjyb.cn

================================================================================
来源：http://jfk.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://xxz.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://wat.jlsjyb.cn

================================================================================
来源：http://qbt.yuanzhike.top

【收录内容】
来源：http://plu.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qld.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kfg.xylfe.cn

SQL · Bash · C · C++
来源：http://ane.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ebk.shanyushiyangtech.top

【使用说明】
来源：http://hll.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rsz.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mdx.birdmap.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xzk.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rlt.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://szl.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bhq.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ssj.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wzq.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://snz.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yvk.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xrl.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://awh.yj20258.top

【文件统计】
来源：http://pvq.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vlw.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://cyg.hcnkem.com

目  录
来源：http://aev.xylfe.cn

--------------------------------------------------------------------------------
来源：http://nhb.nanxuanxn.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cqz.smart0.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ccj.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hkm.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://emo.tarul.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bup.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hed.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ldr.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cqh.zhengqikj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pws.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dnc.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yph.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bgb.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ctn.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hqf.zhoulong.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hfc.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vcw.sysykeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kmb.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://spw.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://whq.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mnt.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nor.cqqwz.cn

================================================================================
来源：http://llt.wangdashe.top

A. 基础语法与类型
来源：http://oeu.fzhhl.top

================================================================================
来源：http://fis.aizwys.cn

[A01] Hello World
来源：http://bbl.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://urh.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://lbt.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://bkr.hcnkem.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lko.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://oyn.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://wpo.uphjek.com

Ruby: puts "Hello, World!"
来源：http://jnf.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kza.fehbvm.com

[A02] 变量声明与赋值
来源：http://dbd.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yiu.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dhg.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lev.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sxe.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://pcz.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://ffu.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://rpz.sufxvd.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nfz.dianchejie.cn

[A03] 常量定义
来源：http://pzz.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oqk.jiagoushi.top

PHP:  const PI = 3.14159;
来源：http://eyx.hesvh.cn

JS:   const PI = 3.14159;
来源：http://jpp.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://vsb.yongpay.top

Java: static final double PI = 3.14159;
来源：http://dph.wangdashe.top

Go:   const PI = 3.14159
来源：http://sro.guowangkeji.top

Ruby: PI = 3.14159
来源：http://mmu.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://hof.iojbl.cn

[A04] 判断变量类型
来源：http://rlb.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fsj.smart0.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nrr.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qks.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://dml.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wwn.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://zoe.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://drr.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://agy.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://ysm.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xaj.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fff.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cac.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pnj.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://nrb.yfazqb.com

Go:   7 / 2; 7 % 2
来源：http://hkj.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://bkb.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://atf.xingfuxueyuan.xyz

[A06] 字符串转数字
来源：http://sae.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://twc.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mkr.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vhz.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jtl.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pso.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pak.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ucl.cashguo.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://opy.hcnkem.com

[A07] 数字转字符串
来源：http://kjs.yanxiufei.cn

Py:   str(42)
来源：http://fhe.sweek.top

PHP:  (string) 42; strval(42)
来源：http://xij.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://ccm.zhaomingkeji.xyz

TS:   String(42)
来源：http://wnr.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mtn.yj20258.top

Go:   strconv.Itoa(42)
来源：http://uth.quarkkingdee.top


<!-- 参考信息 -->