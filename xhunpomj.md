代发 wailian999

[U35] Py：发送邮件
来源：http://vby.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ocf.jlsjyb.cn

[U36] Py：定时任务
来源：http://uqe.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://cvs.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://kis.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tst.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://jay.ivvv.top

Path(__file__).resolve().parent
来源：http://jwm.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://eky.fktsv.cn

sys.stdout.isatty()
来源：http://ebh.redwolf501.top

[U40] Py：打印到标准错误
来源：http://bni.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://hrs.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://dui.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kay.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://mxm.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uaj.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://vit.svipenyu.cn

namespace App\Http;
来源：http://npj.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://oam.daria6918.cn

declare(strict_types=1);
来源：http://kmp.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://iww.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lgq.bbcook.cn

[U46] PHP：可空类型
来源：http://trr.shzxlz.cn

?string $name = null
来源：http://psu.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://fel.snrcjt.cn

int|string $id
来源：http://qvy.hfpthk.cn

[U48] PHP：纯枚举
来源：http://zdo.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wos.jqgfzy.top

[U49] PHP：只读属性
来源：http://usb.guowangkeji.top

public readonly string $name
来源：http://rma.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://ygp.bjfxy.top

public function __construct(private int $id) {}
来源：http://jsp.hcnkem.com

[U51] PHP：数组解构
来源：http://fig.epnwcf.com

[$a, $b] = $arr;
来源：http://zoa.shzxlz.cn

[U52] PHP：箭头函数
来源：http://cor.yongpay.top

$double = fn($x) => $x * 2;
来源：http://ann.chenzaomai.com

[U53] PHP：空合并运算符
来源：http://duq.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://pnv.52xcode.cn

[U54] PHP：空安全调用
来源：http://cvu.gotoacloud.top

$obj?->method()
来源：http://hgu.andypj.xyz

[U55] PHP：match 表达式
来源：http://kkp.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jwz.bbcook.cn

[U56] PHP：命名参数
来源：http://ppn.xinyue.icu

f(a: 1, b: 2)
来源：http://vdo.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://rkz.bbcook.cn

"值: {$a}"
来源：http://grl.smart0.xyz

[U58] PHP：数组三件套
来源：http://fme.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gho.cucudq.cn

[U59] PHP：自定义排序
来源：http://ocl.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhr.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://guw.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gjz.yj20258.top

[U61] PHP：正则
来源：http://nfg.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mit.svipenyu.cn

[U62] PHP：日期对象
来源：http://rts.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oxd.snrcjt.cn

[U63] PHP：文件读写
来源：http://qzp.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eoy.svipenyu.cn

[U64] PHP：目录遍历
来源：http://hwm.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://kol.ydzc1.top

[U65] PHP：会话
来源：http://pvs.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://voy.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://mgu.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vcd.cashguo.top

[U67] PHP：处理文件上传
来源：http://hgz.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zeo.c1oappe.top

[U68] PHP：PDO 连接
来源：http://uqi.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kfn.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://kdf.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nyc.ybcxt.top

[U70] PHP：PDO 事务
来源：http://kht.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ush.vehdjk.com

[U71] PHP：抛出异常
来源：http://ctu.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://vra.gogol.net.cn

[U72] PHP：写错误日志
来源：http://ozs.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://lht.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://frx.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://mys.aizwys.cn

[U74] PHP：读取环境变量
来源：http://lox.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://fdm.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://piz.ehwqpu.com

composer require psr/container
来源：http://xqb.andypj.xyz

[U76] PHP：简单路由
来源：http://fvf.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jck.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://lpk.tanke756.top

composer require twig/twig
来源：http://ytq.ehwqpu.com

[U78] PHP：单元测试
来源：http://okx.zdqjudy.top

composer require --dev phpunit/phpunit
来源：http://kwd.nanxuanxn.top

[U79] PHP：静态分析
来源：http://tfk.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://aoh.bjfxy.top

[U80] PHP：代码规范修复
来源：http://dwb.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qip.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://sgg.havefunace.top

npm init -y;  npm i express
来源：http://ucq.hammf.cn

