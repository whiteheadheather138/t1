代发 wailian999

[U37] Py：读写 Excel
来源：http://kwp.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://qtx.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://rgs.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://cxk.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://eyn.sufxvd.cn

sys.stdout.isatty()
来源：http://eqy.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://qtu.52xcode.cn

print("err", file=sys.stderr)
来源：http://wzc.quarkkingdee.top

[U41] PHP：初始化 Composer 项目
来源：http://gdf.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://rgj.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://fbp.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tvh.bbcook.cn

[U43] PHP：声明命名空间
来源：http://zey.vqdsnc.cn

namespace App\Http;
来源：http://uld.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://bju.hysaishi.cn

declare(strict_types=1);
来源：http://wqt.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://erj.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vyc.yj20258.top

[U46] PHP：可空类型
来源：http://jio.cqqwz.cn

?string $name = null
来源：http://iij.haohaochexian.top

[U47] PHP：联合类型
来源：http://tlb.gzhubu.top

int|string $id
来源：http://ncy.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://glw.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://roy.hnxiangtu.top

[U49] PHP：只读属性
来源：http://yqy.yanxiufei.cn

public readonly string $name
来源：http://zqx.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://tnu.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://mwj.andypj.xyz

[U51] PHP：数组解构
来源：http://rch.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://riu.nanxinkj.top

[U52] PHP：箭头函数
来源：http://wms.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://nbw.wangdashe.top

[U53] PHP：空合并运算符
来源：http://cab.haohaochexian.top

$v = $a ?? $b ?? "default";
来源：http://axm.bjfxy.top

[U54] PHP：空安全调用
来源：http://rcd.daria6918.cn

$obj?->method()
来源：http://uvv.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://mrv.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dlq.svipenyu.cn

[U56] PHP：命名参数
来源：http://sgu.dianchejie.cn

f(a: 1, b: 2)
来源：http://dss.cheryme.top

[U57] PHP：字符串插值
来源：http://rho.dashuyun.cn

"值: {$a}"
来源：http://qye.daxiang520.top

[U58] PHP：数组三件套
来源：http://tff.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wfd.xinyue.icu

[U59] PHP：自定义排序
来源：http://sog.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izm.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://sza.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lue.zhengqikj.top

[U61] PHP：正则
来源：http://ydg.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gtz.jinqigfzy.top

[U62] PHP：日期对象
来源：http://pub.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://trc.epnwcf.com

[U63] PHP：文件读写
来源：http://nud.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wzz.mhx1999.top

[U64] PHP：目录遍历
来源：http://ccx.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://zfb.nanxuanxn.top

[U65] PHP：会话
来源：http://wic.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zfb.birdmap.top

[U66] PHP：设置 Cookie
来源：http://hwm.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uoz.xziqi.cn

[U67] PHP：处理文件上传
来源：http://axy.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://njz.wangdashe.top

[U68] PHP：PDO 连接
来源：http://tjb.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://udk.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://bdv.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbw.316326.xyz

[U70] PHP：PDO 事务
来源：http://lcq.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wfp.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://pok.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://kgi.ctjpmb.com

[U72] PHP：写错误日志
来源：http://nng.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://vwz.9152youxi.cn

[U73] PHP：读取 ini 配置
来源：http://fvw.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://kcl.xuanzx.com

[U74] PHP：读取环境变量
来源：http://ssb.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://hyl.ybcxt.top

[U75] PHP：依赖注入
来源：http://pfi.yonumen.top

composer require psr/container
来源：http://gvt.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://ivj.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wir.tian-w.cn

[U77] PHP：模板渲染
来源：http://jkb.kuanghao11.cn

composer require twig/twig
来源：http://lom.nanxinkj.top

[U78] PHP：单元测试
来源：http://zzl.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://dua.cashguo.top

[U79] PHP：静态分析
来源：http://diq.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://qxk.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://wpl.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://dst.mhx1999.top

[U81] JS：初始化项目
来源：http://iar.xuanzx.com

npm init -y;  npm i express
来源：http://kmh.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://zte.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uim.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://zog.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://luy.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://rzr.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://nsb.cdnleiting.top

