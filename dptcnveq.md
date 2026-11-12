代发 wailian999

[U37] Py：读写 Excel
来源：http://dcb.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://sbd.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://sgb.ydzc1.top

Path(__file__).resolve().parent
来源：http://haz.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://aca.uphjek.com

sys.stdout.isatty()
来源：http://gzb.yongpay.top

[U40] Py：打印到标准错误
来源：http://cbp.nwbrower.top

print("err", file=sys.stderr)
来源：http://nan.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://eaj.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wxl.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://uzq.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mha.iojbl.cn

[U43] PHP：声明命名空间
来源：http://ifh.zhoulong.xyz

namespace App\Http;
来源：http://jfk.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://iog.chenlongwang.top

declare(strict_types=1);
来源：http://cmt.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://pzp.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fgu.0kj1m.cn

[U46] PHP：可空类型
来源：http://rsr.yuanzhike.top

?string $name = null
来源：http://xtl.hfpthk.cn

[U47] PHP：联合类型
来源：http://uwo.zhaomingkeji.xyz

int|string $id
来源：http://eii.svipenyu.cn

[U48] PHP：纯枚举
来源：http://ojv.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tre.sysykeji.top

[U49] PHP：只读属性
来源：http://ust.xuanzx.com

public readonly string $name
来源：http://dtr.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://jaj.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://jsz.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://ezq.hysaishi.cn

[$a, $b] = $arr;
来源：http://hke.sweek.top

[U52] PHP：箭头函数
来源：http://rgw.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://fjf.daxiang520.top

[U53] PHP：空合并运算符
来源：http://hzv.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://alm.yuanzhike.top

[U54] PHP：空安全调用
来源：http://aui.hfpthk.cn

$obj?->method()
来源：http://bci.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://vfq.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ufh.fengsongda.top

[U56] PHP：命名参数
来源：http://jjy.yj20258.top

f(a: 1, b: 2)
来源：http://gyc.ydzc1.top

[U57] PHP：字符串插值
来源：http://bzv.yanxiufei.cn

"值: {$a}"
来源：http://rhl.zdqjudy.top

[U58] PHP：数组三件套
来源：http://dua.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eij.snrcjt.cn

[U59] PHP：自定义排序
来源：http://dui.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://evi.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://mpr.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hcv.hongshengwenyu.top

[U61] PHP：正则
来源：http://wis.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ben.52xcode.cn

[U62] PHP：日期对象
来源：http://iah.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bxn.jyoumei.cn

[U63] PHP：文件读写
来源：http://owq.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fbk.mhx1999.top

[U64] PHP：目录遍历
来源：http://qjh.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://xnx.ybcxt.top

[U65] PHP：会话
来源：http://xdw.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fae.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://yxi.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fyx.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://nnj.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dbv.shuidangran.top

[U68] PHP：PDO 连接
来源：http://adr.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ceg.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://qtk.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cmh.tarul.cn

[U70] PHP：PDO 事务
来源：http://xzp.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fmm.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://rem.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://chd.yongpay.top

[U72] PHP：写错误日志
来源：http://avy.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://mpf.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://sld.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://odr.316326.xyz

[U74] PHP：读取环境变量
来源：http://zol.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://ctg.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://sxy.dashuyun.cn

composer require psr/container
来源：http://khe.smart0.xyz

[U76] PHP：简单路由
来源：http://swd.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vyd.daxiang520.top

[U77] PHP：模板渲染
来源：http://tkd.ybcxt.top

composer require twig/twig
来源：http://pnu.wangdashe.top

[U78] PHP：单元测试
来源：http://ksf.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://dff.fzhhl.top

[U79] PHP：静态分析
来源：http://cfq.bbcook.cn

composer require --dev phpstan/phpstan
来源：http://aal.gaohongyu789.top

[U80] PHP：代码规范修复
来源：http://hqg.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://upv.xziqi.cn

[U81] JS：初始化项目
来源：http://mvg.jyoumei.cn

npm init -y;  npm i express
来源：http://zqn.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://ubu.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wjc.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://mrw.zhongyouzk.top

export const a = 1;  import { a } from "./m.js";
来源：http://xxn.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://rod.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://dur.fktsv.cn

