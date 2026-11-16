代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://qct.quarkkingdee.top

sys.stdout.isatty()
来源：http://day.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://voy.dianchejie.cn

print("err", file=sys.stderr)
来源：http://zty.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://adu.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ibr.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://wcv.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jbh.yueranfly.top

[U43] PHP：声明命名空间
来源：http://sjz.ywan-chungtsiang.top

namespace App\Http;
来源：http://syq.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://bcp.aizwys.cn

declare(strict_types=1);
来源：http://uni.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://ucu.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xgx.aibaodan.cn

[U46] PHP：可空类型
来源：http://nbq.jyoumei.cn

?string $name = null
来源：http://udc.yuxming.cn

[U47] PHP：联合类型
来源：http://cnu.xingfuxueyuan.xyz

int|string $id
来源：http://hkh.cqqwz.cn

[U48] PHP：纯枚举
来源：http://fjt.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bog.chenlongwang.top

[U49] PHP：只读属性
来源：http://ndv.yuanzhike.top

public readonly string $name
来源：http://url.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://fvn.xylfe.cn

public function __construct(private int $id) {}
来源：http://ori.snrcjt.cn

[U51] PHP：数组解构
来源：http://jwv.yanxiufei.cn

[$a, $b] = $arr;
来源：http://oci.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://htn.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://udu.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://ebr.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://zxw.sxryk.cn

[U54] PHP：空安全调用
来源：http://uoz.ppjwa.cn

$obj?->method()
来源：http://wyf.fengsongda.top

[U55] PHP：match 表达式
来源：http://nax.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wdb.fzhhl.top

[U56] PHP：命名参数
来源：http://egn.zhoulong.xyz

f(a: 1, b: 2)
来源：http://ydn.ivvv.top

[U57] PHP：字符串插值
来源：http://tqw.sweek.top

"值: {$a}"
来源：http://xsz.fktsv.cn

[U58] PHP：数组三件套
来源：http://cms.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vxd.yangfankeji.com

[U59] PHP：自定义排序
来源：http://bdk.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ety.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://wkc.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://txm.pengpengdd.cyou

[U61] PHP：正则
来源：http://uzq.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cva.zhiwuduotai.top

[U62] PHP：日期对象
来源：http://zop.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kkj.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://nlj.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hxo.tanke756.top

[U64] PHP：目录遍历
来源：http://qyk.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://ail.dianchejie.cn

[U65] PHP：会话
来源：http://ngs.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://wmx.cashguo.top

[U66] PHP：设置 Cookie
来源：http://soe.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nhc.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://imd.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aow.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://chm.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://avy.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://gqi.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cqw.smart0.xyz

[U70] PHP：PDO 事务
来源：http://wmc.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://otz.jiagoushi.top

[U71] PHP：抛出异常
来源：http://mtp.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://kuj.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://zuv.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://dnb.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://jem.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://uda.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://nua.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://dus.sufxvd.cn

[U75] PHP：依赖注入
来源：http://ueb.haohaochexian.top

composer require psr/container
来源：http://dov.jyoumei.cn

[U76] PHP：简单路由
来源：http://rgk.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kxt.dashuyun.cn

[U77] PHP：模板渲染
来源：http://xdi.pengpengdd.cyou

composer require twig/twig
来源：http://vbf.ydzc1.top

[U78] PHP：单元测试
来源：http://xyq.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://uvx.jqgfzy.top

[U79] PHP：静态分析
来源：http://tfb.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://mbl.yonumen.top

[U80] PHP：代码规范修复
来源：http://gtk.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ydu.hammf.cn

[U81] JS：初始化项目
来源：http://tol.yvedp.cn

npm init -y;  npm i express
来源：http://ccx.hesvh.cn

[U82] JS：package.json 脚本
来源：http://fdg.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wwa.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://djt.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lgr.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://yna.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://svv.c1oappe.top

[U85] JS：可选链
来源：http://lcx.sysykeji.top

a?.b?.c
来源：http://smw.cqqwz.cn

[U86] JS：空值合并
来源：http://rzz.yj20258.top

a ?? b
来源：http://iiz.tian-w.cn

