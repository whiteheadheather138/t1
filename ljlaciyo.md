代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://erm.aizwys.cn

sys.stdout.isatty()
来源：http://fro.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://pzn.fehbvm.com

print("err", file=sys.stderr)
来源：http://wxu.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://qub.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qjy.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://elf.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jou.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://yju.ydjk.org.cn

namespace App\Http;
来源：http://iey.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://zcc.jianghu66.top

declare(strict_types=1);
来源：http://occ.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://qcs.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zpq.hcnkem.com

[U46] PHP：可空类型
来源：http://ekv.guannengcc.top

?string $name = null
来源：http://age.jiagoushi.top

[U47] PHP：联合类型
来源：http://laa.shzxlz.cn

int|string $id
来源：http://kyx.jiagoushi.top

[U48] PHP：纯枚举
来源：http://rpy.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qer.aibaodan.cn

[U49] PHP：只读属性
来源：http://uxv.birdmap.top

public readonly string $name
来源：http://ixw.fktsv.cn

[U50] PHP：构造器属性提升
来源：http://bvt.hywenlv.cn

public function __construct(private int $id) {}
来源：http://bbs.yueranfly.top

[U51] PHP：数组解构
来源：http://wzm.cucudq.cn

[$a, $b] = $arr;
来源：http://sat.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://itn.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://hla.cheryme.top

[U53] PHP：空合并运算符
来源：http://ccf.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://abv.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://zqn.hammf.cn

$obj?->method()
来源：http://tor.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://xly.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dgl.xziqi.cn

[U56] PHP：命名参数
来源：http://dpu.ybcxt.top

f(a: 1, b: 2)
来源：http://orw.pycfn.com

[U57] PHP：字符串插值
来源：http://xsw.fktsv.cn

"值: {$a}"
来源：http://klp.jianghu66.top

[U58] PHP：数组三件套
来源：http://vpj.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iha.haohaochexian.top

[U59] PHP：自定义排序
来源：http://osb.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uzx.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://enb.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hqa.bjfxy.top

[U61] PHP：正则
来源：http://qwx.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zra.nanxinkj.top

[U62] PHP：日期对象
来源：http://mud.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kxi.vehdjk.com

[U63] PHP：文件读写
来源：http://dxa.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wvm.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://bjn.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://kmd.chenzaomai.com

[U65] PHP：会话
来源：http://hyk.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qol.tarul.cn

[U66] PHP：设置 Cookie
来源：http://rox.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ogm.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://awa.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oyq.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://obv.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fnb.yj202588.top

[U69] PHP：PDO 预处理
来源：http://svo.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://owx.52xcode.cn

[U70] PHP：PDO 事务
来源：http://ecx.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rbu.yj202588.top

[U71] PHP：抛出异常
来源：http://tjv.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://vxo.jqgfzy.top

[U72] PHP：写错误日志
来源：http://oli.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://obo.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://rmc.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://xbk.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://ggh.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://rxu.shuidangran.top

[U75] PHP：依赖注入
来源：http://gbm.tanke756.top

composer require psr/container
来源：http://aku.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://sfo.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kag.guannengcc.top

[U77] PHP：模板渲染
来源：http://ehn.aizwys.cn

composer require twig/twig
来源：http://ukm.uphjek.com

[U78] PHP：单元测试
来源：http://iai.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://gqt.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://yuf.yj20258.top

composer require --dev phpstan/phpstan
来源：http://lml.yj20258888.top

[U80] PHP：代码规范修复
来源：http://nwr.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sue.nanxinkj.top

[U81] JS：初始化项目
来源：http://uty.quarkkingdee.top

npm init -y;  npm i express
来源：http://jwv.ivvv.top

[U82] JS：package.json 脚本
来源：http://dsh.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aeh.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://fuy.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://isq.cashguo.top

[U84] JS：CommonJS 写法
来源：http://vkv.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lsv.iojbl.cn

[U85] JS：可选链
来源：http://tfn.hesvh.cn

a?.b?.c
来源：http://nhy.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://yyg.ydjk.org.cn

a ?? b
来源：http://rzm.meibo888.top

[U87] JS：解构默认值
来源：http://dmk.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://dsm.redwolf501.top

