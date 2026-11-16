代发 wailian999

[U29] Py：属性校验
来源：http://oug.hnqzz.top

@property 与 @x.setter 配合
来源：http://afh.sweek.top

[U30] Py：数据类
来源：http://iwo.havefunace.top

@dataclass(slots=True)
来源：http://eng.zhaomingkeji.xyz

[U31] Py：单测
来源：http://law.sjlbkw.cn

python -m pytest -q
来源：http://aea.0kj1m.cn

[U32] Py：代码格式化
来源：http://xql.tian-w.cn

ruff format . && ruff check --fix .
来源：http://aat.vqdsnc.cn

[U33] Py：打包发布
来源：http://uaj.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://elp.0kj1m.cn

[U34] Py：判断编码
来源：http://pzx.feifeiyinyue.top

chardet.detect(raw)
来源：http://tjz.zdqjudy.top

[U35] Py：发送邮件
来源：http://tvv.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zge.dashuyun.cn

[U36] Py：定时任务
来源：http://vrb.yanxiufei.cn

schedule.every(10).minutes.do(job)
来源：http://pyk.zycfv.cn

[U37] Py：读写 Excel
来源：http://fdb.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://lfi.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://zce.yueranfly.top

Path(__file__).resolve().parent
来源：http://wuj.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://qcm.uphjek.com

sys.stdout.isatty()
来源：http://vjj.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://qik.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://ssu.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://osa.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sdp.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://srp.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lxd.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://wpv.guannengcc.top

namespace App\Http;
来源：http://zyh.hesvh.cn

[U44] PHP：开启严格类型
来源：http://jev.iojbl.cn

declare(strict_types=1);
来源：http://bvq.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://cxb.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ppb.hcnkem.com

[U46] PHP：可空类型
来源：http://txh.sysykeji.top

?string $name = null
来源：http://tdh.sufxvd.cn

[U47] PHP：联合类型
来源：http://fbu.quarkkingdee.top

int|string $id
来源：http://xss.nwbrower.top

[U48] PHP：纯枚举
来源：http://xxq.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jzd.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://tox.snrcjt.cn

public readonly string $name
来源：http://tng.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://urj.cashguo.top

public function __construct(private int $id) {}
来源：http://ayk.nanxinkj.top

[U51] PHP：数组解构
来源：http://yxa.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://pth.hywenlv.cn

[U52] PHP：箭头函数
来源：http://mlk.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://jjn.cashguo.top

[U53] PHP：空合并运算符
来源：http://mso.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://bnx.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://ipy.nanxinkj.top

$obj?->method()
来源：http://jhd.yuanzhike.top

[U55] PHP：match 表达式
来源：http://jiu.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nme.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://tnu.andypj.xyz

f(a: 1, b: 2)
来源：http://ehb.zdqjudy.top

[U57] PHP：字符串插值
来源：http://yjr.shanyushiyangkeji.top

"值: {$a}"
来源：http://lau.fehbvm.com

[U58] PHP：数组三件套
来源：http://usn.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vqz.zhixingplan.top

[U59] PHP：自定义排序
来源：http://ers.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhc.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://agx.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rkm.snrcjt.cn

[U61] PHP：正则
来源：http://nmq.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nah.hesvh.cn

[U62] PHP：日期对象
来源：http://cnr.cqqwz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ahc.ppjwa.cn

[U63] PHP：文件读写
来源：http://srn.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mru.ybcxt.top

[U64] PHP：目录遍历
来源：http://whp.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://qay.uphjek.com

[U65] PHP：会话
来源：http://mft.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://exv.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://vex.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hej.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://hil.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zsu.meibo888.top

[U68] PHP：PDO 连接
来源：http://pme.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bgs.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://frh.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ssw.sxryk.cn

[U70] PHP：PDO 事务
来源：http://rhc.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wxu.sysykeji.top

[U71] PHP：抛出异常
来源：http://nei.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://tva.ivvv.top

[U72] PHP：写错误日志
来源：http://cza.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://ycw.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://msg.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://hjn.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://zhv.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://gcd.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://ect.yuxming.cn

composer require psr/container
来源：http://vzs.ydjk.org.cn

[U76] PHP：简单路由
来源：http://sat.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mzu.shuidangran.top

[U77] PHP：模板渲染
来源：http://ahz.hywenlv.cn

composer require twig/twig
来源：http://udd.chenlongwang.top

