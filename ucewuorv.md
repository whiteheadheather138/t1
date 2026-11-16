代发 wailian999

[U37] Py：读写 Excel
来源：http://vdo.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://pvr.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://ioy.xziqi.cn

Path(__file__).resolve().parent
来源：http://gua.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://lfd.yuanzhike.top

sys.stdout.isatty()
来源：http://jdq.ydzc1.top

[U40] Py：打印到标准错误
来源：http://sld.tarul.cn

print("err", file=sys.stderr)
来源：http://wil.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://sfz.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://myj.tian-w.cn

[U42] PHP：PSR-4 自动加载
来源：http://oqt.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oxe.cheryme.top

[U43] PHP：声明命名空间
来源：http://mdr.fehbvm.com

namespace App\Http;
来源：http://bsf.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://jgc.yvedp.cn

declare(strict_types=1);
来源：http://rwh.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://qml.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://usb.fehbvm.com

[U46] PHP：可空类型
来源：http://htm.guowangkeji.top

?string $name = null
来源：http://kpo.kuanghao11.cn

[U47] PHP：联合类型
来源：http://anr.ctjpmb.com

int|string $id
来源：http://mbx.vehdjk.com

[U48] PHP：纯枚举
来源：http://zzl.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rcw.c1oappe.top

[U49] PHP：只读属性
来源：http://rkh.9152youxi.cn

public readonly string $name
来源：http://yuh.nanxinkj.top

[U50] PHP：构造器属性提升
来源：http://fnr.vehdjk.com

public function __construct(private int $id) {}
来源：http://nvy.iojbl.cn

[U51] PHP：数组解构
来源：http://utm.yvedp.cn

[$a, $b] = $arr;
来源：http://qan.fengsongda.top

[U52] PHP：箭头函数
来源：http://egd.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://ihh.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://xxr.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://yht.zdbjq.cn

[U54] PHP：空安全调用
来源：http://lxk.hammf.cn

$obj?->method()
来源：http://gup.yj202588.top

[U55] PHP：match 表达式
来源：http://hsw.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uux.sufxvd.cn

[U56] PHP：命名参数
来源：http://rdk.hywenlv.cn

f(a: 1, b: 2)
来源：http://owc.cdnleiting.top

[U57] PHP：字符串插值
来源：http://vni.yj202588.top

"值: {$a}"
来源：http://ewa.hammf.cn

[U58] PHP：数组三件套
来源：http://miz.gogol.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vgl.0kj1m.cn

[U59] PHP：自定义排序
来源：http://wkq.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pxf.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://wti.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ywn.vehdjk.com

[U61] PHP：正则
来源：http://wni.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ymx.zhixingplan.top

[U62] PHP：日期对象
来源：http://bhj.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xgy.zhijiandao.cn

[U63] PHP：文件读写
来源：http://mzv.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oqt.hesvh.cn

[U64] PHP：目录遍历
来源：http://ymv.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://utb.zhijiandao.cn

[U65] PHP：会话
来源：http://eai.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lta.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://bjn.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://syx.xziqi.cn

[U67] PHP：处理文件上传
来源：http://qhk.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tre.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://wvo.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://naz.sweek.top

[U69] PHP：PDO 预处理
来源：http://qkd.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gof.yj20258888.top

[U70] PHP：PDO 事务
来源：http://tix.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://alz.svipenyu.cn

[U71] PHP：抛出异常
来源：http://jhr.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://obd.jyoumei.cn

[U72] PHP：写错误日志
来源：http://qqx.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://qkr.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://nkq.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://xsx.sweek.top

[U74] PHP：读取环境变量
来源：http://daq.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://xnn.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://coc.jqgufenzy.top

composer require psr/container
来源：http://swx.ydzc1.top

[U76] PHP：简单路由
来源：http://dtg.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://phi.wangdashe.top

[U77] PHP：模板渲染
来源：http://jhp.ywan-chungtsiang.top

composer require twig/twig
来源：http://mog.sweek.top

[U78] PHP：单元测试
来源：http://mqy.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://kqz.fktsv.cn

[U79] PHP：静态分析
来源：http://fox.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://yts.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://hio.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hgu.yfazqb.com

[U81] JS：初始化项目
来源：http://chp.bjfxy.top

