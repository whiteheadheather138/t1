代发 wailian999

[U31] Py：单测
来源：http://sys.redwolf501.top

python -m pytest -q
来源：http://tbe.ivvv.top

[U32] Py：代码格式化
来源：http://ikb.ybcxt.top

ruff format . && ruff check --fix .
来源：http://iea.jyoumei.cn

[U33] Py：打包发布
来源：http://ndy.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://rvn.bbcook.cn

[U34] Py：判断编码
来源：http://ixp.vehdjk.com

chardet.detect(raw)
来源：http://yqt.jinqigfzy.top

[U35] Py：发送邮件
来源：http://ypg.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kzt.yueranfly.top

[U36] Py：定时任务
来源：http://zqh.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://yje.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://jfl.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://oce.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://agp.bbcook.cn

Path(__file__).resolve().parent
来源：http://sjk.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://dcp.hongshengwenyu.top

sys.stdout.isatty()
来源：http://ozs.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://lny.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://aot.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://cwo.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xpi.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://tjq.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dxf.yj20258.top

[U43] PHP：声明命名空间
来源：http://vbj.daxiang520.top

namespace App\Http;
来源：http://vua.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://pbu.zycfv.cn

declare(strict_types=1);
来源：http://kqi.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://rox.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mjg.shzxlz.cn

[U46] PHP：可空类型
来源：http://axg.yfazqb.com

?string $name = null
来源：http://ltv.shzxlz.cn

[U47] PHP：联合类型
来源：http://dgt.fzhhl.top

int|string $id
来源：http://sfu.316326.xyz

[U48] PHP：纯枚举
来源：http://cib.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sps.aibaodan.cn

[U49] PHP：只读属性
来源：http://ybf.kuanghao11.cn

public readonly string $name
来源：http://zce.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://udf.yueranfly.top

public function __construct(private int $id) {}
来源：http://tlz.c1oappe.top

[U51] PHP：数组解构
来源：http://baj.redwolf501.top

[$a, $b] = $arr;
来源：http://zbv.snrcjt.cn

[U52] PHP：箭头函数
来源：http://ajc.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://mss.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://lda.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://yla.snrcjt.cn

[U54] PHP：空安全调用
来源：http://eja.chenzaomai.com

$obj?->method()
来源：http://kuz.zhengqikj.top

[U55] PHP：match 表达式
来源：http://lky.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ylq.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://egq.cucudq.cn

f(a: 1, b: 2)
来源：http://kwb.zycfv.cn

[U57] PHP：字符串插值
来源：http://wrf.yj202588.top

"值: {$a}"
来源：http://cka.redwolf501.top

[U58] PHP：数组三件套
来源：http://rfo.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nox.hcnkem.com

[U59] PHP：自定义排序
来源：http://kjp.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tts.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://swq.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mkt.fengsongda.top

[U61] PHP：正则
来源：http://zak.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xyk.haohaochexian.top

[U62] PHP：日期对象
来源：http://vgb.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ric.cucudq.cn

[U63] PHP：文件读写
来源：http://hjx.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qyl.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://nzw.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://fxu.shanyushiyangtech.top

[U65] PHP：会话
来源：http://yzf.havefunace.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ybk.zhiwuduotai.top

[U66] PHP：设置 Cookie
来源：http://igr.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lgc.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://tuo.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qlw.cashguo.top

[U68] PHP：PDO 连接
来源：http://bjq.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ypk.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://ltl.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gnt.bjfxy.top

[U70] PHP：PDO 事务
来源：http://sca.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hbr.xylfe.cn

[U71] PHP：抛出异常
来源：http://lgh.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://mkm.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://fgo.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://xli.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://drz.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://avu.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://cmg.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://tsb.shuidangran.top

[U75] PHP：依赖注入
来源：http://kds.daxiang520.top

composer require psr/container
来源：http://vqe.jyoumei.cn

[U76] PHP：简单路由
来源：http://awn.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pqx.redwolf501.top

[U77] PHP：模板渲染
来源：http://uhk.0kj1m.cn

composer require twig/twig
来源：http://mcb.gzhubu.top

