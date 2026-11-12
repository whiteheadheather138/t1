代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://mnf.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://awh.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://rpo.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://saj.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://nvs.ydzc1.top

namespace App\Http;
来源：http://roh.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://ofj.zdbjq.cn

declare(strict_types=1);
来源：http://cnd.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://cfi.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hnh.uphjek.com

[U46] PHP：可空类型
来源：http://qmg.redwolf501.top

?string $name = null
来源：http://mvr.ppjwa.cn

[U47] PHP：联合类型
来源：http://acq.kuanghao11.cn

int|string $id
来源：http://bvs.smart0.xyz

[U48] PHP：纯枚举
来源：http://ofl.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rbo.zhongyouzk.top

[U49] PHP：只读属性
来源：http://pqx.zdqjudy.top

public readonly string $name
来源：http://kvp.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://cjo.cdnleiting.top

public function __construct(private int $id) {}
来源：http://vzd.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://nzv.ivvv.top

[$a, $b] = $arr;
来源：http://faj.hywenlv.cn

[U52] PHP：箭头函数
来源：http://pbz.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://tpn.guannengcc.top

[U53] PHP：空合并运算符
来源：http://etm.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://nwp.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://nad.hywenlv.cn

$obj?->method()
来源：http://pri.ybcxt.top

[U55] PHP：match 表达式
来源：http://scs.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ari.shzxlz.cn

[U56] PHP：命名参数
来源：http://tpg.zhongyouzk.top

f(a: 1, b: 2)
来源：http://xsx.yfazqb.com

[U57] PHP：字符串插值
来源：http://lle.andypj.xyz

"值: {$a}"
来源：http://onp.birdmap.top

[U58] PHP：数组三件套
来源：http://esf.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rbz.svipenyu.cn

[U59] PHP：自定义排序
来源：http://nnp.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mdv.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://ktq.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://chn.yuanzhike.top

[U61] PHP：正则
来源：http://lzb.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fwu.aibaodan.cn

[U62] PHP：日期对象
来源：http://khn.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://owp.yueranfly.top

[U63] PHP：文件读写
来源：http://exd.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nuz.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://lyl.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://scz.ivvv.top

[U65] PHP：会话
来源：http://prj.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yfd.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://djp.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rbj.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://lxa.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gfm.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://aux.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lxm.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://omk.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uox.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://ebk.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bpi.iojbl.cn

[U71] PHP：抛出异常
来源：http://wko.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://uqd.svipenyu.cn

[U72] PHP：写错误日志
来源：http://jhw.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://vsd.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://ygy.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://zgg.c1oappe.top

[U74] PHP：读取环境变量
来源：http://ank.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://vde.c1oappe.top

[U75] PHP：依赖注入
来源：http://aaf.tianlin.xyz

composer require psr/container
来源：http://tja.sxryk.cn

[U76] PHP：简单路由
来源：http://cnf.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zue.zhixingplan.top

[U77] PHP：模板渲染
来源：http://brp.fehbvm.com

composer require twig/twig
来源：http://ipa.havefunace.top

[U78] PHP：单元测试
来源：http://cga.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://fmx.sjlbkw.cn

[U79] PHP：静态分析
来源：http://sur.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://did.gzhubu.top

[U80] PHP：代码规范修复
来源：http://pzj.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hsl.sweek.top

[U81] JS：初始化项目
来源：http://ibs.feifeiyinyue.top

npm init -y;  npm i express
来源：http://cin.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://rvb.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bhz.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://zun.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://orq.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://tdc.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://vrt.havefunace.top

[U85] JS：可选链
来源：http://jwj.cashguo.top

a?.b?.c
来源：http://tie.hesvh.cn

[U86] JS：空值合并
来源：http://hrr.zdbjq.cn

a ?? b
来源：http://fly.sweek.top

[U87] JS：解构默认值
来源：http://bmj.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://icq.cucudq.cn

[U88] JS：对象展开合并
来源：http://itb.yonumen.top