npm init -y;  npm i express
来源：http://bpr.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://gmt.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://emp.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://kow.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://ref.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://gbq.epnwcf.com

module.exports = { a };  const { a } = require("./m");
来源：http://uqq.yuanzhike.top

[U85] JS：可选链
来源：http://jlu.ppjwa.cn

a?.b?.c
来源：http://nqa.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://tsw.sjlbkw.cn

a ?? b
来源：http://eat.ehwqpu.com

[U87] JS：解构默认值
来源：http://tnf.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://yeb.andypj.xyz

[U88] JS：对象展开合并
来源：http://ssk.zdqjudy.top

{ ...a, ...b }
来源：http://qfz.cheryme.top

[U89] JS：数组去重
来源：http://yxv.yongpay.top

[...new Set(arr)]
来源：http://mdq.jiagoushi.top

[U90] JS：数字数组排序
来源：http://txt.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://osi.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://ame.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://phf.ivvv.top

[U92] JS：深拷贝
来源：http://bfl.tanke756.top

structuredClone(obj)
来源：http://fev.c1oappe.top

[U93] JS：模板字符串
来源：http://rrl.sjlbkw.cn

`共 ${n} 条`
来源：http://ifz.9152youxi.cn

[U94] JS：箭头函数
来源：http://anm.zhoulong.xyz

const double = x => x * 2;
来源：http://kxw.9152youxi.cn

[U95] JS：Promise 包装
来源：http://gnr.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://gmb.yfazqb.com

[U96] JS：async/await 与异常
来源：http://yif.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://znl.52xcode.cn

[U97] JS：并发请求
来源：http://boq.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://nzf.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://eqc.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ubc.zycfv.cn

[U99] JS：事件监听
来源：http://ikl.gzhubu.top

el.addEventListener("click", e => {})
来源：http://qdg.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://yfl.bjfxy.top

document.querySelector(".item")
来源：http://pdg.cdnleiting.top

[U101] JS：classList 操作
来源：http://sqm.dashuyun.cn

el.classList.toggle("active")
来源：http://xqx.shzxlz.cn

[U102] JS：本地存储
来源：http://dbp.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gzx.xziqi.cn

[U103] JS：定时器
来源：http://mmz.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zpc.daria6918.cn

[U104] JS：防抖
来源：http://tbv.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sto.xziqi.cn

[U105] JS：节流
来源：http://glx.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zji.zhongyouzk.top

[U106] JS：日期格式化
来源：http://quz.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uib.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://sml.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blw.mhx1999.top

[U108] JS：随机整数
来源：http://tni.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nls.jlsjyb.cn

[U109] JS：数组分组
来源：http://nfm.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://arp.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://wor.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xlz.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://vbl.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://nom.fehbvm.com

[U112] JS：字符串补位
来源：http://ytn.0kj1m.cn

"7".padStart(3, "0")
来源：http://ajt.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://gia.wangdashe.top

s.replaceAll("a", "b")
来源：http://qyh.shuidangran.top

[U114] JS：JSON 深比较
来源：http://xbw.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qjs.iojbl.cn

[U115] JS：生成 UUID
来源：http://gnm.tianlin.xyz

crypto.randomUUID()
来源：http://fgv.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://eqx.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://ktv.hnqzz.top

[U117] JS：单元测试
来源：http://bxa.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://wjq.guowangkeji.top

[U118] JS：开发服务器
来源：http://swk.yangfankeji.com

npm i -D vite;  npx vite
来源：http://zgx.0kj1m.cn

[U119] JS：生产构建
来源：http://gum.yongpay.top

npx vite build
来源：http://wfr.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://sbu.meibo888.top

import.meta.env.VITE_API_URL
来源：http://hsp.ydjk.org.cn

================================================================================
来源：http://mye.epnwcf.com

统计汇总
来源：http://toa.sxryk.cn

================================================================================
来源：http://atm.birdmap.top

按语言统计（条）：
来源：http://owk.shanyushiyangkeji.top

Python ......... 252
来源：http://xws.sweek.top

PHP ............ 252
来源：http://rbp.yangfankeji.com

JavaScript ..... 252
来源：http://pfb.jinqigfzy.top

TypeScript ..... 212
来源：http://rpu.jqgufenzy.top

Java ........... 212
来源：http://snj.jinqigufen.top

Go ............. 212
来源：http://jjx.yj202588.top

