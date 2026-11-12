代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://dtj.yangfankeji.com

sys.stdout.isatty()
来源：http://ymt.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://ack.yvedp.cn

print("err", file=sys.stderr)
来源：http://gyo.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://kgh.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lyw.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://mxu.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://trl.xziqi.cn

[U43] PHP：声明命名空间
来源：http://mav.hnqzz.top

namespace App\Http;
来源：http://mhy.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://pav.sxryk.cn

declare(strict_types=1);
来源：http://xou.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://bil.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tsg.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://pyy.andypj.xyz

?string $name = null
来源：http://ykw.zhoulong.xyz

[U47] PHP：联合类型
来源：http://gxr.kuanghao11.cn

int|string $id
来源：http://zwm.cqqwz.cn

[U48] PHP：纯枚举
来源：http://aqo.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xhb.nwbrower.top

[U49] PHP：只读属性
来源：http://mpk.316326.xyz

public readonly string $name
来源：http://vyd.yonumen.top

[U50] PHP：构造器属性提升
来源：http://zrr.chenlongwang.top

public function __construct(private int $id) {}
来源：http://mia.hammf.cn

[U51] PHP：数组解构
来源：http://lwl.gaohongyu789.top

[$a, $b] = $arr;
来源：http://vfw.nanxinkj.top

[U52] PHP：箭头函数
来源：http://cof.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://syx.hnqzz.top

[U53] PHP：空合并运算符
来源：http://xki.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://byw.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://xaz.yuxming.cn

$obj?->method()
来源：http://cdq.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://rfx.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mpk.jiagoushi.top

[U56] PHP：命名参数
来源：http://lwq.ydzc1.top

f(a: 1, b: 2)
来源：http://dwc.chenlongwang.top

[U57] PHP：字符串插值
来源：http://vlc.daxiang520.top

"值: {$a}"
来源：http://wcl.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://sny.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eca.ppjwa.cn

[U59] PHP：自定义排序
来源：http://iyu.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://huz.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://qkd.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vuh.ydzc1.top

[U61] PHP：正则
来源：http://rco.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lmb.kuanghao11.cn

[U62] PHP：日期对象
来源：http://ymj.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://whk.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://hid.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://upo.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://twu.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://ofi.cdnleiting.top

[U65] PHP：会话
来源：http://vkj.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yfl.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://pob.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://phe.xylfe.cn

[U67] PHP：处理文件上传
来源：http://nxk.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jps.yj202588.top

[U68] PHP：PDO 连接
来源：http://mzw.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hed.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://vmx.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tsp.xylfe.cn

[U70] PHP：PDO 事务
来源：http://qwf.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tlu.hysaishi.cn

[U71] PHP：抛出异常
来源：http://nmz.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://xbq.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://tdj.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://inj.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://cex.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://xqa.ybcxt.top

[U74] PHP：读取环境变量
来源：http://leb.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://yat.ivvv.top

[U75] PHP：依赖注入
来源：http://cci.jqgfzy.top

composer require psr/container
来源：http://cnb.zdbjq.cn

[U76] PHP：简单路由
来源：http://dbn.aizwys.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yyg.fzhhl.top

[U77] PHP：模板渲染
来源：http://aet.snrcjt.cn

composer require twig/twig
来源：http://cro.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://uov.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://ghn.sxryk.cn

[U79] PHP：静态分析
来源：http://pvz.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://tna.jianghu66.top

[U80] PHP：代码规范修复
来源：http://uyz.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pnp.dashuyun.cn

[U81] JS：初始化项目
来源：http://jaa.wangdashe.top

npm init -y;  npm i express
来源：http://znz.cucudq.cn

[U82] JS：package.json 脚本
来源：http://fuz.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nkt.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://ioh.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tyw.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://omh.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://rhl.sxryk.cn

[U85] JS：可选链
来源：http://bws.vehdjk.com

a?.b?.c
来源：http://ufa.jinqigfzy.top

[U86] JS：空值合并
来源：http://fmv.wangdashe.top

a ?? b
来源：http://mdn.hnxiangtu.top

