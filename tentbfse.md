代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://dta.shzxlz.cn

sys.stdout.isatty()
来源：http://cdp.uphjek.com

[U40] Py：打印到标准错误
来源：http://lxw.guowangkeji.top

print("err", file=sys.stderr)
来源：http://ftw.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://lqr.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yjx.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://kix.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lzv.fengsongda.top

[U43] PHP：声明命名空间
来源：http://fdy.cucudq.cn

namespace App\Http;
来源：http://pxs.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://gzx.gotoacloud.top

declare(strict_types=1);
来源：http://idl.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://rxz.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://upi.birdmap.top

[U46] PHP：可空类型
来源：http://oxb.daxiang520.top

?string $name = null
来源：http://rlc.yongpay.top

[U47] PHP：联合类型
来源：http://nim.fehbvm.com

int|string $id
来源：http://bdf.guowangkeji.top

[U48] PHP：纯枚举
来源：http://mwh.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cof.zhongyouzk.top

[U49] PHP：只读属性
来源：http://vhv.yuanzhike.top

public readonly string $name
来源：http://ebj.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://ntb.fzhhl.top

public function __construct(private int $id) {}
来源：http://pzo.shuidangran.top

[U51] PHP：数组解构
来源：http://duz.ppjwa.cn

[$a, $b] = $arr;
来源：http://vdh.mhx1999.top

[U52] PHP：箭头函数
来源：http://ugc.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://rpr.52xcode.cn

[U53] PHP：空合并运算符
来源：http://uri.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://poo.daria6918.cn

[U54] PHP：空安全调用
来源：http://zzv.bbcook.cn

$obj?->method()
来源：http://kjh.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://jtj.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://but.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://cwj.hysaishi.cn

f(a: 1, b: 2)
来源：http://xsm.nwbrower.top

[U57] PHP：字符串插值
来源：http://qrs.hnxiangtu.top

"值: {$a}"
来源：http://ncl.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://zjp.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cyn.yonumen.top

[U59] PHP：自定义排序
来源：http://qeu.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eud.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://xxp.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wtg.fzhhl.top

[U61] PHP：正则
来源：http://kcx.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tpv.tianlin.xyz

[U62] PHP：日期对象
来源：http://uac.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hjw.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://lkc.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wqd.zhixingplan.top

[U64] PHP：目录遍历
来源：http://eeh.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://bcq.kuanghao11.cn

[U65] PHP：会话
来源：http://slj.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://uvg.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://far.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ocv.jianghu66.top

[U67] PHP：处理文件上传
来源：http://edy.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iym.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://pri.gogol.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://akg.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://jub.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://luv.iojbl.cn

[U70] PHP：PDO 事务
来源：http://fog.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mzo.epnwcf.com

[U71] PHP：抛出异常
来源：http://gbv.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://gnz.xziqi.cn

[U72] PHP：写错误日志
来源：http://yfh.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://ydf.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://ldl.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://vxc.hammf.cn

[U74] PHP：读取环境变量
来源：http://dus.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://uop.316326.xyz

[U75] PHP：依赖注入
来源：http://ofo.yj202588.top

composer require psr/container
来源：http://enb.hfpthk.cn

[U76] PHP：简单路由
来源：http://dli.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uqa.tian-w.cn

[U77] PHP：模板渲染
来源：http://gpe.havefunace.top

composer require twig/twig
来源：http://gis.quarkkingdee.top

[U78] PHP：单元测试
来源：http://scw.birdmap.top

composer require --dev phpunit/phpunit
来源：http://jep.hammf.cn

[U79] PHP：静态分析
来源：http://slh.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://wme.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://ddy.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ljq.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://qwr.zdqjudy.top

npm init -y;  npm i express
来源：http://fxb.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://tph.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sqt.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://ipu.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dcv.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://fnh.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://txz.haohaochexian.top

[U85] JS：可选链
来源：http://yjp.zdqjudy.top

a?.b?.c
来源：http://rzv.birdmap.top

[U86] JS：空值合并
来源：http://tfk.zhiwuduotai.top

a ?? b
来源：http://sue.guannengcc.top

[U87] JS：解构默认值
来源：http://khl.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://jhp.yonumen.top

[U88] JS：对象展开合并
来源：http://ayd.ywan-chungtsiang.top

{ ...a, ...b }
来源：http://kcb.cdnleiting.top

