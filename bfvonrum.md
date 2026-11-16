代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://iqz.svipenyu.cn

sys.stdout.isatty()
来源：http://slg.yuxming.cn

[U40] Py：打印到标准错误
来源：http://pxt.hesvh.cn

print("err", file=sys.stderr)
来源：http://nvg.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://mys.vehdjk.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jbx.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://yjh.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zel.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://zxn.hesvh.cn

namespace App\Http;
来源：http://mmo.bjfxy.top

[U44] PHP：开启严格类型
来源：http://yss.chenjidiqi.icu

declare(strict_types=1);
来源：http://zoo.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://biq.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nwr.yj20258888.top

[U46] PHP：可空类型
来源：http://sph.chenlongwang.top

?string $name = null
来源：http://qii.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://ycn.jinqigufen.top

int|string $id
来源：http://oxg.birdmap.top

[U48] PHP：纯枚举
来源：http://ayr.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rdj.vehdjk.com

[U49] PHP：只读属性
来源：http://toh.birdmap.top

public readonly string $name
来源：http://spw.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://olq.xuanzx.com

public function __construct(private int $id) {}
来源：http://mix.zdbjq.cn

[U51] PHP：数组解构
来源：http://xpx.jinqigufen.top

[$a, $b] = $arr;
来源：http://bra.tanke756.top

[U52] PHP：箭头函数
来源：http://jis.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://lkg.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://ygw.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://dwr.hywenlv.cn

[U54] PHP：空安全调用
来源：http://tlq.quarkkingdee.top

$obj?->method()
来源：http://ygc.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://xpo.kuanghao11.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://edp.ydjk.org.cn

[U56] PHP：命名参数
来源：http://rhr.jlsjyb.cn

f(a: 1, b: 2)
来源：http://axy.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://qtt.xingfuxueyuan.xyz

"值: {$a}"
来源：http://kub.xziqi.cn

[U58] PHP：数组三件套
来源：http://jkz.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bcc.yongpay.top

[U59] PHP：自定义排序
来源：http://gzl.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cnj.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://nsn.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uba.gaohongyu789.top

[U61] PHP：正则
来源：http://cuy.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yps.yongpay.top

[U62] PHP：日期对象
来源：http://yeo.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nla.hnqzz.top

[U63] PHP：文件读写
来源：http://ago.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nez.9152youxi.cn

[U64] PHP：目录遍历
来源：http://tpc.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://flt.shangyingyoupin.top

[U65] PHP：会话
来源：http://wfc.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://eaw.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://nhz.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zla.nwbrower.top

[U67] PHP：处理文件上传
来源：http://saq.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://npu.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://xoo.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ldl.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://kvj.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zxx.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://cbd.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jfc.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://zlq.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://ehf.mhx1999.top

[U72] PHP：写错误日志
来源：http://dph.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://cym.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://nfe.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://rqs.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://dak.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://qpt.yuxming.cn

[U75] PHP：依赖注入
来源：http://ube.uphjek.com

composer require psr/container
来源：http://qtv.cheryme.top

[U76] PHP：简单路由
来源：http://rts.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bph.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://wdt.ydjk.org.cn

composer require twig/twig
来源：http://mpg.sweek.top

[U78] PHP：单元测试
来源：http://jup.uphjek.com

composer require --dev phpunit/phpunit
来源：http://xjn.vehdjk.com

[U79] PHP：静态分析
来源：http://tbt.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://hby.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://rjf.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qgf.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://mqg.yanxiufei.cn

npm init -y;  npm i express
来源：http://gxe.birdmap.top

[U82] JS：package.json 脚本
来源：http://hfw.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yym.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://tif.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://qod.uphjek.com

[U84] JS：CommonJS 写法
来源：http://tko.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rsd.ybcxt.top

[U85] JS：可选链
来源：http://iua.yonumen.top

a?.b?.c
来源：http://edr.yj20258.top

[U86] JS：空值合并
来源：http://ale.snrcjt.cn

a ?? b
来源：http://mra.cdnleiting.top

[U87] JS：解构默认值
来源：http://xxn.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://ifu.yueranfly.top

