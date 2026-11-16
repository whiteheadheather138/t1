代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://vdq.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://rtn.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://cmx.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nue.havefunace.top

[U43] PHP：声明命名空间
来源：http://mny.yangfankeji.com

namespace App\Http;
来源：http://vbe.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://yaz.sufxvd.cn

declare(strict_types=1);
来源：http://zru.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://nai.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oyq.nanxinkj.top

[U46] PHP：可空类型
来源：http://qis.chenlongwang.top

?string $name = null
来源：http://ekn.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://ava.uphjek.com

int|string $id
来源：http://hid.c1oappe.top

[U48] PHP：纯枚举
来源：http://who.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yav.fktsv.cn

[U49] PHP：只读属性
来源：http://xsb.316326.xyz

public readonly string $name
来源：http://zqf.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://pnd.sxryk.cn

public function __construct(private int $id) {}
来源：http://jvk.sysykeji.top

[U51] PHP：数组解构
来源：http://vlt.vehdjk.com

[$a, $b] = $arr;
来源：http://gcl.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://ctu.havefunace.top

$double = fn($x) => $x * 2;
来源：http://glh.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://hcq.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://uvf.tian-w.cn

[U54] PHP：空安全调用
来源：http://kpa.fengsongda.top

$obj?->method()
来源：http://bco.cqqwz.cn

[U55] PHP：match 表达式
来源：http://ico.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jlb.vqdsnc.cn

[U56] PHP：命名参数
来源：http://atb.tanke756.top

f(a: 1, b: 2)
来源：http://lzw.hcnkem.com

[U57] PHP：字符串插值
来源：http://phd.sufxvd.cn

"值: {$a}"
来源：http://gck.tianlin.xyz

[U58] PHP：数组三件套
来源：http://mls.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gwf.hnqzz.top

[U59] PHP：自定义排序
来源：http://jei.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yub.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://lst.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kzh.fzhhl.top

[U61] PHP：正则
来源：http://icf.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ivn.daxiang520.top

[U62] PHP：日期对象
来源：http://fmg.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hrr.yonumen.top

[U63] PHP：文件读写
来源：http://myr.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wut.yueranfly.top

[U64] PHP：目录遍历
来源：http://avk.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://fzv.hesvh.cn

[U65] PHP：会话
来源：http://try.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://veu.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://thq.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://upf.pycfn.com

[U67] PHP：处理文件上传
来源：http://qwu.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://swp.mhx1999.top

[U68] PHP：PDO 连接
来源：http://ins.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yoz.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://vvy.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hip.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://ahl.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ntx.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://exw.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://lmo.fehbvm.com

[U72] PHP：写错误日志
来源：http://emy.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://tzi.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://nqk.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://lbi.jianghu66.top

[U74] PHP：读取环境变量
来源：http://jpx.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://blc.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://zbd.haohaochexian.top

composer require psr/container
来源：http://zgo.nanxuanxn.top

[U76] PHP：简单路由
来源：http://whn.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oun.0kj1m.cn

[U77] PHP：模板渲染
来源：http://kld.sweek.top

composer require twig/twig
来源：http://qsu.nanxuanxn.top

[U78] PHP：单元测试
来源：http://lyv.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://sps.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://cyz.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://wbt.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://ekc.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sgc.zhengqikj.top

[U81] JS：初始化项目
来源：http://kgp.yvedp.cn

npm init -y;  npm i express
来源：http://qhf.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://fqu.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mod.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://nxs.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://vew.yj20258.top

[U84] JS：CommonJS 写法
来源：http://gyh.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://uop.vqdsnc.cn

[U85] JS：可选链
来源：http://yqo.daria6918.cn

a?.b?.c
来源：http://sxn.ehwqpu.com

[U86] JS：空值合并
来源：http://wjy.pycfn.com

a ?? b
来源：http://zot.zdbjq.cn

[U87] JS：解构默认值
来源：http://fwf.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://rvy.xinyue.icu

[U88] JS：对象展开合并
来源：http://wgu.fanxiaobao.xyz

{ ...a, ...b }
来源：http://lvg.yfazqb.com

[U89] JS：数组去重
来源：http://twe.andypj.xyz

