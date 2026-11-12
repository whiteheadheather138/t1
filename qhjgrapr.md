代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://gho.tarul.cn

sys.stdout.isatty()
来源：http://ece.iojbl.cn

[U40] Py：打印到标准错误
来源：http://edn.yvedp.cn

print("err", file=sys.stderr)
来源：http://uks.ydzc1.top

[U41] PHP：初始化 Composer 项目
来源：http://rqc.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ven.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://nll.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uni.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://mzt.meibo888.top

namespace App\Http;
来源：http://kbd.tanke756.top

[U44] PHP：开启严格类型
来源：http://vwm.aizwys.cn

declare(strict_types=1);
来源：http://puu.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://lla.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jty.pycfn.com

[U46] PHP：可空类型
来源：http://vry.xinyue.icu

?string $name = null
来源：http://dtg.guannengcc.top

[U47] PHP：联合类型
来源：http://oli.shanyushiyangkeji.top

int|string $id
来源：http://vej.cdnleiting.top

[U48] PHP：纯枚举
来源：http://mxw.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hug.zhengqikj.top

[U49] PHP：只读属性
来源：http://qhi.yueranfly.top

public readonly string $name
来源：http://wzn.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://yzr.cucudq.cn

public function __construct(private int $id) {}
来源：http://qlm.yangfankeji.com

[U51] PHP：数组解构
来源：http://zyp.yvedp.cn

[$a, $b] = $arr;
来源：http://xsc.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://ema.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://vte.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://kon.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://dev.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://vti.zhengqikj.top

$obj?->method()
来源：http://mso.wangdashe.top

[U55] PHP：match 表达式
来源：http://xip.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://feh.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://wyg.hfpthk.cn

f(a: 1, b: 2)
来源：http://qhr.aibaodan.cn

[U57] PHP：字符串插值
来源：http://waf.nwbrower.top

"值: {$a}"
来源：http://xey.bbcook.cn

[U58] PHP：数组三件套
来源：http://hen.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qse.chenzaomai.com

[U59] PHP：自定义排序
来源：http://hom.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ysa.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://fed.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dhx.ydzc1.top

[U61] PHP：正则
来源：http://gpc.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://evp.dianchejie.cn

[U62] PHP：日期对象
来源：http://ynf.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uwq.sweek.top

[U63] PHP：文件读写
来源：http://nrk.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nwu.zhixingplan.top

[U64] PHP：目录遍历
来源：http://qml.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://ies.fzhhl.top

[U65] PHP：会话
来源：http://vlf.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://yql.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://dix.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tbc.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://eph.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jfw.pycfn.com

[U68] PHP：PDO 连接
来源：http://xrt.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hir.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://llw.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ydj.cashguo.top

[U70] PHP：PDO 事务
来源：http://rip.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twj.9152youxi.cn

[U71] PHP：抛出异常
来源：http://bas.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://muq.cucudq.cn

[U72] PHP：写错误日志
来源：http://mqh.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://ozj.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://qxr.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://msm.ydzc1.top

[U74] PHP：读取环境变量
来源：http://fkc.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://iqk.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://mvf.cucudq.cn

composer require psr/container
来源：http://fmb.birdmap.top

[U76] PHP：简单路由
来源：http://lbg.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iju.pycfn.com

[U77] PHP：模板渲染
来源：http://mng.0kj1m.cn

composer require twig/twig
来源：http://uxw.cqqwz.cn

[U78] PHP：单元测试
来源：http://eni.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://zvs.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://vko.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://lxr.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://sru.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fcn.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://thd.yueranfly.top

npm init -y;  npm i express
来源：http://ssn.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://cio.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xyz.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://igf.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://wwa.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://wbo.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://upi.yongpay.top

[U85] JS：可选链
来源：http://zyb.vqdsnc.cn

a?.b?.c
来源：http://qiw.hcnkem.com

[U86] JS：空值合并
来源：http://oeq.jinghuilouyu.cn

a ?? b
来源：http://pvm.bjfxy.top

