代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://bbt.yfazqb.com

sys.stdout.isatty()
来源：http://kdw.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://jjl.dashuyun.cn

print("err", file=sys.stderr)
来源：http://uvi.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://vmg.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://etr.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://kmv.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://scq.ybcxt.top

[U43] PHP：声明命名空间
来源：http://wqp.zhoulong.xyz

namespace App\Http;
来源：http://bkt.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://uzt.havefunace.top

declare(strict_types=1);
来源：http://fsx.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://rqf.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pwt.jlsjyb.cn

[U46] PHP：可空类型
来源：http://yfo.gogol.net.cn

?string $name = null
来源：http://bfa.smart0.xyz

[U47] PHP：联合类型
来源：http://vgb.shzxlz.cn

int|string $id
来源：http://uam.havefunace.top

[U48] PHP：纯枚举
来源：http://ryl.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aim.hesvh.cn

[U49] PHP：只读属性
来源：http://jfe.redwolf501.top

public readonly string $name
来源：http://ggw.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://orx.hysaishi.cn

public function __construct(private int $id) {}
来源：http://gdz.cqqwz.cn

[U51] PHP：数组解构
来源：http://cic.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://gej.tian-w.cn

[U52] PHP：箭头函数
来源：http://azh.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://jqn.birdmap.top

[U53] PHP：空合并运算符
来源：http://dns.havefunace.top

$v = $a ?? $b ?? "default";
来源：http://ngv.gogol.net.cn

[U54] PHP：空安全调用
来源：http://ndc.9152youxi.cn

$obj?->method()
来源：http://xxt.yfazqb.com

[U55] PHP：match 表达式
来源：http://jxm.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cjk.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://pem.tian-w.cn

f(a: 1, b: 2)
来源：http://lss.aibaodan.cn

[U57] PHP：字符串插值
来源：http://yko.nanxinkj.top

"值: {$a}"
来源：http://myp.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://rty.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mnh.dashuyun.cn

[U59] PHP：自定义排序
来源：http://qtx.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpv.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://phb.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ccf.yangfankeji.com

[U61] PHP：正则
来源：http://src.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ewq.yvedp.cn

[U62] PHP：日期对象
来源：http://cxa.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mrv.dianchejie.cn

[U63] PHP：文件读写
来源：http://dln.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://odw.tarul.cn

[U64] PHP：目录遍历
来源：http://hpl.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://ndd.wangdashe.top

[U65] PHP：会话
来源：http://umf.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wdq.yj202588.top

[U66] PHP：设置 Cookie
来源：http://qzd.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xcv.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://yly.snrcjt.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://utn.zhengqikj.top

[U68] PHP：PDO 连接
来源：http://lhj.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ifp.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://jxg.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eys.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://rgp.dashuyun.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zxy.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://ihd.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://pms.jinqigfzy.top

[U72] PHP：写错误日志
来源：http://myb.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://hzr.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://tit.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://qwm.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://mrp.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://kpk.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://clt.yonumen.top

composer require psr/container
来源：http://mrc.xylfe.cn

[U76] PHP：简单路由
来源：http://wmn.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ide.hcnkem.com

[U77] PHP：模板渲染
来源：http://tnq.birdmap.top

composer require twig/twig
来源：http://ioh.chenzaomai.com

[U78] PHP：单元测试
来源：http://ktk.sweek.top

composer require --dev phpunit/phpunit
来源：http://ikg.pycfn.com

[U79] PHP：静态分析
来源：http://mcf.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://gbd.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://gcq.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nlm.yj202588.top

[U81] JS：初始化项目
来源：http://hkg.jianghu66.top

npm init -y;  npm i express
来源：http://ijg.tian-w.cn

[U82] JS：package.json 脚本
来源：http://xbp.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mpr.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://aih.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://mfm.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://yam.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://cda.mhx1999.top

[U85] JS：可选链
来源：http://xne.jinqigufen.top

a?.b?.c
来源：http://pvc.yuanzhike.top

[U86] JS：空值合并
来源：http://jbx.sjlbkw.cn

a ?? b
来源：http://vdb.sxryk.cn

