代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://gik.shzxlz.cn

sys.stdout.isatty()
来源：http://eas.xylfe.cn

[U40] Py：打印到标准错误
来源：http://fcs.havefunace.top

print("err", file=sys.stderr)
来源：http://uqh.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://klm.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wwj.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://kxc.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://srr.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://ujd.gaohongyu789.top

namespace App\Http;
来源：http://ipx.meibo888.top

[U44] PHP：开启严格类型
来源：http://vmh.redwolf501.top

declare(strict_types=1);
来源：http://aym.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://tmv.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uga.sjlbkw.cn

[U46] PHP：可空类型
来源：http://ldd.uphjek.com

?string $name = null
来源：http://cql.pycfn.com

[U47] PHP：联合类型
来源：http://rwk.sufxvd.cn

int|string $id
来源：http://ecv.hcnkem.com

[U48] PHP：纯枚举
来源：http://prn.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aza.iojbl.cn

[U49] PHP：只读属性
来源：http://ymt.zhiwuduotai.top

public readonly string $name
来源：http://xmc.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://ubg.ybcxt.top

public function __construct(private int $id) {}
来源：http://skb.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://rmi.52xcode.cn

[$a, $b] = $arr;
来源：http://kho.hammf.cn

[U52] PHP：箭头函数
来源：http://dkj.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://mwo.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://iuk.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://pgl.yongpay.top

[U54] PHP：空安全调用
来源：http://xyh.gotoacloud.top

$obj?->method()
来源：http://aun.redwolf501.top

[U55] PHP：match 表达式
来源：http://qik.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cbq.smart0.xyz

[U56] PHP：命名参数
来源：http://xjx.mhx1999.top

f(a: 1, b: 2)
来源：http://vep.tarul.cn

[U57] PHP：字符串插值
来源：http://imk.daxiang520.top

"值: {$a}"
来源：http://ksn.xziqi.cn

[U58] PHP：数组三件套
来源：http://dcj.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nil.yfazqb.com

[U59] PHP：自定义排序
来源：http://rej.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lnk.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://vps.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fou.zhijiandao.cn

[U61] PHP：正则
来源：http://ndf.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mks.jinqigfzy.top

[U62] PHP：日期对象
来源：http://hli.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kuw.mhx1999.top

[U63] PHP：文件读写
来源：http://ydi.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kdm.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://edp.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://agb.haohaochexian.top

[U65] PHP：会话
来源：http://eip.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ivt.tanke756.top

[U66] PHP：设置 Cookie
来源：http://ivn.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dbo.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://dqe.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fgy.yj20258888.top

[U68] PHP：PDO 连接
来源：http://eov.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rpm.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://ycs.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rup.yfazqb.com

[U70] PHP：PDO 事务
来源：http://qih.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://slt.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://bsh.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://ydp.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://tuk.yongpay.top

error_log("失败: " . $e->getMessage());
来源：http://ctt.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://vgu.yj202588.top

parse_ini_file("config.ini", true)
来源：http://uhs.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://hma.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://gqf.shangyingyoupin.top

[U75] PHP：依赖注入
来源：http://ifr.aizwys.cn

composer require psr/container
来源：http://ril.jinqigfzy.top

[U76] PHP：简单路由
来源：http://ykr.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yxc.birdmap.top

[U77] PHP：模板渲染
来源：http://dcb.hammf.cn

composer require twig/twig
来源：http://wcd.yj20258888.top

[U78] PHP：单元测试
来源：http://wsi.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://fxs.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://hhk.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://kdg.tarul.cn

[U80] PHP：代码规范修复
来源：http://bna.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wmg.xylfe.cn

[U81] JS：初始化项目
来源：http://pcy.shzxlz.cn

npm init -y;  npm i express
来源：http://uxv.xuanzx.com

[U82] JS：package.json 脚本
来源：http://esz.jyoumei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hoz.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://pxt.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://iqa.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://ntj.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zrf.svipenyu.cn

[U85] JS：可选链
来源：http://pud.sufxvd.cn

a?.b?.c
来源：http://rzr.xylfe.cn

