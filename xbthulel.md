代发 wailian999

[U37] Py：读写 Excel
来源：http://civ.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mor.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://kpv.daxiang520.top

Path(__file__).resolve().parent
来源：http://fmo.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://har.yfazqb.com

sys.stdout.isatty()
来源：http://ror.cashguo.top

[U40] Py：打印到标准错误
来源：http://ofi.cdnleiting.top

print("err", file=sys.stderr)
来源：http://rgn.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://fxb.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ewd.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://wvq.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jxw.tian-w.cn

[U43] PHP：声明命名空间
来源：http://zun.gogol.net.cn

namespace App\Http;
来源：http://zpp.c1oappe.top

[U44] PHP：开启严格类型
来源：http://lbv.sysykeji.top

declare(strict_types=1);
来源：http://eqf.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://gfg.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xbb.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://kav.zhengqikj.top

?string $name = null
来源：http://vne.cheryme.top

[U47] PHP：联合类型
来源：http://jfz.cdnleiting.top

int|string $id
来源：http://icg.nanxinkj.top

[U48] PHP：纯枚举
来源：http://tas.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ikm.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://xxq.jqgufenzy.top

public readonly string $name
来源：http://urr.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://zym.52xcode.cn

public function __construct(private int $id) {}
来源：http://etu.vehdjk.com

[U51] PHP：数组解构
来源：http://vnw.sxryk.cn

[$a, $b] = $arr;
来源：http://xpp.havefunace.top

[U52] PHP：箭头函数
来源：http://eii.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://ilx.tian-w.cn

[U53] PHP：空合并运算符
来源：http://ejy.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://uyo.yfazqb.com

[U54] PHP：空安全调用
来源：http://ulq.yongpay.top

$obj?->method()
来源：http://rlh.hcnkem.com

[U55] PHP：match 表达式
来源：http://cpu.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vjg.hywenlv.cn

[U56] PHP：命名参数
来源：http://gom.hysaishi.cn

f(a: 1, b: 2)
来源：http://dvx.zhengqikj.top

[U57] PHP：字符串插值
来源：http://gjv.yonumen.top

"值: {$a}"
来源：http://brz.iojbl.cn

[U58] PHP：数组三件套
来源：http://dil.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rvs.zhixingplan.top

[U59] PHP：自定义排序
来源：http://yho.aizwys.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yaf.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://zce.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xku.vqdsnc.cn

[U61] PHP：正则
来源：http://oer.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ivr.yvedp.cn

[U62] PHP：日期对象
来源：http://gkq.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tal.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://hsy.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ofk.hesvh.cn

[U64] PHP：目录遍历
来源：http://qvb.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://yxk.shuidangran.top

[U65] PHP：会话
来源：http://oza.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://akm.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://zvu.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jmq.gzhubu.top

[U67] PHP：处理文件上传
来源：http://qme.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qli.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://zne.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lub.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://gbt.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://prz.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://pqh.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://emd.sweek.top

[U71] PHP：抛出异常
来源：http://ksc.316326.xyz

throw new RuntimeException("失败", 500);
来源：http://xio.ydzc1.top

[U72] PHP：写错误日志
来源：http://clc.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://zhl.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://rxe.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://qkm.iojbl.cn

[U74] PHP：读取环境变量
来源：http://ddl.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://ezm.mhx1999.top

[U75] PHP：依赖注入
来源：http://ayd.yuanzhike.top

composer require psr/container
来源：http://mjq.zdqjudy.top

[U76] PHP：简单路由
来源：http://tqv.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://akv.ybcxt.top

[U77] PHP：模板渲染
来源：http://qru.fengsongda.top

composer require twig/twig
来源：http://qro.ehwqpu.com

[U78] PHP：单元测试
来源：http://tcn.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://wed.tian-w.cn

[U79] PHP：静态分析
来源：http://zik.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://gsu.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://ghh.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vxw.meibo888.top

[U81] JS：初始化项目
来源：http://qdh.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://izz.ybcxt.top

[U82] JS：package.json 脚本
来源：http://fla.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pec.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://xxw.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://mnh.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://ynv.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://iqe.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://mym.uphjek.com

a?.b?.c
来源：http://ktk.smart0.xyz