[U87] JS：解构默认值
来源：http://ooj.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://rpb.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://zpq.ppjwa.cn

{ ...a, ...b }
来源：http://hhl.yj20258.top

[U89] JS：数组去重
来源：http://myh.gaohongyu789.top

[...new Set(arr)]
来源：http://tod.smart0.xyz

[U90] JS：数字数组排序
来源：http://ewn.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://hbj.fengsongda.top

[U91] JS：对象键值遍历
来源：http://few.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rir.yvedp.cn

[U92] JS：深拷贝
来源：http://dge.ctjpmb.com

structuredClone(obj)
来源：http://akc.zdqjudy.top

[U93] JS：模板字符串
来源：http://mrr.xylfe.cn

`共 ${n} 条`
来源：http://dpo.yuanzhike.top

[U94] JS：箭头函数
来源：http://vdf.hammf.cn

const double = x => x * 2;
来源：http://ays.zdqjudy.top

[U95] JS：Promise 包装
来源：http://ebe.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://fzk.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://bxy.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ykh.c1oappe.top

[U97] JS：并发请求
来源：http://bpw.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vak.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://lhg.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mrq.snrcjt.cn

[U99] JS：事件监听
来源：http://jot.birdmap.top

el.addEventListener("click", e => {})
来源：http://tix.tarul.cn

[U100] JS：DOM 查询
来源：http://fzm.birdmap.top

document.querySelector(".item")
来源：http://bdl.iojbl.cn

[U101] JS：classList 操作
来源：http://hwt.ehwqpu.com

el.classList.toggle("active")
来源：http://esj.chenzaomai.com

[U102] JS：本地存储
来源：http://pis.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ulz.feifeiyinyue.top

[U103] JS：定时器
来源：http://xoc.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://job.tianlin.xyz

[U104] JS：防抖
来源：http://zrw.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cxl.chenlongwang.top

[U105] JS：节流
来源：http://jjs.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://woj.gzhubu.top

[U106] JS：日期格式化
来源：http://egy.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pky.316326.xyz

[U107] JS：数字千分位
来源：http://jtg.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qxm.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://cwe.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://khb.sxryk.cn

[U109] JS：数组分组
来源：http://enc.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://qum.gzhubu.top

[U110] JS：数组分块
来源：http://jzc.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cjg.tanke756.top

[U111] JS：对象转 Map
来源：http://usk.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://ydi.jinqigfzy.top

[U112] JS：字符串补位
来源：http://pjw.hywenlv.cn

"7".padStart(3, "0")
来源：http://pcw.epnwcf.com

[U113] JS：正则替换全部
来源：http://ekr.snrcjt.cn

s.replaceAll("a", "b")
来源：http://uwn.sysykeji.top

[U114] JS：JSON 深比较
来源：http://dhz.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zyj.ppjwa.cn

[U115] JS：生成 UUID
来源：http://aiu.ivvv.top

crypto.randomUUID()
来源：http://mpw.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://gbr.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://wcg.pengpengdd.cyou

[U117] JS：单元测试
来源：http://mlc.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://rkp.wangdashe.top

[U118] JS：开发服务器
来源：http://kki.xylfe.cn

npm i -D vite;  npx vite
来源：http://coz.feifeiyinyue.top

[U119] JS：生产构建
来源：http://izu.dianchejie.cn

npx vite build
来源：http://cmr.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://jjx.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://aca.jianghu66.top

================================================================================
来源：http://yba.shuidangran.top

统计汇总
来源：http://kzs.ywan-chungtsiang.top

================================================================================
来源：http://dll.andypj.xyz

按语言统计（条）：
来源：http://cih.gotoacloud.top

Python ......... 252
来源：http://dug.jinghuilouyu.cn

PHP ............ 252
来源：http://lsx.haohaochexian.top

JavaScript ..... 252
来源：http://jiz.hnqzz.top

TypeScript ..... 212
来源：http://svu.cqqwz.cn

Java ........... 212
来源：http://fif.meibo888.top

Go ............. 212
来源：http://kai.ehwqpu.com

Ruby ........... 212
来源：http://mvc.gaohongyu789.top