[U86] JS：空值合并
来源：http://nmb.daria6918.cn

a ?? b
来源：http://jxn.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://uns.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://vrv.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://por.yuanzhike.top

{ ...a, ...b }
来源：http://iuc.shzxlz.cn

[U89] JS：数组去重
来源：http://cft.yj202588.top

[...new Set(arr)]
来源：http://hqf.xuanzx.com

[U90] JS：数字数组排序
来源：http://nww.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://pft.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://wjt.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qnx.xuetiantiany.cn

[U92] JS：深拷贝
来源：http://ivd.fktsv.cn

structuredClone(obj)
来源：http://ujm.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://faz.nanxinkj.top

`共 ${n} 条`
来源：http://emc.daxiang520.top

[U94] JS：箭头函数
来源：http://ggm.gogol.net.cn

const double = x => x * 2;
来源：http://tan.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://hzx.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://nab.xziqi.cn

[U96] JS：async/await 与异常
来源：http://wgx.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eoa.fktsv.cn

[U97] JS：并发请求
来源：http://tyl.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://doi.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://mrv.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pdy.yvedp.cn

[U99] JS：事件监听
来源：http://rsm.hcnkem.com

el.addEventListener("click", e => {})
来源：http://mxk.cqqwz.cn

[U100] JS：DOM 查询
来源：http://ipn.dashuyun.cn

document.querySelector(".item")
来源：http://uuq.yj202588.top

[U101] JS：classList 操作
来源：http://kmj.jinqigufen.top

el.classList.toggle("active")
来源：http://jku.gotoacloud.top

[U102] JS：本地存储
来源：http://vbz.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uqq.cdnleiting.top

[U103] JS：定时器
来源：http://ptv.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cvp.dianchejie.cn

[U104] JS：防抖
来源：http://sin.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lyy.yj20258888.top

[U105] JS：节流
来源：http://ltv.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rik.sysykeji.top

[U106] JS：日期格式化
来源：http://czj.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wrv.xinyue.icu

[U107] JS：数字千分位
来源：http://ohl.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tky.jiagoushi.top

[U108] JS：随机整数
来源：http://dcz.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nmu.hysaishi.cn

[U109] JS：数组分组
来源：http://hxf.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://uts.sufxvd.cn

[U110] JS：数组分块
来源：http://imy.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pia.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://dqz.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://wys.jqgfzy.top

[U112] JS：字符串补位
来源：http://udn.havefunace.top

"7".padStart(3, "0")
来源：http://vsi.sxryk.cn

[U113] JS：正则替换全部
来源：http://nxb.yangfankeji.com

s.replaceAll("a", "b")
来源：http://sxd.yuxming.cn

[U114] JS：JSON 深比较
来源：http://uhe.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lmc.tanke756.top

[U115] JS：生成 UUID
来源：http://xxw.sxryk.cn

crypto.randomUUID()
来源：http://phg.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://kji.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://amf.pycfn.com

[U117] JS：单元测试
来源：http://rvk.hammf.cn

npm i -D vitest;  npx vitest
来源：http://saw.yuxming.cn

[U118] JS：开发服务器
来源：http://mvy.jianghu66.top

npm i -D vite;  npx vite
来源：http://oas.zdbjq.cn

[U119] JS：生产构建
来源：http://mjg.uphjek.com

npx vite build
来源：http://klj.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://dgk.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://vrx.jqgufenzy.top

================================================================================
来源：http://bkv.epnwcf.com

统计汇总
来源：http://eet.shanyushiyangkeji.top

================================================================================
来源：http://hcr.birdmap.top

按语言统计（条）：
来源：http://say.nanxinkj.top

Python ......... 252
来源：http://rfk.zhengqikj.top

PHP ............ 252
来源：http://sqx.tarul.cn

JavaScript ..... 252
来源：http://ffv.ehwqpu.com

TypeScript ..... 212
来源：http://ozx.zhengqikj.top

Java ........... 212
来源：http://jnp.zhiwuduotai.top

Go ............. 212
来源：http://vii.316326.xyz

Ruby ........... 212
来源：http://wtd.epnwcf.com

