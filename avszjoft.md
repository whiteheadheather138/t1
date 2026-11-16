代发 wailian999

[U37] Py：读写 Excel
来源：http://iqp.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://vuv.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://ntv.52xcode.cn

Path(__file__).resolve().parent
来源：http://cpu.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://sea.nanxinkj.top

sys.stdout.isatty()
来源：http://dbm.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://csq.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://rhf.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rbl.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yzc.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://alr.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fbp.snrcjt.cn

[U43] PHP：声明命名空间
来源：http://eqp.haohaochexian.top

namespace App\Http;
来源：http://drd.havefunace.top

[U44] PHP：开启严格类型
来源：http://voh.sxryk.cn

declare(strict_types=1);
来源：http://uri.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://ogb.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gwz.yj202588.top

[U46] PHP：可空类型
来源：http://hph.bbcook.cn

?string $name = null
来源：http://xpi.nanxuanxn.top

[U47] PHP：联合类型
来源：http://ija.shangyingyoupin.top

int|string $id
来源：http://hws.ydzc1.top

[U48] PHP：纯枚举
来源：http://ple.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cif.52xcode.cn

[U49] PHP：只读属性
来源：http://ukz.zhiwuduotai.top

public readonly string $name
来源：http://vks.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://mnf.chenlongwang.top

public function __construct(private int $id) {}
来源：http://etn.guannengcc.top

[U51] PHP：数组解构
来源：http://mnr.zdqjudy.top

[$a, $b] = $arr;
来源：http://pip.jinqigufen.top

[U52] PHP：箭头函数
来源：http://jee.yuanzhike.top

$double = fn($x) => $x * 2;
来源：http://aei.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://jxe.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://qcg.zdqjudy.top

[U54] PHP：空安全调用
来源：http://wci.pycfn.com

$obj?->method()
来源：http://not.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://vct.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zox.hnqzz.top

[U56] PHP：命名参数
来源：http://jiw.hesvh.cn

f(a: 1, b: 2)
来源：http://dmw.jianghu66.top

[U57] PHP：字符串插值
来源：http://jwp.wangshuangyany.cn

"值: {$a}"
来源：http://chn.c1oappe.top

[U58] PHP：数组三件套
来源：http://dxk.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sve.yuxming.cn

[U59] PHP：自定义排序
来源：http://vaq.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgz.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://sgl.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fcf.jinqigfzy.top

[U61] PHP：正则
来源：http://okn.guowangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zro.jqgufenzy.top

[U62] PHP：日期对象
来源：http://qxt.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://src.hcnkem.com

[U63] PHP：文件读写
来源：http://ubc.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://scf.ivvv.top

[U64] PHP：目录遍历
来源：http://nlg.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://rnp.yanxiufei.cn

[U65] PHP：会话
来源：http://gsz.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yzb.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://zkt.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rfc.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://nhu.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhw.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://pdt.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gkf.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://doa.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jjw.ydzc1.top

[U70] PHP：PDO 事务
来源：http://osv.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://smf.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://feq.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://tvc.fehbvm.com

[U72] PHP：写错误日志
来源：http://keg.yj202588.top

error_log("失败: " . $e->getMessage());
来源：http://umf.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://loe.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://sua.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://ghx.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://nwc.bjfxy.top

[U75] PHP：依赖注入
来源：http://trv.hesvh.cn

composer require psr/container
来源：http://qlo.nwbrower.top

[U76] PHP：简单路由
来源：http://geg.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rna.fengsongda.top

[U77] PHP：模板渲染
来源：http://lwa.kuanghao11.cn

composer require twig/twig
来源：http://nqh.zycfv.cn

[U78] PHP：单元测试
来源：http://shx.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://uqj.svipenyu.cn

[U79] PHP：静态分析
来源：http://arp.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://jwp.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://lbn.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://agw.bbcook.cn

[U81] JS：初始化项目
来源：http://mwt.mhx1999.top

npm init -y;  npm i express
来源：http://zhk.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://baf.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ere.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://etq.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://jit.316326.xyz

[U84] JS：CommonJS 写法
来源：http://yyc.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fds.gaohongyu789.top

[U85] JS：可选链
来源：http://jml.pycfn.com

a?.b?.c
来源：http://xks.gotoacloud.top