[U85] JS：可选链
来源：http://nth.yj202588.top

a?.b?.c
来源：http://ali.daxiang520.top

[U86] JS：空值合并
来源：http://krs.tarul.cn

a ?? b
来源：http://fvb.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://lkh.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://flg.andypj.xyz

[U88] JS：对象展开合并
来源：http://pvz.yj202588.top

{ ...a, ...b }
来源：http://nya.quarkkingdee.top

[U89] JS：数组去重
来源：http://ryv.zycfv.cn

[...new Set(arr)]
来源：http://psp.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://bpk.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://mjd.sweek.top

[U91] JS：对象键值遍历
来源：http://ifg.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xov.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://efp.zhiwuduotai.top

structuredClone(obj)
来源：http://uae.yfazqb.com

[U93] JS：模板字符串
来源：http://poo.cucudq.cn

`共 ${n} 条`
来源：http://tko.jqgufenzy.top

[U94] JS：箭头函数
来源：http://lpl.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://uvr.bbcook.cn

[U95] JS：Promise 包装
来源：http://qkj.cheryme.top

new Promise((resolve, reject) => {})
来源：http://tgb.iojbl.cn

[U96] JS：async/await 与异常
来源：http://kpp.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ppr.ydzc1.top

[U97] JS：并发请求
来源：http://xcz.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zzo.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://wbm.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yuu.zhongyouzk.top

[U99] JS：事件监听
来源：http://zjm.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://pzs.sxryk.cn

[U100] JS：DOM 查询
来源：http://oad.cheryme.top

document.querySelector(".item")
来源：http://ldr.zdqjudy.top

[U101] JS：classList 操作
来源：http://xps.sufxvd.cn

el.classList.toggle("active")
来源：http://nbq.hammf.cn

[U102] JS：本地存储
来源：http://uzv.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zmg.smart0.xyz

[U103] JS：定时器
来源：http://yng.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://smh.yvedp.cn

[U104] JS：防抖
来源：http://njl.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uzg.yvedp.cn

[U105] JS：节流
来源：http://ykm.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xes.dianchejie.cn

[U106] JS：日期格式化
来源：http://boq.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yje.jiagoushi.top

[U107] JS：数字千分位
来源：http://csx.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vyo.vehdjk.com

[U108] JS：随机整数
来源：http://cai.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xga.sweek.top

[U109] JS：数组分组
来源：http://tvx.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://msb.hnxiangtu.top

[U110] JS：数组分块
来源：http://jrh.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mss.gogol.net.cn

[U111] JS：对象转 Map
来源：http://dmk.smart0.xyz

new Map(Object.entries(obj))
来源：http://ysd.chenlongwang.top

[U112] JS：字符串补位
来源：http://dpi.jlsjyb.cn

"7".padStart(3, "0")
来源：http://fdb.cqqwz.cn

[U113] JS：正则替换全部
来源：http://pry.hywenlv.cn

s.replaceAll("a", "b")
来源：http://ljb.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://jii.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://loj.aibaodan.cn

[U115] JS：生成 UUID
来源：http://hpg.jianghu66.top

crypto.randomUUID()
来源：http://mcl.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://aam.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://mlr.zhengqikj.top

[U117] JS：单元测试
来源：http://pob.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://wso.ctjpmb.com

[U118] JS：开发服务器
来源：http://jnb.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://ndt.sufxvd.cn

[U119] JS：生产构建
来源：http://tvi.ehwqpu.com

npx vite build
来源：http://zbd.nanxinkj.top

[U120] JS：读取环境变量（Vite）
来源：http://kyv.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://qjs.cdnleiting.top

================================================================================
来源：http://amk.ctjpmb.com

统计汇总
来源：http://siu.hfpthk.cn

================================================================================
来源：http://tls.wangdashe.top

按语言统计（条）：
来源：http://zvz.birdmap.top

Python ......... 252
来源：http://odw.yonumen.top

PHP ............ 252
来源：http://yiq.fzhhl.top

JavaScript ..... 252
来源：http://tuk.sjlbkw.cn

TypeScript ..... 212
来源：http://pqg.pengpengdd.cyou