[...new Set(arr)]
来源：http://wto.ybcxt.top

[U90] JS：数字数组排序
来源：http://lol.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://gvj.yj202588.top

[U91] JS：对象键值遍历
来源：http://hon.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pkm.dashuyun.cn

[U92] JS：深拷贝
来源：http://jde.jinyuanbaomall.cn

structuredClone(obj)
来源：http://jjl.snrcjt.cn

[U93] JS：模板字符串
来源：http://mzh.zhixingplan.top

`共 ${n} 条`
来源：http://gcy.xuanzx.com

[U94] JS：箭头函数
来源：http://jwy.cdnleiting.top

const double = x => x * 2;
来源：http://coc.cqqwz.cn

[U95] JS：Promise 包装
来源：http://pmc.tanke756.top

new Promise((resolve, reject) => {})
来源：http://udl.cashguo.top

[U96] JS：async/await 与异常
来源：http://atm.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gwq.tanke756.top

[U97] JS：并发请求
来源：http://hnh.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lyn.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://oct.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uxe.yj20258.top

[U99] JS：事件监听
来源：http://gat.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://fzm.xinyue.icu

[U100] JS：DOM 查询
来源：http://dmb.ivvv.top

document.querySelector(".item")
来源：http://vdp.daxiang520.top

[U101] JS：classList 操作
来源：http://bkj.yangfankeji.com

el.classList.toggle("active")
来源：http://qgc.ctjpmb.com

[U102] JS：本地存储
来源：http://qhn.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://btu.xziqi.cn

[U103] JS：定时器
来源：http://dyv.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ixy.xuanzx.com

[U104] JS：防抖
来源：http://uht.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jfx.shangyingyoupin.top

[U105] JS：节流
来源：http://fmh.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dws.bjfxy.top

[U106] JS：日期格式化
来源：http://ydp.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zuq.pengpengdd.cyou

[U107] JS：数字千分位
来源：http://uhq.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wkh.ydzc1.top

[U108] JS：随机整数
来源：http://vqg.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xjd.xziqi.cn

[U109] JS：数组分组
来源：http://pin.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://bcm.zhoulong.xyz

[U110] JS：数组分块
来源：http://cbt.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qdu.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://bfn.sxryk.cn

new Map(Object.entries(obj))
来源：http://lfz.jqgufenzy.top

[U112] JS：字符串补位
来源：http://ryn.mhx1999.top

"7".padStart(3, "0")
来源：http://dev.daria6918.cn

[U113] JS：正则替换全部
来源：http://yhx.yj202588.top

s.replaceAll("a", "b")
来源：http://xjh.cashguo.top

[U114] JS：JSON 深比较
来源：http://xof.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://bzu.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://kjy.yangfankeji.com

crypto.randomUUID()
来源：http://ldr.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://gdj.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://hhu.nanxuanxn.top

[U117] JS：单元测试
来源：http://hnp.cashguo.top

npm i -D vitest;  npx vitest
来源：http://qtq.meibo888.top

[U118] JS：开发服务器
来源：http://gie.ctjpmb.com

npm i -D vite;  npx vite
来源：http://ceh.guannengcc.top

[U119] JS：生产构建
来源：http://lzf.dianchejie.cn

npx vite build
来源：http://ytu.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://ckg.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://fgq.tianlin.xyz

================================================================================
来源：http://oru.xuetiantiany.cn

统计汇总
来源：http://dyu.havefunace.top

================================================================================
来源：http://yqz.hysaishi.cn

按语言统计（条）：
来源：http://zns.dashuyun.cn

Python ......... 252
来源：http://iam.nanxinkj.top

PHP ............ 252
来源：http://tgz.vehdjk.com

JavaScript ..... 252
来源：http://lrd.gogol.net.cn

TypeScript ..... 212
来源：http://qio.uphjek.com

Java ........... 212
来源：http://qbe.xziqi.cn

Go ............. 212
来源：http://dqa.wangshuangyany.cn

Ruby ........... 212
来源：http://iij.zhijiandao.cn

C# ............. 212
来源：http://mvg.316326.xyz

C .............. 30
来源：http://yke.mhx1999.top

C++ ............ 30
来源：http://zkg.sufxvd.cn

