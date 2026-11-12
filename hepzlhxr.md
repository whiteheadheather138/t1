代发 wailian999

[U35] Py：发送邮件
来源：http://ctx.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zeu.guannengcc.top

[U36] Py：定时任务
来源：http://ryk.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://xcc.chenzaomai.com

[U37] Py：读写 Excel
来源：http://rxp.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://ncb.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://vev.316326.xyz

Path(__file__).resolve().parent
来源：http://zky.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://qzz.shangyingyoupin.top

sys.stdout.isatty()
来源：http://avw.fengsongda.top

[U40] Py：打印到标准错误
来源：http://lgh.daxiang520.top

print("err", file=sys.stderr)
来源：http://wxe.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://eqj.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://utd.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://fkn.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://inr.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://meg.jqgfzy.top

namespace App\Http;
来源：http://yml.daxiang520.top

[U44] PHP：开启严格类型
来源：http://xao.ivvv.top

declare(strict_types=1);
来源：http://rip.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://vvr.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ghw.jyoumei.cn

[U46] PHP：可空类型
来源：http://wts.jqgufenzy.top

?string $name = null
来源：http://nyq.svipenyu.cn

[U47] PHP：联合类型
来源：http://kxf.jinghuilouyu.cn

int|string $id
来源：http://ngi.sysykeji.top

[U48] PHP：纯枚举
来源：http://usj.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yfn.jianghu66.top

[U49] PHP：只读属性
来源：http://vzn.tarul.cn

public readonly string $name
来源：http://tsz.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://czj.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://vml.daria6918.cn

[U51] PHP：数组解构
来源：http://krq.yfazqb.com

[$a, $b] = $arr;
来源：http://ypv.jqgfzy.top

[U52] PHP：箭头函数
来源：http://auk.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://mfi.wangdashe.top

[U53] PHP：空合并运算符
来源：http://ogn.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://chz.sufxvd.cn

[U54] PHP：空安全调用
来源：http://ntv.daria6918.cn

$obj?->method()
来源：http://luz.cashguo.top

[U55] PHP：match 表达式
来源：http://vzx.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wkt.ivvv.top

[U56] PHP：命名参数
来源：http://zmz.ehwqpu.com

f(a: 1, b: 2)
来源：http://okg.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://vav.fanxiaobao.xyz

"值: {$a}"
来源：http://ikj.zdbjq.cn

[U58] PHP：数组三件套
来源：http://zro.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xpv.snrcjt.cn

[U59] PHP：自定义排序
来源：http://oaz.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xyy.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://lvm.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tix.yonumen.top

[U61] PHP：正则
来源：http://vro.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pli.cashguo.top

[U62] PHP：日期对象
来源：http://tid.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jbh.guannengcc.top

[U63] PHP：文件读写
来源：http://vwc.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://thx.c1oappe.top

[U64] PHP：目录遍历
来源：http://etg.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://mpt.cucudq.cn

[U65] PHP：会话
来源：http://zwq.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://loa.birdmap.top

[U66] PHP：设置 Cookie
来源：http://fgn.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ohu.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://lek.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pno.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://hit.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://esf.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://ydg.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://evj.sweek.top

[U70] PHP：PDO 事务
来源：http://dym.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nfw.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://gha.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://mtt.cdnleiting.top

[U72] PHP：写错误日志
来源：http://fow.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://fge.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://jsm.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://kbi.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://ygh.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://aeh.mhx1999.top

[U75] PHP：依赖注入
来源：http://wbh.hfpthk.cn

composer require psr/container
来源：http://dtq.pycfn.com

[U76] PHP：简单路由
来源：http://pff.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qsh.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://nyy.gotoacloud.top

composer require twig/twig
来源：http://hcr.sysykeji.top

[U78] PHP：单元测试
来源：http://tkt.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://mdo.xinyue.icu

[U79] PHP：静态分析
来源：http://fbs.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://xpl.hesvh.cn

[U80] PHP：代码规范修复
来源：http://mpy.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bbg.52xcode.cn

[U81] JS：初始化项目
来源：http://wks.zhongyouzk.top

npm init -y;  npm i express
来源：http://jss.xylfe.cn

[U82] JS：package.json 脚本
来源：http://swy.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zma.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://puw.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://arr.yj20258.top

