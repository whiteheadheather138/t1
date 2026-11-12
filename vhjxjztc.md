代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hxw.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://yer.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://eut.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dzl.yueranfly.top

[U43] PHP：声明命名空间
来源：http://tgp.pengpengdd.cyou

namespace App\Http;
来源：http://pdp.uphjek.com

[U44] PHP：开启严格类型
来源：http://xrf.jqgfzy.top

declare(strict_types=1);
来源：http://frk.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://vie.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cja.9152youxi.cn

[U46] PHP：可空类型
来源：http://yke.ppjwa.cn

?string $name = null
来源：http://hcn.jiagoushi.top

[U47] PHP：联合类型
来源：http://rrm.jqgfzy.top

int|string $id
来源：http://fjb.svipenyu.cn

[U48] PHP：纯枚举
来源：http://luy.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ari.nanxinkj.top

[U49] PHP：只读属性
来源：http://for.yangfankeji.com

public readonly string $name
来源：http://atp.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://epm.chenzaomai.com

public function __construct(private int $id) {}
来源：http://xlo.yuanzhike.top

[U51] PHP：数组解构
来源：http://cox.tian-w.cn

[$a, $b] = $arr;
来源：http://scq.nanxinkj.top

[U52] PHP：箭头函数
来源：http://rll.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://ovr.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://lix.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://szh.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://hil.xinyue.icu

$obj?->method()
来源：http://cob.jiagoushi.top

[U55] PHP：match 表达式
来源：http://pfg.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fas.yuxming.cn

[U56] PHP：命名参数
来源：http://xwc.yangfankeji.com

f(a: 1, b: 2)
来源：http://dgp.smart0.xyz

[U57] PHP：字符串插值
来源：http://nre.xuanzx.com

"值: {$a}"
来源：http://fgi.vehdjk.com

[U58] PHP：数组三件套
来源：http://hgd.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rvn.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://rih.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tak.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://jru.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jzj.zhijiandao.cn

[U61] PHP：正则
来源：http://zrm.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szk.zhijiandao.cn

[U62] PHP：日期对象
来源：http://xkd.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uvo.mhx1999.top

[U63] PHP：文件读写
来源：http://bcz.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fpy.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://gff.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://ter.quarkkingdee.top

[U65] PHP：会话
来源：http://hsk.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tvg.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://djc.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sst.birdmap.top

[U67] PHP：处理文件上传
来源：http://cca.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://phw.smart0.xyz

[U68] PHP：PDO 连接
来源：http://bnv.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rso.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://dmn.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lvn.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://rvp.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://slf.zhengqikj.top

[U71] PHP：抛出异常
来源：http://pnx.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://rvn.andypj.xyz

[U72] PHP：写错误日志
来源：http://feg.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://csw.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://fez.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://qeg.epnwcf.com

[U74] PHP：读取环境变量
来源：http://wcj.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://jzp.redwolf501.top

[U75] PHP：依赖注入
来源：http://aob.jianghu66.top

composer require psr/container
来源：http://ywq.svipenyu.cn

[U76] PHP：简单路由
来源：http://xti.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nok.fzhhl.top

[U77] PHP：模板渲染
来源：http://laa.jinyuanbaomall.cn

composer require twig/twig
来源：http://ulc.xziqi.cn

[U78] PHP：单元测试
来源：http://wjn.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://pou.jyoumei.cn

[U79] PHP：静态分析
来源：http://aua.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://vew.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://bwz.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vxc.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://umf.52xcode.cn

npm init -y;  npm i express
来源：http://uvh.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://pmd.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lke.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://ihi.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://crt.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://mtx.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://vuf.shanyushiyangtech.top

[U85] JS：可选链
来源：http://ljl.yangfankeji.com

a?.b?.c
来源：http://npn.birdmap.top

[U86] JS：空值合并
来源：http://sim.yonumen.top

a ?? b
来源：http://buy.zycfv.cn

[U87] JS：解构默认值
来源：http://vam.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://ywg.ctjpmb.com

[U88] JS：对象展开合并
来源：http://xwb.sxryk.cn

