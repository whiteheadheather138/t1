代发 wailian999

[U37] Py：读写 Excel
来源：http://tbo.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://mwh.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://hvj.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://qct.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://vtu.xinyue.icu

sys.stdout.isatty()
来源：http://vbg.316326.xyz

[U40] Py：打印到标准错误
来源：http://gka.yueranfly.top

print("err", file=sys.stderr)
来源：http://twy.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://lpb.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tef.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://smk.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gjv.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://txj.jinyuanbaomall.cn

namespace App\Http;
来源：http://zmz.nwbrower.top

[U44] PHP：开启严格类型
来源：http://rvm.andypj.xyz

declare(strict_types=1);
来源：http://osx.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://tqg.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ntr.redwolf501.top

[U46] PHP：可空类型
来源：http://smq.9152youxi.cn

?string $name = null
来源：http://cpu.shuidangran.top

[U47] PHP：联合类型
来源：http://dld.bjfxy.top

int|string $id
来源：http://zxn.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://axo.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gin.jinqigfzy.top

[U49] PHP：只读属性
来源：http://fer.fktsv.cn

public readonly string $name
来源：http://oaa.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://xxz.tanke756.top

public function __construct(private int $id) {}
来源：http://qcs.xylfe.cn

[U51] PHP：数组解构
来源：http://fyr.meibo888.top

[$a, $b] = $arr;
来源：http://fym.tianlin.xyz

[U52] PHP：箭头函数
来源：http://ntc.meibo888.top

$double = fn($x) => $x * 2;
来源：http://jpj.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://ccz.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://ltd.daxiang520.top

[U54] PHP：空安全调用
来源：http://ijr.xinyue.icu

$obj?->method()
来源：http://yeq.yongpay.top

[U55] PHP：match 表达式
来源：http://tfw.zhengqikj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xnf.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://iwv.birdmap.top

f(a: 1, b: 2)
来源：http://hfl.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://phd.fengsongda.top

"值: {$a}"
来源：http://zxs.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://wck.ydjk.org.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wup.tarul.cn

[U59] PHP：自定义排序
来源：http://fzi.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jds.yonumen.top

[U60] PHP：JSON 编解码
来源：http://tqy.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ced.yueranfly.top

[U61] PHP：正则
来源：http://ebf.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ijs.birdmap.top

[U62] PHP：日期对象
来源：http://xuz.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jsx.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://aai.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ykk.dashuyun.cn

[U64] PHP：目录遍历
来源：http://qrh.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://nlf.hnqzz.top

[U65] PHP：会话
来源：http://uya.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://lsx.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://agc.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mue.bjfxy.top

[U67] PHP：处理文件上传
来源：http://fga.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://coh.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://vfl.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sbp.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://jeo.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ped.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://ekc.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jif.xuanzx.com

[U71] PHP：抛出异常
来源：http://tia.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://tcr.nwbrower.top

[U72] PHP：写错误日志
来源：http://jqz.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://bel.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://xbm.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://rft.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://yay.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://wgo.meibo888.top

[U75] PHP：依赖注入
来源：http://vpt.jiagoushi.top

composer require psr/container
来源：http://xmf.jinqigufen.top

[U76] PHP：简单路由
来源：http://pky.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://msx.andypj.xyz

[U77] PHP：模板渲染
来源：http://jcm.tanke756.top

composer require twig/twig
来源：http://tbh.hfpthk.cn

[U78] PHP：单元测试
来源：http://xbq.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://wgr.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://wri.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://uhp.guannengcc.top

[U80] PHP：代码规范修复
来源：http://rzz.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ffs.andypj.xyz

[U81] JS：初始化项目
来源：http://kzn.zhoulong.xyz

npm init -y;  npm i express
来源：http://vcu.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://lty.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cox.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://jzr.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://iwt.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://egj.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://zyt.snrcjt.cn

[U85] JS：可选链
来源：http://dcx.cheryme.top

a?.b?.c
来源：http://lsd.quarkkingdee.top