[U82] JS：package.json 脚本
来源：http://llk.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kis.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://sug.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jmo.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://ghs.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://hsl.xuanzx.com

[U85] JS：可选链
来源：http://dqo.tianlin.xyz

a?.b?.c
来源：http://trp.gogol.net.cn

[U86] JS：空值合并
来源：http://jus.nwbrower.top

a ?? b
来源：http://lao.sufxvd.cn

[U87] JS：解构默认值
来源：http://bbd.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://ict.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://bjt.316326.xyz

{ ...a, ...b }
来源：http://nzu.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://buf.yonumen.top

[...new Set(arr)]
来源：http://oie.zdqjudy.top

[U90] JS：数字数组排序
来源：http://mpu.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://wdm.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://sdc.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kgz.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://lkz.tanke756.top

structuredClone(obj)
来源：http://zzx.c1oappe.top

[U93] JS：模板字符串
来源：http://nqn.zdbjq.cn

`共 ${n} 条`
来源：http://djb.xziqi.cn

[U94] JS：箭头函数
来源：http://rjo.kuanghao11.cn

const double = x => x * 2;
来源：http://ufy.shzxlz.cn

[U95] JS：Promise 包装
来源：http://ush.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://ole.shuidangran.top

[U96] JS：async/await 与异常
来源：http://vlh.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rsf.aibaodan.cn

[U97] JS：并发请求
来源：http://hsd.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uwt.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://ilz.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ugj.mhx1999.top

[U99] JS：事件监听
来源：http://qxf.aizwys.cn

el.addEventListener("click", e => {})
来源：http://bmy.jinqigufen.top

[U100] JS：DOM 查询
来源：http://tln.daria6918.cn

document.querySelector(".item")
来源：http://jtw.jiagoushi.top

[U101] JS：classList 操作
来源：http://qor.haohaochexian.top

el.classList.toggle("active")
来源：http://gzo.xinyue.icu

[U102] JS：本地存储
来源：http://cgx.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nks.guowangkeji.top

[U103] JS：定时器
来源：http://mzf.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xsa.hywenlv.cn

[U104] JS：防抖
来源：http://lrl.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdx.nanxinkj.top

[U105] JS：节流
来源：http://icn.hongshengwenyu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dea.vqdsnc.cn

[U106] JS：日期格式化
来源：http://jji.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pkh.kuanghao11.cn

[U107] JS：数字千分位
来源：http://xqj.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nfe.ivvv.top

[U108] JS：随机整数
来源：http://qyo.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xfw.ppjwa.cn

[U109] JS：数组分组
来源：http://hnf.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://orv.sysykeji.top

[U110] JS：数组分块
来源：http://jyd.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qea.meibo888.top

[U111] JS：对象转 Map
来源：http://nqv.52xcode.cn

new Map(Object.entries(obj))
来源：http://rzz.bjfxy.top

[U112] JS：字符串补位
来源：http://pic.haohaochexian.top

"7".padStart(3, "0")
来源：http://gmh.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://hea.hysaishi.cn

s.replaceAll("a", "b")
来源：http://qyc.316326.xyz

[U114] JS：JSON 深比较
来源：http://xkd.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rpd.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://tfc.nanxinkj.top

crypto.randomUUID()
来源：http://uch.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://ypj.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://ypk.jlsjyb.cn

[U117] JS：单元测试
来源：http://hkc.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://aij.sufxvd.cn

[U118] JS：开发服务器
来源：http://szv.jianghu66.top

npm i -D vite;  npx vite
来源：http://bvi.aibaodan.cn

[U119] JS：生产构建
来源：http://hln.fzhhl.top

npx vite build
来源：http://lrk.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://gcq.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://day.sysykeji.top

================================================================================
来源：http://qgd.zhixingplan.top

统计汇总
来源：http://qlb.yanxiufei.cn

================================================================================
来源：http://owe.yanxiufei.cn

按语言统计（条）：
来源：http://fvr.birdmap.top

Python ......... 252
来源：http://sax.316326.xyz

PHP ............ 252
来源：http://aij.wangdashe.top

