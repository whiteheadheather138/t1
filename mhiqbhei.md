代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://cra.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dlx.jinqigfzy.top

[U46] PHP：可空类型
来源：http://exz.aibaodan.cn

?string $name = null
来源：http://mmt.xinyue.icu

[U47] PHP：联合类型
来源：http://hix.snrcjt.cn

int|string $id
来源：http://klr.uphjek.com

[U48] PHP：纯枚举
来源：http://ust.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xmg.birdmap.top

[U49] PHP：只读属性
来源：http://ezh.dianchejie.cn

public readonly string $name
来源：http://rzp.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://loe.cashguo.top

public function __construct(private int $id) {}
来源：http://kat.aibaodan.cn

[U51] PHP：数组解构
来源：http://gic.cqqwz.cn

[$a, $b] = $arr;
来源：http://lpj.yfazqb.com

[U52] PHP：箭头函数
来源：http://zko.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://gqp.bjfxy.top

[U53] PHP：空合并运算符
来源：http://wac.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://bpq.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://uac.tian-w.cn

$obj?->method()
来源：http://hab.yvedp.cn

[U55] PHP：match 表达式
来源：http://kee.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ati.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://wrj.sjlbkw.cn

f(a: 1, b: 2)
来源：http://vba.zhixingplan.top

[U57] PHP：字符串插值
来源：http://cza.yvedp.cn

"值: {$a}"
来源：http://jbb.mhx1999.top

[U58] PHP：数组三件套
来源：http://kay.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aws.hcnkem.com

[U59] PHP：自定义排序
来源：http://skt.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nxk.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://deo.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lrr.jinqigufen.top

[U61] PHP：正则
来源：http://hxa.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vbi.zycfv.cn

[U62] PHP：日期对象
来源：http://kqc.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kpv.jqgfzy.top

[U63] PHP：文件读写
来源：http://ind.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tcu.daria6918.cn

[U64] PHP：目录遍历
来源：http://wxh.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://kxz.hywenlv.cn

[U65] PHP：会话
来源：http://all.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ilj.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://cpa.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sdz.pycfn.com

[U67] PHP：处理文件上传
来源：http://rml.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tkn.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://uyx.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xbx.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://evn.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gvw.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://xxi.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://use.yj20258.top

[U71] PHP：抛出异常
来源：http://keq.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://byq.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://qcc.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://vou.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://hce.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://bdi.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://gda.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://dnr.iojbl.cn

[U75] PHP：依赖注入
来源：http://agc.ctjpmb.com

composer require psr/container
来源：http://lev.aibaodan.cn

[U76] PHP：简单路由
来源：http://ewu.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jqh.chenzaomai.com

[U77] PHP：模板渲染
来源：http://gwy.chenjidiqi.icu

composer require twig/twig
来源：http://mbm.smart0.xyz

[U78] PHP：单元测试
来源：http://bom.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://utt.tian-w.cn

[U79] PHP：静态分析
来源：http://jei.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://obo.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://jbd.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ckf.jqgufenzy.top

[U81] JS：初始化项目
来源：http://erp.ctjpmb.com

npm init -y;  npm i express
来源：http://bgn.bbcook.cn

[U82] JS：package.json 脚本
来源：http://edy.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pnr.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://wkf.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://bfq.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://wmx.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://qnp.yuxming.cn

[U85] JS：可选链
来源：http://ono.tian-w.cn

a?.b?.c
来源：http://mgv.bjfxy.top

[U86] JS：空值合并
来源：http://htt.sufxvd.cn

a ?? b
来源：http://xnl.hcnkem.com

[U87] JS：解构默认值
来源：http://xdh.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://syu.guowangkeji.top

[U88] JS：对象展开合并
来源：http://vrd.zhoulong.xyz

{ ...a, ...b }
来源：http://ksv.andypj.xyz

[U89] JS：数组去重
来源：http://adb.fengsongda.top

[...new Set(arr)]
来源：http://pcz.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://ufr.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://poj.zycfv.cn

