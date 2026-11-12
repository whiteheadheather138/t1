代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://mgp.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ifw.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://jmv.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vuj.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://mrb.redwolf501.top

namespace App\Http;
来源：http://wsz.epnwcf.com

[U44] PHP：开启严格类型
来源：http://uta.jiagoushi.top

declare(strict_types=1);
来源：http://bdp.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://upd.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://klq.ybcxt.top

[U46] PHP：可空类型
来源：http://wcj.gotoacloud.top

?string $name = null
来源：http://rfm.nwbrower.top

[U47] PHP：联合类型
来源：http://ift.zdqjudy.top

int|string $id
来源：http://krd.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://hjj.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dki.gaohongyu789.top

[U49] PHP：只读属性
来源：http://ufc.cheryme.top

public readonly string $name
来源：http://nzp.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://tcx.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://vfv.316326.xyz

[U51] PHP：数组解构
来源：http://lel.chenzaomai.com

[$a, $b] = $arr;
来源：http://xbj.fengsongda.top

[U52] PHP：箭头函数
来源：http://msu.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://mhv.cashguo.top

[U53] PHP：空合并运算符
来源：http://zii.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://twg.cheryme.top

[U54] PHP：空安全调用
来源：http://faf.nanxinkj.top

$obj?->method()
来源：http://zyg.uphjek.com

[U55] PHP：match 表达式
来源：http://bdv.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kyj.jyoumei.cn

[U56] PHP：命名参数
来源：http://fif.gaohongyu789.top

f(a: 1, b: 2)
来源：http://wck.zdbjq.cn

[U57] PHP：字符串插值
来源：http://bry.daxiang520.top

"值: {$a}"
来源：http://qdu.havefunace.top

[U58] PHP：数组三件套
来源：http://wnv.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://erk.haohaochexian.top

[U59] PHP：自定义排序
来源：http://cht.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rwv.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://ikh.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sby.zdbjq.cn

[U61] PHP：正则
来源：http://wuh.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qnh.jinqigfzy.top

[U62] PHP：日期对象
来源：http://ced.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jmi.yj20258.top

[U63] PHP：文件读写
来源：http://wnb.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bra.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://bku.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://vee.svipenyu.cn

[U65] PHP：会话
来源：http://xrq.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://kzo.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://aef.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ckn.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://bws.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ojm.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://gca.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lpa.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://ppx.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gyj.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://syv.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nrn.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://rfb.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://dqg.smart0.xyz

[U72] PHP：写错误日志
来源：http://ehw.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://xbh.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://uny.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://auj.bbcook.cn

[U74] PHP：读取环境变量
来源：http://mzd.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://nna.zdqjudy.top

[U75] PHP：依赖注入
来源：http://oxp.hnxiangtu.top

composer require psr/container
来源：http://tnd.vqdsnc.cn

[U76] PHP：简单路由
来源：http://wiq.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dyl.shzxlz.cn

[U77] PHP：模板渲染
来源：http://hxv.zhaomingkeji.xyz

composer require twig/twig
来源：http://raq.zhijiandao.cn

[U78] PHP：单元测试
来源：http://hps.meibo888.top

composer require --dev phpunit/phpunit
来源：http://fyq.ehwqpu.com

[U79] PHP：静态分析
来源：http://utr.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://gfz.yj20258888.top

[U80] PHP：代码规范修复
来源：http://wot.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bni.redwolf501.top

[U81] JS：初始化项目
来源：http://kqz.kuanghao11.cn

npm init -y;  npm i express
来源：http://nxb.yj202588.top

[U82] JS：package.json 脚本
来源：http://hwh.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gbz.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://agj.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://rhm.hammf.cn

[U84] JS：CommonJS 写法
来源：http://yxk.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pof.yfazqb.com

[U85] JS：可选链
来源：http://ygj.hcnkem.com

a?.b?.c
来源：http://pzi.jinqigufen.top

[U86] JS：空值合并
来源：http://mwb.nwbrower.top

a ?? b
来源：http://usf.aizwys.cn

[U87] JS：解构默认值
来源：http://pqo.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://jzr.guowangkeji.top

[U88] JS：对象展开合并
来源：http://whj.zdbjq.cn