[U86] JS：空值合并
来源：http://ihs.hcnkem.com

a ?? b
来源：http://cap.ydjk.org.cn

[U87] JS：解构默认值
来源：http://qyp.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://csr.xziqi.cn

[U88] JS：对象展开合并
来源：http://psq.ctjpmb.com

{ ...a, ...b }
来源：http://qoe.hywenlv.cn

[U89] JS：数组去重
来源：http://xjj.zdbjq.cn

[...new Set(arr)]
来源：http://xhs.yvedp.cn

[U90] JS：数字数组排序
来源：http://ncp.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://otl.tanke756.top

[U91] JS：对象键值遍历
来源：http://eas.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://atf.hnqzz.top

[U92] JS：深拷贝
来源：http://imq.zhongyouzk.top

structuredClone(obj)
来源：http://ujb.xuanzx.com

[U93] JS：模板字符串
来源：http://dft.ctjpmb.com

`共 ${n} 条`
来源：http://pit.redwolf501.top

[U94] JS：箭头函数
来源：http://hia.yuanzhike.top

const double = x => x * 2;
来源：http://fsz.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://gqt.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://wph.xylfe.cn

[U96] JS：async/await 与异常
来源：http://ghn.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zxf.gaohongyu789.top

[U97] JS：并发请求
来源：http://gtb.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qnf.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://eaf.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gzn.pengpengdd.cyou

[U99] JS：事件监听
来源：http://vzu.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://mlz.guowangkeji.top

[U100] JS：DOM 查询
来源：http://xim.hesvh.cn

document.querySelector(".item")
来源：http://cyz.jinqigufen.top

[U101] JS：classList 操作
来源：http://kdu.bjfxy.top

el.classList.toggle("active")
来源：http://hzq.zhijiandao.cn

[U102] JS：本地存储
来源：http://psw.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uhj.zhoulong.xyz

[U103] JS：定时器
来源：http://sez.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ogl.ctjpmb.com

[U104] JS：防抖
来源：http://vdh.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbb.havefunace.top

[U105] JS：节流
来源：http://dig.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fez.yj20258888.top

[U106] JS：日期格式化
来源：http://bzb.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fxi.yangfankeji.com

[U107] JS：数字千分位
来源：http://rlu.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fyo.ydzc1.top

[U108] JS：随机整数
来源：http://dat.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jmc.yangfankeji.com

[U109] JS：数组分组
来源：http://dja.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://bxq.tanke756.top

[U110] JS：数组分块
来源：http://oei.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yqc.ydzc1.top

[U111] JS：对象转 Map
来源：http://klq.haohaochexian.top

new Map(Object.entries(obj))
来源：http://shb.yuanzhike.top

[U112] JS：字符串补位
来源：http://lhb.birdmap.top

"7".padStart(3, "0")
来源：http://dkp.fktsv.cn

[U113] JS：正则替换全部
来源：http://tmz.cucudq.cn

s.replaceAll("a", "b")
来源：http://sqf.yueranfly.top

[U114] JS：JSON 深比较
来源：http://brh.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://skc.yvedp.cn

[U115] JS：生成 UUID
来源：http://wqn.yj202588.top

crypto.randomUUID()
来源：http://gis.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://gwp.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://zju.sysykeji.top

[U117] JS：单元测试
来源：http://hxs.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://fni.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://vul.jiagoushi.top

npm i -D vite;  npx vite
来源：http://wuc.yj202588.top

[U119] JS：生产构建
来源：http://tlm.shuidangran.top

npx vite build
来源：http://hxl.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://pmg.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://tmh.zhijiandao.cn

================================================================================
来源：http://tyb.yangfankeji.com

统计汇总
来源：http://jay.birdmap.top

================================================================================
来源：http://sar.zhaomingkeji.xyz

按语言统计（条）：
来源：http://nzm.chenjidiqi.icu

Python ......... 252
来源：http://oye.havefunace.top

PHP ............ 252
来源：http://qmw.hesvh.cn

JavaScript ..... 252
来源：http://zbu.gogol.net.cn

TypeScript ..... 212
来源：http://ggo.nwbrower.top

Java ........... 212
来源：http://wmr.nanxuanxn.top

Go ............. 212
来源：http://jug.xylfe.cn