Ruby ........... 212
来源：http://tbu.zhixingplan.top

C# ............. 212
来源：http://xiq.redwolf501.top

C .............. 30
来源：http://jqx.xylfe.cn

C++ ............ 30
来源：http://xxg.ivvv.top

SQL ............ 90
来源：http://liu.9152youxi.cn

Bash ........... 80
来源：http://apa.xuetiantiany.cn

Kotlin ......... 15
来源：http://rtd.zhixingplan.top

Swift .......... 15
来源：http://nys.aizwys.cn

Lua ............ 10
来源：http://aex.shangyingyoupin.top

Perl ........... 10
来源：http://ayk.gogol.net.cn

Scala .......... 10
来源：http://ukd.ehwqpu.com

------------------------------------
来源：http://kmj.cdnleiting.top

合计 ........... 2106 条
来源：http://pro.pengpengdd.cyou

按章节统计：
来源：http://azr.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lmn.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://opu.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ivy.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cvo.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qhs.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dyb.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zap.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://byn.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dyw.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pyv.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qbg.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dfa.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://txd.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ecj.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qyz.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nvd.zhoulong.xyz

Q SQL 专题                              90
来源：http://fdd.hysaishi.cn

R Bash 专题                             80
来源：http://hse.tarul.cn

S C / C++ 专题                          60
来源：http://cui.cheryme.top

T 其他语言补充                          60
来源：http://oni.hnxiangtu.top

U 高频实用片段                         120
来源：http://xev.jinyuanbaomall.cn

------------------------------------
来源：http://lgd.c1oappe.top

合计                                  2106 条
来源：http://gtu.fktsv.cn

--------------------------------------------------------------------------------
来源：http://ekv.zhaomingkeji.xyz

使用提醒
来源：http://zjs.shuidangran.top

--------------------------------------------------------------------------------
来源：http://lkq.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xhi.hesvh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mwo.ydzc1.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gzu.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fvo.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://quh.fengsongda.top

—— 文件结束 ——
来源：http://lhe.cdnleiting.top

================================================================================
来源：http://gci.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://nli.xinyue.icu

Common Programming Examples Cheat Book
来源：http://zma.yvedp.cn

================================================================================
来源：http://pft.hnqzz.top

【收录内容】
来源：http://utm.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rmg.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gnw.zdqjudy.top

SQL · Bash · C · C++
来源：http://vpy.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kkz.fzhhl.top

【使用说明】
来源：http://pxo.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ezx.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vcd.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pzk.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cby.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://fff.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dvo.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xur.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tvw.zhongyouzk.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xbh.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zis.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xwv.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://acy.zhongyouzk.top

【文件统计】
来源：http://avi.yuanzhike.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wfw.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://zhi.shzxlz.cn

目  录
来源：http://yko.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://acs.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jss.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kyg.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vsw.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://psm.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zpt.yuxming.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gfx.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://egv.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nol.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kua.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tuk.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uor.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mjy.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xpp.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://guu.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sxv.cucudq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tpd.jqgfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yla.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wdr.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pkw.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fml.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ycb.andypj.xyz

================================================================================
来源：http://taf.jinqigfzy.top

A. 基础语法与类型
来源：http://uig.ywan-chungtsiang.top

================================================================================
来源：http://pwr.ywan-chungtsiang.top

[A01] Hello World
来源：http://xnf.pycfn.com

Py:   print("Hello, World!")
来源：http://hjq.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://gfa.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://uja.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://etm.cdnleiting.top

Java: System.out.println("Hello, World!");
来源：http://tux.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://vjy.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://rqa.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kkq.hammf.cn

[A02] 变量声明与赋值
来源：http://dyk.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qyg.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fxs.bbcook.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zmm.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hhl.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://hgn.hongshengwenyu.top

Go:   name := "Alex"; age := 20
来源：http://fjn.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://xyv.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hir.jiagoushi.top

[A03] 常量定义
来源：http://kvh.shuidangran.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccl.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://cvc.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://sgq.cdnleiting.top

TS:   const PI: number = 3.14159;
来源：http://aie.tarul.cn

Java: static final double PI = 3.14159;
来源：http://zvn.guowangkeji.top

Go:   const PI = 3.14159
来源：http://xuh.gotoacloud.top


<!-- 参考信息 -->