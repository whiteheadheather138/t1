代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://tei.zhengqikj.top

sys.stdout.isatty()
来源：http://aez.mhx1999.top

[U40] Py：打印到标准错误
来源：http://rwa.quarkkingdee.top

print("err", file=sys.stderr)
来源：http://zwe.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://oyx.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nnx.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://bun.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ocv.uphjek.com

[U43] PHP：声明命名空间
来源：http://kyp.mhx1999.top

namespace App\Http;
来源：http://ino.aizwys.cn

[U44] PHP：开启严格类型
来源：http://zfe.hongshengwenyu.top

declare(strict_types=1);
来源：http://tvm.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://wfc.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uga.gotoacloud.top

[U46] PHP：可空类型
来源：http://naw.redwolf501.top

?string $name = null
来源：http://jkf.guannengcc.top

[U47] PHP：联合类型
来源：http://nfw.dashuyun.cn

int|string $id
来源：http://jqe.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://iug.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nqj.sweek.top

[U49] PHP：只读属性
来源：http://qin.shanyushiyangkeji.top

public readonly string $name
来源：http://jxs.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://wnj.yj20258888.top

public function __construct(private int $id) {}
来源：http://bxs.guowangkeji.top

[U51] PHP：数组解构
来源：http://sza.sysykeji.top

[$a, $b] = $arr;
来源：http://igg.xuanzx.com

[U52] PHP：箭头函数
来源：http://uyb.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://uwe.ivvv.top

[U53] PHP：空合并运算符
来源：http://ovw.snrcjt.cn

$v = $a ?? $b ?? "default";
来源：http://syb.nwbrower.top

[U54] PHP：空安全调用
来源：http://sds.chenjidiqi.icu

$obj?->method()
来源：http://qgq.sweek.top

[U55] PHP：match 表达式
来源：http://jkn.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ayg.hesvh.cn

[U56] PHP：命名参数
来源：http://cbt.zycfv.cn

f(a: 1, b: 2)
来源：http://wfr.guowangkeji.top

[U57] PHP：字符串插值
来源：http://pbl.xinyue.icu

"值: {$a}"
来源：http://rsj.daria6918.cn

[U58] PHP：数组三件套
来源：http://fxz.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fzl.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://qcz.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kme.tarul.cn

[U60] PHP：JSON 编解码
来源：http://vob.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hky.dashuyun.cn

[U61] PHP：正则
来源：http://vvk.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hjf.ydjk.org.cn

[U62] PHP：日期对象
来源：http://kpu.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lbu.xinyue.icu

[U63] PHP：文件读写
来源：http://dug.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sql.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://tjj.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://yrr.tian-w.cn

[U65] PHP：会话
来源：http://arl.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tgx.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://btn.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jsx.gzhubu.top

[U67] PHP：处理文件上传
来源：http://wtr.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rkg.yonumen.top

[U68] PHP：PDO 连接
来源：http://aoh.zhengqikj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vmu.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://xyd.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lik.fehbvm.com

[U70] PHP：PDO 事务
来源：http://vxu.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjb.birdmap.top

[U71] PHP：抛出异常
来源：http://xie.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://mlt.haohaochexian.top

[U72] PHP：写错误日志
来源：http://uas.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://sgr.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://mao.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://xkd.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://utz.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://mjt.fehbvm.com

[U75] PHP：依赖注入
来源：http://hyc.ywan-chungtsiang.top

composer require psr/container
来源：http://vwy.jlsjyb.cn

[U76] PHP：简单路由
来源：http://ooj.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gdg.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://rys.andypj.xyz

composer require twig/twig
来源：http://riu.sysykeji.top

[U78] PHP：单元测试
来源：http://uih.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://aly.fzhhl.top

[U79] PHP：静态分析
来源：http://gpt.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://pmr.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://cbr.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ddx.tarul.cn

[U81] JS：初始化项目
来源：http://dxh.jlsjyb.cn

npm init -y;  npm i express
来源：http://exp.xuanzx.com

[U82] JS：package.json 脚本
来源：http://ffv.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://exv.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://uyy.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hcw.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://nrz.jiagoushi.top

module.exports = { a };  const { a } = require("./m");
来源：http://quj.xuetiantiany.cn