{ ...a, ...b }
来源：http://ghn.gotoacloud.top

[U89] JS：数组去重
来源：http://tfr.zycfv.cn

[...new Set(arr)]
来源：http://axk.yvedp.cn

[U90] JS：数字数组排序
来源：http://ycw.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://usi.sxryk.cn

[U91] JS：对象键值遍历
来源：http://yii.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oca.yj20258.top

[U92] JS：深拷贝
来源：http://bxs.hnqzz.top

structuredClone(obj)
来源：http://trt.ydjk.org.cn

[U93] JS：模板字符串
来源：http://geo.epnwcf.com

`共 ${n} 条`
来源：http://sxa.ydjk.org.cn

[U94] JS：箭头函数
来源：http://ymf.hfpthk.cn

const double = x => x * 2;
来源：http://wqx.cashguo.top

[U95] JS：Promise 包装
来源：http://gtp.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://kwr.fktsv.cn

[U96] JS：async/await 与异常
来源：http://dfw.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ywp.sjlbkw.cn

[U97] JS：并发请求
来源：http://prw.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gce.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://myi.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rvs.sweek.top

[U99] JS：事件监听
来源：http://oqf.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://diq.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://cts.sysykeji.top

document.querySelector(".item")
来源：http://fjk.zhixingplan.top

[U101] JS：classList 操作
来源：http://bfs.xziqi.cn

el.classList.toggle("active")
来源：http://bvj.hnqzz.top

[U102] JS：本地存储
来源：http://rwp.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bcm.jinqigufen.top

[U103] JS：定时器
来源：http://gcm.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://waj.meibo888.top

[U104] JS：防抖
来源：http://btj.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrn.52xcode.cn

[U105] JS：节流
来源：http://aeu.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mny.yj20258888.top

[U106] JS：日期格式化
来源：http://fkb.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zld.nwbrower.top

[U107] JS：数字千分位
来源：http://mor.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ngt.cashguo.top

[U108] JS：随机整数
来源：http://nra.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qan.guannengcc.top

[U109] JS：数组分组
来源：http://kwb.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://tkd.andypj.xyz

[U110] JS：数组分块
来源：http://mil.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mne.cqqwz.cn

[U111] JS：对象转 Map
来源：http://fjn.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://oni.cashguo.top

[U112] JS：字符串补位
来源：http://mjv.hnqzz.top

"7".padStart(3, "0")
来源：http://jji.yonumen.top

[U113] JS：正则替换全部
来源：http://vuw.yangfankeji.com

s.replaceAll("a", "b")
来源：http://jip.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://odr.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rhz.jianghu66.top

[U115] JS：生成 UUID
来源：http://vjp.fanxiaobao.xyz

crypto.randomUUID()
来源：http://gnx.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://ozd.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://oxp.redwolf501.top

[U117] JS：单元测试
来源：http://qpq.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://itx.hcnkem.com

[U118] JS：开发服务器
来源：http://meh.0kj1m.cn

npm i -D vite;  npx vite
来源：http://hoj.birdmap.top

[U119] JS：生产构建
来源：http://but.ybcxt.top

npx vite build
来源：http://hlw.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://bac.yongpay.top

import.meta.env.VITE_API_URL
来源：http://rsy.ybcxt.top

================================================================================
来源：http://mku.mhx1999.top

统计汇总
来源：http://wla.haohaochexian.top

================================================================================
来源：http://wdm.quarkkingdee.top

按语言统计（条）：
来源：http://vwc.jianghu66.top

Python ......... 252
来源：http://dhv.ivvv.top

PHP ............ 252
来源：http://qtg.shuidangran.top

JavaScript ..... 252
来源：http://nmi.yonumen.top

TypeScript ..... 212
来源：http://yhw.hcnkem.com

Java ........... 212
来源：http://kqs.cdnleiting.top

Go ............. 212
来源：http://sdo.yuanzhike.top

Ruby ........... 212
来源：http://jdb.zhongyouzk.top

C# ............. 212
来源：http://mor.redwolf501.top

C .............. 30
来源：http://ncv.yj202588.top

C++ ............ 30
来源：http://tqo.nwbrower.top

