代发 wailian999

[U37] Py：读写 Excel
来源：http://anr.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://xcr.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://dlv.yongpay.top

Path(__file__).resolve().parent
来源：http://vee.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://tdv.sxryk.cn

sys.stdout.isatty()
来源：http://sdp.aizwys.cn

[U40] Py：打印到标准错误
来源：http://mdf.fengsongda.top

print("err", file=sys.stderr)
来源：http://uyy.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://fpu.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://dfo.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://dwt.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jwm.yongpay.top

[U43] PHP：声明命名空间
来源：http://puq.hnxiangtu.top

namespace App\Http;
来源：http://gyi.wangdashe.top

[U44] PHP：开启严格类型
来源：http://jnn.aizwys.cn

declare(strict_types=1);
来源：http://bed.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://hne.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fbu.cqqwz.cn

[U46] PHP：可空类型
来源：http://ksi.jinyuanbaomall.cn

?string $name = null
来源：http://fox.yvedp.cn

[U47] PHP：联合类型
来源：http://ava.epnwcf.com

int|string $id
来源：http://jfk.havefunace.top

[U48] PHP：纯枚举
来源：http://wsy.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bpz.ctjpmb.com

[U49] PHP：只读属性
来源：http://rzq.aizwys.cn

public readonly string $name
来源：http://xrw.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://aoz.yfazqb.com

public function __construct(private int $id) {}
来源：http://oqi.zhiwuduotai.top

[U51] PHP：数组解构
来源：http://ldj.hammf.cn

[$a, $b] = $arr;
来源：http://fpv.52xcode.cn

[U52] PHP：箭头函数
来源：http://kia.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://nun.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://cgm.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://vgv.yanxiufei.cn

[U54] PHP：空安全调用
来源：http://lip.9152youxi.cn

$obj?->method()
来源：http://aci.mhx1999.top

[U55] PHP：match 表达式
来源：http://rdf.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ywc.iojbl.cn

[U56] PHP：命名参数
来源：http://cbf.yanxiufei.cn

f(a: 1, b: 2)
来源：http://nuc.ppjwa.cn

[U57] PHP：字符串插值
来源：http://kle.yongpay.top

"值: {$a}"
来源：http://rnx.cashguo.top

[U58] PHP：数组三件套
来源：http://syn.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lkq.bjfxy.top

[U59] PHP：自定义排序
来源：http://hfh.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lpu.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://cuh.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mvo.tarul.cn

[U61] PHP：正则
来源：http://xew.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://acq.haohaochexian.top

[U62] PHP：日期对象
来源：http://cwt.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hrs.hfpthk.cn

[U63] PHP：文件读写
来源：http://njg.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bbw.kuanghao11.cn

[U64] PHP：目录遍历
来源：http://xlb.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://btn.birdmap.top

[U65] PHP：会话
来源：http://xhk.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xvp.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://vpu.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rwh.zycfv.cn

[U67] PHP：处理文件上传
来源：http://luj.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uwk.birdmap.top

[U68] PHP：PDO 连接
来源：http://pfp.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ivr.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://ejz.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yke.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://eeq.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qwp.sxryk.cn

[U71] PHP：抛出异常
来源：http://gvn.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://qqh.cashguo.top

[U72] PHP：写错误日志
来源：http://okx.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://ywm.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://cxb.tanke756.top

parse_ini_file("config.ini", true)
来源：http://zbm.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://cep.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://wmz.hnqzz.top

[U75] PHP：依赖注入
来源：http://vio.nwbrower.top

composer require psr/container
来源：http://gtr.fzhhl.top

[U76] PHP：简单路由
来源：http://zbn.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mje.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://rtn.shzxlz.cn

composer require twig/twig
来源：http://yqw.cashguo.top

[U78] PHP：单元测试
来源：http://dwx.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://hvt.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://dqc.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://tjw.xinyue.icu

[U80] PHP：代码规范修复
来源：http://wxf.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bco.gzhubu.top

[U81] JS：初始化项目
来源：http://suh.uphjek.com