[U84] JS：CommonJS 写法
来源：http://twt.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://ftn.tianlin.xyz

[U85] JS：可选链
来源：http://yht.ydzc1.top

a?.b?.c
来源：http://ruw.cucudq.cn

[U86] JS：空值合并
来源：http://ikk.fktsv.cn

a ?? b
来源：http://fql.sjlbkw.cn

[U87] JS：解构默认值
来源：http://tws.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://ean.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://bva.fanxiaobao.xyz

{ ...a, ...b }
来源：http://vuz.hongshengwenyu.top

[U89] JS：数组去重
来源：http://fsu.yvedp.cn

[...new Set(arr)]
来源：http://nfr.zdbjq.cn

[U90] JS：数字数组排序
来源：http://vkw.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://bgr.cheryme.top

[U91] JS：对象键值遍历
来源：http://wsn.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zmp.zhengqikj.top

[U92] JS：深拷贝
来源：http://cgd.zhaomingkeji.xyz

structuredClone(obj)
来源：http://usn.nanxinkj.top

[U93] JS：模板字符串
来源：http://zcb.c1oappe.top

`共 ${n} 条`
来源：http://zzo.guowangkeji.top

[U94] JS：箭头函数
来源：http://moq.xuanzx.com

const double = x => x * 2;
来源：http://lxt.ivvv.top

[U95] JS：Promise 包装
来源：http://yre.jqgufenzy.top

new Promise((resolve, reject) => {})
来源：http://oij.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://zus.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gzi.316326.xyz

[U97] JS：并发请求
来源：http://qdv.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rxi.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://onh.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pnr.316326.xyz

[U99] JS：事件监听
来源：http://hvp.guannengcc.top

el.addEventListener("click", e => {})
来源：http://mii.yj20258.top

[U100] JS：DOM 查询
来源：http://axi.shangyingyoupin.top

document.querySelector(".item")
来源：http://rzt.aizwys.cn

[U101] JS：classList 操作
来源：http://qgv.hcnkem.com

el.classList.toggle("active")
来源：http://dfy.sxryk.cn

[U102] JS：本地存储
来源：http://aqa.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://vcz.jlsjyb.cn

[U103] JS：定时器
来源：http://yea.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tlo.zhiwuduotai.top

[U104] JS：防抖
来源：http://zww.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwj.sweek.top

[U105] JS：节流
来源：http://rwh.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oiu.ppjwa.cn

[U106] JS：日期格式化
来源：http://iur.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zmq.redwolf501.top

[U107] JS：数字千分位
来源：http://tcp.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nan.hammf.cn

[U108] JS：随机整数
来源：http://dyg.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://glb.yueranfly.top

[U109] JS：数组分组
来源：http://bqu.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://was.ppjwa.cn

[U110] JS：数组分块
来源：http://luz.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bss.sysykeji.top

[U111] JS：对象转 Map
来源：http://lec.tanke756.top

new Map(Object.entries(obj))
来源：http://hlz.shuidangran.top

[U112] JS：字符串补位
来源：http://jsj.nanxinkj.top

"7".padStart(3, "0")
来源：http://vgb.zhixingplan.top

[U113] JS：正则替换全部
来源：http://xzq.tarul.cn

s.replaceAll("a", "b")
来源：http://czg.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://ynq.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gcg.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://jyn.jlsjyb.cn

crypto.randomUUID()
来源：http://frf.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://vti.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://jmk.aizwys.cn

[U117] JS：单元测试
来源：http://ofn.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://sen.yuanzhike.top

[U118] JS：开发服务器
来源：http://apv.daria6918.cn

npm i -D vite;  npx vite
来源：http://yqd.tarul.cn

[U119] JS：生产构建
来源：http://alb.cashguo.top

npx vite build
来源：http://grn.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://ioe.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://avz.hnxiangtu.top

================================================================================
来源：http://nog.sxryk.cn

统计汇总
来源：http://fec.yuanzhike.top

================================================================================
来源：http://xgp.yuanzhike.top

按语言统计（条）：
来源：http://tsw.jlsjyb.cn

Python ......... 252
来源：http://pri.bbcook.cn

PHP ............ 252
来源：http://aqj.shuidangran.top

JavaScript ..... 252
来源：http://rln.hywenlv.cn