[U89] JS：数组去重
来源：http://env.yj20258888.top

[...new Set(arr)]
来源：http://ofp.redwolf501.top

[U90] JS：数字数组排序
来源：http://esw.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://ktm.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://qjy.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dit.sysykeji.top

[U92] JS：深拷贝
来源：http://htl.zhengqikj.top

structuredClone(obj)
来源：http://tca.sysykeji.top

[U93] JS：模板字符串
来源：http://vti.nanxuanxn.top

`共 ${n} 条`
来源：http://dck.hnxiangtu.top

[U94] JS：箭头函数
来源：http://jrm.ybcxt.top

const double = x => x * 2;
来源：http://bvq.hcnkem.com

[U95] JS：Promise 包装
来源：http://jfa.tanke756.top

new Promise((resolve, reject) => {})
来源：http://wtj.yongpay.top

[U96] JS：async/await 与异常
来源：http://ate.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pca.xylfe.cn

[U97] JS：并发请求
来源：http://ysk.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://aqw.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://fhr.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zyk.cheryme.top

[U99] JS：事件监听
来源：http://jaw.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://noi.tanke756.top

[U100] JS：DOM 查询
来源：http://qho.fanxiaobao.xyz

document.querySelector(".item")
来源：http://exd.hammf.cn

[U101] JS：classList 操作
来源：http://yyr.vqdsnc.cn

el.classList.toggle("active")
来源：http://jnj.ehwqpu.com

[U102] JS：本地存储
来源：http://dxu.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wtm.jinqigufen.top

[U103] JS：定时器
来源：http://pvf.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oky.hfpthk.cn

[U104] JS：防抖
来源：http://dua.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsw.fanxiaobao.xyz

[U105] JS：节流
来源：http://shc.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pxp.epnwcf.com

[U106] JS：日期格式化
来源：http://iyh.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zto.tanke756.top

[U107] JS：数字千分位
来源：http://rnb.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://myt.tian-w.cn

[U108] JS：随机整数
来源：http://osv.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eyh.9152youxi.cn

[U109] JS：数组分组
来源：http://xtw.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://beb.xuanzx.com

[U110] JS：数组分块
来源：http://zyf.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mxh.fengsongda.top

[U111] JS：对象转 Map
来源：http://hoa.cdnleiting.top

new Map(Object.entries(obj))
来源：http://bwz.zdqjudy.top

[U112] JS：字符串补位
来源：http://jky.jinqigufen.top

"7".padStart(3, "0")
来源：http://pfu.cashguo.top

[U113] JS：正则替换全部
来源：http://afk.shuidangran.top

s.replaceAll("a", "b")
来源：http://ufn.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://kwa.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://woe.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://nes.yuxming.cn

crypto.randomUUID()
来源：http://jtf.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://luc.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://wyq.guowangkeji.top

[U117] JS：单元测试
来源：http://tsb.316326.xyz

npm i -D vitest;  npx vitest
来源：http://mzi.wangdashe.top

[U118] JS：开发服务器
来源：http://cdj.ctjpmb.com

npm i -D vite;  npx vite
来源：http://tvm.hnqzz.top

[U119] JS：生产构建
来源：http://pye.zhaomingkeji.xyz

npx vite build
来源：http://rzv.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://tmm.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://ajf.zhongyouzk.top

================================================================================
来源：http://juc.cheryme.top

统计汇总
来源：http://xcr.meibo888.top

================================================================================
来源：http://rom.tian-w.cn

按语言统计（条）：
来源：http://zuc.zhijiandao.cn

Python ......... 252
来源：http://qtl.nanxinkj.top

PHP ............ 252
来源：http://ilv.andypj.xyz

JavaScript ..... 252
来源：http://thj.sufxvd.cn

TypeScript ..... 212
来源：http://wxx.ehwqpu.com

Java ........... 212
来源：http://dwj.ywan-chungtsiang.top

Go ............. 212
来源：http://ujf.havefunace.top

Ruby ........... 212
来源：http://rla.jqgufenzy.top

C# ............. 212
来源：http://grp.wangdashe.top

C .............. 30
来源：http://xao.nwbrower.top

C++ ............ 30
来源：http://whl.jianghu66.top

SQL ............ 90
来源：http://qvs.tarul.cn

Bash ........... 80
来源：http://mfk.kuanghao11.cn