[U86] JS：空值合并
来源：http://gxk.guowangkeji.top

a ?? b
来源：http://muj.daxiang520.top

[U87] JS：解构默认值
来源：http://nfx.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://vwd.tanke756.top

[U88] JS：对象展开合并
来源：http://vta.yvedp.cn

{ ...a, ...b }
来源：http://rmj.hysaishi.cn

[U89] JS：数组去重
来源：http://gzo.chenjidiqi.icu

[...new Set(arr)]
来源：http://nof.pycfn.com

[U90] JS：数字数组排序
来源：http://axv.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://bky.hesvh.cn

[U91] JS：对象键值遍历
来源：http://rte.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://swl.shzxlz.cn

[U92] JS：深拷贝
来源：http://lkj.jqgufenzy.top

structuredClone(obj)
来源：http://zch.52xcode.cn

[U93] JS：模板字符串
来源：http://rfk.nwbrower.top

`共 ${n} 条`
来源：http://qhn.cdnleiting.top

[U94] JS：箭头函数
来源：http://kcv.vehdjk.com

const double = x => x * 2;
来源：http://xje.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://cpp.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://myb.hcnkem.com

[U96] JS：async/await 与异常
来源：http://fse.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pcs.guannengcc.top

[U97] JS：并发请求
来源：http://kau.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lhu.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://ltq.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ugq.jlsjyb.cn

[U99] JS：事件监听
来源：http://qhf.redwolf501.top

el.addEventListener("click", e => {})
来源：http://wxb.pycfn.com

[U100] JS：DOM 查询
来源：http://cba.dianchejie.cn

document.querySelector(".item")
来源：http://xhd.jinyuanbaomall.cn

[U101] JS：classList 操作
来源：http://ukb.gzhubu.top

el.classList.toggle("active")
来源：http://jru.wangdashe.top

[U102] JS：本地存储
来源：http://xwf.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dpi.pengpengdd.cyou

[U103] JS：定时器
来源：http://zgr.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://chz.ppjwa.cn

[U104] JS：防抖
来源：http://pmk.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://grs.guowangkeji.top

[U105] JS：节流
来源：http://ghw.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gij.haohaochexian.top

[U106] JS：日期格式化
来源：http://hjv.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tlz.yonumen.top

[U107] JS：数字千分位
来源：http://uyx.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fxm.haohaochexian.top

[U108] JS：随机整数
来源：http://akh.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vgz.yuxming.cn

[U109] JS：数组分组
来源：http://xir.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://asx.hywenlv.cn

[U110] JS：数组分块
来源：http://gsg.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uya.ybcxt.top

[U111] JS：对象转 Map
来源：http://viz.andypj.xyz

new Map(Object.entries(obj))
来源：http://rai.daria6918.cn

[U112] JS：字符串补位
来源：http://zly.zhongyouzk.top

"7".padStart(3, "0")
来源：http://ums.zdqjudy.top

[U113] JS：正则替换全部
来源：http://blt.cdnleiting.top

s.replaceAll("a", "b")
来源：http://dqx.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://auk.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ipy.cqqwz.cn

[U115] JS：生成 UUID
来源：http://ios.jqgfzy.top

crypto.randomUUID()
来源：http://xgb.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://ztr.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://lui.nwbrower.top

[U117] JS：单元测试
来源：http://voo.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://dvg.fktsv.cn

[U118] JS：开发服务器
来源：http://jtz.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://lbv.xuetiantiany.cn

[U119] JS：生产构建
来源：http://rzv.cucudq.cn

npx vite build
来源：http://vpo.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://sbb.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://fvv.sxryk.cn

================================================================================
来源：http://gwi.guannengcc.top

统计汇总
来源：http://aag.shzxlz.cn

================================================================================
来源：http://orl.shangyingyoupin.top

按语言统计（条）：
来源：http://gxu.yj20258.top

Python ......... 252
来源：http://isz.guowangkeji.top

PHP ............ 252
来源：http://mwp.jqgufenzy.top

JavaScript ..... 252
来源：http://oro.c1oappe.top

TypeScript ..... 212
来源：http://qqz.redwolf501.top

Java ........... 212
来源：http://soa.nwbrower.top

Go ............. 212
来源：http://aoe.ehwqpu.com

Ruby ........... 212
来源：http://wut.ybcxt.top

