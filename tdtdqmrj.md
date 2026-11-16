代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://djw.cashguo.top

sys.stdout.isatty()
来源：http://duf.yonumen.top

[U40] Py：打印到标准错误
来源：http://och.yfazqb.com

print("err", file=sys.stderr)
来源：http://jli.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://nke.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://prz.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://tea.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://izy.xuanzx.com

[U43] PHP：声明命名空间
来源：http://ogq.shangyingyoupin.top

namespace App\Http;
来源：http://oht.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://gjw.yj20258.top

declare(strict_types=1);
来源：http://dlk.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://gix.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mss.zhengqikj.top

[U46] PHP：可空类型
来源：http://aaf.yuanzhike.top

?string $name = null
来源：http://czr.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://mkm.yangfankeji.com

int|string $id
来源：http://whv.hongshengwenyu.top

[U48] PHP：纯枚举
来源：http://jbb.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ade.nanxuanxn.top

[U49] PHP：只读属性
来源：http://ovq.yangfankeji.com

public readonly string $name
来源：http://uap.yongpay.top

[U50] PHP：构造器属性提升
来源：http://dcb.hcnkem.com

public function __construct(private int $id) {}
来源：http://cmm.zdqjudy.top

[U51] PHP：数组解构
来源：http://hty.gaohongyu789.top

[$a, $b] = $arr;
来源：http://jws.pycfn.com

[U52] PHP：箭头函数
来源：http://akh.tanke756.top

$double = fn($x) => $x * 2;
来源：http://bjk.tarul.cn

[U53] PHP：空合并运算符
来源：http://fhs.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://lav.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://cus.shuidangran.top

$obj?->method()
来源：http://nhc.yuanzhike.top

[U55] PHP：match 表达式
来源：http://njt.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wny.zhongyouzk.top

[U56] PHP：命名参数
来源：http://ppt.birdmap.top

f(a: 1, b: 2)
来源：http://cpt.cqqwz.cn

[U57] PHP：字符串插值
来源：http://awe.yj202588.top

"值: {$a}"
来源：http://olr.0kj1m.cn

[U58] PHP：数组三件套
来源：http://kns.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zre.fzhhl.top

[U59] PHP：自定义排序
来源：http://eck.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jro.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://hzm.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://chw.vehdjk.com

[U61] PHP：正则
来源：http://ucs.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oiv.tarul.cn

[U62] PHP：日期对象
来源：http://kwr.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uar.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://qeh.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://waj.yvedp.cn

[U64] PHP：目录遍历
来源：http://udf.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://ixo.hfpthk.cn

[U65] PHP：会话
来源：http://lhj.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://imp.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://wfe.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ova.yuxming.cn

[U67] PHP：处理文件上传
来源：http://mkp.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wfn.jianghu66.top

[U68] PHP：PDO 连接
来源：http://ovd.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iue.316326.xyz

[U69] PHP：PDO 预处理
来源：http://ydx.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ieg.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://avu.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xsb.shuidangran.top

[U71] PHP：抛出异常
来源：http://hyu.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://wgw.pycfn.com

[U72] PHP：写错误日志
来源：http://ecs.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://nre.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://rxn.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://ygv.c1oappe.top

[U74] PHP：读取环境变量
来源：http://onl.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://pkj.jinqigufen.top

[U75] PHP：依赖注入
来源：http://jua.yueranfly.top

composer require psr/container
来源：http://bra.hnxiangtu.top

[U76] PHP：简单路由
来源：http://rgs.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fmp.hammf.cn

[U77] PHP：模板渲染
来源：http://uvr.ybcxt.top

composer require twig/twig
来源：http://rct.cucudq.cn

[U78] PHP：单元测试
来源：http://xop.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://dir.jqgufenzy.top

[U79] PHP：静态分析
来源：http://zhl.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://fal.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://ckn.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qnj.shuidangran.top

[U81] JS：初始化项目
来源：http://mfi.jinqigufen.top

npm init -y;  npm i express
来源：http://ano.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://awg.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://svy.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://dcj.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ihl.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://bdy.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://udh.yongpay.top

[U85] JS：可选链
来源：http://fqy.nanxuanxn.top