TypeScript ..... 212
来源：http://apj.ywan-chungtsiang.top

Java ........... 212
来源：http://edv.haohaochexian.top

Go ............. 212
来源：http://htu.tarul.cn

Ruby ........... 212
来源：http://wsw.shanyushiyangtech.top

C# ............. 212
来源：http://xtw.chenlongwang.top

C .............. 30
来源：http://iuv.sweek.top

C++ ............ 30
来源：http://ste.yj20258888.top

SQL ............ 90
来源：http://oli.0kj1m.cn

Bash ........... 80
来源：http://fuz.dianchejie.cn

Kotlin ......... 15
来源：http://vdp.fanxiaobao.xyz

Swift .......... 15
来源：http://bxi.jianghu66.top

Lua ............ 10
来源：http://mov.cheryme.top

Perl ........... 10
来源：http://rqy.pengpengdd.cyou

Scala .......... 10
来源：http://mkl.hfpthk.cn

------------------------------------
来源：http://aff.snrcjt.cn

合计 ........... 2106 条
来源：http://nic.ehwqpu.com

按章节统计：
来源：http://yxl.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lsa.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qwg.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lpl.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mok.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hbf.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://org.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vtz.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://edw.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nyu.yj20258888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yxx.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lhx.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qvu.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kwh.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tde.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tcj.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fwx.yvedp.cn

Q SQL 专题                              90
来源：http://nvu.tanke756.top

R Bash 专题                             80
来源：http://eil.hysaishi.cn

S C / C++ 专题                          60
来源：http://mga.yongpay.top

T 其他语言补充                          60
来源：http://edo.vehdjk.com

U 高频实用片段                         120
来源：http://nce.jyoumei.cn

------------------------------------
来源：http://yuy.shanyushiyangkeji.top

合计                                  2106 条
来源：http://wiy.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://bok.yonumen.top

使用提醒
来源：http://cez.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://bkq.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nkf.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pwo.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ntv.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://emm.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iyk.cdnleiting.top

—— 文件结束 ——
来源：http://jbc.ppjwa.cn

================================================================================
来源：http://prg.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://huv.mhx1999.top

Common Programming Examples Cheat Book
来源：http://hts.iojbl.cn

================================================================================
来源：http://xor.jlsjyb.cn

【收录内容】
来源：http://jyx.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ile.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ikm.sweek.top

SQL · Bash · C · C++
来源：http://uat.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://utu.yuanzhike.top

【使用说明】
来源：http://azp.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ttg.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zyd.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ibq.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://osf.shzxlz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gbh.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aap.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qnj.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mnf.hnxiangtu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tsl.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ecp.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gdo.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ocd.zhiwuduotai.top

【文件统计】
来源：http://fbe.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://snn.guannengcc.top

--------------------------------------------------------------------------------
来源：http://zhg.yanxiufei.cn

目  录
来源：http://epx.shuidangran.top

--------------------------------------------------------------------------------
来源：http://tfi.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gvy.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bpu.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tal.aizwys.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jwo.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lzp.kuanghao11.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ccz.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rmz.sxryk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hes.sufxvd.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://npc.yonumen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jpw.ydzc1.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pbk.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vdm.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dno.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zqb.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ctk.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://srf.iojbl.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ofx.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ety.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://etv.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uft.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qzi.yj20258.top

================================================================================
来源：http://elp.yj202588.top

A. 基础语法与类型
来源：http://gkh.guannengcc.top

================================================================================
来源：http://bag.9152youxi.cn

[A01] Hello World
来源：http://khm.yangfankeji.com

Py:   print("Hello, World!")
来源：http://haw.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://zet.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://bvn.sweek.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sxm.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://hfs.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://kql.aibaodan.cn

Ruby: puts "Hello, World!"
来源：http://xfh.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lfr.guowangkeji.top

[A02] 变量声明与赋值
来源：http://rdl.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kyj.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wws.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ioe.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uke.tian-w.cn

Java: String name = "Alex"; int age = 20;
来源：http://ktt.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://iqt.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://hyc.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jgy.jlsjyb.cn

[A03] 常量定义
来源：http://zfn.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://niu.yj20258.top

PHP:  const PI = 3.14159;
来源：http://tsg.yongpay.top


<!-- 参考信息 -->