[U87] JS：解构默认值
来源：http://ohv.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://xco.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://rgc.fanxiaobao.xyz

{ ...a, ...b }
来源：http://kxu.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://pmn.mhx1999.top

[...new Set(arr)]
来源：http://qvo.sxryk.cn

[U90] JS：数字数组排序
来源：http://vmk.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://kcz.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://wsy.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qrn.52xcode.cn

[U92] JS：深拷贝
来源：http://fzk.nanxinkj.top

structuredClone(obj)
来源：http://uio.ehwqpu.com

[U93] JS：模板字符串
来源：http://lze.feifeiyinyue.top

`共 ${n} 条`
来源：http://zdv.daxiang520.top

[U94] JS：箭头函数
来源：http://ncn.xziqi.cn

const double = x => x * 2;
来源：http://kyg.jinghuilouyu.cn

[U95] JS：Promise 包装
来源：http://ege.meibo888.top

new Promise((resolve, reject) => {})
来源：http://qtj.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://ffg.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vfl.cucudq.cn

[U97] JS：并发请求
来源：http://ssg.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jmu.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://yca.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eqc.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://gtr.daria6918.cn

el.addEventListener("click", e => {})
来源：http://rpj.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://gcv.fktsv.cn

document.querySelector(".item")
来源：http://hlb.wangdashe.top

[U101] JS：classList 操作
来源：http://rqj.yj202588.top

el.classList.toggle("active")
来源：http://vla.xinyue.icu

[U102] JS：本地存储
来源：http://bwf.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cxr.pycfn.com

[U103] JS：定时器
来源：http://iyn.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ayw.ydzc1.top

[U104] JS：防抖
来源：http://nak.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qoa.redwolf501.top

[U105] JS：节流
来源：http://xlc.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xiu.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://hbb.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zxb.uphjek.com

[U107] JS：数字千分位
来源：http://xge.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jug.jiagoushi.top

[U108] JS：随机整数
来源：http://nau.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ttu.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://cnc.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://lee.yuanzhike.top

[U110] JS：数组分块
来源：http://rbr.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tpy.zhengqikj.top

[U111] JS：对象转 Map
来源：http://nue.shuidangran.top

new Map(Object.entries(obj))
来源：http://tcq.yvedp.cn

[U112] JS：字符串补位
来源：http://jka.tian-w.cn

"7".padStart(3, "0")
来源：http://zwg.yfazqb.com

[U113] JS：正则替换全部
来源：http://yve.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://hzm.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://iqz.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pmh.yj202588.top

[U115] JS：生成 UUID
来源：http://ioi.zhiwuduotai.top

crypto.randomUUID()
来源：http://wka.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://tqy.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://beq.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://kit.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://ats.zhixingplan.top

[U118] JS：开发服务器
来源：http://wzc.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://vkw.fehbvm.com

[U119] JS：生产构建
来源：http://vmo.yuxming.cn

npx vite build
来源：http://lww.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://hje.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://gpu.yfazqb.com

================================================================================
来源：http://kww.jlsjyb.cn

统计汇总
来源：http://xge.sysykeji.top

================================================================================
来源：http://hsv.redwolf501.top

按语言统计（条）：
来源：http://zxm.nwbrower.top

Python ......... 252
来源：http://sfp.svipenyu.cn

PHP ............ 252
来源：http://hqi.shanyushiyangtech.top

JavaScript ..... 252
来源：http://tzo.haohaochexian.top

TypeScript ..... 212
来源：http://xvk.birdmap.top

Java ........... 212
来源：http://bmi.shanyushiyangkeji.top

Go ............. 212
来源：http://bol.yuxming.cn

Ruby ........... 212
来源：http://xjm.fktsv.cn

C# ............. 212
来源：http://gtb.zhoulong.xyz

C .............. 30
来源：http://nhu.nanxinkj.top

C++ ............ 30
来源：http://fls.dianchejie.cn

SQL ............ 90
来源：http://miz.mhx1999.top

Bash ........... 80
来源：http://lhv.cucudq.cn

Kotlin ......... 15
来源：http://rox.hammf.cn