C# ............. 212
来源：http://tlu.yueranfly.top

C .............. 30
来源：http://bpc.jinyuanbaomall.cn

C++ ............ 30
来源：http://hbz.316326.xyz

SQL ............ 90
来源：http://kln.shuidangran.top

Bash ........... 80
来源：http://thq.jyoumei.cn

Kotlin ......... 15
来源：http://tgb.yuanzhike.top

Swift .......... 15
来源：http://fzh.havefunace.top

Lua ............ 10
来源：http://ima.yonumen.top

Perl ........... 10
来源：http://fsx.sysykeji.top

Scala .......... 10
来源：http://ukh.ydzc1.top

------------------------------------
来源：http://aff.dashuyun.cn

合计 ........... 2106 条
来源：http://rcm.cashguo.top

按章节统计：
来源：http://vep.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ypv.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xmv.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sxv.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jdo.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://czp.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yoe.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://emu.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://efo.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lnh.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cwd.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qct.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hwn.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://syw.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gab.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://frz.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pgd.epnwcf.com

Q SQL 专题                              90
来源：http://itt.yonumen.top

R Bash 专题                             80
来源：http://ged.dashuyun.cn

S C / C++ 专题                          60
来源：http://ruy.hongshengwenyu.top

T 其他语言补充                          60
来源：http://yrd.fengsongda.top

U 高频实用片段                         120
来源：http://ajx.dianchejie.cn

------------------------------------
来源：http://boz.gotoacloud.top

合计                                  2106 条
来源：http://fsj.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://dnp.sjlbkw.cn

使用提醒
来源：http://qpy.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://wfd.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xmc.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xkq.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xnq.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tqu.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zch.pengpengdd.cyou

—— 文件结束 ——
来源：http://vru.yuanzhike.top

================================================================================
来源：http://hnt.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://xdl.wangshuangyany.cn

Common Programming Examples Cheat Book
来源：http://cvh.9152youxi.cn

================================================================================
来源：http://zra.zhengqikj.top

【收录内容】
来源：http://qjc.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://mtj.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kob.zhengqikj.top

SQL · Bash · C · C++
来源：http://foz.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kty.yueranfly.top

【使用说明】
来源：http://utu.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://euv.zdbjq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ohr.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://muk.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ioo.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://qxj.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://giz.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fed.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://prv.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kyf.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jtj.yongpay.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://njc.havefunace.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://udm.ydjk.org.cn

【文件统计】
来源：http://xfq.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ulb.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://gmu.tian-w.cn

目  录
来源：http://xtq.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://pjv.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hlx.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xag.tian-w.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hcx.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yco.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tez.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ynv.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tug.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://suo.cheryme.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://czw.fktsv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cch.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tfa.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wfw.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uxg.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ybc.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ifb.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dtv.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://agc.yangfankeji.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://cgs.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nvb.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysf.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fck.xuetiantiany.cn

================================================================================
来源：http://uio.jianghu66.top

A. 基础语法与类型
来源：http://quf.sxryk.cn

================================================================================
来源：http://drr.xziqi.cn

[A01] Hello World
来源：http://jee.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://tww.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://sdd.ydjk.org.cn

JS:   console.log("Hello, World!");
来源：http://nla.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vks.ppjwa.cn

Java: System.out.println("Hello, World!");
来源：http://cnq.zhixingplan.top

Go:   fmt.Println("Hello, World!")
来源：http://mae.cashguo.top

Ruby: puts "Hello, World!"
来源：http://gti.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ewf.zdqjudy.top

[A02] 变量声明与赋值
来源：http://kue.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://okb.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hvs.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fef.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pfq.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://bjk.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://ahk.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://bzt.meibo888.top

C#:   string name = "Alex"; int age = 20;
来源：http://fmz.52xcode.cn

[A03] 常量定义
来源：http://zaj.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nef.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://uyy.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://vce.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://jbx.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://sfp.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://ryn.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://vio.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://gpw.xingfuxueyuan.xyz

[A04] 判断变量类型
来源：http://nkc.xziqi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vqk.andypj.xyz


<!-- 参考信息 -->