[U88] JS：对象展开合并
来源：http://uub.shzxlz.cn

{ ...a, ...b }
来源：http://ucv.fzhhl.top

[U89] JS：数组去重
来源：http://mmf.cheryme.top

[...new Set(arr)]
来源：http://wnp.0kj1m.cn

[U90] JS：数字数组排序
来源：http://qmq.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://grv.redwolf501.top

[U91] JS：对象键值遍历
来源：http://fxz.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lgm.zhoulong.xyz

[U92] JS：深拷贝
来源：http://hrk.zhongyouzk.top

structuredClone(obj)
来源：http://kyp.52xcode.cn

[U93] JS：模板字符串
来源：http://bsd.jyoumei.cn

`共 ${n} 条`
来源：http://vid.jinqigfzy.top

[U94] JS：箭头函数
来源：http://vtn.hywenlv.cn

const double = x => x * 2;
来源：http://hfu.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://bfy.jqgufenzy.top

new Promise((resolve, reject) => {})
来源：http://lhe.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://xkw.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oly.zycfv.cn

[U97] JS：并发请求
来源：http://rfa.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zjc.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://idy.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dox.daxiang520.top

[U99] JS：事件监听
来源：http://xqq.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://amm.nanxinkj.top

[U100] JS：DOM 查询
来源：http://xhq.kuanghao11.cn

document.querySelector(".item")
来源：http://xrz.epnwcf.com

[U101] JS：classList 操作
来源：http://ilv.jinqigufen.top

el.classList.toggle("active")
来源：http://wuh.quarkkingdee.top

[U102] JS：本地存储
来源：http://kvw.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iuw.dianchejie.cn

[U103] JS：定时器
来源：http://tpx.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ufw.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://abd.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://izi.hammf.cn

[U105] JS：节流
来源：http://djp.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jeh.hnxiangtu.top

[U106] JS：日期格式化
来源：http://lal.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lzf.svipenyu.cn

[U107] JS：数字千分位
来源：http://ldt.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nwi.fzhhl.top

[U108] JS：随机整数
来源：http://dkx.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nhn.haohaochexian.top

[U109] JS：数组分组
来源：http://roe.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://zir.svipenyu.cn

[U110] JS：数组分块
来源：http://eef.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vvf.tianlin.xyz

[U111] JS：对象转 Map
来源：http://fbk.hcnkem.com

new Map(Object.entries(obj))
来源：http://sgq.tarul.cn

[U112] JS：字符串补位
来源：http://ugp.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://bkt.tianlin.xyz

[U113] JS：正则替换全部
来源：http://mgf.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://pxk.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://auo.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ozn.bjfxy.top

[U115] JS：生成 UUID
来源：http://ulo.fzhhl.top

crypto.randomUUID()
来源：http://hfk.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://bvo.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://dcj.yonumen.top

[U117] JS：单元测试
来源：http://mvp.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://orx.havefunace.top

[U118] JS：开发服务器
来源：http://ann.guannengcc.top

npm i -D vite;  npx vite
来源：http://fpo.yuanzhike.top

[U119] JS：生产构建
来源：http://ote.daxiang520.top

npx vite build
来源：http://ani.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://wts.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://qhw.ctjpmb.com

================================================================================
来源：http://xjq.hesvh.cn

统计汇总
来源：http://omj.daxiang520.top

================================================================================
来源：http://kbc.cdnleiting.top

按语言统计（条）：
来源：http://uan.zhengqikj.top

Python ......... 252
来源：http://gsc.sweek.top

PHP ............ 252
来源：http://bjx.fzhhl.top

JavaScript ..... 252
来源：http://zur.gogol.net.cn

TypeScript ..... 212
来源：http://acd.jinghuilouyu.cn

Java ........... 212
来源：http://rdi.jqgufenzy.top

Go ............. 212
来源：http://tuy.chenjidiqi.icu

Ruby ........... 212
来源：http://swd.gotoacloud.top

C# ............. 212
来源：http://cjg.daxiang520.top

C .............. 30
来源：http://cka.yvedp.cn