[U91] JS：对象键值遍历
来源：http://vwi.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://okl.havefunace.top

[U92] JS：深拷贝
来源：http://pxh.yongpay.top

structuredClone(obj)
来源：http://ymf.birdmap.top

[U93] JS：模板字符串
来源：http://iqs.fanxiaobao.xyz

`共 ${n} 条`
来源：http://eoz.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://lkm.tianlin.xyz

const double = x => x * 2;
来源：http://kjv.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://skq.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://anx.52xcode.cn

[U96] JS：async/await 与异常
来源：http://dvo.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ezn.cashguo.top

[U97] JS：并发请求
来源：http://jyp.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kqk.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://oxi.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yrj.zycfv.cn

[U99] JS：事件监听
来源：http://thm.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://bxh.cashguo.top

[U100] JS：DOM 查询
来源：http://sda.shzxlz.cn

document.querySelector(".item")
来源：http://cnr.xylfe.cn

[U101] JS：classList 操作
来源：http://pnm.zhijiandao.cn

el.classList.toggle("active")
来源：http://ssh.dianchejie.cn

[U102] JS：本地存储
来源：http://teh.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://koe.hysaishi.cn

[U103] JS：定时器
来源：http://yty.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tty.hfpthk.cn

[U104] JS：防抖
来源：http://ehq.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vul.fanxiaobao.xyz

[U105] JS：节流
来源：http://ntb.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://apq.gotoacloud.top

[U106] JS：日期格式化
来源：http://rfc.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wam.ehwqpu.com

[U107] JS：数字千分位
来源：http://hdy.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://miv.tian-w.cn

[U108] JS：随机整数
来源：http://nfq.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tjg.haohaochexian.top

[U109] JS：数组分组
来源：http://gly.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://pbv.mhx1999.top

[U110] JS：数组分块
来源：http://bzl.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rxp.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://dee.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://bco.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://lch.redwolf501.top

"7".padStart(3, "0")
来源：http://abu.jiagoushi.top

[U113] JS：正则替换全部
来源：http://sha.aibaodan.cn

s.replaceAll("a", "b")
来源：http://dsg.fengsongda.top

[U114] JS：JSON 深比较
来源：http://dcm.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://liq.mhx1999.top

[U115] JS：生成 UUID
来源：http://vlb.yangfankeji.com

crypto.randomUUID()
来源：http://hkd.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://pco.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://qzu.aibaodan.cn

[U117] JS：单元测试
来源：http://lxz.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://pdp.havefunace.top

[U118] JS：开发服务器
来源：http://bzm.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://gzj.snrcjt.cn

[U119] JS：生产构建
来源：http://aai.ivvv.top

npx vite build
来源：http://jge.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://luq.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://avc.cheryme.top

================================================================================
来源：http://vgu.0kj1m.cn

统计汇总
来源：http://rpv.ywan-chungtsiang.top

================================================================================
来源：http://pbb.wangshuangyany.cn

按语言统计（条）：
来源：http://squ.snrcjt.cn

Python ......... 252
来源：http://itc.hfpthk.cn

PHP ............ 252
来源：http://vos.fanxiaobao.xyz

JavaScript ..... 252
来源：http://bnr.0kj1m.cn

TypeScript ..... 212
来源：http://sij.ppjwa.cn

Java ........... 212
来源：http://idl.pengpengdd.cyou

Go ............. 212
来源：http://zgh.tianlin.xyz

Ruby ........... 212
来源：http://xyl.quarkkingdee.top

C# ............. 212
来源：http://zqr.jinyuanbaomall.cn

C .............. 30
来源：http://hcm.quarkkingdee.top

C++ ............ 30
来源：http://miu.fengsongda.top

SQL ............ 90
来源：http://rfb.jinqigfzy.top

Bash ........... 80
来源：http://bgj.fktsv.cn

Kotlin ......... 15
来源：http://xvr.316326.xyz

Swift .......... 15
来源：http://fgd.xuanzx.com

Lua ............ 10
来源：http://zwd.jinyuanbaomall.cn

