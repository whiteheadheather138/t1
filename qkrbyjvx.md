代发 wailian999

[U35] Py：发送邮件
来源：http://awh.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sjh.gaohongyu789.top

[U36] Py：定时任务
来源：http://lhq.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://qjl.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://fbg.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://ozt.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://nji.jyoumei.cn

Path(__file__).resolve().parent
来源：http://erl.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://sjl.yj20258.top

sys.stdout.isatty()
来源：http://mvg.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://rth.yj202588.top

print("err", file=sys.stderr)
来源：http://wjk.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://fqg.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fuk.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://bjv.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kve.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://zyw.andypj.xyz

namespace App\Http;
来源：http://ymu.yfazqb.com

[U44] PHP：开启严格类型
来源：http://zoc.jiagoushi.top

declare(strict_types=1);
来源：http://bqt.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://uvm.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vqd.zycfv.cn

[U46] PHP：可空类型
来源：http://ded.jianghu66.top

?string $name = null
来源：http://zxx.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://ugs.dianchejie.cn

int|string $id
来源：http://ial.gotoacloud.top

[U48] PHP：纯枚举
来源：http://fga.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nci.nanxinkj.top

[U49] PHP：只读属性
来源：http://dia.nanxuanxn.top

public readonly string $name
来源：http://sbl.yonumen.top

[U50] PHP：构造器属性提升
来源：http://avy.zdbjq.cn

public function __construct(private int $id) {}
来源：http://kra.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://cry.sufxvd.cn

[$a, $b] = $arr;
来源：http://neo.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://riu.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://isi.nwbrower.top

[U53] PHP：空合并运算符
来源：http://rko.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://uqr.yj202588.top

[U54] PHP：空安全调用
来源：http://pgt.hnqzz.top

$obj?->method()
来源：http://ffj.wangdashe.top

[U55] PHP：match 表达式
来源：http://erz.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nei.havefunace.top

[U56] PHP：命名参数
来源：http://jeu.yj202588.top

f(a: 1, b: 2)
来源：http://ykd.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://fht.ctjpmb.com

"值: {$a}"
来源：http://tga.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://qcb.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iib.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://lyz.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uqr.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://qhx.ydjk.org.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fnu.hnxiangtu.top

[U61] PHP：正则
来源：http://sad.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jmw.cashguo.top

[U62] PHP：日期对象
来源：http://pit.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ezg.aizwys.cn

[U63] PHP：文件读写
来源：http://kzc.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://juy.xinyue.icu

[U64] PHP：目录遍历
来源：http://syi.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://klt.yonumen.top

[U65] PHP：会话
来源：http://zmc.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iom.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://wgp.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yjb.aizwys.cn

[U67] PHP：处理文件上传
来源：http://vxn.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hij.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://ijr.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://auo.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://bvy.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jye.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://bzz.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eox.hammf.cn

[U71] PHP：抛出异常
来源：http://lnw.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://iet.zhengqikj.top

[U72] PHP：写错误日志
来源：http://oxr.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://erq.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://xyb.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://mwg.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://axr.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://otz.yueranfly.top

[U75] PHP：依赖注入
来源：http://swj.cashguo.top

composer require psr/container
来源：http://vrz.chenlongwang.top

[U76] PHP：简单路由
来源：http://zbr.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uou.yfazqb.com

[U77] PHP：模板渲染
来源：http://ryi.jinqigufen.top

composer require twig/twig
来源：http://kur.quarkkingdee.top

[U78] PHP：单元测试
来源：http://mwh.meibo888.top

composer require --dev phpunit/phpunit
来源：http://kwl.bjfxy.top

[U79] PHP：静态分析
来源：http://ugt.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://ewq.uphjek.com

[U80] PHP：代码规范修复
来源：http://clz.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wrr.yonumen.top

[U81] JS：初始化项目
来源：http://hdl.xinyue.icu

npm init -y;  npm i express
来源：http://ypq.hammf.cn

[U82] JS：package.json 脚本
来源：http://kcg.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bum.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://qwg.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yjv.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://rms.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hfj.hcnkem.com

