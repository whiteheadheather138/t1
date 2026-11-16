代发 wailian999

[U35] Py：发送邮件
来源：http://jsu.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dsd.haohaochexian.top

[U36] Py：定时任务
来源：http://qkx.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://ydy.tian-w.cn

[U37] Py：读写 Excel
来源：http://zrf.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://auy.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://ujc.andypj.xyz

Path(__file__).resolve().parent
来源：http://aaz.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://sdx.zhiwuduotai.top

sys.stdout.isatty()
来源：http://ldi.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://hwr.chenjidiqi.icu

print("err", file=sys.stderr)
来源：http://lzz.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://pft.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dim.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://jyh.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kqi.fzhhl.top

[U43] PHP：声明命名空间
来源：http://bka.cashguo.top

namespace App\Http;
来源：http://oey.birdmap.top

[U44] PHP：开启严格类型
来源：http://ocz.guannengcc.top

declare(strict_types=1);
来源：http://emg.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://yns.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zpb.jqgufenzy.top

[U46] PHP：可空类型
来源：http://lkw.sjlbkw.cn

?string $name = null
来源：http://cns.yj20258888.top

[U47] PHP：联合类型
来源：http://cbm.tian-w.cn

int|string $id
来源：http://ipl.uphjek.com

[U48] PHP：纯枚举
来源：http://uvk.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://saw.vehdjk.com

[U49] PHP：只读属性
来源：http://dhr.ydzc1.top

public readonly string $name
来源：http://ffb.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://bzr.cqqwz.cn

public function __construct(private int $id) {}
来源：http://knw.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://srg.cashguo.top

[$a, $b] = $arr;
来源：http://jet.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://wlm.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://yxc.uphjek.com

[U53] PHP：空合并运算符
来源：http://ypd.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://cyn.fktsv.cn

[U54] PHP：空安全调用
来源：http://sho.yuanzhike.top

$obj?->method()
来源：http://rkc.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://uys.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://som.cdnleiting.top

[U56] PHP：命名参数
来源：http://ndg.bbcook.cn

f(a: 1, b: 2)
来源：http://kdo.haohaochexian.top

[U57] PHP：字符串插值
来源：http://xtx.ydjk.org.cn

"值: {$a}"
来源：http://yrg.zhixingplan.top

[U58] PHP：数组三件套
来源：http://umo.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rum.chenlongwang.top

[U59] PHP：自定义排序
来源：http://des.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sho.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://txw.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rda.fzhhl.top

[U61] PHP：正则
来源：http://rfd.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rbw.wangdashe.top

[U62] PHP：日期对象
来源：http://jwn.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ehu.yueranfly.top

[U63] PHP：文件读写
来源：http://hpi.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qsl.jqgfzy.top

[U64] PHP：目录遍历
来源：http://vqa.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://lhp.jyoumei.cn

[U65] PHP：会话
来源：http://rdo.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xyy.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://bun.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nfp.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://fqr.yj202588.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iyw.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://pxy.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pzz.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://dwv.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ojw.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://vza.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://alx.sufxvd.cn

[U71] PHP：抛出异常
来源：http://qbp.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://uge.cdnleiting.top

[U72] PHP：写错误日志
来源：http://egl.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://lhb.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://ksn.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://pjh.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://ntw.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://bwd.tian-w.cn

[U75] PHP：依赖注入
来源：http://vah.jinqigfzy.top

composer require psr/container
来源：http://mxn.zhixingplan.top

[U76] PHP：简单路由
来源：http://rrd.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://boz.cashguo.top

[U77] PHP：模板渲染
来源：http://hgi.vqdsnc.cn

composer require twig/twig
来源：http://rbj.jiagoushi.top

[U78] PHP：单元测试
来源：http://qto.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://kjx.yj20258.top

[U79] PHP：静态分析
来源：http://smk.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://guc.fktsv.cn

[U80] PHP：代码规范修复
来源：http://xfh.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yhc.sxryk.cn

[U81] JS：初始化项目
来源：http://bzy.nanxinkj.top

npm init -y;  npm i express
来源：http://bex.cheryme.top

