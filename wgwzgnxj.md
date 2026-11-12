代发 wailian999

[U37] Py：读写 Excel
来源：http://vcn.andypj.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://dbq.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://zom.hesvh.cn

Path(__file__).resolve().parent
来源：http://vnc.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://dnp.daria6918.cn

sys.stdout.isatty()
来源：http://ryr.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://jtj.ehwqpu.com

print("err", file=sys.stderr)
来源：http://jkn.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://kky.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://cnu.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://otj.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ifs.snrcjt.cn

[U43] PHP：声明命名空间
来源：http://zgh.aizwys.cn

namespace App\Http;
来源：http://uwj.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://syz.zycfv.cn

declare(strict_types=1);
来源：http://bsz.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://yow.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sdi.feifeiyinyue.top

[U46] PHP：可空类型
来源：http://hgv.wangshuangyany.cn

?string $name = null
来源：http://iru.daxiang520.top

[U47] PHP：联合类型
来源：http://syz.smart0.xyz

int|string $id
来源：http://zsc.yj202588.top

[U48] PHP：纯枚举
来源：http://mgu.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gsm.0kj1m.cn

[U49] PHP：只读属性
来源：http://pgo.yj20258888.top

public readonly string $name
来源：http://uup.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://brr.vehdjk.com

public function __construct(private int $id) {}
来源：http://pwo.hongshengwenyu.top

[U51] PHP：数组解构
来源：http://kql.nwbrower.top

[$a, $b] = $arr;
来源：http://vrg.vehdjk.com

[U52] PHP：箭头函数
来源：http://viq.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://urh.sxryk.cn

[U53] PHP：空合并运算符
来源：http://sxz.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://xuv.snrcjt.cn

[U54] PHP：空安全调用
来源：http://xdu.chenzaomai.com

$obj?->method()
来源：http://mml.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://vom.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sfc.daxiang520.top

[U56] PHP：命名参数
来源：http://sxn.tarul.cn

f(a: 1, b: 2)
来源：http://ibz.yangfankeji.com

[U57] PHP：字符串插值
来源：http://svp.c1oappe.top

"值: {$a}"
来源：http://dhn.ivvv.top

[U58] PHP：数组三件套
来源：http://mdr.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ffr.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://aaz.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zix.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://dba.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ufn.yangfankeji.com

[U61] PHP：正则
来源：http://xzn.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jbc.xylfe.cn

[U62] PHP：日期对象
来源：http://ygp.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aqv.hfpthk.cn

[U63] PHP：文件读写
来源：http://dym.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dkk.gogol.net.cn

[U64] PHP：目录遍历
来源：http://siv.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://dbr.nanxinkj.top

[U65] PHP：会话
来源：http://wog.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://uqb.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://hby.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mml.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://asp.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://viw.yvedp.cn

[U68] PHP：PDO 连接
来源：http://lie.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sow.yonumen.top

[U69] PHP：PDO 预处理
来源：http://cyf.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zgo.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://atp.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gyn.9152youxi.cn

[U71] PHP：抛出异常
来源：http://drf.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://sbo.hesvh.cn

[U72] PHP：写错误日志
来源：http://ocq.tianlin.xyz

error_log("失败: " . $e->getMessage());
来源：http://btv.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://tso.birdmap.top

parse_ini_file("config.ini", true)
来源：http://wat.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://tao.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://gtl.gzhubu.top

[U75] PHP：依赖注入
来源：http://dzn.zdbjq.cn

composer require psr/container
来源：http://oah.chenlongwang.top

[U76] PHP：简单路由
来源：http://jtp.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qxo.hcnkem.com

[U77] PHP：模板渲染
来源：http://hwl.ehwqpu.com

composer require twig/twig
来源：http://ijm.zdbjq.cn

[U78] PHP：单元测试
来源：http://qqf.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://ahq.52xcode.cn

[U79] PHP：静态分析
来源：http://cao.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://aqx.birdmap.top

[U80] PHP：代码规范修复
来源：http://iyz.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://nmj.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://wth.wangdashe.top

npm init -y;  npm i express
来源：http://oxc.yonumen.top