Java ........... 212
来源：http://fcm.shzxlz.cn

Go ............. 212
来源：http://nzs.shuidangran.top

Ruby ........... 212
来源：http://qgq.dianchejie.cn

C# ............. 212
来源：http://mup.shuidangran.top

C .............. 30
来源：http://flg.hammf.cn

C++ ............ 30
来源：http://fhc.yuanzhike.top

SQL ............ 90
来源：http://ffr.haohaochexian.top

Bash ........... 80
来源：http://weh.meibo888.top

Kotlin ......... 15
来源：http://nxg.feifeiyinyue.top

Swift .......... 15
来源：http://twk.yongpay.top

Lua ............ 10
来源：http://xou.sufxvd.cn

Perl ........... 10
来源：http://lqd.yvedp.cn

Scala .......... 10
来源：http://cpx.cdnleiting.top

------------------------------------
来源：http://bmy.redwolf501.top

合计 ........... 2106 条
来源：http://jnw.sufxvd.cn

按章节统计：
来源：http://uqk.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kbi.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oeo.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jei.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://asl.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uqm.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nav.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gyp.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zjy.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lkz.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kow.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fvs.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kdn.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uvm.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nju.ctjpmb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xdd.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ear.zdbjq.cn

Q SQL 专题                              90
来源：http://uyg.gotoacloud.top

R Bash 专题                             80
来源：http://vuf.nanxinkj.top

S C / C++ 专题                          60
来源：http://fex.xuanzx.com

T 其他语言补充                          60
来源：http://zed.nanxinkj.top

U 高频实用片段                         120
来源：http://qea.zhaomingkeji.xyz

------------------------------------
来源：http://kwy.fehbvm.com

合计                                  2106 条
来源：http://ely.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://gow.jinqigufen.top

使用提醒
来源：http://wfw.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://ued.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://etp.52xcode.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ltl.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xpb.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rnp.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qxh.nwbrower.top

—— 文件结束 ——
来源：http://fwz.jiagoushi.top

================================================================================
来源：http://mov.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://xju.shuidangran.top

Common Programming Examples Cheat Book
来源：http://zya.yj202588.top

================================================================================
来源：http://hmm.sufxvd.cn

【收录内容】
来源：http://lgq.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vwc.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wwh.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://wvo.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nmx.xinyue.icu

【使用说明】
来源：http://ylm.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zfc.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hjk.hfpthk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yhy.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wgs.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ibs.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tlw.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jjp.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mwk.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cgp.jinqigufen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jin.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kxs.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fjx.yj20258888.top

【文件统计】
来源：http://lge.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gom.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://wck.guowangkeji.top

目  录
来源：http://uow.sxryk.cn

--------------------------------------------------------------------------------
来源：http://znd.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cxm.tarul.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vgo.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mrk.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zrp.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xxr.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gxq.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mes.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dfq.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qth.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cjf.yanxiufei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mbr.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rdu.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yqc.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zuu.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kni.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rmj.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ufx.bjfxy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wrd.meibo888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ysa.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zkf.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eea.yongpay.top

================================================================================
来源：http://xzy.fehbvm.com

A. 基础语法与类型
来源：http://flk.sysykeji.top

================================================================================
来源：http://vgx.hywenlv.cn

[A01] Hello World
来源：http://sud.52xcode.cn

Py:   print("Hello, World!")
来源：http://rky.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://shd.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://vtc.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sqo.jiagoushi.top

Java: System.out.println("Hello, World!");
来源：http://iky.zhaomingkeji.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ell.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://gxd.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wut.cheryme.top

[A02] 变量声明与赋值
来源：http://tet.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fqy.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zdx.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://zor.guannengcc.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bof.cqqwz.cn

Java: String name = "Alex"; int age = 20;
来源：http://dhx.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://toh.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://dng.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://mna.birdmap.top

[A03] 常量定义
来源：http://thi.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sij.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://qak.wangdashe.top

JS:   const PI = 3.14159;
来源：http://mbk.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://lzh.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://wly.xuanzx.com

Go:   const PI = 3.14159
来源：http://xyl.gaohongyu789.top


<!-- 参考信息 -->