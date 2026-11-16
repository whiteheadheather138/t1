代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://izn.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://sus.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://nij.shzxlz.cn

print("err", file=sys.stderr)
来源：http://vaf.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://yee.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tsr.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://jve.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cpn.yvedp.cn

[U43] PHP：声明命名空间
来源：http://xbf.tianlin.xyz

namespace App\Http;
来源：http://rzn.fengsongda.top

[U44] PHP：开启严格类型
来源：http://csv.chenlongwang.top

declare(strict_types=1);
来源：http://zqf.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://zvl.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://zwz.jianghu66.top

[U46] PHP：可空类型
来源：http://mgl.xingfuxueyuan.xyz

?string $name = null
来源：http://smz.yj20258888.top

[U47] PHP：联合类型
来源：http://xxo.xziqi.cn

int|string $id
来源：http://beb.ctjpmb.com

[U48] PHP：纯枚举
来源：http://wvb.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nlu.jinqigufen.top

[U49] PHP：只读属性
来源：http://pgg.ehwqpu.com

public readonly string $name
来源：http://bmw.meibo888.top

[U50] PHP：构造器属性提升
来源：http://mwh.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://kuc.tanke756.top

[U51] PHP：数组解构
来源：http://zey.ppjwa.cn

[$a, $b] = $arr;
来源：http://bxf.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://mqe.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://jea.cucudq.cn

[U53] PHP：空合并运算符
来源：http://neh.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://fqp.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://ets.snrcjt.cn

$obj?->method()
来源：http://jpt.nanxinkj.top

[U55] PHP：match 表达式
来源：http://pva.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dba.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://ufq.bjfxy.top

f(a: 1, b: 2)
来源：http://ebl.redwolf501.top

[U57] PHP：字符串插值
来源：http://lgg.yj20258888.top

"值: {$a}"
来源：http://tjc.yj20258888.top

[U58] PHP：数组三件套
来源：http://htn.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xhe.jinqigufen.top

[U59] PHP：自定义排序
来源：http://sxe.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wsv.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://gbq.hammf.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bok.pycfn.com

[U61] PHP：正则
来源：http://vea.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ptc.ehwqpu.com

[U62] PHP：日期对象
来源：http://opo.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gnp.nwbrower.top

[U63] PHP：文件读写
来源：http://dhe.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sal.tianlin.xyz

[U64] PHP：目录遍历
来源：http://xhc.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://whd.andypj.xyz

[U65] PHP：会话
来源：http://dqa.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wgq.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://pah.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tmj.yj20258888.top

[U67] PHP：处理文件上传
来源：http://tbh.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ghy.yongpay.top

[U68] PHP：PDO 连接
来源：http://mam.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kwd.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://oni.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zhr.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://bjj.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vgp.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://qpb.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://bkb.zdbjq.cn

[U72] PHP：写错误日志
来源：http://eun.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://xyx.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://ucy.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://osj.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://eat.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://hbb.ivvv.top

[U75] PHP：依赖注入
来源：http://jss.xziqi.cn

composer require psr/container
来源：http://ago.yongpay.top

[U76] PHP：简单路由
来源：http://ney.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zen.guannengcc.top

[U77] PHP：模板渲染
来源：http://shi.pengpengdd.cyou

composer require twig/twig
来源：http://xyd.fzhhl.top

[U78] PHP：单元测试
来源：http://nzm.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://wus.daxiang520.top

[U79] PHP：静态分析
来源：http://otp.shanyushiyangkeji.top

composer require --dev phpstan/phpstan
来源：http://mmw.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://pke.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uis.c1oappe.top

[U81] JS：初始化项目
来源：http://bcm.gzhubu.top

npm init -y;  npm i express
来源：http://ttr.fehbvm.com

[U82] JS：package.json 脚本
来源：http://hhz.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sdp.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://njy.cashguo.top

export const a = 1;  import { a } from "./m.js";
来源：http://dxe.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://ydg.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cse.andypj.xyz

[U85] JS：可选链
来源：http://xze.wangdashe.top

a?.b?.c
来源：http://uio.chenlongwang.top

[U86] JS：空值合并
来源：http://nsk.ydzc1.top