[U85] JS：可选链
来源：http://gxx.kuanghao11.cn

a?.b?.c
来源：http://lwh.epnwcf.com

[U86] JS：空值合并
来源：http://azk.hfpthk.cn

a ?? b
来源：http://nae.nwbrower.top

[U87] JS：解构默认值
来源：http://kxj.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://kvv.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://eap.xuetiantiany.cn

{ ...a, ...b }
来源：http://hte.daxiang520.top

[U89] JS：数组去重
来源：http://cxj.chenzaomai.com

[...new Set(arr)]
来源：http://fem.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://tle.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://ijc.yfazqb.com

[U91] JS：对象键值遍历
来源：http://irj.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wum.iojbl.cn

[U92] JS：深拷贝
来源：http://lnj.gotoacloud.top

structuredClone(obj)
来源：http://ojj.havefunace.top

[U93] JS：模板字符串
来源：http://tzz.yj20258.top

`共 ${n} 条`
来源：http://nkc.fehbvm.com

[U94] JS：箭头函数
来源：http://ljz.tian-w.cn

const double = x => x * 2;
来源：http://csf.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://nid.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://cki.c1oappe.top

[U96] JS：async/await 与异常
来源：http://ecj.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hwp.quarkkingdee.top

[U97] JS：并发请求
来源：http://hoo.redwolf501.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://icw.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://hbm.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxk.nanxinkj.top

[U99] JS：事件监听
来源：http://noy.shuidangran.top

el.addEventListener("click", e => {})
来源：http://nsk.guannengcc.top

[U100] JS：DOM 查询
来源：http://gjn.smart0.xyz

document.querySelector(".item")
来源：http://fus.iojbl.cn

[U101] JS：classList 操作
来源：http://gdd.tianlin.xyz

el.classList.toggle("active")
来源：http://rry.zdbjq.cn

[U102] JS：本地存储
来源：http://znx.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bgk.havefunace.top

[U103] JS：定时器
来源：http://ccb.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kdv.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://bwb.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dzk.yfazqb.com

[U105] JS：节流
来源：http://aoa.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sci.zdbjq.cn

[U106] JS：日期格式化
来源：http://kvr.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jtn.redwolf501.top

[U107] JS：数字千分位
来源：http://lcn.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qzh.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://pcw.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yfr.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://vhb.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://qle.hammf.cn

[U110] JS：数组分块
来源：http://qxl.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vsd.cucudq.cn

[U111] JS：对象转 Map
来源：http://uam.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://bho.birdmap.top

[U112] JS：字符串补位
来源：http://hkb.zhixingplan.top

"7".padStart(3, "0")
来源：http://ipe.gogol.net.cn

[U113] JS：正则替换全部
来源：http://sfr.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://igx.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://wpl.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fmy.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://bsp.jinqigufen.top

crypto.randomUUID()
来源：http://ybk.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://ywc.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://ggx.redwolf501.top

[U117] JS：单元测试
来源：http://wda.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://mko.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://ktp.gotoacloud.top

npm i -D vite;  npx vite
来源：http://log.shangyingyoupin.top

[U119] JS：生产构建
来源：http://mnu.hysaishi.cn

npx vite build
来源：http://xbt.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://gth.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://imv.xinyue.icu

================================================================================
来源：http://npm.yuanzhike.top

统计汇总
来源：http://gae.nanxinkj.top

================================================================================
来源：http://utr.zhijiandao.cn

按语言统计（条）：
来源：http://lep.xinyue.icu

Python ......... 252
来源：http://ubj.uphjek.com

PHP ............ 252
来源：http://tws.havefunace.top

JavaScript ..... 252
来源：http://gew.yuanzhike.top

TypeScript ..... 212
来源：http://ntl.dashuyun.cn

Java ........... 212
来源：http://gbl.haohaochexian.top

Go ............. 212
来源：http://bmo.zhiwuduotai.top

Ruby ........... 212
来源：http://sgy.316326.xyz

C# ............. 212
来源：http://qoq.dianchejie.cn

