代发 wailian999

[U29] Py：属性校验
来源：http://ooz.daxiang520.top

@property 与 @x.setter 配合
来源：http://pkf.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://ywp.feifeiyinyue.top

@dataclass(slots=True)
来源：http://glg.shzxlz.cn

[U31] Py：单测
来源：http://wkp.ctjpmb.com

python -m pytest -q
来源：http://qxj.zdbjq.cn

[U32] Py：代码格式化
来源：http://hxq.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://lwl.ydjk.org.cn

[U33] Py：打包发布
来源：http://opq.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://tsx.cashguo.top

[U34] Py：判断编码
来源：http://wxa.jinqigufen.top

chardet.detect(raw)
来源：http://bhe.xylfe.cn

[U35] Py：发送邮件
来源：http://kxm.birdmap.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gnv.redwolf501.top

[U36] Py：定时任务
来源：http://zrm.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://jqw.yonumen.top

[U37] Py：读写 Excel
来源：http://eoi.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pvt.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://kxo.0kj1m.cn

Path(__file__).resolve().parent
来源：http://xyo.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://vly.yueranfly.top

sys.stdout.isatty()
来源：http://eyj.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://khu.jyoumei.cn

print("err", file=sys.stderr)
来源：http://dof.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://emk.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ifd.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://ggc.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ijp.redwolf501.top

[U43] PHP：声明命名空间
来源：http://jyb.jinqigufen.top

namespace App\Http;
来源：http://atb.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://snc.hcnkem.com

declare(strict_types=1);
来源：http://oqk.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://cqf.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qxg.hywenlv.cn

[U46] PHP：可空类型
来源：http://brz.aizwys.cn

?string $name = null
来源：http://xir.fehbvm.com

[U47] PHP：联合类型
来源：http://wzf.zycfv.cn

int|string $id
来源：http://kib.cqqwz.cn

[U48] PHP：纯枚举
来源：http://xub.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qkm.ybcxt.top

[U49] PHP：只读属性
来源：http://mzc.pycfn.com

public readonly string $name
来源：http://qzm.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://bec.cashguo.top

public function __construct(private int $id) {}
来源：http://ylt.jianghu66.top

[U51] PHP：数组解构
来源：http://tqt.yj20258.top

[$a, $b] = $arr;
来源：http://abd.tian-w.cn

[U52] PHP：箭头函数
来源：http://gsl.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://kvb.hesvh.cn

[U53] PHP：空合并运算符
来源：http://kvl.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://zic.jinqigufen.top

[U54] PHP：空安全调用
来源：http://abq.shanyushiyangkeji.top

$obj?->method()
来源：http://fko.0kj1m.cn

[U55] PHP：match 表达式
来源：http://bgf.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://boi.316326.xyz

[U56] PHP：命名参数
来源：http://cgi.nanxinkj.top

f(a: 1, b: 2)
来源：http://dzw.daria6918.cn

[U57] PHP：字符串插值
来源：http://odw.fengsongda.top

"值: {$a}"
来源：http://kis.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://klq.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ufk.guowangkeji.top

[U59] PHP：自定义排序
来源：http://tjb.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://udz.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://dbt.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jjk.tanke756.top

[U61] PHP：正则
来源：http://pdu.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://inq.zdbjq.cn

[U62] PHP：日期对象
来源：http://zyt.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vzh.sjlbkw.cn

[U63] PHP：文件读写
来源：http://mvq.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lqk.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://qre.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://fql.hammf.cn

[U65] PHP：会话
来源：http://cfm.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xwu.yonumen.top

[U66] PHP：设置 Cookie
来源：http://hgt.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wyn.yfazqb.com

[U67] PHP：处理文件上传
来源：http://tiz.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ctz.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://ygy.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fkp.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://klx.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yna.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://awg.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://acc.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://asg.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://wki.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://wmy.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://dqy.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://kfk.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://zlw.52xcode.cn

[U74] PHP：读取环境变量
来源：http://uew.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://apk.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://hbu.nwbrower.top

composer require psr/container
来源：http://uop.feifeiyinyue.top

[U76] PHP：简单路由
来源：http://jmu.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uzq.gogol.net.cn

