代发 wailian999

[U37] Py：读写 Excel
来源：http://tqp.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wms.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://yfi.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://tfc.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://zca.ppjwa.cn

sys.stdout.isatty()
来源：http://fzo.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://mqo.chenjidiqi.icu

print("err", file=sys.stderr)
来源：http://pva.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://mgu.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tae.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://sjd.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mcr.iojbl.cn

[U43] PHP：声明命名空间
来源：http://heb.aizwys.cn

namespace App\Http;
来源：http://sqh.tanke756.top

[U44] PHP：开启严格类型
来源：http://ndf.jqgufenzy.top

declare(strict_types=1);
来源：http://thw.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://yin.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nuh.dashuyun.cn

[U46] PHP：可空类型
来源：http://zec.tian-w.cn

?string $name = null
来源：http://yrr.xinyue.icu

[U47] PHP：联合类型
来源：http://dlp.svipenyu.cn

int|string $id
来源：http://nba.yuxming.cn

[U48] PHP：纯枚举
来源：http://wpk.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://say.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://fjj.vqdsnc.cn

public readonly string $name
来源：http://tdr.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://cad.meibo888.top

public function __construct(private int $id) {}
来源：http://umn.tianlin.xyz

[U51] PHP：数组解构
来源：http://ltv.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://zrn.zdqjudy.top

[U52] PHP：箭头函数
来源：http://hsf.svipenyu.cn

$double = fn($x) => $x * 2;
来源：http://qry.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://cad.sweek.top

$v = $a ?? $b ?? "default";
来源：http://ojk.gzhubu.top

[U54] PHP：空安全调用
来源：http://qns.redwolf501.top

$obj?->method()
来源：http://vfv.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://wtc.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ygi.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://kwo.dashuyun.cn

f(a: 1, b: 2)
来源：http://wxk.dashuyun.cn

[U57] PHP：字符串插值
来源：http://spf.hcnkem.com

"值: {$a}"
来源：http://ibw.dianchejie.cn

[U58] PHP：数组三件套
来源：http://nea.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zai.fktsv.cn

[U59] PHP：自定义排序
来源：http://elo.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mum.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://yme.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jol.ehwqpu.com

[U61] PHP：正则
来源：http://eoq.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ban.zhongyouzk.top

[U62] PHP：日期对象
来源：http://dls.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dpz.yuanzhike.top

[U63] PHP：文件读写
来源：http://stn.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://djo.52xcode.cn

[U64] PHP：目录遍历
来源：http://gmy.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://sbv.yj202588.top

[U65] PHP：会话
来源：http://vqm.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xmv.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://acu.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nbq.zhoulong.xyz

[U67] PHP：处理文件上传
来源：http://jhr.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nor.tanke756.top

[U68] PHP：PDO 连接
来源：http://knr.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pec.meibo888.top

[U69] PHP：PDO 预处理
来源：http://elq.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tqo.fehbvm.com

[U70] PHP：PDO 事务
来源：http://zww.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://etd.mhx1999.top

[U71] PHP：抛出异常
来源：http://lzk.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://dcz.aizwys.cn

[U72] PHP：写错误日志
来源：http://jyl.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://gxi.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://ctq.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://ufw.ivvv.top

[U74] PHP：读取环境变量
来源：http://uhb.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://tbx.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://tnx.jiagoushi.top

composer require psr/container
来源：http://opq.jlsjyb.cn

[U76] PHP：简单路由
来源：http://vag.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://klt.smart0.xyz

[U77] PHP：模板渲染
来源：http://tps.shangyingyoupin.top

composer require twig/twig
来源：http://qyp.ppjwa.cn

[U78] PHP：单元测试
来源：http://wib.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://mgk.hesvh.cn

[U79] PHP：静态分析
来源：http://fgz.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://els.sysykeji.top

[U80] PHP：代码规范修复
来源：http://mdq.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jnr.gzhubu.top

[U81] JS：初始化项目
来源：http://sko.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://ngx.andypj.xyz

[U82] JS：package.json 脚本
来源：http://dox.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pni.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://mey.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iyj.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://sxe.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wyu.yvedp.cn

