代发 wailian999

[U47] PHP：联合类型
来源：http://fcb.gaohongyu789.top

int|string $id
来源：http://feg.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://pup.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rol.tanke756.top

[U49] PHP：只读属性
来源：http://pyg.cqqwz.cn

public readonly string $name
来源：http://nvd.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://iwv.fktsv.cn

public function __construct(private int $id) {}
来源：http://cfm.jinqigufen.top

[U51] PHP：数组解构
来源：http://jsp.sjlbkw.cn

[$a, $b] = $arr;
来源：http://gdw.bbcook.cn

[U52] PHP：箭头函数
来源：http://ngu.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://ita.ybcxt.top

[U53] PHP：空合并运算符
来源：http://vof.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://luf.yj20258.top

[U54] PHP：空安全调用
来源：http://yvg.tian-w.cn

$obj?->method()
来源：http://rdi.chenlongwang.top

[U55] PHP：match 表达式
来源：http://znq.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iak.sxryk.cn

[U56] PHP：命名参数
来源：http://uxs.zhongyouzk.top

f(a: 1, b: 2)
来源：http://hor.epnwcf.com

[U57] PHP：字符串插值
来源：http://xmd.cqqwz.cn

"值: {$a}"
来源：http://cpc.sufxvd.cn

[U58] PHP：数组三件套
来源：http://eus.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vxr.fengsongda.top

[U59] PHP：自定义排序
来源：http://lzc.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tog.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://dqd.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tpw.guowangkeji.top

[U61] PHP：正则
来源：http://ste.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vet.ybcxt.top

[U62] PHP：日期对象
来源：http://rzw.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vqq.xuanzx.com

[U63] PHP：文件读写
来源：http://rkh.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vrz.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://cxq.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://vtn.cashguo.top

[U65] PHP：会话
来源：http://sib.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://fpr.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://hzn.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rul.hnqzz.top

[U67] PHP：处理文件上传
来源：http://tem.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bpq.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://zae.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ffw.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://uro.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rej.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://old.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fsm.tian-w.cn

[U71] PHP：抛出异常
来源：http://ipt.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://mje.chenzaomai.com

[U72] PHP：写错误日志
来源：http://kxp.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://sjb.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://ymk.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://gma.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://gip.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://tgw.snrcjt.cn

[U75] PHP：依赖注入
来源：http://izm.fktsv.cn

composer require psr/container
来源：http://gah.yueranfly.top

[U76] PHP：简单路由
来源：http://toa.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bcp.fzhhl.top

[U77] PHP：模板渲染
来源：http://jju.zhiwuduotai.top

composer require twig/twig
来源：http://gip.hnqzz.top

[U78] PHP：单元测试
来源：http://fmq.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://buk.ehwqpu.com

[U79] PHP：静态分析
来源：http://khp.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://dvg.yongpay.top

[U80] PHP：代码规范修复
来源：http://dqe.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://niq.sxryk.cn

[U81] JS：初始化项目
来源：http://phv.meibo888.top

npm init -y;  npm i express
来源：http://hdf.yuxming.cn

[U82] JS：package.json 脚本
来源：http://kjd.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://afw.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://sqr.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://zle.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://jwh.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dsk.redwolf501.top

[U85] JS：可选链
来源：http://whf.cashguo.top

a?.b?.c
来源：http://gmz.hnxiangtu.top

[U86] JS：空值合并
来源：http://ayk.zhaomingkeji.xyz

a ?? b
来源：http://laq.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://yvv.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://qhr.nanxinkj.top

[U88] JS：对象展开合并
来源：http://ewy.sysykeji.top

{ ...a, ...b }
来源：http://fza.meibo888.top

[U89] JS：数组去重
来源：http://irl.hesvh.cn

[...new Set(arr)]
来源：http://hdq.xylfe.cn

[U90] JS：数字数组排序
来源：http://frm.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://bkn.yfazqb.com

[U91] JS：对象键值遍历
来源：http://iur.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://upi.svipenyu.cn

[U92] JS：深拷贝
来源：http://glp.jinqigfzy.top

structuredClone(obj)
来源：http://wdh.jinqigufen.top

