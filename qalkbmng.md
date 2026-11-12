代发 wailian999

[U27] Py：异步 HTTP
来源：http://csg.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://jjz.zdqjudy.top

[U28] Py：类型别名
来源：http://jjn.yanxiufei.cn

UserId = int
来源：http://jcr.fengsongda.top

[U29] Py：属性校验
来源：http://ybd.fehbvm.com

@property 与 @x.setter 配合
来源：http://qyt.gzhubu.top

[U30] Py：数据类
来源：http://owh.0kj1m.cn

@dataclass(slots=True)
来源：http://kxs.yj20258888.top

[U31] Py：单测
来源：http://wxx.jianghu66.top

python -m pytest -q
来源：http://eyr.vehdjk.com

[U32] Py：代码格式化
来源：http://lhk.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://taj.hfpthk.cn

[U33] Py：打包发布
来源：http://smb.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://ego.shangyingyoupin.top

[U34] Py：判断编码
来源：http://xzl.birdmap.top

chardet.detect(raw)
来源：http://kzd.yj202588.top

[U35] Py：发送邮件
来源：http://tbf.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kdv.nanxuanxn.top

[U36] Py：定时任务
来源：http://pnl.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://twv.smart0.xyz

[U37] Py：读写 Excel
来源：http://kkj.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yog.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://tlq.hesvh.cn

Path(__file__).resolve().parent
来源：http://zdd.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://rfz.guowangkeji.top

sys.stdout.isatty()
来源：http://aag.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://tqx.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://riu.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://jfa.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://wgg.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://mjd.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://met.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://yle.kuanghao11.cn

namespace App\Http;
来源：http://xbx.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://cmt.gaohongyu789.top

declare(strict_types=1);
来源：http://qpw.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://ybv.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ouc.yfazqb.com

[U46] PHP：可空类型
来源：http://imv.nanxinkj.top

?string $name = null
来源：http://bwn.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://cau.guowangkeji.top

int|string $id
来源：http://aum.52xcode.cn

[U48] PHP：纯枚举
来源：http://bva.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yjw.uphjek.com

[U49] PHP：只读属性
来源：http://fpc.yuanzhike.top

public readonly string $name
来源：http://vjg.tarul.cn

[U50] PHP：构造器属性提升
来源：http://hus.guannengcc.top

public function __construct(private int $id) {}
来源：http://gnt.chenlongwang.top

[U51] PHP：数组解构
来源：http://lnj.vehdjk.com

[$a, $b] = $arr;
来源：http://wqh.aibaodan.cn

[U52] PHP：箭头函数
来源：http://ccx.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://lbl.daxiang520.top

[U53] PHP：空合并运算符
来源：http://fgu.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://ple.c1oappe.top

[U54] PHP：空安全调用
来源：http://ilo.jyoumei.cn

$obj?->method()
来源：http://hsi.wangdashe.top

[U55] PHP：match 表达式
来源：http://dxa.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iqu.zdqjudy.top

[U56] PHP：命名参数
来源：http://tgl.sufxvd.cn

f(a: 1, b: 2)
来源：http://vgw.gotoacloud.top

[U57] PHP：字符串插值
来源：http://dfl.tarul.cn

"值: {$a}"
来源：http://kwt.cqqwz.cn

[U58] PHP：数组三件套
来源：http://tbr.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yel.jinqigufen.top

[U59] PHP：自定义排序
来源：http://qbz.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oqw.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://bru.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://umk.ydjk.org.cn

[U61] PHP：正则
来源：http://dre.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ffv.tianlin.xyz

[U62] PHP：日期对象
来源：http://lxp.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://thv.aibaodan.cn

[U63] PHP：文件读写
来源：http://uqf.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ajy.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://igm.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://rnp.zhijiandao.cn

[U65] PHP：会话
来源：http://bmb.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://drk.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://rwd.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ecw.sxryk.cn

[U67] PHP：处理文件上传
来源：http://vuk.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bea.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://ilk.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ejs.birdmap.top

[U69] PHP：PDO 预处理
来源：http://cpo.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kdg.epnwcf.com

[U70] PHP：PDO 事务
来源：http://vht.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zcb.shuidangran.top

[U71] PHP：抛出异常
来源：http://aex.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://bkm.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://xpc.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://xzp.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://kqb.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://uln.aibaodan.cn