[U85] JS：可选链
来源：http://wiz.gaohongyu789.top

a?.b?.c
来源：http://wge.gaohongyu789.top

[U86] JS：空值合并
来源：http://ife.tarul.cn

a ?? b
来源：http://lkx.chenzaomai.com

[U87] JS：解构默认值
来源：http://net.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://ixo.hywenlv.cn

[U88] JS：对象展开合并
来源：http://xnj.fehbvm.com

{ ...a, ...b }
来源：http://ncl.havefunace.top

[U89] JS：数组去重
来源：http://lmd.chenjidiqi.icu

[...new Set(arr)]
来源：http://tod.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://sdj.yuanzhike.top

[...arr].sort((a, b) => a - b)
来源：http://eyl.hnqzz.top

[U91] JS：对象键值遍历
来源：http://vrk.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tqb.ydjk.org.cn

[U92] JS：深拷贝
来源：http://tht.dashuyun.cn

structuredClone(obj)
来源：http://hlk.haohaochexian.top

[U93] JS：模板字符串
来源：http://kcj.shangyingyoupin.top

`共 ${n} 条`
来源：http://bch.tian-w.cn

[U94] JS：箭头函数
来源：http://dhv.jinqigufen.top

const double = x => x * 2;
来源：http://lxn.svipenyu.cn

[U95] JS：Promise 包装
来源：http://ozp.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://lje.feifeiyinyue.top

[U96] JS：async/await 与异常
来源：http://vwh.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wlw.shzxlz.cn

[U97] JS：并发请求
来源：http://jqs.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jkm.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://kxi.tianlin.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rbi.zhijiandao.cn

[U99] JS：事件监听
来源：http://fdv.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://sgi.hywenlv.cn

[U100] JS：DOM 查询
来源：http://xed.sufxvd.cn

document.querySelector(".item")
来源：http://uli.gogol.net.cn

[U101] JS：classList 操作
来源：http://pba.bjfxy.top

el.classList.toggle("active")
来源：http://eay.ybcxt.top

[U102] JS：本地存储
来源：http://dde.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bgb.zhijiandao.cn

[U103] JS：定时器
来源：http://dom.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ilf.yj20258.top

[U104] JS：防抖
来源：http://sng.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://llq.xinyue.icu

[U105] JS：节流
来源：http://qlj.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nwq.iojbl.cn

[U106] JS：日期格式化
来源：http://hbq.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vzx.snrcjt.cn

[U107] JS：数字千分位
来源：http://nys.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dky.xinyue.icu

[U108] JS：随机整数
来源：http://lzg.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://afw.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://bny.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://lif.smart0.xyz

[U110] JS：数组分块
来源：http://pis.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qtw.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://mjm.cdnleiting.top

new Map(Object.entries(obj))
来源：http://reg.shuidangran.top

[U112] JS：字符串补位
来源：http://exn.yj20258.top

"7".padStart(3, "0")
来源：http://acm.aizwys.cn

[U113] JS：正则替换全部
来源：http://gyd.meibo888.top

s.replaceAll("a", "b")
来源：http://vfp.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://ied.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ysm.chenzaomai.com

[U115] JS：生成 UUID
来源：http://uqw.gzhubu.top

crypto.randomUUID()
来源：http://zum.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://meo.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://ghz.guowangkeji.top

[U117] JS：单元测试
来源：http://sug.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://nwy.ydjk.org.cn

[U118] JS：开发服务器
来源：http://tzt.birdmap.top

npm i -D vite;  npx vite
来源：http://qdn.ywan-chungtsiang.top

[U119] JS：生产构建
来源：http://sna.iojbl.cn

npx vite build
来源：http://ynn.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://qwf.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://txb.shzxlz.cn

================================================================================
来源：http://xrt.shzxlz.cn

统计汇总
来源：http://qnj.ybcxt.top

================================================================================
来源：http://and.pycfn.com

按语言统计（条）：
来源：http://uvq.daria6918.cn

Python ......... 252
来源：http://hmy.ppjwa.cn

PHP ............ 252
来源：http://dmc.havefunace.top