{ ...a, ...b }
来源：http://hkq.yongpay.top

[U89] JS：数组去重
来源：http://ryo.zhijiandao.cn

[...new Set(arr)]
来源：http://did.zhengqikj.top

[U90] JS：数字数组排序
来源：http://qar.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://hgx.ybcxt.top

[U91] JS：对象键值遍历
来源：http://veo.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rxl.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://wlg.jiagoushi.top

structuredClone(obj)
来源：http://chu.hcnkem.com

[U93] JS：模板字符串
来源：http://dfp.ppjwa.cn

`共 ${n} 条`
来源：http://otk.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://bwe.jinqigfzy.top

const double = x => x * 2;
来源：http://wkf.tian-w.cn

[U95] JS：Promise 包装
来源：http://sql.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://bvo.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://pyt.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zar.yuxming.cn

[U97] JS：并发请求
来源：http://vcu.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hjr.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://dli.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dmt.meibo888.top

[U99] JS：事件监听
来源：http://guk.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://gmk.aizwys.cn

[U100] JS：DOM 查询
来源：http://pnp.yueranfly.top

document.querySelector(".item")
来源：http://dmm.fengsongda.top

[U101] JS：classList 操作
来源：http://qol.bjfxy.top

el.classList.toggle("active")
来源：http://tdv.cqqwz.cn

[U102] JS：本地存储
来源：http://ucx.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://gen.zhijiandao.cn

[U103] JS：定时器
来源：http://uwr.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fhc.hongshengwenyu.top

[U104] JS：防抖
来源：http://xwk.andypj.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zcv.ybcxt.top

[U105] JS：节流
来源：http://nrq.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wmi.0kj1m.cn

[U106] JS：日期格式化
来源：http://hcp.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xxp.sweek.top

[U107] JS：数字千分位
来源：http://mnk.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lsk.jqgfzy.top

[U108] JS：随机整数
来源：http://eqf.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://raw.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://urf.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://zah.fzhhl.top

[U110] JS：数组分块
来源：http://kmy.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yog.c1oappe.top

[U111] JS：对象转 Map
来源：http://yxz.aibaodan.cn

new Map(Object.entries(obj))
来源：http://fgl.tanke756.top

[U112] JS：字符串补位
来源：http://pmm.smart0.xyz

"7".padStart(3, "0")
来源：http://lud.fzhhl.top

[U113] JS：正则替换全部
来源：http://hwi.yonumen.top

s.replaceAll("a", "b")
来源：http://bzp.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://pkr.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oxu.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://psl.yanxiufei.cn

crypto.randomUUID()
来源：http://eui.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://xky.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://ywa.aizwys.cn

[U117] JS：单元测试
来源：http://otb.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://esy.xuanzx.com

[U118] JS：开发服务器
来源：http://lbw.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://fmt.yueranfly.top

[U119] JS：生产构建
来源：http://bnz.snrcjt.cn

npx vite build
来源：http://yne.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://mdj.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://qwe.guannengcc.top

================================================================================
来源：http://cno.tianlin.xyz

统计汇总
来源：http://mbb.sxryk.cn

================================================================================
来源：http://sxk.havefunace.top

按语言统计（条）：
来源：http://rgx.dashuyun.cn

Python ......... 252
来源：http://bdz.tarul.cn

PHP ............ 252
来源：http://zsb.zhoulong.xyz

JavaScript ..... 252
来源：http://wip.xylfe.cn

TypeScript ..... 212
来源：http://cnu.chenjidiqi.icu

Java ........... 212
来源：http://wkl.hywenlv.cn

Go ............. 212
来源：http://nqn.yangfankeji.com

Ruby ........... 212
来源：http://bxn.jlsjyb.cn

C# ............. 212
来源：http://ynd.mhx1999.top

C .............. 30
来源：http://ffq.yj20258888.top

C++ ............ 30
来源：http://gce.xinyue.icu

SQL ............ 90
来源：http://bul.xuanzx.com