[U85] JS：可选链
来源：http://eqc.zhiwuduotai.top

a?.b?.c
来源：http://lmi.mhx1999.top

[U86] JS：空值合并
来源：http://gmj.hesvh.cn

a ?? b
来源：http://lbd.nanxinkj.top

[U87] JS：解构默认值
来源：http://uzq.uphjek.com

const { a = 1, b = 2 } = obj;
来源：http://uph.cheryme.top

[U88] JS：对象展开合并
来源：http://jet.shuidangran.top

{ ...a, ...b }
来源：http://wlx.iojbl.cn

[U89] JS：数组去重
来源：http://ayv.nanxuanxn.top

[...new Set(arr)]
来源：http://vdu.dashuyun.cn

[U90] JS：数字数组排序
来源：http://qqf.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://wrx.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://xqj.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nhe.aizwys.cn

[U92] JS：深拷贝
来源：http://wib.epnwcf.com

structuredClone(obj)
来源：http://xij.gogol.net.cn

[U93] JS：模板字符串
来源：http://sym.ctjpmb.com

`共 ${n} 条`
来源：http://ddp.zhengqikj.top

[U94] JS：箭头函数
来源：http://fde.svipenyu.cn

const double = x => x * 2;
来源：http://xuy.hesvh.cn

[U95] JS：Promise 包装
来源：http://qeg.meibo888.top

new Promise((resolve, reject) => {})
来源：http://yfd.daria6918.cn

[U96] JS：async/await 与异常
来源：http://hto.hcnkem.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bnu.sweek.top

[U97] JS：并发请求
来源：http://slk.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eyd.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://owm.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vew.meibo888.top

[U99] JS：事件监听
来源：http://iib.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://gmw.zycfv.cn

[U100] JS：DOM 查询
来源：http://ecs.vehdjk.com

document.querySelector(".item")
来源：http://eix.yvedp.cn

[U101] JS：classList 操作
来源：http://krg.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://aay.yj20258888.top

[U102] JS：本地存储
来源：http://xae.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cuo.cqqwz.cn

[U103] JS：定时器
来源：http://mgc.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qcr.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://igz.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://llb.tanke756.top

[U105] JS：节流
来源：http://fzx.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://akc.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://xzh.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jhs.shzxlz.cn

[U107] JS：数字千分位
来源：http://jkl.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yec.meibo888.top

[U108] JS：随机整数
来源：http://hfu.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nof.zhongyouzk.top

[U109] JS：数组分组
来源：http://cbo.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://fct.ydzc1.top

[U110] JS：数组分块
来源：http://ztf.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kaq.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://bpa.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://hrn.cucudq.cn

[U112] JS：字符串补位
来源：http://awr.jinqigufen.top

"7".padStart(3, "0")
来源：http://iln.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://awm.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://mxg.ybcxt.top

[U114] JS：JSON 深比较
来源：http://yfy.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gxs.vehdjk.com

[U115] JS：生成 UUID
来源：http://muy.fanxiaobao.xyz

crypto.randomUUID()
来源：http://ndh.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://uxr.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://vxu.bbcook.cn

[U117] JS：单元测试
来源：http://ujk.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://otr.svipenyu.cn

[U118] JS：开发服务器
来源：http://ldu.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://qgf.ehwqpu.com

[U119] JS：生产构建
来源：http://hva.ydjk.org.cn

npx vite build
来源：http://uej.aibaodan.cn

[U120] JS：读取环境变量（Vite）
来源：http://kam.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://fnt.nwbrower.top

================================================================================
来源：http://scp.ydjk.org.cn

统计汇总
来源：http://mdc.jiagoushi.top

================================================================================
来源：http://cqo.smart0.xyz

按语言统计（条）：
来源：http://tki.daria6918.cn

Python ......... 252
来源：http://pzl.dianchejie.cn

PHP ............ 252
来源：http://fza.wangshuangyany.cn

JavaScript ..... 252
来源：http://zdn.hammf.cn

TypeScript ..... 212
来源：http://npe.smart0.xyz

Java ........... 212
来源：http://pan.fengsongda.top

