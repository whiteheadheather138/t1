代发 wailian999

[U27] Py：异步 HTTP
来源：http://kmk.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://cgx.shuidangran.top

[U28] Py：类型别名
来源：http://pug.quarkkingdee.top

UserId = int
来源：http://utv.shzxlz.cn

[U29] Py：属性校验
来源：http://qrq.haohaochexian.top

@property 与 @x.setter 配合
来源：http://kpg.gaohongyu789.top

[U30] Py：数据类
来源：http://dta.pengpengdd.cyou

@dataclass(slots=True)
来源：http://lko.vqdsnc.cn

[U31] Py：单测
来源：http://pgt.hammf.cn

python -m pytest -q
来源：http://jap.guannengcc.top

[U32] Py：代码格式化
来源：http://pzp.zycfv.cn

ruff format . && ruff check --fix .
来源：http://ovd.hesvh.cn

[U33] Py：打包发布
来源：http://hye.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://rud.yfazqb.com

[U34] Py：判断编码
来源：http://xfm.hnxiangtu.top

chardet.detect(raw)
来源：http://tla.xuanzx.com

[U35] Py：发送邮件
来源：http://psm.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zju.guowangkeji.top

[U36] Py：定时任务
来源：http://aus.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://toy.bjfxy.top

[U37] Py：读写 Excel
来源：http://udj.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://cze.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://cvz.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://oic.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://tmp.9152youxi.cn

sys.stdout.isatty()
来源：http://tro.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://biu.jianghu66.top

print("err", file=sys.stderr)
来源：http://lna.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://tnj.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ayg.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://qnd.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rpi.tanke756.top

[U43] PHP：声明命名空间
来源：http://dwd.redwolf501.top

namespace App\Http;
来源：http://vip.hnqzz.top

[U44] PHP：开启严格类型
来源：http://tdd.shzxlz.cn

declare(strict_types=1);
来源：http://juw.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://eiq.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tro.smart0.xyz

[U46] PHP：可空类型
来源：http://qlb.fanxiaobao.xyz

?string $name = null
来源：http://uhy.cheryme.top

[U47] PHP：联合类型
来源：http://zft.sjlbkw.cn

int|string $id
来源：http://vuy.guannengcc.top

[U48] PHP：纯枚举
来源：http://sdk.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zmk.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://sax.xingfuxueyuan.xyz

public readonly string $name
来源：http://fda.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://lty.nanxinkj.top

public function __construct(private int $id) {}
来源：http://opx.zhongyouzk.top

[U51] PHP：数组解构
来源：http://qco.xuanzx.com

[$a, $b] = $arr;
来源：http://qlu.cashguo.top

[U52] PHP：箭头函数
来源：http://jyy.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://gvj.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://oqj.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://pdn.bjfxy.top

[U54] PHP：空安全调用
来源：http://iml.ivvv.top

$obj?->method()
来源：http://zcm.yangfankeji.com

[U55] PHP：match 表达式
来源：http://dcv.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ted.xylfe.cn

[U56] PHP：命名参数
来源：http://dsr.316326.xyz

f(a: 1, b: 2)
来源：http://thu.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://itq.ywan-chungtsiang.top

"值: {$a}"
来源：http://ctf.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://ifk.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://frt.hysaishi.cn

[U59] PHP：自定义排序
来源：http://ntb.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tkz.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://eft.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fni.daria6918.cn

[U61] PHP：正则
来源：http://yzy.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bzy.jlsjyb.cn

[U62] PHP：日期对象
来源：http://xnx.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lds.sweek.top

[U63] PHP：文件读写
来源：http://hlo.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gxy.guannengcc.top

[U64] PHP：目录遍历
来源：http://nvv.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://xoh.redwolf501.top

[U65] PHP：会话
来源：http://mwr.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://aya.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://mzx.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zqv.guannengcc.top

[U67] PHP：处理文件上传
来源：http://tvn.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zoo.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://eer.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://htj.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://hpf.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vln.sxryk.cn

[U70] PHP：PDO 事务
来源：http://jcx.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fjw.yuxming.cn

[U71] PHP：抛出异常
来源：http://jmi.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://ued.yj202588.top

[U72] PHP：写错误日志
来源：http://ybc.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://okp.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://dcc.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://fct.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://tso.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://miy.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://qij.cashguo.top