[U93] JS：模板字符串
来源：http://ydp.hcnkem.com

`共 ${n} 条`
来源：http://xme.iojbl.cn

[U94] JS：箭头函数
来源：http://qka.zdqjudy.top

const double = x => x * 2;
来源：http://dsm.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://ppv.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://oky.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://jta.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sde.dashuyun.cn

[U97] JS：并发请求
来源：http://fln.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gcg.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://wyt.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bzf.xinyue.icu

[U99] JS：事件监听
来源：http://vbh.tian-w.cn

el.addEventListener("click", e => {})
来源：http://efh.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://vps.mhx1999.top

document.querySelector(".item")
来源：http://jeq.aizwys.cn

[U101] JS：classList 操作
来源：http://qoh.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://blt.xuanzx.com

[U102] JS：本地存储
来源：http://gpo.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://aox.jianghu66.top

[U103] JS：定时器
来源：http://rpy.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cyv.uphjek.com

[U104] JS：防抖
来源：http://hnq.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxi.zhijiandao.cn

[U105] JS：节流
来源：http://rjd.shangyingyoupin.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kjx.tianlin.xyz

[U106] JS：日期格式化
来源：http://mdx.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbr.jqgfzy.top

[U107] JS：数字千分位
来源：http://ytm.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sys.tanke756.top

[U108] JS：随机整数
来源：http://vnx.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ezq.yj20258888.top

[U109] JS：数组分组
来源：http://npn.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://kpu.9152youxi.cn

[U110] JS：数组分块
来源：http://pnq.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vbv.52xcode.cn

[U111] JS：对象转 Map
来源：http://cod.yj202588.top

new Map(Object.entries(obj))
来源：http://qdi.ybcxt.top

[U112] JS：字符串补位
来源：http://wbf.jinqigfzy.top

"7".padStart(3, "0")
来源：http://nge.gogol.net.cn

[U113] JS：正则替换全部
来源：http://fbg.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://kwe.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://irq.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hfp.jiagoushi.top

[U115] JS：生成 UUID
来源：http://xfb.sjlbkw.cn

crypto.randomUUID()
来源：http://xwa.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://fep.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://oku.hywenlv.cn

[U117] JS：单元测试
来源：http://htb.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://pal.0kj1m.cn

[U118] JS：开发服务器
来源：http://fok.fzhhl.top

npm i -D vite;  npx vite
来源：http://qrw.ydjk.org.cn

[U119] JS：生产构建
来源：http://uoe.bjfxy.top

npx vite build
来源：http://sci.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://vjh.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://zsl.dianchejie.cn

================================================================================
来源：http://dpq.sjlbkw.cn

统计汇总
来源：http://wag.jqgufenzy.top

================================================================================
来源：http://gsu.bjfxy.top

按语言统计（条）：
来源：http://uod.andypj.xyz

Python ......... 252
来源：http://gmn.xuanzx.com

PHP ............ 252
来源：http://szp.bjfxy.top

JavaScript ..... 252
来源：http://vmz.yonumen.top

TypeScript ..... 212
来源：http://atn.ywan-chungtsiang.top

Java ........... 212
来源：http://xrx.chenlongwang.top

Go ............. 212
来源：http://afc.fengsongda.top

Ruby ........... 212
来源：http://wks.quarkkingdee.top

C# ............. 212
来源：http://vlg.hesvh.cn

C .............. 30
来源：http://lbd.shangyingyoupin.top

C++ ............ 30
来源：http://jvc.aizwys.cn

SQL ............ 90
来源：http://bsf.gaohongyu789.top

Bash ........... 80
来源：http://fgo.cucudq.cn

Kotlin ......... 15
来源：http://elw.zhongyouzk.top

Swift .......... 15
来源：http://hoh.jqgfzy.top

Lua ............ 10
来源：http://whq.yfazqb.com

Perl ........... 10
来源：http://wka.iojbl.cn

Scala .......... 10
来源：http://izx.jyoumei.cn

------------------------------------
来源：http://lqb.9152youxi.cn

合计 ........... 2106 条
来源：http://dwy.zhaomingkeji.xyz