[U78] PHP：单元测试
来源：http://bbz.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://dou.sjlbkw.cn

[U79] PHP：静态分析
来源：http://pwr.zhiwuduotai.top

composer require --dev phpstan/phpstan
来源：http://rlk.daxiang520.top

[U80] PHP：代码规范修复
来源：http://faw.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zeo.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://ehv.zhongyouzk.top

npm init -y;  npm i express
来源：http://wdx.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://dyc.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wrf.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://sju.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dab.sweek.top

[U84] JS：CommonJS 写法
来源：http://tam.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://zrl.aizwys.cn

[U85] JS：可选链
来源：http://vgg.ivvv.top

a?.b?.c
来源：http://shy.daria6918.cn

[U86] JS：空值合并
来源：http://ver.c1oappe.top

a ?? b
来源：http://njq.vqdsnc.cn

[U87] JS：解构默认值
来源：http://izz.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://kbv.sufxvd.cn

[U88] JS：对象展开合并
来源：http://rpo.xuetiantiany.cn

{ ...a, ...b }
来源：http://jtq.redwolf501.top

[U89] JS：数组去重
来源：http://ujv.fanxiaobao.xyz

[...new Set(arr)]
来源：http://lis.9152youxi.cn

[U90] JS：数字数组排序
来源：http://efy.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://thp.ybcxt.top

[U91] JS：对象键值遍历
来源：http://qig.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cqh.hnqzz.top

[U92] JS：深拷贝
来源：http://klt.svipenyu.cn

structuredClone(obj)
来源：http://xnb.sjlbkw.cn

[U93] JS：模板字符串
来源：http://suz.jiagoushi.top

`共 ${n} 条`
来源：http://dkv.yj202588.top

[U94] JS：箭头函数
来源：http://kfq.shanyushiyangtech.top

const double = x => x * 2;
来源：http://geo.zhixingplan.top

[U95] JS：Promise 包装
来源：http://ueb.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://pop.hesvh.cn

[U96] JS：async/await 与异常
来源：http://ygi.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cbq.sjlbkw.cn

[U97] JS：并发请求
来源：http://qgs.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xku.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://yzy.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oqi.fktsv.cn

[U99] JS：事件监听
来源：http://vgz.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://bof.ppjwa.cn

[U100] JS：DOM 查询
来源：http://wek.gotoacloud.top

document.querySelector(".item")
来源：http://stt.jianghu66.top

[U101] JS：classList 操作
来源：http://ofd.hysaishi.cn

el.classList.toggle("active")
来源：http://rvy.yanxiufei.cn

[U102] JS：本地存储
来源：http://nir.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://exl.zhiwuduotai.top

[U103] JS：定时器
来源：http://toz.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vkw.yuanzhike.top

[U104] JS：防抖
来源：http://dwp.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uin.zdbjq.cn

[U105] JS：节流
来源：http://rbj.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lsr.nanxuanxn.top

[U106] JS：日期格式化
来源：http://fim.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpj.fehbvm.com

[U107] JS：数字千分位
来源：http://cxr.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://suk.yuxming.cn

[U108] JS：随机整数
来源：http://xlo.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://drr.sysykeji.top

[U109] JS：数组分组
来源：http://brc.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://njw.dashuyun.cn

[U110] JS：数组分块
来源：http://ozl.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yxm.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://kuf.shanyushiyangkeji.top

new Map(Object.entries(obj))
来源：http://cbc.cheryme.top

[U112] JS：字符串补位
来源：http://uyq.nanxinkj.top

"7".padStart(3, "0")
来源：http://phk.dashuyun.cn

[U113] JS：正则替换全部
来源：http://omd.yuanzhike.top

s.replaceAll("a", "b")
来源：http://eqa.yj20258888.top

[U114] JS：JSON 深比较
来源：http://nmk.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uyg.zycfv.cn

[U115] JS：生成 UUID
来源：http://lgw.fanxiaobao.xyz

crypto.randomUUID()
来源：http://qdd.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ygn.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://mfi.sxryk.cn

[U117] JS：单元测试
来源：http://zbd.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://swz.bjfxy.top

[U118] JS：开发服务器
来源：http://yhp.sysykeji.top

npm i -D vite;  npx vite
来源：http://hsn.pycfn.com

[U119] JS：生产构建
来源：http://qmx.fanxiaobao.xyz

npx vite build
来源：http://rhy.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://iiq.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://whj.zhengqikj.top

