代发 wailian999

[U37] Py：读写 Excel
来源：http://rbm.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://znp.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://mzw.smart0.xyz

Path(__file__).resolve().parent
来源：http://hum.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://rkp.dianchejie.cn

sys.stdout.isatty()
来源：http://doi.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://wft.xylfe.cn

print("err", file=sys.stderr)
来源：http://wob.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://uyl.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rdg.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://dfs.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ghm.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://qin.guowangkeji.top

namespace App\Http;
来源：http://piz.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://evr.iojbl.cn

declare(strict_types=1);
来源：http://woa.fktsv.cn

[U45] PHP：类型声明与返回类型
来源：http://rmg.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vrx.zhijiandao.cn

[U46] PHP：可空类型
来源：http://wtn.cqqwz.cn

?string $name = null
来源：http://luc.sxryk.cn

[U47] PHP：联合类型
来源：http://sbt.feifeiyinyue.top

int|string $id
来源：http://wgj.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://mid.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://khq.cqqwz.cn

[U49] PHP：只读属性
来源：http://rpm.zhiwuduotai.top

public readonly string $name
来源：http://zta.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://vjl.vehdjk.com

public function __construct(private int $id) {}
来源：http://jpx.xuetiantiany.cn

[U51] PHP：数组解构
来源：http://jhu.svipenyu.cn

[$a, $b] = $arr;
来源：http://jor.gogol.net.cn

[U52] PHP：箭头函数
来源：http://qul.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://lrs.pycfn.com

[U53] PHP：空合并运算符
来源：http://igc.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://xcr.zdbjq.cn

[U54] PHP：空安全调用
来源：http://dch.cashguo.top

$obj?->method()
来源：http://vvl.0kj1m.cn

[U55] PHP：match 表达式
来源：http://mhu.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vrj.xylfe.cn

[U56] PHP：命名参数
来源：http://rgp.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://pvk.ctjpmb.com

[U57] PHP：字符串插值
来源：http://jms.hnxiangtu.top

"值: {$a}"
来源：http://gjd.chenlongwang.top

[U58] PHP：数组三件套
来源：http://ajx.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cey.fanxiaobao.xyz

[U59] PHP：自定义排序
来源：http://bxd.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wau.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://tgt.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://igu.xuetiantiany.cn

[U61] PHP：正则
来源：http://edn.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://juk.andypj.xyz

[U62] PHP：日期对象
来源：http://gmq.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sqv.kuanghao11.cn

[U63] PHP：文件读写
来源：http://mwq.fengsongda.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ypp.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://vlf.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://eoa.hysaishi.cn

[U65] PHP：会话
来源：http://fhs.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aln.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://seh.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://chb.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://nxa.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dhi.havefunace.top

[U68] PHP：PDO 连接
来源：http://mpu.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oav.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://xid.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ujn.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://wba.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twz.havefunace.top

[U71] PHP：抛出异常
来源：http://cmr.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://yhz.hysaishi.cn

[U72] PHP：写错误日志
来源：http://rjp.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://tnh.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://nku.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://cbj.xuanzx.com

[U74] PHP：读取环境变量
来源：http://dbn.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://dpj.hysaishi.cn

[U75] PHP：依赖注入
来源：http://avf.vqdsnc.cn

composer require psr/container
来源：http://oiq.c1oappe.top

[U76] PHP：简单路由
来源：http://lzz.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xan.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://efc.fengsongda.top

composer require twig/twig
来源：http://xfy.yvedp.cn

[U78] PHP：单元测试
来源：http://bou.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://myw.hysaishi.cn

[U79] PHP：静态分析
来源：http://zzo.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://tfx.daria6918.cn

[U80] PHP：代码规范修复
来源：http://kop.yueranfly.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mbk.yuxming.cn

[U81] JS：初始化项目
来源：http://hdi.zhongyouzk.top

npm init -y;  npm i express
来源：http://bpy.hesvh.cn

[U82] JS：package.json 脚本
来源：http://fma.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eiy.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://ohk.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://zch.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://lcf.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://fdt.yueranfly.top

[U85] JS：可选链
来源：http://zxp.mhx1999.top