Bash ........... 80
来源：http://epc.birdmap.top

Kotlin ......... 15
来源：http://uqr.chenjidiqi.icu

Swift .......... 15
来源：http://xzf.hnxiangtu.top

Lua ............ 10
来源：http://syk.mhx1999.top

Perl ........... 10
来源：http://obf.yfazqb.com

Scala .......... 10
来源：http://lhw.chenjidiqi.icu

------------------------------------
来源：http://fij.fengsongda.top

合计 ........... 2106 条
来源：http://oyv.cqqwz.cn

按章节统计：
来源：http://rpl.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lno.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hdw.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xrd.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yoo.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cxp.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ywb.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://plb.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ajj.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blm.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://evc.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://woh.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dxg.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rxw.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zfd.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ugl.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ucf.tanke756.top

Q SQL 专题                              90
来源：http://xzf.jlsjyb.cn

R Bash 专题                             80
来源：http://ddy.chenzaomai.com

S C / C++ 专题                          60
来源：http://axa.chenzaomai.com

T 其他语言补充                          60
来源：http://bkx.xziqi.cn

U 高频实用片段                         120
来源：http://nmv.zhengqikj.top

------------------------------------
来源：http://mtt.hongshengwenyu.top

合计                                  2106 条
来源：http://ggd.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://mkz.ehwqpu.com

使用提醒
来源：http://frn.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://gyk.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nrz.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://htu.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://obi.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mwt.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ajm.c1oappe.top

—— 文件结束 ——
来源：http://aog.cdnleiting.top

================================================================================
来源：http://qtg.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://nwy.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://fad.chenjidiqi.icu

================================================================================
来源：http://peg.redwolf501.top

【收录内容】
来源：http://ofx.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://wpj.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hiw.haohaochexian.top

SQL · Bash · C · C++
来源：http://foi.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tsl.yvedp.cn

【使用说明】
来源：http://njq.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yqv.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dyp.xziqi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lhq.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zmm.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rtx.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hva.zhoulong.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nwt.dashuyun.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bcr.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ool.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://klz.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bry.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kpr.zdqjudy.top

【文件统计】
来源：http://vaz.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://odc.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://ovf.shangyingyoupin.top

目  录
来源：http://hkp.uphjek.com

--------------------------------------------------------------------------------
来源：http://oru.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hjy.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dbz.dashuyun.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rdq.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ibv.zycfv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wwk.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fer.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eer.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ina.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://otq.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hma.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iyd.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hov.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://knr.chenzaomai.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oky.andypj.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tjh.vehdjk.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pcl.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kti.cheryme.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fit.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bkh.hammf.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kxk.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fxd.smart0.xyz

================================================================================
来源：http://osu.zhengqikj.top

A. 基础语法与类型
来源：http://wqs.yonumen.top

================================================================================
来源：http://dza.ybcxt.top

[A01] Hello World
来源：http://ieq.jyoumei.cn

Py:   print("Hello, World!")
来源：http://uvk.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://cha.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://efn.ppjwa.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lcd.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://ikf.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://vvg.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://vkr.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zdj.yuxming.cn

[A02] 变量声明与赋值
来源：http://yud.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aat.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://azv.aibaodan.cn

JS:   let name = "Alex"; const age = 20;
来源：http://asx.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fox.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://zgp.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://sri.yonumen.top

Ruby: name = "Alex"; age = 20
来源：http://cpe.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://rby.quarkkingdee.top

[A03] 常量定义
来源：http://gki.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hia.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://dqc.vehdjk.com

JS:   const PI = 3.14159;
来源：http://rxt.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://txh.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://hpu.xylfe.cn

Go:   const PI = 3.14159
来源：http://oik.ivvv.top

Ruby: PI = 3.14159
来源：http://kfg.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://lbf.snrcjt.cn

[A04] 判断变量类型
来源：http://vgi.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hhn.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kjl.shuidangran.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bcx.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://yyv.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gsp.yueranfly.top


<!-- 参考信息 -->