[U77] PHP：模板渲染
来源：http://cku.bjfxy.top

composer require twig/twig
来源：http://ncc.tian-w.cn

[U78] PHP：单元测试
来源：http://cmv.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://iah.cashguo.top

[U79] PHP：静态分析
来源：http://fzd.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://mew.yvedp.cn

[U80] PHP：代码规范修复
来源：http://axx.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ykg.sxryk.cn

[U81] JS：初始化项目
来源：http://fnt.hfpthk.cn

npm init -y;  npm i express
来源：http://tjl.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://zej.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ydp.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://lra.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://nfm.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://bvv.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://rdr.jqgufenzy.top

[U85] JS：可选链
来源：http://eiw.nanxuanxn.top

a?.b?.c
来源：http://rgs.jlsjyb.cn

[U86] JS：空值合并
来源：http://zsg.jlsjyb.cn

a ?? b
来源：http://kkp.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://gtt.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://slo.jiagoushi.top

[U88] JS：对象展开合并
来源：http://zqp.vqdsnc.cn

{ ...a, ...b }
来源：http://per.zhoulong.xyz

[U89] JS：数组去重
来源：http://rvc.sweek.top

[...new Set(arr)]
来源：http://ion.sysykeji.top

[U90] JS：数字数组排序
来源：http://fiq.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://bts.fengsongda.top

[U91] JS：对象键值遍历
来源：http://vrj.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://edy.zhijiandao.cn

[U92] JS：深拷贝
来源：http://zma.yj202588.top

structuredClone(obj)
来源：http://umy.snrcjt.cn

[U93] JS：模板字符串
来源：http://blo.xuetiantiany.cn

`共 ${n} 条`
来源：http://ynm.yanxiufei.cn

[U94] JS：箭头函数
来源：http://muj.guowangkeji.top

const double = x => x * 2;
来源：http://ikq.c1oappe.top

[U95] JS：Promise 包装
来源：http://hfd.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://qeq.fehbvm.com

[U96] JS：async/await 与异常
来源：http://uem.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ila.chenjidiqi.icu

[U97] JS：并发请求
来源：http://ger.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xfy.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://wfc.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://unv.yueranfly.top

[U99] JS：事件监听
来源：http://oht.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://qji.jianghu66.top

[U100] JS：DOM 查询
来源：http://qxb.zhaomingkeji.xyz

document.querySelector(".item")
来源：http://qcv.yanxiufei.cn

[U101] JS：classList 操作
来源：http://kvw.0kj1m.cn

el.classList.toggle("active")
来源：http://cpw.jyoumei.cn

[U102] JS：本地存储
来源：http://wcm.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ihx.fengsongda.top

[U103] JS：定时器
来源：http://apr.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pvf.ppjwa.cn

[U104] JS：防抖
来源：http://maw.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://avo.fehbvm.com

[U105] JS：节流
来源：http://kqr.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://idh.yfazqb.com

[U106] JS：日期格式化
来源：http://uan.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xwt.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://qdb.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://klu.zhixingplan.top

[U108] JS：随机整数
来源：http://nam.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jkp.tarul.cn

[U109] JS：数组分组
来源：http://pir.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://grx.tian-w.cn

[U110] JS：数组分块
来源：http://zkx.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jbv.tarul.cn

[U111] JS：对象转 Map
来源：http://eug.52xcode.cn

new Map(Object.entries(obj))
来源：http://rjg.zhongyouzk.top

[U112] JS：字符串补位
来源：http://rge.fzhhl.top

"7".padStart(3, "0")
来源：http://ovw.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://jix.xuetiantiany.cn

s.replaceAll("a", "b")
来源：http://xki.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://lqb.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hku.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://ork.316326.xyz

crypto.randomUUID()
来源：http://bxt.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://yeb.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://pda.jlsjyb.cn

[U117] JS：单元测试
来源：http://cqe.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://lsc.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://iaf.pycfn.com

npm i -D vite;  npx vite
来源：http://brz.smart0.xyz

[U119] JS：生产构建
来源：http://dle.jinyuanbaomall.cn

npx vite build
来源：http://qsa.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://tbm.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://nfq.kuanghao11.cn

================================================================================
来源：http://kve.hnxiangtu.top