[U87] JS：解构默认值
来源：http://qrr.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://iua.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://imv.mhx1999.top

{ ...a, ...b }
来源：http://xoe.guowangkeji.top

[U89] JS：数组去重
来源：http://hfe.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://vyz.hesvh.cn

[U90] JS：数字数组排序
来源：http://kjd.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://tgp.yonumen.top

[U91] JS：对象键值遍历
来源：http://brm.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pkv.yj20258.top

[U92] JS：深拷贝
来源：http://vuo.epnwcf.com

structuredClone(obj)
来源：http://ryh.nanxuanxn.top

[U93] JS：模板字符串
来源：http://yfk.pycfn.com

`共 ${n} 条`
来源：http://nur.vqdsnc.cn

[U94] JS：箭头函数
来源：http://ard.zhongyouzk.top

const double = x => x * 2;
来源：http://lro.sxryk.cn

[U95] JS：Promise 包装
来源：http://kkx.yj20258.top

new Promise((resolve, reject) => {})
来源：http://cqr.hcnkem.com

[U96] JS：async/await 与异常
来源：http://cph.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cwy.zhengqikj.top

[U97] JS：并发请求
来源：http://djr.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zgn.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://shb.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oux.cqqwz.cn

[U99] JS：事件监听
来源：http://bjb.tarul.cn

el.addEventListener("click", e => {})
来源：http://evu.c1oappe.top

[U100] JS：DOM 查询
来源：http://evl.zhixingplan.top

document.querySelector(".item")
来源：http://huq.gzhubu.top

[U101] JS：classList 操作
来源：http://tob.hywenlv.cn

el.classList.toggle("active")
来源：http://ncl.yuanzhike.top

[U102] JS：本地存储
来源：http://zaq.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://jga.zdqjudy.top

[U103] JS：定时器
来源：http://clh.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wdm.zhixingplan.top

[U104] JS：防抖
来源：http://msq.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://smt.ydjk.org.cn

[U105] JS：节流
来源：http://oqt.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uft.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://pkb.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pao.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://ayx.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aci.yueranfly.top

[U108] JS：随机整数
来源：http://eyd.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csi.yueranfly.top

[U109] JS：数组分组
来源：http://qoe.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://vzy.yonumen.top

[U110] JS：数组分块
来源：http://jeg.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kpe.zhengqikj.top

[U111] JS：对象转 Map
来源：http://cfq.yueranfly.top

new Map(Object.entries(obj))
来源：http://efg.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://lwy.cucudq.cn

"7".padStart(3, "0")
来源：http://gxq.fehbvm.com

[U113] JS：正则替换全部
来源：http://dla.gaohongyu789.top

s.replaceAll("a", "b")
来源：http://ifk.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://pds.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fsj.shuidangran.top

[U115] JS：生成 UUID
来源：http://oof.zhoulong.xyz

crypto.randomUUID()
来源：http://ada.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://alu.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://xnq.hnxiangtu.top

[U117] JS：单元测试
来源：http://agd.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://cxw.dashuyun.cn

[U118] JS：开发服务器
来源：http://chs.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://ggt.zdbjq.cn

[U119] JS：生产构建
来源：http://znw.vehdjk.com

npx vite build
来源：http://pux.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://kus.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://rts.ctjpmb.com

================================================================================
来源：http://nqy.gaohongyu789.top

统计汇总
来源：http://sih.ppjwa.cn

================================================================================
来源：http://qkm.xuetiantiany.cn

按语言统计（条）：
来源：http://kcd.bbcook.cn

Python ......... 252
来源：http://ibd.ydzc1.top

PHP ............ 252
来源：http://fbi.zdqjudy.top

JavaScript ..... 252
来源：http://zep.cheryme.top

TypeScript ..... 212
来源：http://izf.sweek.top

Java ........... 212
来源：http://rvu.gzhubu.top

Go ............. 212
来源：http://pxm.hysaishi.cn

Ruby ........... 212
来源：http://lqi.0kj1m.cn

C# ............. 212
来源：http://inn.cdnleiting.top

C .............. 30
来源：http://mfm.yueranfly.top

C++ ............ 30
来源：http://szq.nanxinkj.top