composer require psr/container
来源：http://ptt.gogol.net.cn

[U76] PHP：简单路由
来源：http://vtb.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hup.cucudq.cn

[U77] PHP：模板渲染
来源：http://gyj.nanxinkj.top

composer require twig/twig
来源：http://xxs.zdqjudy.top

[U78] PHP：单元测试
来源：http://rij.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://gby.yvedp.cn

[U79] PHP：静态分析
来源：http://zdn.yj20258.top

composer require --dev phpstan/phpstan
来源：http://zcu.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://byf.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iwz.316326.xyz

[U81] JS：初始化项目
来源：http://zzf.9152youxi.cn

npm init -y;  npm i express
来源：http://zct.hcnkem.com

[U82] JS：package.json 脚本
来源：http://sbx.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://izt.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://nxx.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://cit.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://ptr.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://dny.zdqjudy.top

[U85] JS：可选链
来源：http://qqi.jinqigufen.top

a?.b?.c
来源：http://jti.bjfxy.top

[U86] JS：空值合并
来源：http://bxk.andypj.xyz

a ?? b
来源：http://hpg.yonumen.top

[U87] JS：解构默认值
来源：http://guf.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://fto.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://lrh.fzhhl.top

{ ...a, ...b }
来源：http://xol.iojbl.cn

[U89] JS：数组去重
来源：http://uai.kuanghao11.cn

[...new Set(arr)]
来源：http://nns.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://kzl.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://ymi.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://cco.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ins.hysaishi.cn

[U92] JS：深拷贝
来源：http://sqh.fanxiaobao.xyz

structuredClone(obj)
来源：http://cgb.ydjk.org.cn

[U93] JS：模板字符串
来源：http://jbv.hnxiangtu.top

`共 ${n} 条`
来源：http://ukj.fehbvm.com

[U94] JS：箭头函数
来源：http://wmf.jinghuilouyu.cn

const double = x => x * 2;
来源：http://dyx.smart0.xyz

[U95] JS：Promise 包装
来源：http://sxd.cheryme.top

new Promise((resolve, reject) => {})
来源：http://ysx.meibo888.top

[U96] JS：async/await 与异常
来源：http://sen.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dkl.ehwqpu.com

[U97] JS：并发请求
来源：http://rqh.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cwb.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://slg.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yya.iojbl.cn

[U99] JS：事件监听
来源：http://gdb.yfazqb.com

el.addEventListener("click", e => {})
来源：http://huv.cqqwz.cn

[U100] JS：DOM 查询
来源：http://twq.sjlbkw.cn

document.querySelector(".item")
来源：http://poa.gotoacloud.top

[U101] JS：classList 操作
来源：http://gmr.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://uuh.tanke756.top

[U102] JS：本地存储
来源：http://jgq.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vgm.yvedp.cn

[U103] JS：定时器
来源：http://xsb.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pmj.tianlin.xyz

[U104] JS：防抖
来源：http://cnx.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbc.shangyingyoupin.top

[U105] JS：节流
来源：http://mve.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://byb.ehwqpu.com

[U106] JS：日期格式化
来源：http://ncf.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xcj.ydjk.org.cn

[U107] JS：数字千分位
来源：http://rnc.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ocb.52xcode.cn

[U108] JS：随机整数
来源：http://gsg.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://btu.yj20258.top

[U109] JS：数组分组
来源：http://swe.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://cbh.gzhubu.top

[U110] JS：数组分块
来源：http://hbc.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zso.nwbrower.top

[U111] JS：对象转 Map
来源：http://kxf.jqgfzy.top

new Map(Object.entries(obj))
来源：http://aug.chenlongwang.top

[U112] JS：字符串补位
来源：http://wex.jqgufenzy.top

"7".padStart(3, "0")
来源：http://jfm.iojbl.cn

[U113] JS：正则替换全部
来源：http://wcd.hcnkem.com

s.replaceAll("a", "b")
来源：http://exe.yj20258888.top

[U114] JS：JSON 深比较
来源：http://yst.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nen.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://ptr.iojbl.cn

crypto.randomUUID()
来源：http://nnk.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://hvo.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://suf.kuanghao11.cn

[U117] JS：单元测试
来源：http://tek.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://kpx.yanxiufei.cn

[U118] JS：开发服务器
来源：http://jza.jyoumei.cn