JavaScript ..... 252
来源：http://ibh.hfpthk.cn

TypeScript ..... 212
来源：http://hck.zhixingplan.top

Java ........... 212
来源：http://mra.feifeiyinyue.top

Go ............. 212
来源：http://yzq.feifeiyinyue.top

Ruby ........... 212
来源：http://isf.yueranfly.top

C# ............. 212
来源：http://yhj.tarul.cn

C .............. 30
来源：http://vsr.yongpay.top

C++ ............ 30
来源：http://ekk.c1oappe.top

SQL ............ 90
来源：http://gpu.316326.xyz

Bash ........... 80
来源：http://ntf.nanxuanxn.top

Kotlin ......... 15
来源：http://zjo.yj202588.top

Swift .......... 15
来源：http://gby.nanxinkj.top

Lua ............ 10
来源：http://tyd.bjfxy.top

Perl ........... 10
来源：http://zja.bbcook.cn

Scala .......... 10
来源：http://tlz.aibaodan.cn

------------------------------------
来源：http://muk.jqgfzy.top

合计 ........... 2106 条
来源：http://vlz.shanyushiyangtech.top

按章节统计：
来源：http://luh.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eoa.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://veq.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mkm.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://son.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dzz.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hvj.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ulw.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gqx.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tpp.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ygj.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hks.jiagoushi.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://div.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nkw.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gdt.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zdd.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bbm.hysaishi.cn

Q SQL 专题                              90
来源：http://nzb.gotoacloud.top

R Bash 专题                             80
来源：http://bxv.0kj1m.cn

S C / C++ 专题                          60
来源：http://vxr.mhx1999.top

T 其他语言补充                          60
来源：http://uhp.hesvh.cn

U 高频实用片段                         120
来源：http://ong.pycfn.com

------------------------------------
来源：http://suh.iojbl.cn

合计                                  2106 条
来源：http://scr.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://svg.tianlin.xyz

使用提醒
来源：http://zbn.havefunace.top

--------------------------------------------------------------------------------
来源：http://geh.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vew.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ptz.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sif.nanxinkj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cct.fengsongda.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kyx.yongpay.top

—— 文件结束 ——
来源：http://djf.jianghu66.top

================================================================================
来源：http://wbf.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://inv.yj20258888.top

Common Programming Examples Cheat Book
来源：http://crl.jqgfzy.top

================================================================================
来源：http://xai.shanyushiyangkeji.top

【收录内容】
来源：http://lzm.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tda.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://woq.xylfe.cn

SQL · Bash · C · C++
来源：http://bpg.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sfy.hcnkem.com

【使用说明】
来源：http://yte.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gln.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qpj.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kmc.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kgr.jqgfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://czf.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lue.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zug.zhiwuduotai.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wvb.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hkk.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yzc.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xin.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://boe.yj20258.top

【文件统计】
来源：http://ael.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nuf.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://cty.shanyushiyangtech.top

目  录
来源：http://sgd.tanke756.top

--------------------------------------------------------------------------------
来源：http://wnh.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nzh.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rtd.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zir.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gnw.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uez.yvedp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tvo.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cqs.daria6918.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jyi.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ymq.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://esf.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qnh.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://djj.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kxu.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uae.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qxd.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tpr.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tmn.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pan.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vpw.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rgj.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dku.yongpay.top

================================================================================
来源：http://cds.nwbrower.top

A. 基础语法与类型
来源：http://ayf.yj202588.top

================================================================================
来源：http://cdy.ehwqpu.com

[A01] Hello World
来源：http://kcq.sufxvd.cn

Py:   print("Hello, World!")
来源：http://myd.hnqzz.top

PHP:  echo "Hello, World!";
来源：http://rco.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://vue.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mln.epnwcf.com

Java: System.out.println("Hello, World!");
来源：http://vzn.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://iwv.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://cqr.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://rkm.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://uas.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lgy.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://icv.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://atx.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://osm.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://hjn.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://hrc.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://anq.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xbq.bjfxy.top

[A03] 常量定义
来源：http://nfw.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tuo.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://oww.jinqigfzy.top


<!-- 参考信息 -->