[U78] PHP：单元测试
来源：http://ccb.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://mwc.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://iop.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://czc.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://ycr.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ytk.svipenyu.cn

[U81] JS：初始化项目
来源：http://sdi.nanxuanxn.top

npm init -y;  npm i express
来源：http://yoq.bjfxy.top

[U82] JS：package.json 脚本
来源：http://oby.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dmn.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://vdy.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://uai.yj202588.top

[U84] JS：CommonJS 写法
来源：http://pur.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://dpv.hnqzz.top

[U85] JS：可选链
来源：http://uvj.yfazqb.com

a?.b?.c
来源：http://omw.hnxiangtu.top

[U86] JS：空值合并
来源：http://blg.xingfuxueyuan.xyz

a ?? b
来源：http://zhc.zhixingplan.top

[U87] JS：解构默认值
来源：http://srw.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://iiy.aizwys.cn

[U88] JS：对象展开合并
来源：http://bkb.iojbl.cn

{ ...a, ...b }
来源：http://sxb.zhiwuduotai.top

[U89] JS：数组去重
来源：http://gml.bjfxy.top

[...new Set(arr)]
来源：http://fpd.jqgfzy.top

[U90] JS：数字数组排序
来源：http://pet.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://cmm.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://psc.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dis.hywenlv.cn

[U92] JS：深拷贝
来源：http://nos.gzhubu.top

structuredClone(obj)
来源：http://xns.jinqigufen.top

[U93] JS：模板字符串
来源：http://xyq.yueranfly.top

`共 ${n} 条`
来源：http://xnw.jqgfzy.top

[U94] JS：箭头函数
来源：http://xjl.bbcook.cn

const double = x => x * 2;
来源：http://xne.shuidangran.top

[U95] JS：Promise 包装
来源：http://rsh.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://ppd.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://dlo.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pxa.c1oappe.top

[U97] JS：并发请求
来源：http://tib.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://anu.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://qpt.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yzr.zhiwuduotai.top

[U99] JS：事件监听
来源：http://hsb.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://xjp.ivvv.top

[U100] JS：DOM 查询
来源：http://ktr.shzxlz.cn

document.querySelector(".item")
来源：http://wmv.havefunace.top

[U101] JS：classList 操作
来源：http://wao.zhixingplan.top

el.classList.toggle("active")
来源：http://xtt.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://ocf.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oue.gogol.net.cn

[U103] JS：定时器
来源：http://sib.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hgp.yonumen.top

[U104] JS：防抖
来源：http://bel.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wei.cqqwz.cn

[U105] JS：节流
来源：http://dlq.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hxz.xinyue.icu

[U106] JS：日期格式化
来源：http://btb.zhixingplan.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://riq.aizwys.cn

[U107] JS：数字千分位
来源：http://oem.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://esg.tarul.cn

[U108] JS：随机整数
来源：http://mqx.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ide.yuxming.cn

[U109] JS：数组分组
来源：http://dxx.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://rsv.yangfankeji.com

[U110] JS：数组分块
来源：http://dtm.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xec.yj20258888.top

[U111] JS：对象转 Map
来源：http://jip.bbcook.cn

new Map(Object.entries(obj))
来源：http://kbr.ybcxt.top

[U112] JS：字符串补位
来源：http://ogf.quarkkingdee.top

"7".padStart(3, "0")
来源：http://kus.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://dlf.cdnleiting.top

s.replaceAll("a", "b")
来源：http://dcv.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://zac.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pqi.vehdjk.com

[U115] JS：生成 UUID
来源：http://shw.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://vuc.sxryk.cn

[U116] JS：类型检查（JSDoc）
来源：http://trz.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://lpp.xylfe.cn

[U117] JS：单元测试
来源：http://kkw.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://xez.ydzc1.top

[U118] JS：开发服务器
来源：http://hkn.daria6918.cn

npm i -D vite;  npx vite
来源：http://thd.shangyingyoupin.top

[U119] JS：生产构建
来源：http://lyy.hysaishi.cn

npx vite build
来源：http://gfh.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://vbg.meibo888.top

import.meta.env.VITE_API_URL
来源：http://mhm.ywan-chungtsiang.top

================================================================================
来源：http://lgj.jqgufenzy.top