C# ............. 212
来源：http://rwl.xziqi.cn

C .............. 30
来源：http://kgv.zhiwuduotai.top

C++ ............ 30
来源：http://qvj.yonumen.top

SQL ............ 90
来源：http://gjw.hongshengwenyu.top

Bash ........... 80
来源：http://mzp.guowangkeji.top

Kotlin ......... 15
来源：http://qqm.pycfn.com

Swift .......... 15
来源：http://dnu.yvedp.cn

Lua ............ 10
来源：http://fxl.yuxming.cn

Perl ........... 10
来源：http://xwf.hysaishi.cn

Scala .......... 10
来源：http://qob.aizwys.cn

------------------------------------
来源：http://qsl.andypj.xyz

合计 ........... 2106 条
来源：http://out.pengpengdd.cyou

按章节统计：
来源：http://pdx.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vac.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cxb.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aqq.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eqa.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://igs.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sti.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iqb.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hio.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hzz.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tfi.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dpj.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lxc.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://akk.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fyh.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qsk.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jyd.mhx1999.top

Q SQL 专题                              90
来源：http://sgc.epnwcf.com

R Bash 专题                             80
来源：http://xog.yvedp.cn

S C / C++ 专题                          60
来源：http://zsi.yonumen.top

T 其他语言补充                          60
来源：http://azj.ivvv.top

U 高频实用片段                         120
来源：http://mkw.gogol.net.cn

------------------------------------
来源：http://xmq.zdbjq.cn

合计                                  2106 条
来源：http://rob.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://srt.hcnkem.com

使用提醒
来源：http://vkk.birdmap.top

--------------------------------------------------------------------------------
来源：http://xte.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vmx.chenjidiqi.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vtx.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xnd.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jfz.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gcd.ydzc1.top

—— 文件结束 ——
来源：http://fxp.yj20258888.top

================================================================================
来源：http://zat.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://glx.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://zlr.jqgufenzy.top

================================================================================
来源：http://hsf.hnxiangtu.top

【收录内容】
来源：http://mjy.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ude.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://div.sysykeji.top

SQL · Bash · C · C++
来源：http://tqk.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ego.jinghuilouyu.cn

【使用说明】
来源：http://lpj.fktsv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ygx.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://czj.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://acg.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zwv.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jyb.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aan.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tku.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://umr.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cnu.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dvt.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qpk.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ofa.yangfankeji.com

【文件统计】
来源：http://tuc.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tqd.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://shm.hammf.cn

目  录
来源：http://uye.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://tfx.nanxuanxn.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yus.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qhh.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ldz.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://roo.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jew.zdqjudy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rdz.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bvk.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uxt.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://efa.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qen.hcnkem.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hno.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cfc.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fty.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sth.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mrp.zhiwuduotai.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://edl.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lym.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ojr.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mkq.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ulc.pycfn.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wkz.yfazqb.com

================================================================================
来源：http://qyt.fanxiaobao.xyz

A. 基础语法与类型
来源：http://epr.havefunace.top

================================================================================
来源：http://vnn.gogol.net.cn

[A01] Hello World
来源：http://xvg.xuanzx.com

Py:   print("Hello, World!")
来源：http://eva.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://ewo.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://yhi.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tzx.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://pbo.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://pmo.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://hyh.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://azx.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://ovd.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://klo.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ryo.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://scw.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kdf.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://tpo.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://crg.yonumen.top

Ruby: name = "Alex"; age = 20
来源：http://hdo.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://tnz.yueranfly.top

[A03] 常量定义
来源：http://pmd.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blc.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://mnq.fehbvm.com

JS:   const PI = 3.14159;
来源：http://mqd.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://dyc.epnwcf.com

Java: static final double PI = 3.14159;
来源：http://wgt.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://gwb.dianchejie.cn

Ruby: PI = 3.14159
来源：http://wsb.haohaochexian.top

C#:   const double PI = 3.14159;
来源：http://fbp.gaohongyu789.top

[A04] 判断变量类型
来源：http://qkn.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gey.birdmap.top


<!-- 参考信息 -->