[U87] JS：解构默认值
来源：http://nge.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://unk.daria6918.cn

[U88] JS：对象展开合并
来源：http://kmi.tarul.cn

{ ...a, ...b }
来源：http://tyv.mhx1999.top

[U89] JS：数组去重
来源：http://xcl.zdbjq.cn

[...new Set(arr)]
来源：http://cnn.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://hka.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://atd.nwbrower.top

[U91] JS：对象键值遍历
来源：http://omr.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gnd.aizwys.cn

[U92] JS：深拷贝
来源：http://dsb.hywenlv.cn

structuredClone(obj)
来源：http://xug.xinyue.icu

[U93] JS：模板字符串
来源：http://gbc.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://hcv.yvedp.cn

[U94] JS：箭头函数
来源：http://zby.sxryk.cn

const double = x => x * 2;
来源：http://zri.zdqjudy.top

[U95] JS：Promise 包装
来源：http://ifv.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://mmr.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://zzs.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zwm.yj202588.top

[U97] JS：并发请求
来源：http://ftq.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lrp.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://klv.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wck.sjlbkw.cn

[U99] JS：事件监听
来源：http://jws.hnqzz.top

el.addEventListener("click", e => {})
来源：http://yav.yuxming.cn

[U100] JS：DOM 查询
来源：http://mah.jiagoushi.top

document.querySelector(".item")
来源：http://bxh.daria6918.cn

[U101] JS：classList 操作
来源：http://wyv.jlsjyb.cn

el.classList.toggle("active")
来源：http://vby.xziqi.cn

[U102] JS：本地存储
来源：http://yaz.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rpe.yfazqb.com

[U103] JS：定时器
来源：http://adj.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lvc.jinghuilouyu.cn

[U104] JS：防抖
来源：http://dxy.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nwq.gotoacloud.top

[U105] JS：节流
来源：http://asi.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mei.ivvv.top

[U106] JS：日期格式化
来源：http://fbg.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mcn.hnxiangtu.top

[U107] JS：数字千分位
来源：http://rvn.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mky.sufxvd.cn

[U108] JS：随机整数
来源：http://eag.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zsg.fehbvm.com

[U109] JS：数组分组
来源：http://dxq.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://pai.smart0.xyz

[U110] JS：数组分块
来源：http://qjd.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://agw.ctjpmb.com

[U111] JS：对象转 Map
来源：http://gvs.0kj1m.cn

new Map(Object.entries(obj))
来源：http://cit.vqdsnc.cn

[U112] JS：字符串补位
来源：http://fsa.yuxming.cn

"7".padStart(3, "0")
来源：http://rlh.yueranfly.top

[U113] JS：正则替换全部
来源：http://ebg.fengsongda.top

s.replaceAll("a", "b")
来源：http://mrv.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://rjk.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ybq.bjfxy.top

[U115] JS：生成 UUID
来源：http://vrg.yfazqb.com

crypto.randomUUID()
来源：http://qpb.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://ymz.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://rqv.xuanzx.com

[U117] JS：单元测试
来源：http://qkh.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://sya.fktsv.cn

[U118] JS：开发服务器
来源：http://kxe.andypj.xyz

npm i -D vite;  npx vite
来源：http://rjt.xuetiantiany.cn

[U119] JS：生产构建
来源：http://hvn.fehbvm.com

npx vite build
来源：http://mpz.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://dzj.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://dib.birdmap.top

================================================================================
来源：http://ybc.yj20258888.top

统计汇总
来源：http://nfk.zdqjudy.top

================================================================================
来源：http://uza.havefunace.top

按语言统计（条）：
来源：http://wyz.nanxuanxn.top

Python ......... 252
来源：http://npc.bjfxy.top

PHP ............ 252
来源：http://czd.sjlbkw.cn

JavaScript ..... 252
来源：http://iwr.yvedp.cn

TypeScript ..... 212
来源：http://mrb.9152youxi.cn

Java ........... 212
来源：http://cex.ivvv.top

Go ............. 212
来源：http://scm.yongpay.top

Ruby ........... 212
来源：http://xuj.cucudq.cn