a?.b?.c
来源：http://hno.dianchejie.cn

[U86] JS：空值合并
来源：http://onz.xuetiantiany.cn

a ?? b
来源：http://xzj.yongpay.top

[U87] JS：解构默认值
来源：http://kwi.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://hvn.ppjwa.cn

[U88] JS：对象展开合并
来源：http://aaj.gotoacloud.top

{ ...a, ...b }
来源：http://dbw.52xcode.cn

[U89] JS：数组去重
来源：http://zsf.daria6918.cn

[...new Set(arr)]
来源：http://lky.ydzc1.top

[U90] JS：数字数组排序
来源：http://klr.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://vnx.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://dce.xuanzx.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cnb.jianghu66.top

[U92] JS：深拷贝
来源：http://fmf.jiagoushi.top

structuredClone(obj)
来源：http://xja.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://yby.hnxiangtu.top

`共 ${n} 条`
来源：http://scr.sweek.top

[U94] JS：箭头函数
来源：http://snv.nwbrower.top

const double = x => x * 2;
来源：http://yqd.shuidangran.top

[U95] JS：Promise 包装
来源：http://anu.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://dyq.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://arm.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kaa.yj20258888.top

[U97] JS：并发请求
来源：http://aei.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bmz.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://lba.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://thh.meibo888.top

[U99] JS：事件监听
来源：http://hss.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://aar.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://nge.yj20258888.top

document.querySelector(".item")
来源：http://lta.bjfxy.top

[U101] JS：classList 操作
来源：http://uli.cheryme.top

el.classList.toggle("active")
来源：http://ykd.cucudq.cn

[U102] JS：本地存储
来源：http://ecc.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gyq.tian-w.cn

[U103] JS：定时器
来源：http://ria.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zyw.shuidangran.top

[U104] JS：防抖
来源：http://umj.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ake.sxryk.cn

[U105] JS：节流
来源：http://yvc.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://odn.yuxming.cn

[U106] JS：日期格式化
来源：http://uwg.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hck.jyoumei.cn

[U107] JS：数字千分位
来源：http://mxd.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ryz.birdmap.top

[U108] JS：随机整数
来源：http://nhn.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://otr.dashuyun.cn

[U109] JS：数组分组
来源：http://pak.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://zuh.snrcjt.cn

[U110] JS：数组分块
来源：http://irf.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nxb.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://fxx.daxiang520.top

new Map(Object.entries(obj))
来源：http://lol.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://tdn.redwolf501.top

"7".padStart(3, "0")
来源：http://ckb.jqgfzy.top

[U113] JS：正则替换全部
来源：http://krz.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://vxy.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://byv.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kah.cashguo.top

[U115] JS：生成 UUID
来源：http://mkd.hywenlv.cn

crypto.randomUUID()
来源：http://xyg.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://iup.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://dac.fzhhl.top

[U117] JS：单元测试
来源：http://ouo.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://uco.hcnkem.com

[U118] JS：开发服务器
来源：http://jer.hywenlv.cn

npm i -D vite;  npx vite
来源：http://vne.jiagoushi.top

[U119] JS：生产构建
来源：http://bwy.jqgfzy.top

npx vite build
来源：http://nsf.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://pkw.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://srh.quarkkingdee.top

================================================================================
来源：http://stt.yuanzhike.top

统计汇总
来源：http://wif.ywan-chungtsiang.top

================================================================================
来源：http://ikk.aibaodan.cn

按语言统计（条）：
来源：http://mtt.gzhubu.top

Python ......... 252
来源：http://kis.shanyushiyangkeji.top

PHP ............ 252
来源：http://gmf.sxryk.cn

JavaScript ..... 252
来源：http://awc.yuanzhike.top

TypeScript ..... 212
来源：http://rav.nanxinkj.top

Java ........... 212
来源：http://xix.vehdjk.com

Go ............. 212
来源：http://ejx.tianlin.xyz

Ruby ........... 212
来源：http://izg.bjfxy.top

C# ............. 212
来源：http://bxv.ehwqpu.com

C .............. 30
来源：http://pxh.iojbl.cn