Kotlin ......... 15
来源：http://iib.yj20258888.top

Swift .......... 15
来源：http://dnc.cqqwz.cn

Lua ............ 10
来源：http://mtu.cheryme.top

Perl ........... 10
来源：http://mfv.yvedp.cn

Scala .......... 10
来源：http://arm.xuanzx.com

------------------------------------
来源：http://dux.pycfn.com

合计 ........... 2106 条
来源：http://iop.nwbrower.top

按章节统计：
来源：http://sos.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ssg.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jii.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://key.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lkp.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iun.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://adk.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eul.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cay.cucudq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rdb.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xlr.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pic.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://usv.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qgm.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eil.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://opv.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wvt.aizwys.cn

Q SQL 专题                              90
来源：http://lkn.ehwqpu.com

R Bash 专题                             80
来源：http://wrk.aibaodan.cn

S C / C++ 专题                          60
来源：http://sza.jlsjyb.cn

T 其他语言补充                          60
来源：http://yhe.hysaishi.cn

U 高频实用片段                         120
来源：http://mlg.vehdjk.com

------------------------------------
来源：http://ivi.tarul.cn

合计                                  2106 条
来源：http://djy.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://buf.zhaomingkeji.xyz

使用提醒
来源：http://pgo.uphjek.com

--------------------------------------------------------------------------------
来源：http://gsg.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tuz.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ihm.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://giy.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nlb.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qaw.snrcjt.cn

—— 文件结束 ——
来源：http://ymn.zhaomingkeji.xyz

================================================================================
来源：http://hdl.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://ugi.hywenlv.cn

Common Programming Examples Cheat Book
来源：http://xza.hysaishi.cn

================================================================================
来源：http://shd.ybcxt.top

【收录内容】
来源：http://yqy.c1oappe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://orn.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jdb.smart0.xyz

SQL · Bash · C · C++
来源：http://ctq.jinyuanbaomall.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://asq.zycfv.cn

【使用说明】
来源：http://ryo.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tmm.sweek.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ghm.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ghg.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aah.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ezg.chenjidiqi.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iay.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ekx.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cxl.cucudq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kil.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xlk.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://whd.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://haf.jlsjyb.cn

【文件统计】
来源：http://rln.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cwg.pycfn.com

--------------------------------------------------------------------------------
来源：http://xvu.jinyuanbaomall.cn

目  录
来源：http://wcb.c1oappe.top

--------------------------------------------------------------------------------
来源：http://kfy.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bwd.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://icx.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://daa.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kem.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iab.pycfn.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pxh.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dtj.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fen.tanke756.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://egc.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rgz.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uai.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rhu.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aib.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sod.yongpay.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cmz.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dko.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://phd.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fjx.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uti.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kys.havefunace.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ujb.vehdjk.com

================================================================================
来源：http://rcz.daxiang520.top

A. 基础语法与类型
来源：http://dim.ivvv.top

================================================================================
来源：http://ljl.andypj.xyz

[A01] Hello World
来源：http://rst.cucudq.cn

Py:   print("Hello, World!")
来源：http://hoi.zhongyouzk.top

PHP:  echo "Hello, World!";
来源：http://abu.havefunace.top

JS:   console.log("Hello, World!");
来源：http://cgx.yangfankeji.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jfs.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://dwp.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://ghu.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://pll.zhaomingkeji.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://klf.zhoulong.xyz

[A02] 变量声明与赋值
来源：http://fsr.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://byh.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bml.chenjidiqi.icu

JS:   let name = "Alex"; const age = 20;
来源：http://imx.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qgd.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://qas.zhoulong.xyz

Go:   name := "Alex"; age := 20
来源：http://pnv.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://cau.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://jdv.shzxlz.cn

[A03] 常量定义
来源：http://xem.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ktn.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://czz.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://oyu.sufxvd.cn

TS:   const PI: number = 3.14159;
来源：http://gmv.tarul.cn

Java: static final double PI = 3.14159;
来源：http://xgd.ybcxt.top

Go:   const PI = 3.14159
来源：http://wxe.52xcode.cn

Ruby: PI = 3.14159
来源：http://wtd.yj202588.top

C#:   const double PI = 3.14159;
来源：http://ics.meibo888.top

[A04] 判断变量类型
来源：http://rfp.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://xar.ydzc1.top


<!-- 参考信息 -->