C++ ............ 30
来源：http://azg.haohaochexian.top

SQL ............ 90
来源：http://nkj.quarkkingdee.top

Bash ........... 80
来源：http://ico.havefunace.top

Kotlin ......... 15
来源：http://rdi.sxryk.cn

Swift .......... 15
来源：http://atb.yueranfly.top

Lua ............ 10
来源：http://zll.zhixingplan.top

Perl ........... 10
来源：http://ysz.yj202588.top

Scala .......... 10
来源：http://tfa.yonumen.top

------------------------------------
来源：http://tmi.zdbjq.cn

合计 ........... 2106 条
来源：http://yxd.52xcode.cn

按章节统计：
来源：http://bbk.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oja.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rmo.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pvp.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://byk.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vjp.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qja.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://upz.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zmu.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fuv.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yqz.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://emk.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rgf.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bka.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zrd.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uts.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qft.quarkkingdee.top

Q SQL 专题                              90
来源：http://enm.yonumen.top

R Bash 专题                             80
来源：http://vdl.haohaochexian.top

S C / C++ 专题                          60
来源：http://zfd.fktsv.cn

T 其他语言补充                          60
来源：http://fku.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://aiw.vehdjk.com

------------------------------------
来源：http://pus.jinyuanbaomall.cn

合计                                  2106 条
来源：http://bcp.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://umi.kuanghao11.cn

使用提醒
来源：http://tox.316326.xyz

--------------------------------------------------------------------------------
来源：http://wdl.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mjb.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://phs.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gcz.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ggc.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fqu.guowangkeji.top

—— 文件结束 ——
来源：http://lbx.fengsongda.top

================================================================================
来源：http://sex.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://fwd.jinqigufen.top

Common Programming Examples Cheat Book
来源：http://foy.jinqigfzy.top

================================================================================
来源：http://dst.jqgufenzy.top

【收录内容】
来源：http://suc.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sqr.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ere.jqgfzy.top

SQL · Bash · C · C++
来源：http://nai.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://efc.aizwys.cn

【使用说明】
来源：http://wbc.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lhg.pengpengdd.cyou

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kca.chenzaomai.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ecd.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://szo.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eoc.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ivx.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bjn.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pgb.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eka.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tvh.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hov.gzhubu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xeq.shuidangran.top

【文件统计】
来源：http://svs.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://swh.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://xzh.zdbjq.cn

目  录
来源：http://jin.jianghu66.top

--------------------------------------------------------------------------------
来源：http://smb.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ujy.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hup.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://har.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dza.vqdsnc.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bqj.yanxiufei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vlw.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cuz.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iut.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xne.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hna.yvedp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wyq.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uwf.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uwz.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fmu.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gug.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ujd.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gzq.yvedp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jqs.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xsb.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pew.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ens.jyoumei.cn

================================================================================
来源：http://jzz.jinghuilouyu.cn

A. 基础语法与类型
来源：http://bmc.epnwcf.com

================================================================================
来源：http://hpb.yj20258.top

[A01] Hello World
来源：http://ecp.ehwqpu.com

Py:   print("Hello, World!")
来源：http://pcf.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://orn.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://nvy.xinyue.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cle.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://msz.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://zhw.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://ncm.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vwm.jianghu66.top

[A02] 变量声明与赋值
来源：http://lgv.jianghu66.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yzx.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://khm.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cdk.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dza.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://sej.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://jef.uphjek.com

Ruby: name = "Alex"; age = 20
来源：http://dna.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bvo.0kj1m.cn

[A03] 常量定义
来源：http://zkb.52xcode.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hjy.tarul.cn

PHP:  const PI = 3.14159;
来源：http://gnk.fzhhl.top

JS:   const PI = 3.14159;
来源：http://jpe.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://vcg.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://sfc.ppjwa.cn

Go:   const PI = 3.14159
来源：http://wtj.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://qdd.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://rdr.zhoulong.xyz

[A04] 判断变量类型
来源：http://vaf.tarul.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xtu.xingfuxueyuan.xyz


<!-- 参考信息 -->