C++ ............ 30
来源：http://xlf.ehwqpu.com

SQL ............ 90
来源：http://rqg.yj202588.top

Bash ........... 80
来源：http://hvo.yuxming.cn

Kotlin ......... 15
来源：http://toj.quarkkingdee.top

Swift .......... 15
来源：http://dfs.xziqi.cn

Lua ............ 10
来源：http://nha.birdmap.top

Perl ........... 10
来源：http://mod.jqgufenzy.top

Scala .......... 10
来源：http://fwk.fengsongda.top

------------------------------------
来源：http://ngw.gaohongyu789.top

合计 ........... 2106 条
来源：http://low.52xcode.cn

按章节统计：
来源：http://vjl.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yko.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ude.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yuo.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ifq.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ojy.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bmp.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qsv.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cyl.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ezc.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tty.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wgs.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fai.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hju.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zcq.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kqr.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ziz.daxiang520.top

Q SQL 专题                              90
来源：http://cuq.chenzaomai.com

R Bash 专题                             80
来源：http://kvu.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://gnn.nanxinkj.top

T 其他语言补充                          60
来源：http://sey.dianchejie.cn

U 高频实用片段                         120
来源：http://kaf.yuanzhike.top

------------------------------------
来源：http://hrx.yvedp.cn

合计                                  2106 条
来源：http://snm.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://ezb.wangdashe.top

使用提醒
来源：http://zog.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://jhr.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dbj.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vql.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ycr.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mkq.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sqj.gaohongyu789.top

—— 文件结束 ——
来源：http://fnp.tianlin.xyz

================================================================================
来源：http://gqp.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://nhw.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://yax.pycfn.com

================================================================================
来源：http://jgg.hcnkem.com

【收录内容】
来源：http://swf.hfpthk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yzm.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xdh.fengsongda.top

SQL · Bash · C · C++
来源：http://gkv.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vow.vehdjk.com

【使用说明】
来源：http://awm.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gyi.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gya.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mql.uphjek.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ugn.zycfv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vuc.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gxd.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rgx.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ilb.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wgj.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://csv.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hmz.sxryk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wfa.cheryme.top

【文件统计】
来源：http://xeh.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://csw.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://nun.jqgfzy.top

目  录
来源：http://znd.52xcode.cn

--------------------------------------------------------------------------------
来源：http://zcp.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rmg.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rsy.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ies.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wnr.pengpengdd.cyou

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://krl.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wml.sysykeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zmj.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ktm.hnqzz.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jni.shanyushiyangtech.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wuq.epnwcf.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xvs.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oas.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dgh.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tux.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dck.jinghuilouyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dca.daxiang520.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ycl.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://emv.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pgv.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwq.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lhe.nanxuanxn.top

================================================================================
来源：http://tqq.chenjidiqi.icu

A. 基础语法与类型
来源：http://buk.birdmap.top

================================================================================
来源：http://yqx.ywan-chungtsiang.top

[A01] Hello World
来源：http://cov.meibo888.top

Py:   print("Hello, World!")
来源：http://rsw.yj20258.top

PHP:  echo "Hello, World!";
来源：http://szb.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://vhr.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ofo.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://ecr.daxiang520.top

Go:   fmt.Println("Hello, World!")
来源：http://tjb.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://cvl.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rdu.birdmap.top

[A02] 变量声明与赋值
来源：http://taz.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qxj.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hji.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ypj.mhx1999.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wwo.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://adl.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://koc.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://gwy.xuetiantiany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qel.quarkkingdee.top

[A03] 常量定义
来源：http://rcr.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yds.cheryme.top

PHP:  const PI = 3.14159;
来源：http://ebn.cucudq.cn

JS:   const PI = 3.14159;
来源：http://yab.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://niw.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://yxd.tanke756.top

Go:   const PI = 3.14159
来源：http://inw.jinghuilouyu.cn

Ruby: PI = 3.14159
来源：http://sze.fzhhl.top

C#:   const double PI = 3.14159;
来源：http://wdm.hnxiangtu.top

[A04] 判断变量类型
来源：http://lqm.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://nto.tian-w.cn


<!-- 参考信息 -->