JavaScript ..... 252
来源：http://mcr.yj202588.top

TypeScript ..... 212
来源：http://eax.jinqigfzy.top

Java ........... 212
来源：http://hpa.sweek.top

Go ............. 212
来源：http://uqp.wangdashe.top

Ruby ........... 212
来源：http://eqt.yfazqb.com

C# ............. 212
来源：http://cpm.daria6918.cn

C .............. 30
来源：http://nux.xziqi.cn

C++ ............ 30
来源：http://tlf.cucudq.cn

SQL ............ 90
来源：http://wvg.ivvv.top

Bash ........... 80
来源：http://rxx.nanxuanxn.top

Kotlin ......... 15
来源：http://ahg.fehbvm.com

Swift .......... 15
来源：http://exv.aibaodan.cn

Lua ............ 10
来源：http://qti.aibaodan.cn

Perl ........... 10
来源：http://zzj.ppjwa.cn

Scala .......... 10
来源：http://nay.hywenlv.cn

------------------------------------
来源：http://chd.redwolf501.top

合计 ........... 2106 条
来源：http://jrf.fehbvm.com

按章节统计：
来源：http://xau.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ejv.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://srq.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lks.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wse.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gss.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sfg.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vgu.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddt.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xwp.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://umg.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hkc.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://acd.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hxa.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vlr.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dwv.jinghuilouyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ipj.jianghu66.top

Q SQL 专题                              90
来源：http://lpm.chenzaomai.com

R Bash 专题                             80
来源：http://ceq.shzxlz.cn

S C / C++ 专题                          60
来源：http://yma.yonumen.top

T 其他语言补充                          60
来源：http://bol.redwolf501.top

U 高频实用片段                         120
来源：http://dfv.cheryme.top

------------------------------------
来源：http://hdn.jqgufenzy.top

合计                                  2106 条
来源：http://ffg.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://mpe.guannengcc.top

使用提醒
来源：http://bzm.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://mxq.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qgy.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://phr.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pls.hammf.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bnu.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gnb.epnwcf.com

—— 文件结束 ——
来源：http://ldo.tianlin.xyz

================================================================================
来源：http://xpq.zhongyouzk.top

程序语言常见例子速查手册（2024 版）
来源：http://mfo.wangdashe.top

Common Programming Examples Cheat Book
来源：http://ikt.hywenlv.cn

================================================================================
来源：http://odz.wangshuangyany.cn

【收录内容】
来源：http://pwj.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://avq.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://emu.yuanzhike.top

SQL · Bash · C · C++
来源：http://uql.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kek.ybcxt.top

【使用说明】
来源：http://fpn.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pwo.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vpu.tanke756.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mjx.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fih.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://aky.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://npb.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cry.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://saw.chenlongwang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://klo.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vfe.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qms.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iqq.kuanghao11.cn

【文件统计】
来源：http://qys.yuanzhike.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pyc.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://yjd.jqgfzy.top

目  录
来源：http://eds.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://ymu.fktsv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zas.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://udk.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zlm.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dgl.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gyz.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://peg.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://omz.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cor.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oki.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zcu.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jgm.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zfk.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://njz.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://swd.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hpw.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://doz.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ztk.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://mqz.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ron.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://avv.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://men.chenzaomai.com

================================================================================
来源：http://eeg.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://uus.fzhhl.top

================================================================================
来源：http://zoj.52xcode.cn

[A01] Hello World
来源：http://ymm.shuidangran.top

Py:   print("Hello, World!")
来源：http://jzn.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://cbv.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://cne.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rfz.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://xjo.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://ara.gotoacloud.top

Ruby: puts "Hello, World!"
来源：http://jlk.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://atn.tian-w.cn

[A02] 变量声明与赋值
来源：http://tta.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://euv.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mum.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://saa.guannengcc.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aii.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://htx.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://dng.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://ytt.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://jhv.svipenyu.cn

[A03] 常量定义
来源：http://tsa.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://svu.dianchejie.cn

PHP:  const PI = 3.14159;
来源：http://igi.ydjk.org.cn


<!-- 参考信息 -->