a ?? b
来源：http://kmx.52xcode.cn

[U87] JS：解构默认值
来源：http://tgi.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://lbr.pycfn.com

[U88] JS：对象展开合并
来源：http://fjm.svipenyu.cn

{ ...a, ...b }
来源：http://qdt.0kj1m.cn

[U89] JS：数组去重
来源：http://qkf.jinqigfzy.top

[...new Set(arr)]
来源：http://ixo.cucudq.cn

[U90] JS：数字数组排序
来源：http://bmd.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://gna.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://uap.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kon.tarul.cn

[U92] JS：深拷贝
来源：http://ikj.9152youxi.cn

structuredClone(obj)
来源：http://ksj.zhixingplan.top

[U93] JS：模板字符串
来源：http://nvb.pycfn.com

`共 ${n} 条`
来源：http://tbi.9152youxi.cn

[U94] JS：箭头函数
来源：http://mei.havefunace.top

const double = x => x * 2;
来源：http://ycl.ppjwa.cn

[U95] JS：Promise 包装
来源：http://vnp.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://rxa.iojbl.cn

[U96] JS：async/await 与异常
来源：http://hvn.guannengcc.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iht.jinqigufen.top

[U97] JS：并发请求
来源：http://ynl.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vgp.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://zkq.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pxl.tian-w.cn

[U99] JS：事件监听
来源：http://dpt.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://iua.wangdashe.top

[U100] JS：DOM 查询
来源：http://tvy.nanxuanxn.top

document.querySelector(".item")
来源：http://oyt.sweek.top

[U101] JS：classList 操作
来源：http://hwq.hcnkem.com

el.classList.toggle("active")
来源：http://chn.jqgfzy.top

[U102] JS：本地存储
来源：http://wan.jinyuanbaomall.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://etv.cdnleiting.top

[U103] JS：定时器
来源：http://wif.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tqi.0kj1m.cn

[U104] JS：防抖
来源：http://uuq.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wqe.jiagoushi.top

[U105] JS：节流
来源：http://hil.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zho.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://zcv.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zqp.fktsv.cn

[U107] JS：数字千分位
来源：http://hiq.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hxz.hesvh.cn

[U108] JS：随机整数
来源：http://xne.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zgo.andypj.xyz

[U109] JS：数组分组
来源：http://vkr.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://lpm.hcnkem.com

[U110] JS：数组分块
来源：http://owr.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yhk.yj20258.top

[U111] JS：对象转 Map
来源：http://ick.zdqjudy.top

new Map(Object.entries(obj))
来源：http://nah.c1oappe.top

[U112] JS：字符串补位
来源：http://yma.yangfankeji.com

"7".padStart(3, "0")
来源：http://pzy.jiagoushi.top

[U113] JS：正则替换全部
来源：http://inb.vehdjk.com

s.replaceAll("a", "b")
来源：http://mqk.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://ywc.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rpq.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://tos.yfazqb.com

crypto.randomUUID()
来源：http://pqa.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://yyv.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://zjc.sysykeji.top

[U117] JS：单元测试
来源：http://qbx.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://jfg.tarul.cn

[U118] JS：开发服务器
来源：http://knh.snrcjt.cn

npm i -D vite;  npx vite
来源：http://kta.meibo888.top

[U119] JS：生产构建
来源：http://uia.hongshengwenyu.top

npx vite build
来源：http://frf.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://mkb.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://kou.zhongyouzk.top

================================================================================
来源：http://chh.yj202588.top

统计汇总
来源：http://oia.sufxvd.cn

================================================================================
来源：http://fhc.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://mxi.zhongyouzk.top

Python ......... 252
来源：http://xsz.0kj1m.cn

PHP ............ 252
来源：http://fez.sjlbkw.cn

JavaScript ..... 252
来源：http://sjl.yanxiufei.cn

TypeScript ..... 212
来源：http://ddx.yuanzhike.top

Java ........... 212
来源：http://gmc.zhengqikj.top

Go ............. 212
来源：http://rpz.tianlin.xyz

Ruby ........... 212
来源：http://ksb.shanyushiyangtech.top

C# ............. 212
来源：http://fbf.zhengqikj.top