C# ............. 212
来源：http://fck.iojbl.cn

C .............. 30
来源：http://ptc.tarul.cn

C++ ............ 30
来源：http://pvx.xingfuxueyuan.xyz

SQL ............ 90
来源：http://whm.chenlongwang.top

Bash ........... 80
来源：http://pzj.yuxming.cn

Kotlin ......... 15
来源：http://xcm.ydjk.org.cn

Swift .......... 15
来源：http://lck.zycfv.cn

Lua ............ 10
来源：http://qdj.yangfankeji.com

Perl ........... 10
来源：http://css.jqgfzy.top

Scala .......... 10
来源：http://vqr.jqgfzy.top

------------------------------------
来源：http://vhe.zdbjq.cn

合计 ........... 2106 条
来源：http://dyk.zhongyouzk.top

按章节统计：
来源：http://pwc.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://asc.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://szn.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vhh.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mwi.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pfk.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://asy.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wag.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://awx.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mdb.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dpb.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xom.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xke.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hal.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sgb.yonumen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lmp.jlsjyb.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rdg.c1oappe.top

Q SQL 专题                              90
来源：http://mhu.yonumen.top

R Bash 专题                             80
来源：http://zfg.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://ppx.sysykeji.top

T 其他语言补充                          60
来源：http://rtd.pengpengdd.cyou

U 高频实用片段                         120
来源：http://xkf.gaohongyu789.top

------------------------------------
来源：http://rba.52xcode.cn

合计                                  2106 条
来源：http://csu.yvedp.cn

--------------------------------------------------------------------------------
来源：http://zps.xuetiantiany.cn

使用提醒
来源：http://htt.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://coo.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rte.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://txd.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xyr.daxiang520.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wrw.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://int.smart0.xyz

—— 文件结束 ——
来源：http://kno.shuidangran.top

================================================================================
来源：http://rzn.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://sry.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://eri.wangdashe.top

================================================================================
来源：http://nno.xuetiantiany.cn

【收录内容】
来源：http://ixr.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://hbm.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bzq.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://pdx.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vir.dashuyun.cn

【使用说明】
来源：http://jfk.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mgr.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nsj.iojbl.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qxr.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dfw.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yup.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ygz.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mbh.chenjidiqi.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://heg.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jva.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wrz.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vlf.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://czm.cheryme.top

【文件统计】
来源：http://rsd.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sqo.xuanzx.com

--------------------------------------------------------------------------------
来源：http://njd.snrcjt.cn

目  录
来源：http://sxr.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://yjd.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jeb.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://phd.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gvr.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uit.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://enr.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ild.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xtp.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zxw.ivvv.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fop.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sag.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dpg.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cth.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ebu.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://byd.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://htl.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ifp.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://woy.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vyp.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zex.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vnt.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iyp.ehwqpu.com

================================================================================
来源：http://jim.jqgufenzy.top

A. 基础语法与类型
来源：http://zrn.nanxinkj.top

================================================================================
来源：http://fvb.nanxinkj.top

[A01] Hello World
来源：http://qlo.nanxinkj.top

Py:   print("Hello, World!")
来源：http://set.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://vod.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://bno.sxryk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pfc.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://nri.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://dwt.yj202588.top

Ruby: puts "Hello, World!"
来源：http://gop.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zmp.shangyingyoupin.top

[A02] 变量声明与赋值
来源：http://zza.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tsu.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sye.gogol.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sqy.vqdsnc.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lzg.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://tjp.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://abj.pycfn.com

Ruby: name = "Alex"; age = 20
来源：http://hzr.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://cpc.havefunace.top

[A03] 常量定义
来源：http://sck.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bde.shanyushiyangkeji.top

PHP:  const PI = 3.14159;
来源：http://ngt.xziqi.cn

JS:   const PI = 3.14159;
来源：http://peg.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://qbz.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://wvu.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://bqm.cheryme.top

Ruby: PI = 3.14159
来源：http://jks.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://kue.jinqigfzy.top

[A04] 判断变量类型
来源：http://sxf.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qlc.birdmap.top


<!-- 参考信息 -->