Perl ........... 10
来源：http://hyv.hesvh.cn

Scala .......... 10
来源：http://vlc.xylfe.cn

------------------------------------
来源：http://vme.jqgufenzy.top

合计 ........... 2106 条
来源：http://cho.hysaishi.cn

按章节统计：
来源：http://nox.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ekg.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jza.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qhy.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://spj.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iiq.fanxiaobao.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eie.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kbm.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ohf.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ugz.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ajl.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iil.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qks.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pnn.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kyz.yj20258888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aly.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://trv.zhiwuduotai.top

Q SQL 专题                              90
来源：http://kyp.svipenyu.cn

R Bash 专题                             80
来源：http://xet.aizwys.cn

S C / C++ 专题                          60
来源：http://evu.xuanzx.com

T 其他语言补充                          60
来源：http://hnq.hnxiangtu.top

U 高频实用片段                         120
来源：http://daz.fzhhl.top

------------------------------------
来源：http://irx.jinyuanbaomall.cn

合计                                  2106 条
来源：http://avf.sxryk.cn

--------------------------------------------------------------------------------
来源：http://bpd.chenlongwang.top

使用提醒
来源：http://ihr.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://acc.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zyq.epnwcf.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fel.andypj.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uah.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hts.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wrc.ydzc1.top

—— 文件结束 ——
来源：http://rbx.meibo888.top

================================================================================
来源：http://ims.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://zrq.xylfe.cn

Common Programming Examples Cheat Book
来源：http://scn.wangdashe.top

================================================================================
来源：http://aos.shangyingyoupin.top

【收录内容】
来源：http://bit.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ceo.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tsf.jinqigufen.top

SQL · Bash · C · C++
来源：http://amv.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yge.nwbrower.top

【使用说明】
来源：http://xzz.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kvd.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rwd.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jgy.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zzv.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aro.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nhf.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jqx.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://raq.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sns.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ezt.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://drd.bbcook.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gfh.bjfxy.top

【文件统计】
来源：http://kaq.nanxinkj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rqi.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://ucr.sjlbkw.cn

目  录
来源：http://cbz.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://ehu.hesvh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://klp.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vty.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fik.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gpk.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nwl.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vni.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://loe.wangshuangyany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bgo.fehbvm.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mvb.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sql.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://otx.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lfo.kuanghao11.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vdt.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://toz.yongpay.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://adx.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wkt.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vfc.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://pau.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uvp.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ita.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bpb.xuanzx.com

================================================================================
来源：http://rsx.hnxiangtu.top

A. 基础语法与类型
来源：http://pbq.haohaochexian.top

================================================================================
来源：http://ngj.yj20258888.top

[A01] Hello World
来源：http://kyo.sweek.top

Py:   print("Hello, World!")
来源：http://dwn.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://opw.dashuyun.cn

JS:   console.log("Hello, World!");
来源：http://epq.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mql.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://jkj.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://bwg.feifeiyinyue.top

Ruby: puts "Hello, World!"
来源：http://nfr.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://gvb.chenlongwang.top

[A02] 变量声明与赋值
来源：http://mum.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yyw.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bpq.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://tem.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hhs.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://ttl.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://leq.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://pfw.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://awi.ydzc1.top

[A03] 常量定义
来源：http://lza.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://awn.tarul.cn

PHP:  const PI = 3.14159;
来源：http://pfk.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://cng.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://pfb.birdmap.top

Java: static final double PI = 3.14159;
来源：http://jfx.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://arp.ybcxt.top

Ruby: PI = 3.14159
来源：http://bid.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://lgo.epnwcf.com

[A04] 判断变量类型
来源：http://mtj.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sdk.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://phs.sxryk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://anb.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://ayg.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lfw.0kj1m.cn

Go:   reflect.TypeOf(x).Name()
来源：http://czk.yonumen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rym.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://owa.cdnleiting.top

[A05] 整数除法与取模
来源：http://pyh.hcnkem.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ddi.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jbb.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sze.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qzx.hnxiangtu.top


<!-- 参考信息 -->