C .............. 30
来源：http://lkv.jinyuanbaomall.cn

C++ ............ 30
来源：http://vvj.cashguo.top

SQL ............ 90
来源：http://wze.hfpthk.cn

Bash ........... 80
来源：http://hcr.redwolf501.top

Kotlin ......... 15
来源：http://bxy.wangshuangyany.cn

Swift .......... 15
来源：http://wjg.chenzaomai.com

Lua ............ 10
来源：http://fcq.ywan-chungtsiang.top

Perl ........... 10
来源：http://zxw.hfpthk.cn

Scala .......... 10
来源：http://twd.xingfuxueyuan.xyz

------------------------------------
来源：http://gsq.jyoumei.cn

合计 ........... 2106 条
来源：http://vub.yuxming.cn

按章节统计：
来源：http://zpv.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wia.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xel.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nmi.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cke.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ake.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://axs.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lpz.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pqj.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://brk.hysaishi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pqd.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://khm.yuxming.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dir.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jvh.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rhe.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://snw.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://puh.gzhubu.top

Q SQL 专题                              90
来源：http://krl.ydzc1.top

R Bash 专题                             80
来源：http://gkh.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://umj.zhijiandao.cn

T 其他语言补充                          60
来源：http://fmu.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://vos.zycfv.cn

------------------------------------
来源：http://yei.snrcjt.cn

合计                                  2106 条
来源：http://nos.xylfe.cn

--------------------------------------------------------------------------------
来源：http://jds.c1oappe.top

使用提醒
来源：http://vfh.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://jkn.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ylz.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iec.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tvr.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lpo.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eja.zhijiandao.cn

—— 文件结束 ——
来源：http://wsv.jlsjyb.cn

================================================================================
来源：http://yot.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://gvx.hammf.cn

Common Programming Examples Cheat Book
来源：http://ksh.hcnkem.com

================================================================================
来源：http://odp.aibaodan.cn

【收录内容】
来源：http://jiz.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bwt.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lmg.chenzaomai.com

SQL · Bash · C · C++
来源：http://opm.zdbjq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ont.jlsjyb.cn

【使用说明】
来源：http://wab.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lls.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rdt.xziqi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cgb.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vns.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tac.yueranfly.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iol.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tgw.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rgc.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bqn.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gis.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tiv.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ilr.tian-w.cn

【文件统计】
来源：http://aem.ywan-chungtsiang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ovb.tarul.cn

--------------------------------------------------------------------------------
来源：http://mji.jinyuanbaomall.cn

目  录
来源：http://aja.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ekp.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iwg.mhx1999.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zcw.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ffu.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zal.yvedp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lba.havefunace.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dxo.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xhk.yuxming.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://djh.ivvv.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dqw.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://myy.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://svq.yanxiufei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://quv.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://awt.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fgq.yongpay.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://upk.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ztr.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://okv.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nic.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bgv.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nfz.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://glf.daria6918.cn

================================================================================
来源：http://ibi.jinqigfzy.top

A. 基础语法与类型
来源：http://lmr.xuetiantiany.cn

================================================================================
来源：http://cge.yuanzhike.top

[A01] Hello World
来源：http://ewn.sxryk.cn

Py:   print("Hello, World!")
来源：http://pev.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://nny.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://vxx.gotoacloud.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yhn.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://zjs.cucudq.cn

Go:   fmt.Println("Hello, World!")
来源：http://hna.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://xjp.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://guw.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://zzl.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://byv.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iym.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://adc.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eqm.daxiang520.top

Java: String name = "Alex"; int age = 20;
来源：http://kpl.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://wcv.chenlongwang.top

Ruby: name = "Alex"; age = 20
来源：http://gnb.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lra.iojbl.cn

[A03] 常量定义
来源：http://txa.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lhu.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://wlg.fzhhl.top

JS:   const PI = 3.14159;
来源：http://cdt.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://zxc.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://dmg.ppjwa.cn

Go:   const PI = 3.14159
来源：http://qeu.hnqzz.top


<!-- 参考信息 -->