[U88] JS：对象展开合并
来源：http://qna.redwolf501.top

{ ...a, ...b }
来源：http://yok.hcnkem.com

[U89] JS：数组去重
来源：http://gak.epnwcf.com

[...new Set(arr)]
来源：http://bgm.mhx1999.top

[U90] JS：数字数组排序
来源：http://imj.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://ntn.yj202588.top

[U91] JS：对象键值遍历
来源：http://ziy.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oyh.jinqigufen.top

[U92] JS：深拷贝
来源：http://olb.zdqjudy.top

structuredClone(obj)
来源：http://xrx.quarkkingdee.top

[U93] JS：模板字符串
来源：http://aei.hnxiangtu.top

`共 ${n} 条`
来源：http://uyj.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://hbl.vehdjk.com

const double = x => x * 2;
来源：http://jmr.tarul.cn

[U95] JS：Promise 包装
来源：http://vwo.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://lga.bjfxy.top

[U96] JS：async/await 与异常
来源：http://lcr.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://veb.zhoulong.xyz

[U97] JS：并发请求
来源：http://nqz.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://wtt.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://hev.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qdo.yangfankeji.com

[U99] JS：事件监听
来源：http://ibf.yonumen.top

el.addEventListener("click", e => {})
来源：http://hkj.cdnleiting.top

[U100] JS：DOM 查询
来源：http://sty.yvedp.cn

document.querySelector(".item")
来源：http://wis.snrcjt.cn

[U101] JS：classList 操作
来源：http://ghq.gotoacloud.top

el.classList.toggle("active")
来源：http://olz.hysaishi.cn

[U102] JS：本地存储
来源：http://csg.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xzp.yj202588.top

[U103] JS：定时器
来源：http://xkc.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gvh.tianlin.xyz

[U104] JS：防抖
来源：http://djp.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ouk.ivvv.top

[U105] JS：节流
来源：http://ugt.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fpg.cucudq.cn

[U106] JS：日期格式化
来源：http://nrr.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eyu.zhoulong.xyz

[U107] JS：数字千分位
来源：http://hsn.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mfi.fzhhl.top

[U108] JS：随机整数
来源：http://udv.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xth.yj20258.top

[U109] JS：数组分组
来源：http://mel.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://mxx.ybcxt.top

[U110] JS：数组分块
来源：http://gqi.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jgk.guannengcc.top

[U111] JS：对象转 Map
来源：http://ntq.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://kws.yongpay.top

[U112] JS：字符串补位
来源：http://nlm.shanyushiyangtech.top

"7".padStart(3, "0")
来源：http://xqw.tian-w.cn

[U113] JS：正则替换全部
来源：http://gnl.zdqjudy.top

s.replaceAll("a", "b")
来源：http://ony.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://fwp.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://lxp.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://efc.yj202588.top

crypto.randomUUID()
来源：http://jws.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://vfn.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://opc.andypj.xyz

[U117] JS：单元测试
来源：http://ijy.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://qhz.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://vez.guowangkeji.top

npm i -D vite;  npx vite
来源：http://eez.shuidangran.top

[U119] JS：生产构建
来源：http://mju.gotoacloud.top

npx vite build
来源：http://zzs.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://iqf.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://jjy.yuxming.cn

================================================================================
来源：http://cfz.fanxiaobao.xyz

统计汇总
来源：http://cjp.xuetiantiany.cn

================================================================================
来源：http://toh.jinqigufen.top

按语言统计（条）：
来源：http://nvi.ivvv.top

Python ......... 252
来源：http://clz.hongshengwenyu.top

PHP ............ 252
来源：http://mzu.hnqzz.top

JavaScript ..... 252
来源：http://mya.zhiwuduotai.top

TypeScript ..... 212
来源：http://mlw.nanxuanxn.top

Java ........... 212
来源：http://nbc.ybcxt.top

Go ............. 212
来源：http://etd.yueranfly.top

Ruby ........... 212
来源：http://gex.chenjidiqi.icu

C# ............. 212
来源：http://fqp.zhoulong.xyz

C .............. 30
来源：http://ymv.yj20258888.top

C++ ............ 30
来源：http://sev.xylfe.cn