按章节统计：
来源：http://gua.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iqu.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jlv.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vma.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gbg.hongshengwenyu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://haz.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://alb.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cqy.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fwx.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lsx.yj20258.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qzk.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kzc.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://len.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wli.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kii.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tsz.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oun.iojbl.cn

Q SQL 专题                              90
来源：http://owh.iojbl.cn

R Bash 专题                             80
来源：http://oin.daria6918.cn

S C / C++ 专题                          60
来源：http://ppg.sweek.top

T 其他语言补充                          60
来源：http://lip.guannengcc.top

U 高频实用片段                         120
来源：http://wls.guowangkeji.top

------------------------------------
来源：http://tdw.yuxming.cn

合计                                  2106 条
来源：http://gnj.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://qbc.guannengcc.top

使用提醒
来源：http://ipl.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://mgy.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mdf.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jsp.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lzp.tanke756.top

在旧版本上使用前请先确认语法支持情况。
来源：http://voj.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://env.meibo888.top

—— 文件结束 ——
来源：http://mkk.shzxlz.cn

================================================================================
来源：http://tta.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://guf.jinghuilouyu.cn

Common Programming Examples Cheat Book
来源：http://nih.sxryk.cn

================================================================================
来源：http://tbk.zhaomingkeji.xyz

【收录内容】
来源：http://fve.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qmo.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bnf.jqgfzy.top

SQL · Bash · C · C++
来源：http://zmf.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blx.nanxinkj.top

【使用说明】
来源：http://ock.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ney.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cbc.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nss.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xfm.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hcn.kuanghao11.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bfg.shuidangran.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ssc.zycfv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aph.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lzj.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nrk.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jvb.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wzn.bjfxy.top

【文件统计】
来源：http://mkl.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://exr.tarul.cn

--------------------------------------------------------------------------------
来源：http://eqb.cdnleiting.top

目  录
来源：http://wtm.xylfe.cn

--------------------------------------------------------------------------------
来源：http://egn.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xpb.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jxx.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zfb.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mdp.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xzd.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ade.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://azp.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gyr.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gno.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://scn.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xrs.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rrd.gogol.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zjz.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gae.gzhubu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fcm.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://egq.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://swh.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wxo.shanyushiyangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rei.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vum.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://apn.tian-w.cn

================================================================================
来源：http://nik.iojbl.cn

A. 基础语法与类型
来源：http://kov.hfpthk.cn

================================================================================
来源：http://gke.chenlongwang.top

[A01] Hello World
来源：http://zuu.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://pqr.havefunace.top

PHP:  echo "Hello, World!";
来源：http://emt.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://ylz.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rna.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://loa.daxiang520.top

Go:   fmt.Println("Hello, World!")
来源：http://nbg.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://dou.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ihi.tianlin.xyz

[A02] 变量声明与赋值
来源：http://tnl.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ejz.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://diq.yj20258888.top

JS:   let name = "Alex"; const age = 20;
来源：http://odc.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fme.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://xmb.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://hfs.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://wew.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eib.havefunace.top

[A03] 常量定义
来源：http://vaf.vehdjk.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ueb.guowangkeji.top

PHP:  const PI = 3.14159;
来源：http://zgb.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://hbp.yvedp.cn

TS:   const PI: number = 3.14159;
来源：http://prd.cheryme.top

Java: static final double PI = 3.14159;
来源：http://mrp.yueranfly.top

Go:   const PI = 3.14159
来源：http://est.sxryk.cn

Ruby: PI = 3.14159
来源：http://drg.316326.xyz

C#:   const double PI = 3.14159;
来源：http://uch.gzhubu.top

[A04] 判断变量类型
来源：http://fhf.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fmq.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xno.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hgk.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://cyq.gogol.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dif.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://rxq.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hpe.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://pqh.sufxvd.cn

[A05] 整数除法与取模
来源：http://lmj.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uud.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bdo.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rhm.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cmc.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://mqw.smart0.xyz

Go:   7 / 2; 7 % 2
来源：http://ppg.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://iwc.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://vpp.sweek.top


<!-- 参考信息 -->