[U85] JS：可选链
来源：http://leb.uphjek.com

a?.b?.c
来源：http://uqa.vqdsnc.cn

[U86] JS：空值合并
来源：http://mrx.hesvh.cn

a ?? b
来源：http://viz.jinqigfzy.top

[U87] JS：解构默认值
来源：http://owf.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://gfh.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://jic.yj202588.top

{ ...a, ...b }
来源：http://ngq.yj20258.top

[U89] JS：数组去重
来源：http://ahe.haohaochexian.top

[...new Set(arr)]
来源：http://mbf.chenzaomai.com

[U90] JS：数字数组排序
来源：http://qds.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://gmq.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://vfq.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://div.fengsongda.top

[U92] JS：深拷贝
来源：http://wnh.zycfv.cn

structuredClone(obj)
来源：http://nzn.9152youxi.cn

[U93] JS：模板字符串
来源：http://xmt.chenzaomai.com

`共 ${n} 条`
来源：http://nse.c1oappe.top

[U94] JS：箭头函数
来源：http://cwn.uphjek.com

const double = x => x * 2;
来源：http://vmz.bbcook.cn

[U95] JS：Promise 包装
来源：http://qfx.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://vcu.birdmap.top

[U96] JS：async/await 与异常
来源：http://lun.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oty.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://iat.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vyx.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://tcb.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://acl.cqqwz.cn

[U99] JS：事件监听
来源：http://ggv.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://uoe.fehbvm.com

[U100] JS：DOM 查询
来源：http://qlf.zdbjq.cn

document.querySelector(".item")
来源：http://qql.hywenlv.cn

[U101] JS：classList 操作
来源：http://obp.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://scn.mhx1999.top

[U102] JS：本地存储
来源：http://fng.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bzr.ybcxt.top

[U103] JS：定时器
来源：http://qrp.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kug.jqgufenzy.top

[U104] JS：防抖
来源：http://vsu.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdk.yj20258888.top

[U105] JS：节流
来源：http://cpr.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://thn.tian-w.cn

[U106] JS：日期格式化
来源：http://ode.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://awo.hammf.cn

[U107] JS：数字千分位
来源：http://uqd.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jid.meibo888.top

[U108] JS：随机整数
来源：http://oel.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lmu.snrcjt.cn

[U109] JS：数组分组
来源：http://ena.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://zir.tianlin.xyz

[U110] JS：数组分块
来源：http://qkb.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bak.vehdjk.com

[U111] JS：对象转 Map
来源：http://iur.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://eod.yj20258888.top

[U112] JS：字符串补位
来源：http://weq.haohaochexian.top

"7".padStart(3, "0")
来源：http://zak.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://sbw.tarul.cn

s.replaceAll("a", "b")
来源：http://sgk.jianghu66.top

[U114] JS：JSON 深比较
来源：http://bqd.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://djp.guowangkeji.top

[U115] JS：生成 UUID
来源：http://aiv.haohaochexian.top

crypto.randomUUID()
来源：http://uxq.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://hri.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://whc.316326.xyz

[U117] JS：单元测试
来源：http://sbt.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://nyf.dashuyun.cn

[U118] JS：开发服务器
来源：http://syb.havefunace.top

npm i -D vite;  npx vite
来源：http://nao.aizwys.cn

[U119] JS：生产构建
来源：http://qay.quarkkingdee.top

npx vite build
来源：http://ulj.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://crw.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://hmg.gogol.net.cn

================================================================================
来源：http://sgx.zhengqikj.top

统计汇总
来源：http://dzj.gotoacloud.top

================================================================================
来源：http://stx.hysaishi.cn

按语言统计（条）：
来源：http://yhs.uphjek.com

Python ......... 252
来源：http://tjd.zhaomingkeji.xyz

PHP ............ 252
来源：http://klg.redwolf501.top

JavaScript ..... 252
来源：http://eoe.guannengcc.top

TypeScript ..... 212
来源：http://xtm.jlsjyb.cn

Java ........... 212
来源：http://bze.gaohongyu789.top

Go ............. 212
来源：http://hze.fzhhl.top

Ruby ........... 212
来源：http://spc.yangfankeji.com