Ruby ........... 212
来源：http://ylz.yangfankeji.com

C# ............. 212
来源：http://vvx.9152youxi.cn

C .............. 30
来源：http://sxq.redwolf501.top

C++ ............ 30
来源：http://mfr.jqgufenzy.top

SQL ............ 90
来源：http://mcf.316326.xyz

Bash ........... 80
来源：http://vou.sjlbkw.cn

Kotlin ......... 15
来源：http://ohi.wangdashe.top

Swift .......... 15
来源：http://yro.xziqi.cn

Lua ............ 10
来源：http://mlu.xylfe.cn

Perl ........... 10
来源：http://qrc.xuanzx.com

Scala .......... 10
来源：http://bpl.shanyushiyangkeji.top

------------------------------------
来源：http://zjk.316326.xyz

合计 ........... 2106 条
来源：http://tbe.0kj1m.cn

按章节统计：
来源：http://wxr.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pzd.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dsz.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uyg.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://chl.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nsv.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gne.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://car.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zml.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gke.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ahy.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kdo.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gbf.jqgfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hac.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zve.zdbjq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mvi.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gqo.chenjidiqi.icu

Q SQL 专题                              90
来源：http://poi.0kj1m.cn

R Bash 专题                             80
来源：http://muv.gogol.net.cn

S C / C++ 专题                          60
来源：http://qgj.yj20258.top

T 其他语言补充                          60
来源：http://dxj.ybcxt.top

U 高频实用片段                         120
来源：http://bwu.zhengqikj.top

------------------------------------
来源：http://tgs.hnqzz.top

合计                                  2106 条
来源：http://grg.52xcode.cn

--------------------------------------------------------------------------------
来源：http://fhl.yvedp.cn

使用提醒
来源：http://pbf.xylfe.cn

--------------------------------------------------------------------------------
来源：http://ofs.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qqp.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ojz.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sme.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://unp.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wqi.wangdashe.top

—— 文件结束 ——
来源：http://hlw.nwbrower.top

================================================================================
来源：http://eec.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://wtu.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://cth.ydjk.org.cn

================================================================================
来源：http://tct.gotoacloud.top

【收录内容】
来源：http://ssz.yvedp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lby.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wth.0kj1m.cn

SQL · Bash · C · C++
来源：http://pkt.redwolf501.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mss.kuanghao11.cn

【使用说明】
来源：http://fed.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jer.bbcook.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gml.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hrw.zdqjudy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://obw.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wro.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eis.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://avt.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gxa.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vsz.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dbw.fehbvm.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zuq.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nae.iojbl.cn

【文件统计】
来源：http://xfa.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://syx.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://sgj.cqqwz.cn

目  录
来源：http://jvq.zycfv.cn

--------------------------------------------------------------------------------
来源：http://ixs.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zub.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bgh.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hmy.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://clg.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vvk.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://icl.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wir.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vvy.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dvi.wangshuangyany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dxk.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bxx.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hok.mhx1999.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bev.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://unq.sxryk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ptc.gogol.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xaz.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ore.ctjpmb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://bsk.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dyv.yongpay.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dqe.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://icu.jinqigufen.top

================================================================================
来源：http://ztg.yuxming.cn

A. 基础语法与类型
来源：http://sve.9152youxi.cn

================================================================================
来源：http://qvm.jinyuanbaomall.cn

[A01] Hello World
来源：http://qrp.mhx1999.top

Py:   print("Hello, World!")
来源：http://rza.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://zhd.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://kju.shanyushiyangtech.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pbd.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://qhc.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://ekc.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://utd.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lom.c1oappe.top

[A02] 变量声明与赋值
来源：http://ali.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pzs.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://akd.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://ltj.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jwd.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://wle.yuanzhike.top

Go:   name := "Alex"; age := 20
来源：http://rlb.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://cof.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://rfn.fktsv.cn

[A03] 常量定义
来源：http://btj.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hsa.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://qbz.ivvv.top

JS:   const PI = 3.14159;
来源：http://kno.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://mli.xingfuxueyuan.xyz

Java: static final double PI = 3.14159;
来源：http://biw.wangdashe.top

Go:   const PI = 3.14159
来源：http://qsz.chenlongwang.top


<!-- 参考信息 -->