npm i -D vite;  npx vite
来源：http://njz.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://yjo.aibaodan.cn

npx vite build
来源：http://fyp.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://dho.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://irw.jianghu66.top

================================================================================
来源：http://sbh.guowangkeji.top

统计汇总
来源：http://alz.yonumen.top

================================================================================
来源：http://eni.jinqigfzy.top

按语言统计（条）：
来源：http://ggq.gogol.net.cn

Python ......... 252
来源：http://pir.jqgfzy.top

PHP ............ 252
来源：http://rcy.xinyue.icu

JavaScript ..... 252
来源：http://fbx.bjfxy.top

TypeScript ..... 212
来源：http://ygs.zdqjudy.top

Java ........... 212
来源：http://phn.xziqi.cn

Go ............. 212
来源：http://zun.daxiang520.top

Ruby ........... 212
来源：http://elx.jianghu66.top

C# ............. 212
来源：http://qqj.shanyushiyangtech.top

C .............. 30
来源：http://dbr.zhixingplan.top

C++ ............ 30
来源：http://gnr.xinyue.icu

SQL ............ 90
来源：http://jpt.fanxiaobao.xyz

Bash ........... 80
来源：http://ppx.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://duv.ehwqpu.com

Swift .......... 15
来源：http://yho.vqdsnc.cn

Lua ............ 10
来源：http://qhi.guowangkeji.top

Perl ........... 10
来源：http://kdd.shuidangran.top

Scala .......... 10
来源：http://ilf.zhixingplan.top

------------------------------------
来源：http://dbq.ehwqpu.com

合计 ........... 2106 条
来源：http://bqx.aibaodan.cn

按章节统计：
来源：http://ifx.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cww.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pda.hysaishi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dda.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lsn.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hef.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fik.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://drq.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mnx.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jrm.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zkp.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ipj.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ayd.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gsd.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zuo.yj20258.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hmk.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://osk.nanxinkj.top

Q SQL 专题                              90
来源：http://inu.uphjek.com

R Bash 专题                             80
来源：http://sww.nanxinkj.top

S C / C++ 专题                          60
来源：http://ftu.zycfv.cn

T 其他语言补充                          60
来源：http://ifw.haohaochexian.top

U 高频实用片段                         120
来源：http://pit.jqgfzy.top

------------------------------------
来源：http://jpt.yvedp.cn

合计                                  2106 条
来源：http://adc.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://cxy.pycfn.com

使用提醒
来源：http://rrq.yj20258.top

--------------------------------------------------------------------------------
来源：http://gez.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dsz.tarul.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rmx.ydjk.org.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gyr.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://faq.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nvw.shanyushiyangtech.top

—— 文件结束 ——
来源：http://vwf.9152youxi.cn

================================================================================
来源：http://jwn.xuanzx.com

程序语言常见例子速查手册（2024 版）
来源：http://aox.fehbvm.com

Common Programming Examples Cheat Book
来源：http://cch.316326.xyz

================================================================================
来源：http://hua.ybcxt.top

【收录内容】
来源：http://rmr.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zqq.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kco.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://yiu.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sbw.hnxiangtu.top

【使用说明】
来源：http://vph.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kwu.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fbi.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jeg.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sdp.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tfw.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lct.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://azr.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cpg.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hgl.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mtf.tian-w.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fia.hfpthk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mwz.cqqwz.cn

【文件统计】
来源：http://ekt.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cgi.hnqzz.top

--------------------------------------------------------------------------------
来源：http://hhb.aizwys.cn

目  录
来源：http://dyb.fehbvm.com

--------------------------------------------------------------------------------
来源：http://nll.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qzf.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wex.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xnp.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vdh.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://djt.pycfn.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tdj.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eka.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hxs.fehbvm.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kkq.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://muc.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vhb.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oif.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://czk.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zns.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ocs.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://szl.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oki.fengsongda.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://svs.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qnn.jiagoushi.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xwx.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://emg.hammf.cn

================================================================================
来源：http://wqd.chenjidiqi.icu

A. 基础语法与类型
来源：http://rqp.meibo888.top

================================================================================
来源：http://plc.cheryme.top

[A01] Hello World
来源：http://qqf.uphjek.com

Py:   print("Hello, World!")
来源：http://jml.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://vtc.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://nfo.xziqi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aet.epnwcf.com


<!-- 参考信息 -->