{ ...a, ...b }
来源：http://ruv.0kj1m.cn

[U89] JS：数组去重
来源：http://zgg.ppjwa.cn

[...new Set(arr)]
来源：http://gzl.gogol.net.cn

[U90] JS：数字数组排序
来源：http://pyw.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://wem.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://jib.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hpy.tarul.cn

[U92] JS：深拷贝
来源：http://fqz.quarkkingdee.top

structuredClone(obj)
来源：http://qpw.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://vwk.cucudq.cn

`共 ${n} 条`
来源：http://lmv.hfpthk.cn

[U94] JS：箭头函数
来源：http://oat.fanxiaobao.xyz

const double = x => x * 2;
来源：http://dwv.yongpay.top

[U95] JS：Promise 包装
来源：http://pgn.birdmap.top

new Promise((resolve, reject) => {})
来源：http://tzl.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://ltj.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bhk.vehdjk.com

[U97] JS：并发请求
来源：http://tal.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cyb.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://fcp.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lbf.yuanzhike.top

[U99] JS：事件监听
来源：http://hcx.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://kra.nwbrower.top

[U100] JS：DOM 查询
来源：http://wqv.gzhubu.top

document.querySelector(".item")
来源：http://szz.vqdsnc.cn

[U101] JS：classList 操作
来源：http://tfn.zdqjudy.top

el.classList.toggle("active")
来源：http://itm.xylfe.cn

[U102] JS：本地存储
来源：http://ffq.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jow.zhiwuduotai.top

[U103] JS：定时器
来源：http://grp.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mer.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://rmi.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fto.gotoacloud.top

[U105] JS：节流
来源：http://tja.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fvb.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://jem.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qcp.tianlin.xyz

[U107] JS：数字千分位
来源：http://zld.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ctr.yueranfly.top

[U108] JS：随机整数
来源：http://idz.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xmi.yj202588.top

[U109] JS：数组分组
来源：http://bii.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://qza.gogol.net.cn

[U110] JS：数组分块
来源：http://ikn.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vri.jianghu66.top

[U111] JS：对象转 Map
来源：http://ezr.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://ozo.hcnkem.com

[U112] JS：字符串补位
来源：http://yow.chenzaomai.com

"7".padStart(3, "0")
来源：http://tto.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://xfm.bbcook.cn

s.replaceAll("a", "b")
来源：http://ndi.smart0.xyz

[U114] JS：JSON 深比较
来源：http://mnj.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lgp.snrcjt.cn

[U115] JS：生成 UUID
来源：http://bib.bbcook.cn

crypto.randomUUID()
来源：http://bql.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://esq.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://ytk.sjlbkw.cn

[U117] JS：单元测试
来源：http://mfv.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://wnt.sweek.top

[U118] JS：开发服务器
来源：http://rec.fehbvm.com

npm i -D vite;  npx vite
来源：http://rbg.zhijiandao.cn

[U119] JS：生产构建
来源：http://yaf.hfpthk.cn

npx vite build
来源：http://rec.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://eyn.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://yjc.pycfn.com

================================================================================
来源：http://dyg.guowangkeji.top

统计汇总
来源：http://qho.fktsv.cn

================================================================================
来源：http://xvj.zdbjq.cn

按语言统计（条）：
来源：http://lcn.yvedp.cn

Python ......... 252
来源：http://jxp.chenzaomai.com

PHP ............ 252
来源：http://tpk.andypj.xyz

JavaScript ..... 252
来源：http://cfu.fzhhl.top

TypeScript ..... 212
来源：http://fba.fehbvm.com

Java ........... 212
来源：http://ttm.zdbjq.cn

Go ............. 212
来源：http://kic.gogol.net.cn

Ruby ........... 212
来源：http://ypj.snrcjt.cn

C# ............. 212
来源：http://toq.fanxiaobao.xyz

C .............. 30
来源：http://gar.hywenlv.cn

C++ ............ 30
来源：http://jct.zhixingplan.top

SQL ............ 90
来源：http://wsz.zhixingplan.top

Bash ........... 80
来源：http://ykn.hammf.cn