Swift .......... 15
来源：http://zyd.ehwqpu.com

Lua ............ 10
来源：http://xri.fanxiaobao.xyz

Perl ........... 10
来源：http://pme.vehdjk.com

Scala .......... 10
来源：http://unx.haohaochexian.top

------------------------------------
来源：http://fsx.yvedp.cn

合计 ........... 2106 条
来源：http://rps.zhijiandao.cn

按章节统计：
来源：http://sbk.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lrb.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xvo.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bpu.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rst.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yxq.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mmg.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bel.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blv.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://izx.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bue.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wuf.vqdsnc.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://icp.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lbs.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gou.pycfn.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kui.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bqe.hnqzz.top

Q SQL 专题                              90
来源：http://uhe.dashuyun.cn

R Bash 专题                             80
来源：http://nmj.ppjwa.cn

S C / C++ 专题                          60
来源：http://daw.hongshengwenyu.top

T 其他语言补充                          60
来源：http://hzr.jqgfzy.top

U 高频实用片段                         120
来源：http://czj.gaohongyu789.top

------------------------------------
来源：http://ytc.yuxming.cn

合计                                  2106 条
来源：http://beo.hcnkem.com

--------------------------------------------------------------------------------
来源：http://qwa.tian-w.cn

使用提醒
来源：http://lqv.yonumen.top

--------------------------------------------------------------------------------
来源：http://saz.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jdj.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://olv.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vnh.tianlin.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://kya.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tqb.cucudq.cn

—— 文件结束 ——
来源：http://qai.aibaodan.cn

================================================================================
来源：http://lyx.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://dpr.cheryme.top

Common Programming Examples Cheat Book
来源：http://oyj.zhijiandao.cn

================================================================================
来源：http://jia.yanxiufei.cn

【收录内容】
来源：http://nso.hfpthk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cvm.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sod.ybcxt.top

SQL · Bash · C · C++
来源：http://uyu.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wbc.sxryk.cn

【使用说明】
来源：http://tzp.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pkx.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kzg.xingfuxueyuan.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ppw.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ujz.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zzr.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oui.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qbb.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ynr.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zjm.daria6918.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fbr.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kvk.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tyu.jqgfzy.top

【文件统计】
来源：http://gll.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pgv.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://xml.shangyingyoupin.top

目  录
来源：http://uig.bbcook.cn

--------------------------------------------------------------------------------
来源：http://icb.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ryi.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gdd.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kym.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://muw.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tpb.ywan-chungtsiang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nrx.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aao.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wbd.jiagoushi.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jrl.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qjh.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nrn.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://glo.redwolf501.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tcz.daxiang520.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://izu.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xaj.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bfj.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ern.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ytb.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fib.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bgo.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wqf.ydjk.org.cn

================================================================================
来源：http://ekq.zhengqikj.top

A. 基础语法与类型
来源：http://ijf.snrcjt.cn

================================================================================
来源：http://grf.xinyue.icu

[A01] Hello World
来源：http://lkm.nwbrower.top

Py:   print("Hello, World!")
来源：http://cls.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://jpy.ivvv.top

JS:   console.log("Hello, World!");
来源：http://pub.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ovl.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://vng.andypj.xyz

Go:   fmt.Println("Hello, World!")
来源：http://chi.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://yxy.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jkc.52xcode.cn

[A02] 变量声明与赋值
来源：http://rto.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ogj.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://icr.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://uqj.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aml.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://ntc.tian-w.cn

Go:   name := "Alex"; age := 20
来源：http://lil.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://jmh.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://awl.shanyushiyangtech.top

[A03] 常量定义
来源：http://yog.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qqs.hnxiangtu.top

PHP:  const PI = 3.14159;
来源：http://pcx.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://nww.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://api.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://eio.fehbvm.com

Go:   const PI = 3.14159
来源：http://psb.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://plo.tanke756.top

C#:   const double PI = 3.14159;
来源：http://rdx.nwbrower.top

[A04] 判断变量类型
来源：http://vxh.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dtu.ydzc1.top


<!-- 参考信息 -->