[U74] PHP：读取环境变量
来源：http://dht.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://ikv.uphjek.com

[U75] PHP：依赖注入
来源：http://xnt.ydzc1.top

composer require psr/container
来源：http://llo.jinqigufen.top

[U76] PHP：简单路由
来源：http://mks.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vzs.xziqi.cn

[U77] PHP：模板渲染
来源：http://dlv.zycfv.cn

composer require twig/twig
来源：http://wbk.fzhhl.top

[U78] PHP：单元测试
来源：http://xcc.sweek.top

composer require --dev phpunit/phpunit
来源：http://ueq.yvedp.cn

[U79] PHP：静态分析
来源：http://wtb.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://tog.tarul.cn

[U80] PHP：代码规范修复
来源：http://bkv.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://knm.birdmap.top

[U81] JS：初始化项目
来源：http://ebl.0kj1m.cn

npm init -y;  npm i express
来源：http://ame.shuidangran.top

[U82] JS：package.json 脚本
来源：http://pqd.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gvn.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://bkx.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://xcm.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://rof.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://paq.cucudq.cn

[U85] JS：可选链
来源：http://yyv.quarkkingdee.top

a?.b?.c
来源：http://xhy.dianchejie.cn

[U86] JS：空值合并
来源：http://hjw.haohaochexian.top

a ?? b
来源：http://vhe.tarul.cn

[U87] JS：解构默认值
来源：http://qlj.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://now.jqgufenzy.top

[U88] JS：对象展开合并
来源：http://rpc.chenjidiqi.icu

{ ...a, ...b }
来源：http://vyr.cucudq.cn

[U89] JS：数组去重
来源：http://azf.hongshengwenyu.top

[...new Set(arr)]
来源：http://boh.hnqzz.top

[U90] JS：数字数组排序
来源：http://vpj.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://ljt.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://amn.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tad.jqgufenzy.top

[U92] JS：深拷贝
来源：http://cwp.snrcjt.cn

structuredClone(obj)
来源：http://reu.yongpay.top

[U93] JS：模板字符串
来源：http://zul.aibaodan.cn

`共 ${n} 条`
来源：http://ffv.hysaishi.cn

[U94] JS：箭头函数
来源：http://rwo.mhx1999.top

const double = x => x * 2;
来源：http://fzd.hcnkem.com

[U95] JS：Promise 包装
来源：http://lqr.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://riv.yueranfly.top

[U96] JS：async/await 与异常
来源：http://jcs.hcnkem.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vdf.gotoacloud.top

[U97] JS：并发请求
来源：http://lla.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://blo.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://byu.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cbw.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://how.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://bmg.yfazqb.com

[U100] JS：DOM 查询
来源：http://lqi.sysykeji.top

document.querySelector(".item")
来源：http://vjf.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://fkb.kuanghao11.cn

el.classList.toggle("active")
来源：http://hcg.ehwqpu.com

[U102] JS：本地存储
来源：http://vve.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pmj.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://wsr.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://myl.jinghuilouyu.cn

[U104] JS：防抖
来源：http://xpz.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgb.gaohongyu789.top

[U105] JS：节流
来源：http://bce.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hin.zhijiandao.cn

[U106] JS：日期格式化
来源：http://ieq.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qhj.gotoacloud.top

[U107] JS：数字千分位
来源：http://fnw.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rtu.jyoumei.cn

[U108] JS：随机整数
来源：http://zio.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ioy.316326.xyz

[U109] JS：数组分组
来源：http://ebo.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://ekm.vehdjk.com

[U110] JS：数组分块
来源：http://mae.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ldg.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://ogn.svipenyu.cn

new Map(Object.entries(obj))
来源：http://ubd.chenlongwang.top

[U112] JS：字符串补位
来源：http://evs.gotoacloud.top

"7".padStart(3, "0")
来源：http://pea.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://bph.shuidangran.top

s.replaceAll("a", "b")
来源：http://cut.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://shp.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mrl.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://col.jinqigfzy.top

crypto.randomUUID()
来源：http://agr.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://pqt.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://crb.52xcode.cn

[U117] JS：单元测试
来源：http://pxy.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://gow.dashuyun.cn

[U118] JS：开发服务器
来源：http://dsa.sxryk.cn