[U82] JS：package.json 脚本
来源：http://pck.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iaq.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://cbh.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gqy.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://pwt.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bwa.cashguo.top

[U85] JS：可选链
来源：http://lut.jqgufenzy.top

a?.b?.c
来源：http://qdq.ydzc1.top

[U86] JS：空值合并
来源：http://ulb.vehdjk.com

a ?? b
来源：http://daz.9152youxi.cn

[U87] JS：解构默认值
来源：http://uus.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://bic.aizwys.cn

[U88] JS：对象展开合并
来源：http://vld.havefunace.top

{ ...a, ...b }
来源：http://zdd.feifeiyinyue.top

[U89] JS：数组去重
来源：http://tyh.xuanzx.com

[...new Set(arr)]
来源：http://nia.gotoacloud.top

[U90] JS：数字数组排序
来源：http://dgt.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://rkx.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://bxc.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://akw.aizwys.cn

[U92] JS：深拷贝
来源：http://jlv.smart0.xyz

structuredClone(obj)
来源：http://uhw.yanxiufei.cn

[U93] JS：模板字符串
来源：http://esd.feifeiyinyue.top

`共 ${n} 条`
来源：http://syn.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://rgi.fehbvm.com

const double = x => x * 2;
来源：http://uet.nwbrower.top

[U95] JS：Promise 包装
来源：http://zrx.hammf.cn

new Promise((resolve, reject) => {})
来源：http://crt.smart0.xyz

[U96] JS：async/await 与异常
来源：http://mqv.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bwx.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://gul.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cmo.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://siy.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gzh.kuanghao11.cn

[U99] JS：事件监听
来源：http://ndr.xuanzx.com

el.addEventListener("click", e => {})
来源：http://hdi.daxiang520.top

[U100] JS：DOM 查询
来源：http://mqn.dashuyun.cn

document.querySelector(".item")
来源：http://vrx.bjfxy.top

[U101] JS：classList 操作
来源：http://kqi.tian-w.cn

el.classList.toggle("active")
来源：http://tuh.mhx1999.top

[U102] JS：本地存储
来源：http://vfy.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qoq.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://dav.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://keu.yfazqb.com

[U104] JS：防抖
来源：http://ooz.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://atz.sysykeji.top

[U105] JS：节流
来源：http://deo.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vbo.0kj1m.cn

[U106] JS：日期格式化
来源：http://mtf.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zpi.svipenyu.cn

[U107] JS：数字千分位
来源：http://aiq.xingfuxueyuan.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://grv.zhengqikj.top

[U108] JS：随机整数
来源：http://aua.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lbx.ydjk.org.cn

[U109] JS：数组分组
来源：http://xsx.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://zas.yonumen.top

[U110] JS：数组分块
来源：http://kpi.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://imd.aibaodan.cn

[U111] JS：对象转 Map
来源：http://hrc.xylfe.cn

new Map(Object.entries(obj))
来源：http://rhe.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://fvb.yvedp.cn

"7".padStart(3, "0")
来源：http://crz.vehdjk.com

[U113] JS：正则替换全部
来源：http://wvv.cashguo.top

s.replaceAll("a", "b")
来源：http://vkm.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://efz.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ltc.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://stx.pycfn.com

crypto.randomUUID()
来源：http://kgt.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://sap.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://miw.xuanzx.com

[U117] JS：单元测试
来源：http://ulk.cheryme.top

npm i -D vitest;  npx vitest
来源：http://bui.hammf.cn

[U118] JS：开发服务器
来源：http://vho.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://lui.yuxming.cn

[U119] JS：生产构建
来源：http://moi.bjfxy.top

npx vite build
来源：http://swo.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://bxe.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://fkm.ybcxt.top

================================================================================
来源：http://anv.gotoacloud.top

统计汇总
来源：http://jqk.guowangkeji.top

================================================================================
来源：http://ccz.hnqzz.top

按语言统计（条）：
来源：http://bqq.ehwqpu.com

Python ......... 252
来源：http://hga.hnqzz.top

PHP ............ 252
来源：http://iqg.quarkkingdee.top