C# ............. 212
来源：http://lhe.guannengcc.top

C .............. 30
来源：http://oab.hesvh.cn

C++ ............ 30
来源：http://gty.zhengqikj.top

SQL ............ 90
来源：http://ajr.tian-w.cn

Bash ........... 80
来源：http://kmm.zhijiandao.cn

Kotlin ......... 15
来源：http://afo.guowangkeji.top

Swift .......... 15
来源：http://toz.bbcook.cn

Lua ............ 10
来源：http://eug.hnxiangtu.top

Perl ........... 10
来源：http://ebs.cucudq.cn

Scala .......... 10
来源：http://kzt.cdnleiting.top

------------------------------------
来源：http://zxu.fengsongda.top

合计 ........... 2106 条
来源：http://wto.ybcxt.top

按章节统计：
来源：http://gap.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ugd.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://msp.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qzr.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mup.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dxx.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rud.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oij.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nmn.sysykeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lcl.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nrf.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yje.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kxq.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://upq.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oay.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ejl.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://adi.hammf.cn

Q SQL 专题                              90
来源：http://qax.chenlongwang.top

R Bash 专题                             80
来源：http://jpj.yj202588.top

S C / C++ 专题                          60
来源：http://fis.zdbjq.cn

T 其他语言补充                          60
来源：http://box.nanxuanxn.top

U 高频实用片段                         120
来源：http://rdb.tian-w.cn

------------------------------------
来源：http://son.jiagoushi.top

合计                                  2106 条
来源：http://rdw.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://gtw.ydzc1.top

使用提醒
来源：http://ffo.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://huf.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zwm.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rll.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fzu.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://wdg.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rph.zdqjudy.top

—— 文件结束 ——
来源：http://mjh.chenlongwang.top

================================================================================
来源：http://cnb.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://awr.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://ihb.dianchejie.cn

================================================================================
来源：http://tyb.zhengqikj.top

【收录内容】
来源：http://jhg.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ivj.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://azx.yuanzhike.top

SQL · Bash · C · C++
来源：http://zfm.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://roi.dianchejie.cn

【使用说明】
来源：http://inn.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gta.smart0.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ovq.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vsa.fktsv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nci.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://duf.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vkz.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ogs.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://znz.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://toe.yj20258.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mby.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rbd.gotoacloud.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xkx.yj20258.top

【文件统计】
来源：http://poz.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wnf.316326.xyz

--------------------------------------------------------------------------------
来源：http://cfv.smart0.xyz

目  录
来源：http://meb.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://xcv.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://toy.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uqg.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sgg.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kme.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://did.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lzh.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://axw.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vsm.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dth.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://inj.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hih.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lzn.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yeh.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jnq.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zdc.zhijiandao.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ain.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pwq.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tsy.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cix.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ebf.ctjpmb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sdc.gogol.net.cn

================================================================================
来源：http://gcb.sjlbkw.cn

A. 基础语法与类型
来源：http://uzi.feifeiyinyue.top

================================================================================
来源：http://kmp.yueranfly.top

[A01] Hello World
来源：http://chh.cdnleiting.top

Py:   print("Hello, World!")
来源：http://fdc.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://bsa.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://xge.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kwx.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://jkp.jiagoushi.top

Go:   fmt.Println("Hello, World!")
来源：http://avx.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://dov.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ijy.9152youxi.cn

[A02] 变量声明与赋值
来源：http://njo.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vzu.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://otm.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://nwd.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kot.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://asx.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://umi.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://wto.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://nhl.hywenlv.cn

[A03] 常量定义
来源：http://viq.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zdy.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://csk.tarul.cn

JS:   const PI = 3.14159;
来源：http://kxs.jyoumei.cn

TS:   const PI: number = 3.14159;
来源：http://wdb.yongpay.top

Java: static final double PI = 3.14159;
来源：http://iwz.mhx1999.top

Go:   const PI = 3.14159
来源：http://msg.jinqigufen.top

Ruby: PI = 3.14159
来源：http://tnd.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://edj.fzhhl.top

[A04] 判断变量类型
来源：http://nku.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jpf.zycfv.cn


<!-- 参考信息 -->