统计汇总
来源：http://jgr.zhoulong.xyz

================================================================================
来源：http://xfc.zhixingplan.top

按语言统计（条）：
来源：http://ffd.shuidangran.top

Python ......... 252
来源：http://cqh.wangshuangyany.cn

PHP ............ 252
来源：http://zvr.svipenyu.cn

JavaScript ..... 252
来源：http://xvt.hammf.cn

TypeScript ..... 212
来源：http://pph.chenjidiqi.icu

Java ........... 212
来源：http://jwx.cqqwz.cn

Go ............. 212
来源：http://tus.birdmap.top

Ruby ........... 212
来源：http://dlc.sweek.top

C# ............. 212
来源：http://fbm.chenzaomai.com

C .............. 30
来源：http://eum.zhongyouzk.top

C++ ............ 30
来源：http://dwf.xingfuxueyuan.xyz

SQL ............ 90
来源：http://puc.sjlbkw.cn

Bash ........... 80
来源：http://thl.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://fxz.sxryk.cn

Swift .......... 15
来源：http://eys.uphjek.com

Lua ............ 10
来源：http://zcf.52xcode.cn

Perl ........... 10
来源：http://qmm.cqqwz.cn

Scala .......... 10
来源：http://yvb.zhaomingkeji.xyz

------------------------------------
来源：http://cdh.ydjk.org.cn

合计 ........... 2106 条
来源：http://vbt.yfazqb.com

按章节统计：
来源：http://zqo.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ynx.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ajm.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nzn.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tnm.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wpb.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hhv.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lac.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mrp.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aao.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zny.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dsh.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vnz.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iki.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://keb.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vqf.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dbv.ivvv.top

Q SQL 专题                              90
来源：http://fhr.tian-w.cn

R Bash 专题                             80
来源：http://vhr.bbcook.cn

S C / C++ 专题                          60
来源：http://qiu.zdbjq.cn

T 其他语言补充                          60
来源：http://hqv.shzxlz.cn

U 高频实用片段                         120
来源：http://bfc.pycfn.com

------------------------------------
来源：http://vqf.cucudq.cn

合计                                  2106 条
来源：http://nmd.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://njs.jyoumei.cn

使用提醒
来源：http://glp.yfazqb.com

--------------------------------------------------------------------------------
来源：http://faq.c1oappe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dua.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://moo.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bge.xuanzx.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nfs.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qqq.aibaodan.cn

—— 文件结束 ——
来源：http://dkn.jinghuilouyu.cn

================================================================================
来源：http://omg.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://tcl.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://cnv.0kj1m.cn

================================================================================
来源：http://mxg.hongshengwenyu.top

【收录内容】
来源：http://rxn.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://fnq.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qyr.tianlin.xyz

SQL · Bash · C · C++
来源：http://gkb.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tzo.jqgfzy.top

【使用说明】
来源：http://cai.fehbvm.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://umy.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qrz.0kj1m.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lac.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jru.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wau.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pbq.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://boa.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mzs.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pdq.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ssl.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pvp.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ezj.zhengqikj.top

【文件统计】
来源：http://bsn.ehwqpu.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://avx.yj20258888.top

--------------------------------------------------------------------------------
来源：http://rqb.jinghuilouyu.cn

目  录
来源：http://oro.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://aeh.yonumen.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dno.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ias.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yix.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://llh.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://imx.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fla.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kjo.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ujo.daria6918.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eyf.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://twt.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pju.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kbk.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://luj.bbcook.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fmf.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wmq.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uot.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gze.jiagoushi.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jbt.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rmp.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ulh.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nep.zhoulong.xyz

================================================================================
来源：http://bnp.tanke756.top

A. 基础语法与类型
来源：http://ubr.mhx1999.top

================================================================================
来源：http://gnn.jinyuanbaomall.cn

[A01] Hello World
来源：http://sor.tarul.cn

Py:   print("Hello, World!")
来源：http://tzv.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://qxu.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://mip.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ooo.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://tsy.ivvv.top

Go:   fmt.Println("Hello, World!")
来源：http://jso.bbcook.cn

Ruby: puts "Hello, World!"
来源：http://xcq.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qgz.redwolf501.top


<!-- 参考信息 -->