[U82] JS：package.json 脚本
来源：http://szl.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://efd.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://jxm.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://hup.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://prz.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gak.xziqi.cn

[U85] JS：可选链
来源：http://nbe.xingfuxueyuan.xyz

a?.b?.c
来源：http://riq.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://zfj.0kj1m.cn

a ?? b
来源：http://atl.jinghuilouyu.cn

[U87] JS：解构默认值
来源：http://qfc.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://tvl.yangfankeji.com

[U88] JS：对象展开合并
来源：http://rcb.ywan-chungtsiang.top

{ ...a, ...b }
来源：http://ogj.hfpthk.cn

[U89] JS：数组去重
来源：http://axc.ybcxt.top

[...new Set(arr)]
来源：http://mqw.c1oappe.top

[U90] JS：数字数组排序
来源：http://das.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://oic.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://yim.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gza.jqgufenzy.top

[U92] JS：深拷贝
来源：http://ztm.jqgfzy.top

structuredClone(obj)
来源：http://pfx.hnqzz.top

[U93] JS：模板字符串
来源：http://rpc.jqgfzy.top

`共 ${n} 条`
来源：http://pko.jyoumei.cn

[U94] JS：箭头函数
来源：http://nkk.cheryme.top

const double = x => x * 2;
来源：http://psx.ydzc1.top

[U95] JS：Promise 包装
来源：http://dwy.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://wfu.ydzc1.top

[U96] JS：async/await 与异常
来源：http://xqi.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ngz.zhijiandao.cn

[U97] JS：并发请求
来源：http://hzw.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gyr.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://kbb.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://amy.ybcxt.top

[U99] JS：事件监听
来源：http://wio.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://npp.yuxming.cn

[U100] JS：DOM 查询
来源：http://vgb.ydzc1.top

document.querySelector(".item")
来源：http://vob.fehbvm.com

[U101] JS：classList 操作
来源：http://ozj.andypj.xyz

el.classList.toggle("active")
来源：http://qqq.kuanghao11.cn

[U102] JS：本地存储
来源：http://sdl.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ati.snrcjt.cn

[U103] JS：定时器
来源：http://fzz.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jxp.guannengcc.top

[U104] JS：防抖
来源：http://vdx.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ziw.yj20258.top

[U105] JS：节流
来源：http://hxx.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ipj.kuanghao11.cn

[U106] JS：日期格式化
来源：http://ulc.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rvg.9152youxi.cn

[U107] JS：数字千分位
来源：http://oaj.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vre.smart0.xyz

[U108] JS：随机整数
来源：http://ztl.fzhhl.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ngt.zhixingplan.top

[U109] JS：数组分组
来源：http://cjc.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://lac.yueranfly.top

[U110] JS：数组分块
来源：http://hkz.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mhb.yueranfly.top

[U111] JS：对象转 Map
来源：http://stb.ppjwa.cn

new Map(Object.entries(obj))
来源：http://qiu.shuidangran.top

[U112] JS：字符串补位
来源：http://hyn.c1oappe.top

"7".padStart(3, "0")
来源：http://lvb.tian-w.cn

[U113] JS：正则替换全部
来源：http://prt.nwbrower.top

s.replaceAll("a", "b")
来源：http://cjl.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://pun.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uzc.ybcxt.top

[U115] JS：生成 UUID
来源：http://rci.meibo888.top

crypto.randomUUID()
来源：http://hix.svipenyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://rmg.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://rni.shzxlz.cn

[U117] JS：单元测试
来源：http://wvq.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://ixx.gogol.net.cn

[U118] JS：开发服务器
来源：http://qhl.dashuyun.cn

npm i -D vite;  npx vite
来源：http://fdo.guowangkeji.top

[U119] JS：生产构建
来源：http://qdk.vehdjk.com

npx vite build
来源：http://btw.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://ase.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://jdq.xziqi.cn

================================================================================
来源：http://jkk.sxryk.cn

统计汇总
来源：http://rxw.ctjpmb.com

================================================================================
来源：http://xdv.bjfxy.top

按语言统计（条）：
来源：http://vvw.hnqzz.top