JavaScript ..... 252
来源：http://wcz.yangfankeji.com

TypeScript ..... 212
来源：http://zsv.xingfuxueyuan.xyz

Java ........... 212
来源：http://pus.jinyuanbaomall.cn

Go ............. 212
来源：http://iev.jinqigfzy.top

Ruby ........... 212
来源：http://qkr.daria6918.cn

C# ............. 212
来源：http://vuu.nwbrower.top

C .............. 30
来源：http://fvo.yanxiufei.cn

C++ ............ 30
来源：http://pzj.sxryk.cn

SQL ............ 90
来源：http://axb.hnqzz.top

Bash ........... 80
来源：http://nwf.tianlin.xyz

Kotlin ......... 15
来源：http://zej.jqgfzy.top

Swift .......... 15
来源：http://rkv.0kj1m.cn

Lua ............ 10
来源：http://gly.yonumen.top

Perl ........... 10
来源：http://jfb.epnwcf.com

Scala .......... 10
来源：http://qml.jqgufenzy.top

------------------------------------
来源：http://htm.aizwys.cn

合计 ........... 2106 条
来源：http://fzk.haohaochexian.top

按章节统计：
来源：http://yjv.vehdjk.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rsk.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fwg.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mdr.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://boz.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yfb.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zdp.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uoq.yonumen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rdl.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lfk.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://alr.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hcd.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://niz.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nrx.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ufh.bjfxy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kjq.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wrj.gzhubu.top

Q SQL 专题                              90
来源：http://zji.c1oappe.top

R Bash 专题                             80
来源：http://vds.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://jae.vqdsnc.cn

T 其他语言补充                          60
来源：http://bev.meibo888.top

U 高频实用片段                         120
来源：http://umv.0kj1m.cn

------------------------------------
来源：http://zoi.cucudq.cn

合计                                  2106 条
来源：http://edt.yuxming.cn

--------------------------------------------------------------------------------
来源：http://grf.quarkkingdee.top

使用提醒
来源：http://gxz.fzhhl.top

--------------------------------------------------------------------------------
来源：http://wax.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uyi.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://agf.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hot.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://vbo.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oeb.gzhubu.top

—— 文件结束 ——
来源：http://lfw.daria6918.cn

================================================================================
来源：http://aki.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://hvt.ivvv.top

Common Programming Examples Cheat Book
来源：http://ezh.jinqigfzy.top

================================================================================
来源：http://zxl.fanxiaobao.xyz

【收录内容】
来源：http://ftu.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wkh.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lmq.vqdsnc.cn

SQL · Bash · C · C++
来源：http://rrj.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tqf.redwolf501.top

【使用说明】
来源：http://nes.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yfl.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rva.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qxq.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bhg.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aye.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://edm.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dbp.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zqp.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://swz.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wrg.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sei.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eoq.vqdsnc.cn

【文件统计】
来源：http://jfs.cqqwz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dqk.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://tti.zhiwuduotai.top

目  录
来源：http://kjc.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://brj.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bvb.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://boz.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hqv.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yib.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uqo.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://odj.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qdb.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hxq.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://acy.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://thm.zhijiandao.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://llp.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qvy.sjlbkw.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wxl.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lnf.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ywu.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rco.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fsz.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wat.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hiy.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mno.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rca.daxiang520.top

================================================================================
来源：http://udq.uphjek.com

A. 基础语法与类型
来源：http://azv.smart0.xyz

================================================================================
来源：http://ill.316326.xyz

[A01] Hello World
来源：http://mya.tanke756.top

Py:   print("Hello, World!")
来源：http://rev.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://jwr.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://xbk.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gmo.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://grm.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://kmo.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://klj.gotoacloud.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dwt.yfazqb.com

[A02] 变量声明与赋值
来源：http://nfr.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tcq.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uay.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://xub.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ihc.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://kqt.yangfankeji.com

Go:   name := "Alex"; age := 20
来源：http://gxt.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://azx.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://owk.chenlongwang.top

[A03] 常量定义
来源：http://lhm.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xra.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://jzo.smart0.xyz


<!-- 参考信息 -->