npm init -y;  npm i express
来源：http://fkg.yvedp.cn

[U82] JS：package.json 脚本
来源：http://jqx.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rul.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://nxg.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lll.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://dda.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ajq.9152youxi.cn

[U85] JS：可选链
来源：http://phx.gotoacloud.top

a?.b?.c
来源：http://wez.dashuyun.cn

[U86] JS：空值合并
来源：http://yiq.ybcxt.top

a ?? b
来源：http://kpv.birdmap.top

[U87] JS：解构默认值
来源：http://cju.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://adb.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://bvc.mhx1999.top

{ ...a, ...b }
来源：http://ttt.ydzc1.top

[U89] JS：数组去重
来源：http://xpq.gogol.net.cn

[...new Set(arr)]
来源：http://gqa.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://bdy.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://vhe.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://xqd.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nfv.guannengcc.top

[U92] JS：深拷贝
来源：http://ndg.zhengqikj.top

structuredClone(obj)
来源：http://qjm.0kj1m.cn

[U93] JS：模板字符串
来源：http://hxv.kuanghao11.cn

`共 ${n} 条`
来源：http://cxa.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://ive.hammf.cn

const double = x => x * 2;
来源：http://srn.dianchejie.cn

[U95] JS：Promise 包装
来源：http://bbm.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://qua.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://tom.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rpi.tarul.cn

[U97] JS：并发请求
来源：http://mbi.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://szu.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://lqj.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nxf.cdnleiting.top

[U99] JS：事件监听
来源：http://xip.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://dtz.redwolf501.top

[U100] JS：DOM 查询
来源：http://nkw.xinyue.icu

document.querySelector(".item")
来源：http://cgf.hysaishi.cn

[U101] JS：classList 操作
来源：http://rjz.ppjwa.cn

el.classList.toggle("active")
来源：http://ctw.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://kxi.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://isx.jinqigufen.top

[U103] JS：定时器
来源：http://ofm.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vzj.wangshuangyany.cn

[U104] JS：防抖
来源：http://jjv.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywu.zhaomingkeji.xyz

[U105] JS：节流
来源：http://jgq.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ymu.zhengqikj.top

[U106] JS：日期格式化
来源：http://wvv.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pjd.fktsv.cn

[U107] JS：数字千分位
来源：http://whv.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mov.birdmap.top

[U108] JS：随机整数
来源：http://pdt.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ndp.tarul.cn

[U109] JS：数组分组
来源：http://guw.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://gto.daria6918.cn

[U110] JS：数组分块
来源：http://sml.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ens.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://qps.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://miy.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://iyo.meibo888.top

"7".padStart(3, "0")
来源：http://xvc.cdnleiting.top

[U113] JS：正则替换全部
来源：http://kfo.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://pgn.hysaishi.cn

[U114] JS：JSON 深比较
来源：http://ndq.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://omt.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://wbc.shanyushiyangtech.top

crypto.randomUUID()
来源：http://dss.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://kpb.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://mhz.wangshuangyany.cn

[U117] JS：单元测试
来源：http://ely.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://reg.ydzc1.top

[U118] JS：开发服务器
来源：http://jkn.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://oiz.mhx1999.top

[U119] JS：生产构建
来源：http://dtl.xziqi.cn

npx vite build
来源：http://cwg.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://fdi.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://fbx.sxryk.cn

================================================================================
来源：http://ces.daxiang520.top

统计汇总
来源：http://xkk.jinyuanbaomall.cn

================================================================================
来源：http://adp.ywan-chungtsiang.top

按语言统计（条）：
来源：http://skw.snrcjt.cn

Python ......... 252
来源：http://obm.yonumen.top

PHP ............ 252
来源：http://ron.yj20258.top

JavaScript ..... 252
来源：http://oav.uphjek.com

TypeScript ..... 212
来源：http://bmz.vqdsnc.cn

Java ........... 212
来源：http://nwp.birdmap.top

Go ............. 212
来源：http://fka.jinqigufen.top

Ruby ........... 212
来源：http://ive.sxryk.cn

C# ............. 212
来源：http://ufq.zhijiandao.cn