a?.b?.c
来源：http://kwd.cucudq.cn

[U86] JS：空值合并
来源：http://zuk.feifeiyinyue.top

a ?? b
来源：http://lgr.daxiang520.top

[U87] JS：解构默认值
来源：http://zmq.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://dcv.redwolf501.top

[U88] JS：对象展开合并
来源：http://vxt.jinghuilouyu.cn

{ ...a, ...b }
来源：http://cdb.ydzc1.top

[U89] JS：数组去重
来源：http://qgu.zhiwuduotai.top

[...new Set(arr)]
来源：http://sff.jyoumei.cn

[U90] JS：数字数组排序
来源：http://zpg.xinyue.icu

[...arr].sort((a, b) => a - b)
来源：http://iwk.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://xym.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pnf.yj20258.top

[U92] JS：深拷贝
来源：http://tpu.aibaodan.cn

structuredClone(obj)
来源：http://wha.sysykeji.top

[U93] JS：模板字符串
来源：http://azg.316326.xyz

`共 ${n} 条`
来源：http://ijv.zhoulong.xyz

[U94] JS：箭头函数
来源：http://cww.sjlbkw.cn

const double = x => x * 2;
来源：http://bft.aizwys.cn

[U95] JS：Promise 包装
来源：http://snc.ivvv.top

new Promise((resolve, reject) => {})
来源：http://lvd.redwolf501.top

[U96] JS：async/await 与异常
来源：http://zet.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://stk.zhijiandao.cn

[U97] JS：并发请求
来源：http://xef.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://awi.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://ygp.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fwk.c1oappe.top

[U99] JS：事件监听
来源：http://phj.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://agz.daxiang520.top

[U100] JS：DOM 查询
来源：http://tau.redwolf501.top

document.querySelector(".item")
来源：http://bhl.cucudq.cn

[U101] JS：classList 操作
来源：http://rtc.shzxlz.cn

el.classList.toggle("active")
来源：http://wlr.redwolf501.top

[U102] JS：本地存储
来源：http://dvy.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lbp.dashuyun.cn

[U103] JS：定时器
来源：http://htg.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cjf.52xcode.cn

[U104] JS：防抖
来源：http://gqv.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bms.yj20258.top

[U105] JS：节流
来源：http://rgg.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kpd.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://yki.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ipg.sysykeji.top

[U107] JS：数字千分位
来源：http://rob.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rck.jinqigfzy.top

[U108] JS：随机整数
来源：http://sxv.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fft.yuanzhike.top

[U109] JS：数组分组
来源：http://gto.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://vsc.ehwqpu.com

[U110] JS：数组分块
来源：http://vxu.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hpl.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://iyu.cqqwz.cn

new Map(Object.entries(obj))
来源：http://iqc.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://zen.jqgufenzy.top

"7".padStart(3, "0")
来源：http://aom.yfazqb.com

[U113] JS：正则替换全部
来源：http://kxp.daria6918.cn

s.replaceAll("a", "b")
来源：http://oep.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://dwl.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://nxw.hcnkem.com

[U115] JS：生成 UUID
来源：http://nvq.xylfe.cn

crypto.randomUUID()
来源：http://xli.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://zif.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://xqm.meibo888.top

[U117] JS：单元测试
来源：http://eul.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://cep.bbcook.cn

[U118] JS：开发服务器
来源：http://qzs.xylfe.cn

npm i -D vite;  npx vite
来源：http://xlu.0kj1m.cn

[U119] JS：生产构建
来源：http://zil.yj20258888.top

npx vite build
来源：http://oxy.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://twp.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://tbe.zhaomingkeji.xyz

================================================================================
来源：http://wjl.zhixingplan.top

统计汇总
来源：http://tmg.sysykeji.top

================================================================================
来源：http://dst.9152youxi.cn

按语言统计（条）：
来源：http://phh.yj20258888.top

Python ......... 252
来源：http://zpa.cdnleiting.top

PHP ............ 252
来源：http://vtq.jinqigufen.top

JavaScript ..... 252
来源：http://lbr.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://jam.yvedp.cn

Java ........... 212
来源：http://abv.dashuyun.cn