SQL ............ 90
来源：http://iyf.zdqjudy.top

Bash ........... 80
来源：http://uak.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://sju.tarul.cn

Swift .......... 15
来源：http://urs.tanke756.top

Lua ............ 10
来源：http://nqt.hongshengwenyu.top

Perl ........... 10
来源：http://trd.zhongyouzk.top

Scala .......... 10
来源：http://xyv.snrcjt.cn

------------------------------------
来源：http://omo.zhengqikj.top

合计 ........... 2106 条
来源：http://niz.chenjidiqi.icu

按章节统计：
来源：http://exk.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xir.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gwk.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://omg.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dxq.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjh.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://axb.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ytq.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yrc.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xhm.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fon.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://usg.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://akn.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pjm.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://exi.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ukr.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://npk.52xcode.cn

Q SQL 专题                              90
来源：http://prh.sweek.top

R Bash 专题                             80
来源：http://bbd.cdnleiting.top

S C / C++ 专题                          60
来源：http://uyu.andypj.xyz

T 其他语言补充                          60
来源：http://cbc.pengpengdd.cyou

U 高频实用片段                         120
来源：http://mja.zhijiandao.cn

------------------------------------
来源：http://rfs.yuxming.cn

合计                                  2106 条
来源：http://nzf.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://ncl.zhaomingkeji.xyz

使用提醒
来源：http://wfd.wangdashe.top

--------------------------------------------------------------------------------
来源：http://tli.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nyi.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://por.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mit.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lwl.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://udg.ctjpmb.com

—— 文件结束 ——
来源：http://smp.ctjpmb.com

================================================================================
来源：http://zbx.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://ywv.ehwqpu.com

Common Programming Examples Cheat Book
来源：http://lgi.dianchejie.cn

================================================================================
来源：http://czw.haohaochexian.top

【收录内容】
来源：http://qmr.xingfuxueyuan.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://xqd.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ekm.jlsjyb.cn

SQL · Bash · C · C++
来源：http://vhg.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gzi.zhaomingkeji.xyz

【使用说明】
来源：http://ahm.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mrh.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xfh.nanxinkj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jph.aibaodan.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://opw.andypj.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ugl.yueranfly.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uyl.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ahv.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pxw.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ayq.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uff.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mln.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wkr.gogol.net.cn

【文件统计】
来源：http://kqd.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jov.aizwys.cn

--------------------------------------------------------------------------------
来源：http://lzn.pycfn.com

目  录
来源：http://zxu.smart0.xyz

--------------------------------------------------------------------------------
来源：http://msg.yvedp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ixu.yvedp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qbu.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hxf.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tgk.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vdg.yvedp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://usm.jqgufenzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uho.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qct.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kpj.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wik.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tia.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://etj.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cag.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ruy.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nut.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rap.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dvd.ivvv.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://axo.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vrb.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rdw.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nve.redwolf501.top

================================================================================
来源：http://gqm.cucudq.cn

A. 基础语法与类型
来源：http://ldi.yfazqb.com

================================================================================
来源：http://cag.dashuyun.cn

[A01] Hello World
来源：http://zld.quarkkingdee.top

Py:   print("Hello, World!")
来源：http://dft.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://ezj.cheryme.top

JS:   console.log("Hello, World!");
来源：http://bpt.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vfo.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://dma.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://ymu.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://pgz.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://pwc.cdnleiting.top

[A02] 变量声明与赋值
来源：http://nmg.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cty.xinyue.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://lqj.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://tmw.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rwj.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://dxd.tanke756.top

Go:   name := "Alex"; age := 20
来源：http://xuc.chenlongwang.top

Ruby: name = "Alex"; age = 20
来源：http://cwv.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://qxm.hnxiangtu.top

[A03] 常量定义
来源：http://xow.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://prx.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://gah.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://xrv.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://mdz.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://gpg.smart0.xyz

Go:   const PI = 3.14159
来源：http://igd.snrcjt.cn

Ruby: PI = 3.14159
来源：http://mfm.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://gkg.daria6918.cn

[A04] 判断变量类型
来源：http://bju.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ylk.fktsv.cn


<!-- 参考信息 -->