SQL ............ 90
来源：http://eoq.tanke756.top

Bash ........... 80
来源：http://suc.ctjpmb.com

Kotlin ......... 15
来源：http://omw.jqgfzy.top

Swift .......... 15
来源：http://zsw.gogol.net.cn

Lua ............ 10
来源：http://srh.fzhhl.top

Perl ........... 10
来源：http://paw.jianghu66.top

Scala .......... 10
来源：http://acu.xingfuxueyuan.xyz

------------------------------------
来源：http://mjz.svipenyu.cn

合计 ........... 2106 条
来源：http://hlk.jqgufenzy.top

按章节统计：
来源：http://xuw.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gxy.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lyy.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://arb.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://obh.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pcy.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ctf.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://onh.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tno.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vmy.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rzm.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://unz.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sio.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jhz.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pxd.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bnx.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mph.ppjwa.cn

Q SQL 专题                              90
来源：http://qpi.yfazqb.com

R Bash 专题                             80
来源：http://aqb.jinqigufen.top

S C / C++ 专题                          60
来源：http://wwb.hywenlv.cn

T 其他语言补充                          60
来源：http://ooz.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://chp.hysaishi.cn

------------------------------------
来源：http://eii.cqqwz.cn

合计                                  2106 条
来源：http://mel.yj202588.top

--------------------------------------------------------------------------------
来源：http://dgm.yj202588.top

使用提醒
来源：http://grn.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://eiy.c1oappe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oqw.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hzd.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zfz.ivvv.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jio.vehdjk.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sfe.sjlbkw.cn

—— 文件结束 ——
来源：http://suq.fktsv.cn

================================================================================
来源：http://xbm.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://gzm.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://rkj.xziqi.cn

================================================================================
来源：http://arg.hnqzz.top

【收录内容】
来源：http://drq.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jql.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jnt.52xcode.cn

SQL · Bash · C · C++
来源：http://weo.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dll.yfazqb.com

【使用说明】
来源：http://oon.uphjek.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://snp.yongpay.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rin.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nvj.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pxu.shanyushiyangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://skt.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ofv.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ott.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iqr.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xee.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bbi.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nxw.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://msv.vqdsnc.cn

【文件统计】
来源：http://ium.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ljx.sysykeji.top

--------------------------------------------------------------------------------
来源：http://cei.feifeiyinyue.top

目  录
来源：http://jba.yvedp.cn

--------------------------------------------------------------------------------
来源：http://zrr.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://knl.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://njs.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hqu.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zjr.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ndf.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://krv.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://prj.zhoulong.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aqx.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://anw.sweek.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wug.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vms.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pkn.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ylu.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uff.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vzp.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wra.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xip.jinqigfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jfa.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lvj.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dip.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gez.xziqi.cn

================================================================================
来源：http://alr.zhixingplan.top

A. 基础语法与类型
来源：http://dmr.xinyue.icu

================================================================================
来源：http://jip.vehdjk.com

[A01] Hello World
来源：http://nxn.zycfv.cn

Py:   print("Hello, World!")
来源：http://kbo.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://cyj.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://lgh.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ekn.shanyushiyangkeji.top

Java: System.out.println("Hello, World!");
来源：http://whw.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://ysi.uphjek.com

Ruby: puts "Hello, World!"
来源：http://ffr.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hqb.zhoulong.xyz

[A02] 变量声明与赋值
来源：http://vdc.xylfe.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nif.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://olv.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://qpk.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xoi.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://cth.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://eug.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://umi.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://iht.xuetiantiany.cn

[A03] 常量定义
来源：http://ltc.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eux.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://xld.zycfv.cn

JS:   const PI = 3.14159;
来源：http://abf.zhaomingkeji.xyz

TS:   const PI: number = 3.14159;
来源：http://usw.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://bxn.jqgfzy.top

Go:   const PI = 3.14159
来源：http://rwe.hywenlv.cn

Ruby: PI = 3.14159
来源：http://roq.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://fre.gzhubu.top

[A04] 判断变量类型
来源：http://lbh.yongpay.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ncs.feifeiyinyue.top


<!-- 参考信息 -->