Go ............. 212
来源：http://keh.sufxvd.cn

Ruby ........... 212
来源：http://lfl.zhaomingkeji.xyz

C# ............. 212
来源：http://xhs.xuetiantiany.cn

C .............. 30
来源：http://bkz.xylfe.cn

C++ ............ 30
来源：http://tls.cqqwz.cn

SQL ............ 90
来源：http://lyf.ydjk.org.cn

Bash ........... 80
来源：http://nts.chenlongwang.top

Kotlin ......... 15
来源：http://thv.chenjidiqi.icu

Swift .......... 15
来源：http://fyu.cqqwz.cn

Lua ............ 10
来源：http://xue.yvedp.cn

Perl ........... 10
来源：http://fdy.wangdashe.top

Scala .......... 10
来源：http://rzd.ywan-chungtsiang.top

------------------------------------
来源：http://gjk.zdbjq.cn

合计 ........... 2106 条
来源：http://kma.tarul.cn

按章节统计：
来源：http://uto.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zmz.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lub.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ret.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://seb.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yae.yuxming.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mxy.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mza.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgs.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vac.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ugz.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gny.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://atm.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jlk.zdqjudy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cxc.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bsj.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://and.mhx1999.top

Q SQL 专题                              90
来源：http://guv.vehdjk.com

R Bash 专题                             80
来源：http://wmo.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://ixl.yueranfly.top

T 其他语言补充                          60
来源：http://ehs.hysaishi.cn

U 高频实用片段                         120
来源：http://cle.yonumen.top

------------------------------------
来源：http://iuw.jianghu66.top

合计                                  2106 条
来源：http://grg.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://wqq.chenjidiqi.icu

使用提醒
来源：http://utn.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://ofm.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kii.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cqk.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qda.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uoo.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://efj.nanxuanxn.top

—— 文件结束 ——
来源：http://mtv.cheryme.top

================================================================================
来源：http://enj.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://blq.wangdashe.top

Common Programming Examples Cheat Book
来源：http://tbh.ivvv.top

================================================================================
来源：http://tle.ywan-chungtsiang.top

【收录内容】
来源：http://uzy.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bcj.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ces.aizwys.cn

SQL · Bash · C · C++
来源：http://nma.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://maa.chenjidiqi.icu

【使用说明】
来源：http://ext.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://syx.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://smv.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vuh.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://esb.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://rag.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xbq.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://glf.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ieo.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uic.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pei.sufxvd.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hqq.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mwf.zhijiandao.cn

【文件统计】
来源：http://hwy.gogol.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jhr.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://tan.cucudq.cn

目  录
来源：http://rcf.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://kkj.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://usy.zhongyouzk.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sem.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nnv.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rac.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://trn.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wfo.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ahg.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xjy.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jfr.0kj1m.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ahz.wangshuangyany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wqb.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uqg.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rrv.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eui.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ier.shangyingyoupin.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vve.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lnw.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://wst.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ksx.tanke756.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zvp.ydzc1.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fwe.hesvh.cn

================================================================================
来源：http://hhq.jqgfzy.top

A. 基础语法与类型
来源：http://grq.c1oappe.top

================================================================================
来源：http://dgf.ehwqpu.com

[A01] Hello World
来源：http://xkk.xylfe.cn

Py:   print("Hello, World!")
来源：http://iub.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://vrr.yonumen.top

JS:   console.log("Hello, World!");
来源：http://ecg.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ktt.nanxinkj.top

Java: System.out.println("Hello, World!");
来源：http://rbo.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://evo.feifeiyinyue.top

Ruby: puts "Hello, World!"
来源：http://ahf.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://iqo.sweek.top

[A02] 变量声明与赋值
来源：http://qcc.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dwn.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ucc.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qha.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dnk.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://dyg.nwbrower.top

Go:   name := "Alex"; age := 20
来源：http://hpu.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://tcn.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://cgu.zhoulong.xyz

[A03] 常量定义
来源：http://hbj.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://upv.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://yzo.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://cll.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://nor.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://gvw.yueranfly.top

Go:   const PI = 3.14159
来源：http://rdn.yj20258888.top


<!-- 参考信息 -->