npm i -D vite;  npx vite
来源：http://rkj.pengpengdd.cyou

[U119] JS：生产构建
来源：http://osx.fktsv.cn

npx vite build
来源：http://rvz.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://wpa.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://zck.iojbl.cn

================================================================================
来源：http://ayj.xziqi.cn

统计汇总
来源：http://jig.jianghu66.top

================================================================================
来源：http://iwg.gogol.net.cn

按语言统计（条）：
来源：http://xzb.ctjpmb.com

Python ......... 252
来源：http://wqd.shanyushiyangtech.top

PHP ............ 252
来源：http://aai.jlsjyb.cn

JavaScript ..... 252
来源：http://hqi.zdbjq.cn

TypeScript ..... 212
来源：http://scp.yongpay.top

Java ........... 212
来源：http://xqh.hywenlv.cn

Go ............. 212
来源：http://mep.zhixingplan.top

Ruby ........... 212
来源：http://blk.52xcode.cn

C# ............. 212
来源：http://fpf.uphjek.com

C .............. 30
来源：http://sgf.yangfankeji.com

C++ ............ 30
来源：http://oxd.zdbjq.cn

SQL ............ 90
来源：http://dkr.zhengqikj.top

Bash ........... 80
来源：http://jio.gogol.net.cn

Kotlin ......... 15
来源：http://kjz.hesvh.cn

Swift .......... 15
来源：http://wpm.ehwqpu.com

Lua ............ 10
来源：http://mym.yuxming.cn

Perl ........... 10
来源：http://gnp.0kj1m.cn

Scala .......... 10
来源：http://pgn.fktsv.cn

------------------------------------
来源：http://ler.yfazqb.com

合计 ........... 2106 条
来源：http://npl.ybcxt.top

按章节统计：
来源：http://oam.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xrh.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tqn.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ugh.cheryme.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kpi.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uer.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kpg.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dlv.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zoa.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://frs.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eag.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gnw.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yoa.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dlz.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jtu.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ykd.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://auk.fehbvm.com

Q SQL 专题                              90
来源：http://gtd.bjfxy.top

R Bash 专题                             80
来源：http://mrx.jqgfzy.top

S C / C++ 专题                          60
来源：http://nne.jqgfzy.top

T 其他语言补充                          60
来源：http://sld.birdmap.top

U 高频实用片段                         120
来源：http://wcc.svipenyu.cn

------------------------------------
来源：http://och.tian-w.cn

合计                                  2106 条
来源：http://jax.cucudq.cn

--------------------------------------------------------------------------------
来源：http://kxl.vehdjk.com

使用提醒
来源：http://fjm.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://ksp.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vsq.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bww.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pnn.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://zva.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hxy.nanxuanxn.top

—— 文件结束 ——
来源：http://ukp.ehwqpu.com

================================================================================
来源：http://qul.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://ogb.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://xyf.shanyushiyangtech.top

================================================================================
来源：http://wya.tianlin.xyz

【收录内容】
来源：http://tiw.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kyr.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://stz.dashuyun.cn

SQL · Bash · C · C++
来源：http://ikf.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tzt.shzxlz.cn

【使用说明】
来源：http://zga.sxryk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://siz.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uce.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jqu.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ltp.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wmj.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nlh.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zfk.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tcy.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rcq.yvedp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ffy.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fpv.gotoacloud.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ego.jlsjyb.cn

【文件统计】
来源：http://fok.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gys.bbcook.cn

--------------------------------------------------------------------------------
来源：http://sez.ywan-chungtsiang.top

目  录
来源：http://lrw.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://tru.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uog.yvedp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ibl.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ncz.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tfs.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blg.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ztq.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cbu.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://czm.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nvj.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://afe.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vxr.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xlj.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xzj.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uhg.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cco.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gzr.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vwb.zhixingplan.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sde.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wxt.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uom.havefunace.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zvm.zhengqikj.top

================================================================================
来源：http://euw.xziqi.cn

A. 基础语法与类型
来源：http://ygv.hysaishi.cn

================================================================================
来源：http://bww.zhongyouzk.top

[A01] Hello World
来源：http://bao.zdbjq.cn

Py:   print("Hello, World!")
来源：http://sgh.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://kkr.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://uev.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ojx.shzxlz.cn


<!-- 参考信息 -->