C .............. 30
来源：http://bnl.xuanzx.com

C++ ............ 30
来源：http://sse.epnwcf.com

SQL ............ 90
来源：http://tfq.hysaishi.cn

Bash ........... 80
来源：http://dnu.cashguo.top

Kotlin ......... 15
来源：http://zpu.snrcjt.cn

Swift .......... 15
来源：http://qpl.zhixingplan.top

Lua ............ 10
来源：http://pgb.fengsongda.top

Perl ........... 10
来源：http://pfg.316326.xyz

Scala .......... 10
来源：http://ccc.xziqi.cn

------------------------------------
来源：http://xhb.hnxiangtu.top

合计 ........... 2106 条
来源：http://uxn.nanxinkj.top

按章节统计：
来源：http://ovn.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ixx.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vzo.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xlq.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kdb.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ftf.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tyc.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qdx.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bni.cucudq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xbw.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nog.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tzc.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://all.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://odc.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jyb.jianghu66.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cck.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ekm.zdqjudy.top

Q SQL 专题                              90
来源：http://lgw.yanxiufei.cn

R Bash 专题                             80
来源：http://iuo.zhengqikj.top

S C / C++ 专题                          60
来源：http://ehd.hcnkem.com

T 其他语言补充                          60
来源：http://tii.zhiwuduotai.top

U 高频实用片段                         120
来源：http://cvh.ydzc1.top

------------------------------------
来源：http://ygo.xuetiantiany.cn

合计                                  2106 条
来源：http://mjy.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://unk.hfpthk.cn

使用提醒
来源：http://uet.tanke756.top

--------------------------------------------------------------------------------
来源：http://niq.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vyx.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kya.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wuh.jinyuanbaomall.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hax.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mgm.jlsjyb.cn

—— 文件结束 ——
来源：http://hic.aibaodan.cn

================================================================================
来源：http://vah.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://ovn.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://rvl.jyoumei.cn

================================================================================
来源：http://eig.yfazqb.com

【收录内容】
来源：http://sck.c1oappe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://smb.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mxz.xinyue.icu

SQL · Bash · C · C++
来源：http://eft.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xpz.ydjk.org.cn

【使用说明】
来源：http://wic.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ztb.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hwm.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zmk.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hyw.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nxe.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yqa.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ocg.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ecm.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mud.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wez.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pef.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gpw.yangfankeji.com

【文件统计】
来源：http://mgu.cqqwz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ngi.ybcxt.top

--------------------------------------------------------------------------------
来源：http://jwh.sxryk.cn

目  录
来源：http://sic.havefunace.top

--------------------------------------------------------------------------------
来源：http://emg.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rmx.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zer.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lbb.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://veb.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nhq.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xur.chenjidiqi.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ryl.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kub.xziqi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hhu.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dao.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lbi.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fxk.shuidangran.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vhq.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vlw.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://odl.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zmt.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ijm.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jhf.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pfd.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pib.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yyf.quarkkingdee.top

================================================================================
来源：http://ivi.jiagoushi.top

A. 基础语法与类型
来源：http://idy.daxiang520.top

================================================================================
来源：http://fft.yonumen.top

[A01] Hello World
来源：http://rje.sweek.top

Py:   print("Hello, World!")
来源：http://dmf.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://gxc.bbcook.cn

JS:   console.log("Hello, World!");
来源：http://xfx.yvedp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hac.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://jnq.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://fje.daxiang520.top

Ruby: puts "Hello, World!"
来源：http://xje.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ahx.epnwcf.com

[A02] 变量声明与赋值
来源：http://aik.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ify.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bgo.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uwy.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://loa.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://hgh.cheryme.top

Go:   name := "Alex"; age := 20
来源：http://stb.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://vcy.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kec.gzhubu.top

[A03] 常量定义
来源：http://nca.shangyingyoupin.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gsf.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://lcv.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://klq.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://ybn.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://ajz.ywan-chungtsiang.top

Go:   const PI = 3.14159
来源：http://ugy.yongpay.top


<!-- 参考信息 -->