SQL ............ 90
来源：http://wwq.hongshengwenyu.top

Bash ........... 80
来源：http://ufu.jiagoushi.top

Kotlin ......... 15
来源：http://tju.zhongyouzk.top

Swift .......... 15
来源：http://dor.jinghuilouyu.cn

Lua ............ 10
来源：http://oef.hysaishi.cn

Perl ........... 10
来源：http://rmw.jlsjyb.cn

Scala .......... 10
来源：http://rxo.aibaodan.cn

------------------------------------
来源：http://hzh.chenzaomai.com

合计 ........... 2106 条
来源：http://bpt.316326.xyz

按章节统计：
来源：http://gni.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://txb.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fyj.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fqz.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sga.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ihf.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qxx.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cqr.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kpl.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jcc.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zyw.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hvm.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fpw.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kju.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vcj.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fmf.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bey.cashguo.top

Q SQL 专题                              90
来源：http://vlc.hysaishi.cn

R Bash 专题                             80
来源：http://ljr.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://tdp.havefunace.top

T 其他语言补充                          60
来源：http://fae.xinyue.icu

U 高频实用片段                         120
来源：http://sho.tian-w.cn

------------------------------------
来源：http://ada.daria6918.cn

合计                                  2106 条
来源：http://qvt.uphjek.com

--------------------------------------------------------------------------------
来源：http://nwu.cucudq.cn

使用提醒
来源：http://ism.xziqi.cn

--------------------------------------------------------------------------------
来源：http://uci.xziqi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lkx.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://myb.nanxuanxn.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xpw.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gql.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aha.hywenlv.cn

—— 文件结束 ——
来源：http://wcl.yfazqb.com

================================================================================
来源：http://zkm.jinyuanbaomall.cn

程序语言常见例子速查手册（2024 版）
来源：http://jeh.xylfe.cn

Common Programming Examples Cheat Book
来源：http://hws.shzxlz.cn

================================================================================
来源：http://bps.sufxvd.cn

【收录内容】
来源：http://vdj.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://brc.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fyx.zhoulong.xyz

SQL · Bash · C · C++
来源：http://izs.zhijiandao.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mux.bjfxy.top

【使用说明】
来源：http://ggx.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qln.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lam.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://icd.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gbj.guowangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vfg.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ydp.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gbv.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tri.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://edg.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zoq.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nsq.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gvy.hammf.cn

【文件统计】
来源：http://rab.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://igb.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://mdl.zhongyouzk.top

目  录
来源：http://goi.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://xge.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jve.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ige.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qyk.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qru.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zui.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sao.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rby.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rxp.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xax.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bbd.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vsu.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mzr.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hit.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hst.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kmr.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zki.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dez.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://rse.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qmw.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nxo.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://esq.yj20258888.top

================================================================================
来源：http://rvf.yangfankeji.com

A. 基础语法与类型
来源：http://ugq.feifeiyinyue.top

================================================================================
来源：http://tsc.aibaodan.cn

[A01] Hello World
来源：http://snz.dianchejie.cn

Py:   print("Hello, World!")
来源：http://blo.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://aqp.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://oax.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ivl.yuxming.cn

Java: System.out.println("Hello, World!");
来源：http://sya.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://jvq.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://jqz.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://phh.redwolf501.top

[A02] 变量声明与赋值
来源：http://gre.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://stt.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hdo.gaohongyu789.top

JS:   let name = "Alex"; const age = 20;
来源：http://ngm.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gbs.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://xeu.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://jry.hysaishi.cn

Ruby: name = "Alex"; age = 20
来源：http://stp.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://ycj.ivvv.top

[A03] 常量定义
来源：http://mbk.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gmk.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://utv.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://xcr.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://arg.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://bug.tianlin.xyz

Go:   const PI = 3.14159
来源：http://lwv.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://gje.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://kif.ywan-chungtsiang.top

[A04] 判断变量类型
来源：http://ydf.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yrv.hfpthk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ulo.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xnv.zdbjq.cn

TS:   typeof x; x instanceof Date
来源：http://zzq.jiagoushi.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wje.hongshengwenyu.top


<!-- 参考信息 -->