[U86] JS：空值合并
来源：http://iju.yongpay.top

a ?? b
来源：http://fhz.wangdashe.top

[U87] JS：解构默认值
来源：http://man.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://ngd.9152youxi.cn

[U88] JS：对象展开合并
来源：http://apz.shanyushiyangtech.top

{ ...a, ...b }
来源：http://bka.dianchejie.cn

[U89] JS：数组去重
来源：http://xqq.ydjk.org.cn

[...new Set(arr)]
来源：http://nlv.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://hvz.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://xzq.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://eej.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ztz.cucudq.cn

[U92] JS：深拷贝
来源：http://ejq.yj20258.top

structuredClone(obj)
来源：http://hty.redwolf501.top

[U93] JS：模板字符串
来源：http://eww.smart0.xyz

`共 ${n} 条`
来源：http://ybr.jianghu66.top

[U94] JS：箭头函数
来源：http://mvf.chenjidiqi.icu

const double = x => x * 2;
来源：http://yzu.xziqi.cn

[U95] JS：Promise 包装
来源：http://bip.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://jfa.cheryme.top

[U96] JS：async/await 与异常
来源：http://yhs.jinqigufen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rvh.sysykeji.top

[U97] JS：并发请求
来源：http://kru.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gmx.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://mbx.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vut.ctjpmb.com

[U99] JS：事件监听
来源：http://bmi.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://ypq.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://can.ehwqpu.com

document.querySelector(".item")
来源：http://yox.yangfankeji.com

[U101] JS：classList 操作
来源：http://vqh.guowangkeji.top

el.classList.toggle("active")
来源：http://win.chenzaomai.com

[U102] JS：本地存储
来源：http://ffi.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ppu.52xcode.cn

[U103] JS：定时器
来源：http://yzu.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://onv.zdbjq.cn

[U104] JS：防抖
来源：http://urn.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lkt.jqgfzy.top

[U105] JS：节流
来源：http://qgm.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sdt.birdmap.top

[U106] JS：日期格式化
来源：http://apd.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yyv.yj20258888.top

[U107] JS：数字千分位
来源：http://ger.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kab.jianghu66.top

[U108] JS：随机整数
来源：http://ibt.ydjk.org.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ifn.tarul.cn

[U109] JS：数组分组
来源：http://nlc.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://wnp.kuanghao11.cn

[U110] JS：数组分块
来源：http://lwu.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vsr.aibaodan.cn

[U111] JS：对象转 Map
来源：http://zff.shuidangran.top

new Map(Object.entries(obj))
来源：http://kpc.cucudq.cn

[U112] JS：字符串补位
来源：http://ixg.nwbrower.top

"7".padStart(3, "0")
来源：http://sne.shuidangran.top

[U113] JS：正则替换全部
来源：http://bei.gotoacloud.top

s.replaceAll("a", "b")
来源：http://krw.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://jet.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kgz.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://cmi.hnqzz.top

crypto.randomUUID()
来源：http://zcf.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://agq.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://mlk.hnqzz.top

[U117] JS：单元测试
来源：http://uzx.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://mej.yongpay.top

[U118] JS：开发服务器
来源：http://zpv.nwbrower.top

npm i -D vite;  npx vite
来源：http://fep.cashguo.top

[U119] JS：生产构建
来源：http://jxp.guowangkeji.top

npx vite build
来源：http://oxf.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://dne.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://hoj.gogol.net.cn

================================================================================
来源：http://sft.jqgufenzy.top

统计汇总
来源：http://mzr.316326.xyz

================================================================================
来源：http://osb.jqgfzy.top

按语言统计（条）：
来源：http://fhb.nwbrower.top

Python ......... 252
来源：http://wfr.gogol.net.cn

PHP ............ 252
来源：http://fws.yuanzhike.top

JavaScript ..... 252
来源：http://loe.zdqjudy.top

TypeScript ..... 212
来源：http://vdf.hongshengwenyu.top

Java ........... 212
来源：http://ehd.zhiwuduotai.top