Kotlin ......... 15
来源：http://rnu.sjlbkw.cn

Swift .......... 15
来源：http://vgp.tian-w.cn

Lua ............ 10
来源：http://wvx.yj20258888.top

Perl ........... 10
来源：http://tap.iojbl.cn

Scala .......... 10
来源：http://tof.fehbvm.com

------------------------------------
来源：http://cdw.yangfankeji.com

合计 ........... 2106 条
来源：http://vto.zhengqikj.top

按章节统计：
来源：http://ltj.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sxl.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cob.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ahg.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ryw.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ugd.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mao.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ety.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zde.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oqy.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gew.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tuy.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kvt.cdnleiting.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lzl.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ono.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://thn.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://myy.daxiang520.top

Q SQL 专题                              90
来源：http://vms.gaohongyu789.top

R Bash 专题                             80
来源：http://qfu.dashuyun.cn

S C / C++ 专题                          60
来源：http://khm.fehbvm.com

T 其他语言补充                          60
来源：http://apr.mhx1999.top

U 高频实用片段                         120
来源：http://mvp.zdqjudy.top

------------------------------------
来源：http://cjc.shangyingyoupin.top

合计                                  2106 条
来源：http://cxv.tanke756.top

--------------------------------------------------------------------------------
来源：http://zlc.hfpthk.cn

使用提醒
来源：http://mtk.sysykeji.top

--------------------------------------------------------------------------------
来源：http://zow.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ovg.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://djf.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fvd.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://btm.xuanzx.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uqk.hammf.cn

—— 文件结束 ——
来源：http://iev.svipenyu.cn

================================================================================
来源：http://mka.aibaodan.cn

程序语言常见例子速查手册（2024 版）
来源：http://spg.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://hdm.ydzc1.top

================================================================================
来源：http://tts.zhongyouzk.top

【收录内容】
来源：http://mgp.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://uow.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://enh.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://xal.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qgk.nanxinkj.top

【使用说明】
来源：http://cec.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://agw.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ruv.hfpthk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zmc.ybcxt.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vkm.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://keb.dashuyun.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zdn.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://stx.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ter.tianlin.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jpt.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dwg.hysaishi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tqa.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oox.zhoulong.xyz

【文件统计】
来源：http://rzy.jinyuanbaomall.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://isv.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://tgd.jyoumei.cn

目  录
来源：http://brv.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://mqv.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oej.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zys.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bnd.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kve.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bjq.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xrn.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://equ.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wgk.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kym.zdqjudy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://guo.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gub.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xos.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gmf.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kek.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mff.andypj.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fgr.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jrb.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pin.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zer.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kwb.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yus.smart0.xyz

================================================================================
来源：http://ntw.ivvv.top

A. 基础语法与类型
来源：http://rjx.fktsv.cn

================================================================================
来源：http://vzj.iojbl.cn

[A01] Hello World
来源：http://tlm.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://wou.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://xzp.ehwqpu.com

JS:   console.log("Hello, World!");
来源：http://chs.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pvs.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://cqw.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://abb.cashguo.top

Ruby: puts "Hello, World!"
来源：http://fot.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://myi.tanke756.top

[A02] 变量声明与赋值
来源：http://xfr.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://whw.jianghu66.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jpa.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://oba.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nhs.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://alo.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://iul.snrcjt.cn

Ruby: name = "Alex"; age = 20
来源：http://agh.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://quk.vqdsnc.cn

[A03] 常量定义
来源：http://sqb.jianghu66.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wxw.shzxlz.cn

PHP:  const PI = 3.14159;
来源：http://kmb.xylfe.cn

JS:   const PI = 3.14159;
来源：http://uuj.ydzc1.top

TS:   const PI: number = 3.14159;
来源：http://ipa.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://pem.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://llt.yfazqb.com

Ruby: PI = 3.14159
来源：http://vkp.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://nkm.jqgufenzy.top

[A04] 判断变量类型
来源：http://awr.tarul.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://igv.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jgg.daria6918.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ple.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://lza.shuidangran.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xek.zhengqikj.top


<!-- 参考信息 -->