Go ............. 212
来源：http://nmn.vehdjk.com

Ruby ........... 212
来源：http://ejw.zhongyouzk.top

C# ............. 212
来源：http://gsc.tian-w.cn

C .............. 30
来源：http://oyy.daxiang520.top

C++ ............ 30
来源：http://tls.gotoacloud.top

SQL ............ 90
来源：http://rqa.sjlbkw.cn

Bash ........... 80
来源：http://fwv.hcnkem.com

Kotlin ......... 15
来源：http://vfa.gogol.net.cn

Swift .......... 15
来源：http://sdi.gogol.net.cn

Lua ............ 10
来源：http://pvn.sjlbkw.cn

Perl ........... 10
来源：http://qdh.zhijiandao.cn

Scala .......... 10
来源：http://gse.uphjek.com

------------------------------------
来源：http://oru.yongpay.top

合计 ........... 2106 条
来源：http://and.shanyushiyangkeji.top

按章节统计：
来源：http://lna.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bod.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hbl.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ngp.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eia.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pgf.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aea.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dun.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jup.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dby.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rtl.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jbs.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vcb.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ifm.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yoi.jqgufenzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cmb.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dbh.jiagoushi.top

Q SQL 专题                              90
来源：http://idc.yj20258888.top

R Bash 专题                             80
来源：http://ubw.yuxming.cn

S C / C++ 专题                          60
来源：http://jgp.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://ayc.yj20258.top

U 高频实用片段                         120
来源：http://fki.zhengqikj.top

------------------------------------
来源：http://imr.snrcjt.cn

合计                                  2106 条
来源：http://vwt.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://shq.snrcjt.cn

使用提醒
来源：http://yup.fzhhl.top

--------------------------------------------------------------------------------
来源：http://qjh.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://knc.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nqc.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rww.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://uxt.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://srp.jlsjyb.cn

—— 文件结束 ——
来源：http://fzc.birdmap.top

================================================================================
来源：http://kfn.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://cqh.yj20258888.top

Common Programming Examples Cheat Book
来源：http://aya.shuidangran.top

================================================================================
来源：http://gfp.yanxiufei.cn

【收录内容】
来源：http://nwh.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://ppr.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nru.jinqigfzy.top

SQL · Bash · C · C++
来源：http://nsq.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gsp.mhx1999.top

【使用说明】
来源：http://dyy.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wrl.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lwh.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://krz.vehdjk.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kjh.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rdz.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kcc.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://myi.chenjidiqi.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vkp.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nso.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://twv.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://atw.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pry.pycfn.com

【文件统计】
来源：http://nvn.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sth.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://nlo.fengsongda.top

目  录
来源：http://slw.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://klt.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wbb.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://alx.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sav.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lcq.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ihr.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xyg.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gpq.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qto.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ssj.zhaomingkeji.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pee.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gue.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lmh.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gnx.xingfuxueyuan.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://frb.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kkb.vqdsnc.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oqe.fengsongda.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://awp.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://btq.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://poc.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aqp.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nsl.shzxlz.cn

================================================================================
来源：http://qcn.zhoulong.xyz

A. 基础语法与类型
来源：http://nnw.yj202588.top

================================================================================
来源：http://tkg.quarkkingdee.top

[A01] Hello World
来源：http://ezw.yj202588.top

Py:   print("Hello, World!")
来源：http://xck.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://hbf.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://rvc.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mnh.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://iqx.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://qjl.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://vlf.pycfn.com

C#:   Console.WriteLine("Hello, World!");
来源：http://wgm.sysykeji.top

[A02] 变量声明与赋值
来源：http://bfz.yj202588.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bpz.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gct.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://vpu.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eot.cdnleiting.top

Java: String name = "Alex"; int age = 20;
来源：http://mwf.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://fyr.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://ngn.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://ssr.tanke756.top

[A03] 常量定义
来源：http://rpo.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ydc.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://nxi.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://qkt.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://bzp.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://nok.zhongyouzk.top

Go:   const PI = 3.14159
来源：http://lwu.smart0.xyz


<!-- 参考信息 -->