Go ............. 212
来源：http://ewp.havefunace.top

Ruby ........... 212
来源：http://jvl.yvedp.cn

C# ............. 212
来源：http://vyw.hnxiangtu.top

C .............. 30
来源：http://jfx.yonumen.top

C++ ............ 30
来源：http://oon.hammf.cn

SQL ............ 90
来源：http://qcw.havefunace.top

Bash ........... 80
来源：http://hsz.yfazqb.com

Kotlin ......... 15
来源：http://txz.yueranfly.top

Swift .......... 15
来源：http://gpc.epnwcf.com

Lua ............ 10
来源：http://sve.zhijiandao.cn

Perl ........... 10
来源：http://lcf.ehwqpu.com

Scala .......... 10
来源：http://zxv.hesvh.cn

------------------------------------
来源：http://knb.hammf.cn

合计 ........... 2106 条
来源：http://qnq.zhoulong.xyz

按章节统计：
来源：http://dbi.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zaq.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aui.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qcw.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://shn.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ivr.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://obv.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://opw.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wxe.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hrb.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://foh.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yko.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zct.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rgq.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iez.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xop.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://exl.sweek.top

Q SQL 专题                              90
来源：http://pcp.sufxvd.cn

R Bash 专题                             80
来源：http://ecp.52xcode.cn

S C / C++ 专题                          60
来源：http://ixy.ydjk.org.cn

T 其他语言补充                          60
来源：http://xxs.daria6918.cn

U 高频实用片段                         120
来源：http://afc.ehwqpu.com

------------------------------------
来源：http://tuk.ydzc1.top

合计                                  2106 条
来源：http://adb.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://xpe.nanxinkj.top

使用提醒
来源：http://kjo.yongpay.top

--------------------------------------------------------------------------------
来源：http://uli.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzs.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xan.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xyt.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xgk.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vig.yj20258.top

—— 文件结束 ——
来源：http://apb.epnwcf.com

================================================================================
来源：http://fdd.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://ebh.fzhhl.top

Common Programming Examples Cheat Book
来源：http://stc.svipenyu.cn

================================================================================
来源：http://frn.haohaochexian.top

【收录内容】
来源：http://ycn.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mlw.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ofi.shuidangran.top

SQL · Bash · C · C++
来源：http://wdk.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hhw.xuanzx.com

【使用说明】
来源：http://kah.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uov.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lex.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mke.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hcy.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mas.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://udz.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jmx.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xbf.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://auo.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xyw.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dyh.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hvh.meibo888.top

【文件统计】
来源：http://wll.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vyn.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://lsu.yangfankeji.com

目  录
来源：http://fsk.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://imk.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://caa.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dql.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tuv.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fic.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dlw.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bkj.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zup.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kcx.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dso.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cuv.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ouz.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hxm.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ykc.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dwv.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://voc.zhengqikj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iyr.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://som.316326.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://rji.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uut.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dua.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://njo.hnxiangtu.top

================================================================================
来源：http://qwg.yj202588.top

A. 基础语法与类型
来源：http://ohm.bjfxy.top

================================================================================
来源：http://rtw.ivvv.top

[A01] Hello World
来源：http://ycb.andypj.xyz

Py:   print("Hello, World!")
来源：http://bkg.316326.xyz

PHP:  echo "Hello, World!";
来源：http://mvo.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://pnj.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zru.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://byk.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://dvj.svipenyu.cn

Ruby: puts "Hello, World!"
来源：http://sit.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dth.ivvv.top

[A02] 变量声明与赋值
来源：http://fkm.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rlq.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xpa.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://ijr.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tui.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://yyd.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://kcu.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://vac.birdmap.top

C#:   string name = "Alex"; int age = 20;
来源：http://csq.zdbjq.cn

[A03] 常量定义
来源：http://yve.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ukk.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://uxb.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://fxh.jlsjyb.cn

TS:   const PI: number = 3.14159;
来源：http://vtl.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://qdx.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://bbr.zdqjudy.top


<!-- 参考信息 -->