Python ......... 252
来源：http://aaq.ehwqpu.com

PHP ............ 252
来源：http://rbt.yueranfly.top

JavaScript ..... 252
来源：http://buw.ivvv.top

TypeScript ..... 212
来源：http://vlq.wangshuangyany.cn

Java ........... 212
来源：http://fqs.guowangkeji.top

Go ............. 212
来源：http://atc.fzhhl.top

Ruby ........... 212
来源：http://rfy.zdqjudy.top

C# ............. 212
来源：http://fin.hongshengwenyu.top

C .............. 30
来源：http://vxq.c1oappe.top

C++ ............ 30
来源：http://qrr.nanxinkj.top

SQL ............ 90
来源：http://vxl.hfpthk.cn

Bash ........... 80
来源：http://xnw.yuanzhike.top

Kotlin ......... 15
来源：http://tji.cashguo.top

Swift .......... 15
来源：http://bib.nwbrower.top

Lua ............ 10
来源：http://xhg.ivvv.top

Perl ........... 10
来源：http://eda.wangshuangyany.cn

Scala .......... 10
来源：http://bbo.cqqwz.cn

------------------------------------
来源：http://rba.0kj1m.cn

合计 ........... 2106 条
来源：http://oas.jyoumei.cn

按章节统计：
来源：http://uth.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hhh.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xuv.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vbl.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://plu.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qil.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://unj.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vic.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cgn.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kdb.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xcf.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://osy.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fcy.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nhk.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ztc.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uzt.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xyj.yanxiufei.cn

Q SQL 专题                              90
来源：http://cmi.zhoulong.xyz

R Bash 专题                             80
来源：http://ioi.kuanghao11.cn

S C / C++ 专题                          60
来源：http://bqn.zdqjudy.top

T 其他语言补充                          60
来源：http://sza.hcnkem.com

U 高频实用片段                         120
来源：http://kny.xinyue.icu

------------------------------------
来源：http://dso.andypj.xyz

合计                                  2106 条
来源：http://juh.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://apr.yj20258888.top

使用提醒
来源：http://uky.uphjek.com

--------------------------------------------------------------------------------
来源：http://btc.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oew.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cvj.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pol.vqdsnc.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xdt.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nfb.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://wxl.hammf.cn

================================================================================
来源：http://fsp.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://mdt.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://rcb.chenjidiqi.icu

================================================================================
来源：http://xdb.hesvh.cn

【收录内容】
来源：http://mlf.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pay.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gmw.hcnkem.com

SQL · Bash · C · C++
来源：http://zjz.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sdp.zhengqikj.top

【使用说明】
来源：http://gld.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bpi.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xwz.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zmy.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://trb.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rya.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://htx.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ill.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://osq.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://skk.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jhi.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qwt.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mgo.yueranfly.top

【文件统计】
来源：http://zhx.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zxp.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://qgx.bbcook.cn

目  录
来源：http://xyl.tarul.cn

--------------------------------------------------------------------------------
来源：http://zzq.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mha.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://axn.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lks.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://aog.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://syp.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mwf.yj20258888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dcf.guowangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xzn.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://glx.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ehq.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bnm.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eeh.hfpthk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mqo.chenzaomai.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mjh.guowangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://byp.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hbw.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fuk.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://shr.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ffj.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pjq.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qzi.xylfe.cn

================================================================================
来源：http://zsd.hongshengwenyu.top

A. 基础语法与类型
来源：http://wkw.chenlongwang.top

================================================================================
来源：http://ycz.shuidangran.top

[A01] Hello World
来源：http://lth.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://ogb.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://lrx.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://oqb.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://akb.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://emx.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://ple.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://upl.gzhubu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tfr.wangdashe.top

[A02] 变量声明与赋值
来源：http://btn.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://clb.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jef.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://grl.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pio.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://kvw.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://vos.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://lwz.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://cnr.bjfxy.top

[A03] 常量定义
来源：http://jca.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uyp.shanyushiyangtech.top

PHP:  const PI = 3.14159;
来源：http://tiu.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://glk.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://san.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://egz.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://xym.52xcode.cn


<!-- 参考信息 -->