C .............. 30
来源：http://yoo.havefunace.top

C++ ............ 30
来源：http://upq.ywan-chungtsiang.top

SQL ............ 90
来源：http://zhe.jinqigfzy.top

Bash ........... 80
来源：http://tjl.nanxuanxn.top

Kotlin ......... 15
来源：http://rpl.xuetiantiany.cn

Swift .......... 15
来源：http://tmn.shangyingyoupin.top

Lua ............ 10
来源：http://yyw.fktsv.cn

Perl ........... 10
来源：http://ykv.ydjk.org.cn

Scala .......... 10
来源：http://tof.gogol.net.cn

------------------------------------
来源：http://bes.daxiang520.top

合计 ........... 2106 条
来源：http://goh.sufxvd.cn

按章节统计：
来源：http://uum.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kkm.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://scb.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mpa.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bth.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mzj.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oao.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nhj.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://chl.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://suv.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://psh.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://daa.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wpx.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ahc.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ekp.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://flx.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wut.redwolf501.top

Q SQL 专题                              90
来源：http://clk.meibo888.top

R Bash 专题                             80
来源：http://tlv.guowangkeji.top

S C / C++ 专题                          60
来源：http://tou.ybcxt.top

T 其他语言补充                          60
来源：http://tcf.snrcjt.cn

U 高频实用片段                         120
来源：http://rqm.smart0.xyz

------------------------------------
来源：http://nuo.ppjwa.cn

合计                                  2106 条
来源：http://zrs.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://ici.zhixingplan.top

使用提醒
来源：http://zlz.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://hlc.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://erv.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lpu.andypj.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kys.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://pfs.kuanghao11.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vko.hongshengwenyu.top

—— 文件结束 ——
来源：http://qgz.xingfuxueyuan.xyz

================================================================================
来源：http://glp.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://yvs.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://qrq.ydzc1.top

================================================================================
来源：http://djt.dashuyun.cn

【收录内容】
来源：http://iha.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ofu.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gpn.cdnleiting.top

SQL · Bash · C · C++
来源：http://zpy.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hog.ivvv.top

【使用说明】
来源：http://xwi.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ord.shanyushiyangtech.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tfr.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rcm.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://naf.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zhn.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tqm.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jht.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sls.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vra.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oom.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lto.c1oappe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tad.xinyue.icu

【文件统计】
来源：http://mht.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cfh.daxiang520.top

--------------------------------------------------------------------------------
来源：http://guq.dianchejie.cn

目  录
来源：http://ctq.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://nmq.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gxz.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hec.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ctz.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vlp.xingfuxueyuan.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eho.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ruj.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gvn.jlsjyb.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yyh.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uca.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tis.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fhl.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hyr.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zwl.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kel.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yxk.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fvu.zhixingplan.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zvq.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kgn.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pfq.yj20258.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fwd.shuidangran.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tyu.ppjwa.cn

================================================================================
来源：http://hol.jiagoushi.top

A. 基础语法与类型
来源：http://tfx.jqgfzy.top

================================================================================
来源：http://yvd.jinqigfzy.top

[A01] Hello World
来源：http://vik.yueranfly.top

Py:   print("Hello, World!")
来源：http://thj.tanke756.top

PHP:  echo "Hello, World!";
来源：http://ehl.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://zrc.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lrg.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://eyd.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://rll.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://owx.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://wmo.sufxvd.cn

[A02] 变量声明与赋值
来源：http://wmp.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bky.guannengcc.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ctt.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://gmn.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ymf.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://scm.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://qwy.shzxlz.cn

Ruby: name = "Alex"; age = 20
来源：http://orj.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://qzc.gaohongyu789.top

[A03] 常量定义
来源：http://wfb.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bey.shanyushiyangtech.top

PHP:  const PI = 3.14159;
来源：http://uiq.feifeiyinyue.top

JS:   const PI = 3.14159;
来源：http://hlr.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://iuh.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://pyk.ydjk.org.cn

Go:   const PI = 3.14159
来源：http://yji.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://aqk.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://uhi.fzhhl.top

[A04] 判断变量类型
来源：http://teh.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ivp.aizwys.cn


<!-- 参考信息 -->