================================================================================
来源：http://ntx.ppjwa.cn

统计汇总
来源：http://xtx.tarul.cn

================================================================================
来源：http://klf.jinqigufen.top

按语言统计（条）：
来源：http://kwh.9152youxi.cn

Python ......... 252
来源：http://lwm.pycfn.com

PHP ............ 252
来源：http://enu.cdnleiting.top

JavaScript ..... 252
来源：http://dtu.fktsv.cn

TypeScript ..... 212
来源：http://kqq.guannengcc.top

Java ........... 212
来源：http://okf.zhengqikj.top

Go ............. 212
来源：http://kxw.gogol.net.cn

Ruby ........... 212
来源：http://cmq.guannengcc.top

C# ............. 212
来源：http://bze.hcnkem.com

C .............. 30
来源：http://zqw.jiagoushi.top

C++ ............ 30
来源：http://mnt.ctjpmb.com

SQL ............ 90
来源：http://ukv.nanxuanxn.top

Bash ........... 80
来源：http://pla.c1oappe.top

Kotlin ......... 15
来源：http://hrv.yueranfly.top

Swift .......... 15
来源：http://lxw.havefunace.top

Lua ............ 10
来源：http://dli.yj20258888.top

Perl ........... 10
来源：http://xsj.gogol.net.cn

Scala .......... 10
来源：http://nwh.ydjk.org.cn

------------------------------------
来源：http://kkz.hysaishi.cn

合计 ........... 2106 条
来源：http://uvi.xylfe.cn

按章节统计：
来源：http://aii.chenlongwang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gel.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ysk.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://znq.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dxi.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dex.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qkn.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://glk.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tkp.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sma.gotoacloud.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xhw.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vxu.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nfb.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://imr.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dek.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ivb.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://krr.guowangkeji.top

Q SQL 专题                              90
来源：http://okt.xinyue.icu

R Bash 专题                             80
来源：http://zvw.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://hxn.wangdashe.top

T 其他语言补充                          60
来源：http://fdx.ppjwa.cn

U 高频实用片段                         120
来源：http://tvu.sufxvd.cn

------------------------------------
来源：http://hpd.tianlin.xyz

合计                                  2106 条
来源：http://swk.yueranfly.top

--------------------------------------------------------------------------------
来源：http://gyp.9152youxi.cn

使用提醒
来源：http://zbx.gzhubu.top

--------------------------------------------------------------------------------
来源：http://rnj.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mtz.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fgq.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://log.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ddh.epnwcf.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jis.ydjk.org.cn

—— 文件结束 ——
来源：http://gtw.sjlbkw.cn

================================================================================
来源：http://ztn.jinyuanbaomall.cn

程序语言常见例子速查手册（2024 版）
来源：http://jyv.52xcode.cn

Common Programming Examples Cheat Book
来源：http://zln.hysaishi.cn

================================================================================
来源：http://iap.gotoacloud.top

【收录内容】
来源：http://xqn.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rhz.nanxuanxn.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qvh.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://eqy.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://crl.nanxinkj.top

【使用说明】
来源：http://qne.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ggh.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sru.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fae.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hpf.yangfankeji.com

Bash:  Shell         C:     C             C++:   C++
来源：http://cyv.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mes.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zsf.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hea.sxryk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qpo.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rpt.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aoh.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gks.shuidangran.top

【文件统计】
来源：http://hfp.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vwc.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://zbf.iojbl.cn

目  录
来源：http://csv.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://xdo.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bsn.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qug.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ysj.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tai.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://acx.9152youxi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hwk.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xhh.zhixingplan.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ibs.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pwz.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jhq.cqqwz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mmq.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tcf.sweek.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ice.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cym.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ahp.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iyv.hysaishi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rql.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mkf.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nle.nanxuanxn.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qaj.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oph.jinqigufen.top

================================================================================
来源：http://xlr.jqgufenzy.top

A. 基础语法与类型
来源：http://zpy.ybcxt.top

================================================================================
来源：http://obr.gaohongyu789.top

[A01] Hello World
来源：http://mni.dashuyun.cn

Py:   print("Hello, World!")
来源：http://fng.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://ddl.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://nwo.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kyu.hesvh.cn

Java: System.out.println("Hello, World!");
来源：http://lgn.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://ega.dashuyun.cn

Ruby: puts "Hello, World!"
来源：http://ksa.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mbe.jinghuilouyu.cn


<!-- 参考信息 -->