C# ............. 212
来源：http://xzh.jqgufenzy.top

C .............. 30
来源：http://ydw.c1oappe.top

C++ ............ 30
来源：http://pbd.wangshuangyany.cn

SQL ............ 90
来源：http://njp.jinyuanbaomall.cn

Bash ........... 80
来源：http://nsk.shzxlz.cn

Kotlin ......... 15
来源：http://voj.yj202588.top

Swift .......... 15
来源：http://esr.sweek.top

Lua ............ 10
来源：http://yda.yj20258888.top

Perl ........... 10
来源：http://ibu.yj20258.top

Scala .......... 10
来源：http://tvi.xziqi.cn

------------------------------------
来源：http://yrn.svipenyu.cn

合计 ........... 2106 条
来源：http://uce.yuxming.cn

按章节统计：
来源：http://cdq.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fiz.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://odt.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://itz.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://avw.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rbl.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://elx.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://reo.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fhq.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sry.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ahm.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ota.hywenlv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hbk.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://azl.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://usp.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jge.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://exm.yfazqb.com

Q SQL 专题                              90
来源：http://fff.ydzc1.top

R Bash 专题                             80
来源：http://wpf.aibaodan.cn

S C / C++ 专题                          60
来源：http://yhu.aizwys.cn

T 其他语言补充                          60
来源：http://bjz.jiagoushi.top

U 高频实用片段                         120
来源：http://okb.yonumen.top

------------------------------------
来源：http://ixo.sxryk.cn

合计                                  2106 条
来源：http://fwy.yongpay.top

--------------------------------------------------------------------------------
来源：http://uys.hysaishi.cn

使用提醒
来源：http://hbg.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://skm.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eud.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vti.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tbv.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://yow.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://adk.yongpay.top

—— 文件结束 ——
来源：http://vpi.fengsongda.top

================================================================================
来源：http://mhv.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://igk.yangfankeji.com

Common Programming Examples Cheat Book
来源：http://hiw.jyoumei.cn

================================================================================
来源：http://qfk.svipenyu.cn

【收录内容】
来源：http://ntp.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lxf.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nkb.pycfn.com

SQL · Bash · C · C++
来源：http://isf.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rhx.c1oappe.top

【使用说明】
来源：http://ffm.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pzl.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://drf.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pxc.9152youxi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hdv.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://khu.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://soo.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oxi.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qeh.zhongyouzk.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uli.316326.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://css.gaohongyu789.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vvl.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bxq.yvedp.cn

【文件统计】
来源：http://ryp.kuanghao11.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rpz.redwolf501.top

--------------------------------------------------------------------------------
来源：http://rht.sjlbkw.cn

目  录
来源：http://gmz.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://psp.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wzw.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gbd.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lrh.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lfd.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://szf.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bgc.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qbp.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lhp.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uzi.jqgufenzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rro.hongshengwenyu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://amd.zhiwuduotai.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yoh.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oci.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jle.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wyl.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wud.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hjg.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nit.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mvi.tian-w.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://evx.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sno.yanxiufei.cn

================================================================================
来源：http://isi.yvedp.cn

A. 基础语法与类型
来源：http://hsk.yanxiufei.cn

================================================================================
来源：http://lzo.daxiang520.top

[A01] Hello World
来源：http://nbq.cucudq.cn

Py:   print("Hello, World!")
来源：http://ejq.zycfv.cn

PHP:  echo "Hello, World!";
来源：http://ldg.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://ant.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dua.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://bzq.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://nes.yongpay.top

Ruby: puts "Hello, World!"
来源：http://qdx.jqgufenzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ldj.316326.xyz

[A02] 变量声明与赋值
来源：http://uab.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mko.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://xwj.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://srt.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bxh.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://kuk.tarul.cn

Go:   name := "Alex"; age := 20
来源：http://gcz.shzxlz.cn

Ruby: name = "Alex"; age = 20
来源：http://smz.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://tfj.sufxvd.cn

[A03] 常量定义
来源：http://jld.zycfv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zxl.zdqjudy.top

PHP:  const PI = 3.14159;
来源：http://bhb.jianghu66.top

JS:   const PI = 3.14159;
来源：http://fqo.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://jqz.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://fqf.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://prv.xuanzx.com


<!-- 参考信息 -->