统计汇总
来源：http://isr.jianghu66.top

================================================================================
来源：http://yta.pycfn.com

按语言统计（条）：
来源：http://pus.316326.xyz

Python ......... 252
来源：http://hye.sysykeji.top

PHP ............ 252
来源：http://buo.zycfv.cn

JavaScript ..... 252
来源：http://bst.snrcjt.cn

TypeScript ..... 212
来源：http://cel.jiagoushi.top

Java ........... 212
来源：http://nlv.tarul.cn

Go ............. 212
来源：http://rby.zhongyouzk.top

Ruby ........... 212
来源：http://nmu.yuxming.cn

C# ............. 212
来源：http://igy.52xcode.cn

C .............. 30
来源：http://uaw.cucudq.cn

C++ ............ 30
来源：http://qsh.shangyingyoupin.top

SQL ............ 90
来源：http://crd.daxiang520.top

Bash ........... 80
来源：http://umw.xinyue.icu

Kotlin ......... 15
来源：http://imi.dashuyun.cn

Swift .......... 15
来源：http://jly.shzxlz.cn

Lua ............ 10
来源：http://wju.hnxiangtu.top

Perl ........... 10
来源：http://qtk.pycfn.com

Scala .......... 10
来源：http://igh.yj20258.top

------------------------------------
来源：http://ced.yangfankeji.com

合计 ........... 2106 条
来源：http://uth.c1oappe.top

按章节统计：
来源：http://ypx.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jmm.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wzz.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dwg.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iki.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sla.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fan.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uto.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zlp.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kmz.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ngp.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://irl.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://crb.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pzo.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://upe.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://isb.jyoumei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ybr.cdnleiting.top

Q SQL 专题                              90
来源：http://kmy.ybcxt.top

R Bash 专题                             80
来源：http://ekx.nanxinkj.top

S C / C++ 专题                          60
来源：http://ojc.kuanghao11.cn

T 其他语言补充                          60
来源：http://yqs.chenjidiqi.icu

U 高频实用片段                         120
来源：http://ykm.nanxuanxn.top

------------------------------------
来源：http://ozz.ydjk.org.cn

合计                                  2106 条
来源：http://byu.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://uuf.bjfxy.top

使用提醒
来源：http://nzo.redwolf501.top

--------------------------------------------------------------------------------
来源：http://qhn.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://woh.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tvx.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eej.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ovc.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rds.jinqigufen.top

—— 文件结束 ——
来源：http://nim.xziqi.cn

================================================================================
来源：http://nai.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://nig.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://iik.xylfe.cn

================================================================================
来源：http://uaf.cucudq.cn

【收录内容】
来源：http://wcg.cashguo.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dul.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://luq.9152youxi.cn

SQL · Bash · C · C++
来源：http://unt.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kdf.ivvv.top

【使用说明】
来源：http://sij.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://toa.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bdb.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wjm.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vci.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nxo.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xkc.shuidangran.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://afa.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vvt.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iqu.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jkt.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ojl.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sbh.316326.xyz

【文件统计】
来源：http://hnh.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zyv.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://gvd.nanxinkj.top

目  录
来源：http://eqb.jianghu66.top

--------------------------------------------------------------------------------
来源：http://mix.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sju.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lea.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lih.meibo888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vfb.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pmt.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jfz.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jtn.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yid.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hvq.gzhubu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://izc.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mee.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lha.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lfq.ydzc1.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xiu.jqgfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gnv.52xcode.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xmr.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nrh.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bzf.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ajt.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aok.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qqu.xingfuxueyuan.xyz

================================================================================
来源：http://ltf.hnqzz.top

A. 基础语法与类型
来源：http://civ.shanyushiyangkeji.top

================================================================================
来源：http://yry.nanxuanxn.top

[A01] Hello World
来源：http://sga.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://efd.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://dpv.cdnleiting.top

JS:   console.log("Hello, World!");
来源：http://boe.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nxd.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://ovu.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://kmf.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://pyw.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yiy.yonumen.top

[A02] 变量声明与赋值
来源：http://jlg.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://txn.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://eqj.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://agp.ybcxt.top


<!-- 参考信息 -->