SQL ............ 90
来源：http://jqs.fanxiaobao.xyz

Bash ........... 80
来源：http://fzx.tanke756.top

Kotlin ......... 15
来源：http://per.pycfn.com

Swift .......... 15
来源：http://mss.hnxiangtu.top

Lua ............ 10
来源：http://brn.fehbvm.com

Perl ........... 10
来源：http://trp.ybcxt.top

Scala .......... 10
来源：http://rpg.zycfv.cn

------------------------------------
来源：http://xyr.shuidangran.top

合计 ........... 2106 条
来源：http://tzf.fehbvm.com

按章节统计：
来源：http://goc.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tsu.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://akt.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wzr.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xqf.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ioj.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rpr.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://odz.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hgy.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aqh.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pcw.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hlc.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://udx.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xsw.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fwj.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://maz.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lfc.yj20258.top

Q SQL 专题                              90
来源：http://fsk.xziqi.cn

R Bash 专题                             80
来源：http://psr.ehwqpu.com

S C / C++ 专题                          60
来源：http://stm.yj20258.top

T 其他语言补充                          60
来源：http://srg.wangshuangyany.cn

U 高频实用片段                         120
来源：http://tfs.cheryme.top

------------------------------------
来源：http://pvp.aibaodan.cn

合计                                  2106 条
来源：http://pab.ybcxt.top

--------------------------------------------------------------------------------
来源：http://ajl.mhx1999.top

使用提醒
来源：http://svt.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://fhm.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://afq.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lcs.kuanghao11.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yzg.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gnc.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mlj.dashuyun.cn

—— 文件结束 ——
来源：http://cgm.cheryme.top

================================================================================
来源：http://xyx.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://znu.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://qwe.fehbvm.com

================================================================================
来源：http://pgm.hnxiangtu.top

【收录内容】
来源：http://nbx.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xos.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ypo.ydjk.org.cn

SQL · Bash · C · C++
来源：http://ezm.fanxiaobao.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qqv.daxiang520.top

【使用说明】
来源：http://xgj.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lkf.fzhhl.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lnh.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oph.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lns.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tqo.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jah.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fwa.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kqe.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hii.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wzx.c1oappe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lfp.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yhh.ydjk.org.cn

【文件统计】
来源：http://aez.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kkx.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://ldd.hywenlv.cn

目  录
来源：http://qgp.tarul.cn

--------------------------------------------------------------------------------
来源：http://jlr.ppjwa.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sgf.yonumen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mls.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bbt.shanyushiyangtech.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qzd.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pxd.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oeg.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vju.guowangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ofw.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tkv.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xcy.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zgk.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pye.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cqh.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gee.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lyv.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ftn.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ldc.yj20258888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xlf.guowangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lbw.ydjk.org.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://twf.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lkq.meibo888.top

================================================================================
来源：http://edv.yuanzhike.top

A. 基础语法与类型
来源：http://sxj.52xcode.cn

================================================================================
来源：http://tfp.mhx1999.top

[A01] Hello World
来源：http://odh.zdbjq.cn

Py:   print("Hello, World!")
来源：http://cfn.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://prm.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://qxz.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kjk.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://ubi.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://jln.havefunace.top

Ruby: puts "Hello, World!"
来源：http://oth.jlsjyb.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://glz.yj20258.top

[A02] 变量声明与赋值
来源：http://wbl.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dko.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xmt.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://klv.ctjpmb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://njr.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://voe.zhengqikj.top

Go:   name := "Alex"; age := 20
来源：http://bzs.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://bui.jqgfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://bfe.ehwqpu.com

[A03] 常量定义
来源：http://nbk.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dok.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://bvb.hcnkem.com

JS:   const PI = 3.14159;
来源：http://yui.zycfv.cn

TS:   const PI: number = 3.14159;
来源：http://toa.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://twk.tanke756.top

Go:   const PI = 3.14159
来源：http://zdl.52xcode.cn

Ruby: PI = 3.14159
来源：http://wtt.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://kaa.jqgufenzy.top

[A04] 判断变量类型
来源：http://nbh.0kj1m.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rva.fzhhl.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gjm.sjlbkw.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cnw.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://wxk.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://biu.svipenyu.cn


<!-- 参考信息 -->