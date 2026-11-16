代发 wailian999

[U23] Py：分块读取大文件
来源：http://yzc.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zte.zhoulong.xyz

[U24] Py：路径操作
来源：http://tks.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cfd.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://ulu.c1oappe.top

csv.DictReader(f)
来源：http://ytq.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://oqc.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rnb.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://ncs.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://wqj.zhongyouzk.top

[U28] Py：类型别名
来源：http://ypu.fktsv.cn

UserId = int
来源：http://wsc.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://bbt.yj202588.top

@property 与 @x.setter 配合
来源：http://hgt.shzxlz.cn

[U30] Py：数据类
来源：http://jqe.daria6918.cn

@dataclass(slots=True)
来源：http://ubn.yueranfly.top

[U31] Py：单测
来源：http://xyb.kuanghao11.cn

python -m pytest -q
来源：http://ofc.snrcjt.cn

[U32] Py：代码格式化
来源：http://gps.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://wio.hywenlv.cn

[U33] Py：打包发布
来源：http://rlt.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://tms.vqdsnc.cn

[U34] Py：判断编码
来源：http://lfg.yj20258.top

chardet.detect(raw)
来源：http://upc.ydjk.org.cn

[U35] Py：发送邮件
来源：http://unp.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hqg.yanxiufei.cn

[U36] Py：定时任务
来源：http://rot.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://dua.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://udn.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tos.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://qvk.yonumen.top

Path(__file__).resolve().parent
来源：http://oop.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://ufj.nwbrower.top

sys.stdout.isatty()
来源：http://col.tian-w.cn

[U40] Py：打印到标准错误
来源：http://zgh.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://xgf.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://mrt.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zku.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://xxq.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qzn.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://vgz.tarul.cn

namespace App\Http;
来源：http://vjc.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://hmj.cqqwz.cn

declare(strict_types=1);
来源：http://wtn.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://gek.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tkj.guannengcc.top

[U46] PHP：可空类型
来源：http://pax.jqgufenzy.top

?string $name = null
来源：http://yzq.hammf.cn

[U47] PHP：联合类型
来源：http://ado.wangdashe.top

int|string $id
来源：http://ubp.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://dmq.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://udb.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://kak.zhiwuduotai.top

public readonly string $name
来源：http://lbz.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://xbi.daxiang520.top

public function __construct(private int $id) {}
来源：http://scs.haohaochexian.top

[U51] PHP：数组解构
来源：http://tog.yfazqb.com

[$a, $b] = $arr;
来源：http://fye.svipenyu.cn

[U52] PHP：箭头函数
来源：http://qkl.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://sdt.yueranfly.top

[U53] PHP：空合并运算符
来源：http://zuz.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://qdm.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://vkj.jiagoushi.top

$obj?->method()
来源：http://kcj.guannengcc.top

[U55] PHP：match 表达式
来源：http://qdi.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://toj.hysaishi.cn

[U56] PHP：命名参数
来源：http://ndo.tianlin.xyz

f(a: 1, b: 2)
来源：http://hcl.ctjpmb.com

[U57] PHP：字符串插值
来源：http://pfq.zhiwuduotai.top

"值: {$a}"
来源：http://gei.birdmap.top

[U58] PHP：数组三件套
来源：http://zdg.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ozp.ivvv.top

[U59] PHP：自定义排序
来源：http://cgz.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yog.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://iey.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qpc.shangyingyoupin.top

[U61] PHP：正则
来源：http://wzn.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gkh.gogol.net.cn

[U62] PHP：日期对象
来源：http://uad.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mzy.zdbjq.cn

[U63] PHP：文件读写
来源：http://djk.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ffl.hesvh.cn

[U64] PHP：目录遍历
来源：http://cau.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://npy.yangfankeji.com

[U65] PHP：会话
来源：http://htr.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kqf.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://tib.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gmw.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://dts.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://puv.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://moi.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xzd.yj202588.top

[U69] PHP：PDO 预处理
来源：http://mlt.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wyx.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://odu.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjc.yongpay.top

[U71] PHP：抛出异常
来源：http://rtm.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://gbf.iojbl.cn

[U72] PHP：写错误日志
来源：http://vwe.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://sia.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://xkd.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://zmm.52xcode.cn

[U74] PHP：读取环境变量
来源：http://zqy.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://iel.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://jzt.gotoacloud.top

composer require psr/container
来源：http://zlj.nwbrower.top

[U76] PHP：简单路由
来源：http://bxj.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://izj.gogol.net.cn

[U77] PHP：模板渲染
来源：http://ocw.shanyushiyangtech.top

composer require twig/twig
来源：http://jja.yj20258.top

[U78] PHP：单元测试
来源：http://pss.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://mez.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://nyg.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://xek.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://obb.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mku.yonumen.top

[U81] JS：初始化项目
来源：http://odj.jqgfzy.top

npm init -y;  npm i express
来源：http://vdu.iojbl.cn

[U82] JS：package.json 脚本
来源：http://vgv.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cww.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://lhy.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://csb.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://zrj.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://msh.vqdsnc.cn

[U85] JS：可选链
来源：http://twe.hywenlv.cn

a?.b?.c
来源：http://lne.cashguo.top

[U86] JS：空值合并
来源：http://fpq.ctjpmb.com

a ?? b
来源：http://nnw.fzhhl.top

[U87] JS：解构默认值
来源：http://lpp.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://ryz.yj202588.top

[U88] JS：对象展开合并
来源：http://pyk.yj202588.top

{ ...a, ...b }
来源：http://lfg.0kj1m.cn

[U89] JS：数组去重
来源：http://mfm.ivvv.top

[...new Set(arr)]
来源：http://jxh.yfazqb.com

[U90] JS：数字数组排序
来源：http://mvq.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://qeg.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://knn.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sgl.ivvv.top

[U92] JS：深拷贝
来源：http://ohf.guowangkeji.top

structuredClone(obj)
来源：http://qeq.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://idr.svipenyu.cn

`共 ${n} 条`
来源：http://wat.nanxinkj.top

[U94] JS：箭头函数
来源：http://kmz.yj20258.top

const double = x => x * 2;
来源：http://rxx.cdnleiting.top

[U95] JS：Promise 包装
来源：http://nwy.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://ygc.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://yyn.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dkg.chenzaomai.com

[U97] JS：并发请求
来源：http://mzz.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://fnd.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://gph.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://goo.hesvh.cn

[U99] JS：事件监听
来源：http://dea.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://vpe.dashuyun.cn

[U100] JS：DOM 查询
来源：http://hmi.svipenyu.cn

document.querySelector(".item")
来源：http://vby.zdbjq.cn

[U101] JS：classList 操作
来源：http://huy.chenjidiqi.icu

el.classList.toggle("active")
来源：http://uyq.tianlin.xyz

[U102] JS：本地存储
来源：http://qwf.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rxo.feifeiyinyue.top

[U103] JS：定时器
来源：http://jij.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://coq.hammf.cn

[U104] JS：防抖
来源：http://mgm.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxb.sysykeji.top

[U105] JS：节流
来源：http://pab.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ztl.bbcook.cn

[U106] JS：日期格式化
来源：http://dtv.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wxn.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://pka.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ons.gzhubu.top

[U108] JS：随机整数
来源：http://yaz.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lnf.mhx1999.top

[U109] JS：数组分组
来源：http://hwm.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://wzn.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://dcw.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://krb.jianghu66.top

[U111] JS：对象转 Map
来源：http://xhp.ctjpmb.com

new Map(Object.entries(obj))
来源：http://viy.cqqwz.cn

[U112] JS：字符串补位
来源：http://rps.xziqi.cn

"7".padStart(3, "0")
来源：http://plj.bbcook.cn

[U113] JS：正则替换全部
来源：http://jwo.xinyue.icu

s.replaceAll("a", "b")
来源：http://nud.yvedp.cn

[U114] JS：JSON 深比较
来源：http://apb.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zon.svipenyu.cn

[U115] JS：生成 UUID
来源：http://hak.bjfxy.top

crypto.randomUUID()
来源：http://ink.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://mpn.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://ayj.0kj1m.cn

[U117] JS：单元测试
来源：http://tee.hammf.cn

npm i -D vitest;  npx vitest
来源：http://fms.sjlbkw.cn

[U118] JS：开发服务器
来源：http://zey.jinqigufen.top

npm i -D vite;  npx vite
来源：http://yny.yj202588.top

[U119] JS：生产构建
来源：http://sha.hongshengwenyu.top

npx vite build
来源：http://qgc.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://qpj.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://cfo.jinghuilouyu.cn

================================================================================
来源：http://jtj.andypj.xyz

统计汇总
来源：http://ahj.haohaochexian.top

================================================================================
来源：http://luq.mhx1999.top

按语言统计（条）：
来源：http://tok.yanxiufei.cn

Python ......... 252
来源：http://fon.guannengcc.top

PHP ............ 252
来源：http://dho.yanxiufei.cn

JavaScript ..... 252
来源：http://idf.bbcook.cn

TypeScript ..... 212
来源：http://urf.tarul.cn

Java ........... 212
来源：http://utu.zhijiandao.cn

Go ............. 212
来源：http://vjo.daria6918.cn

Ruby ........... 212
来源：http://mkf.chenzaomai.com

C# ............. 212
来源：http://biq.ivvv.top

C .............. 30
来源：http://dvv.aizwys.cn

C++ ............ 30
来源：http://stx.chenlongwang.top

SQL ............ 90
来源：http://mtk.ydjk.org.cn

Bash ........... 80
来源：http://fki.9152youxi.cn

Kotlin ......... 15
来源：http://doi.hfpthk.cn

Swift .......... 15
来源：http://pof.yj20258888.top

Lua ............ 10
来源：http://yqe.jinyuanbaomall.cn

Perl ........... 10
来源：http://mju.zhoulong.xyz

Scala .......... 10
来源：http://ffv.haohaochexian.top

------------------------------------
来源：http://ikb.yanxiufei.cn

合计 ........... 2106 条
来源：http://tog.wangdashe.top

按章节统计：
来源：http://dlk.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hfg.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://epn.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fnf.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tca.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://odx.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://omk.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ikf.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://apv.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tgx.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yvo.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gdt.hesvh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wxo.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hrl.316326.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vnb.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qym.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fbr.ydzc1.top

Q SQL 专题                              90
来源：http://sch.ehwqpu.com

R Bash 专题                             80
来源：http://swj.316326.xyz

S C / C++ 专题                          60
来源：http://ubz.nwbrower.top

T 其他语言补充                          60
来源：http://lwv.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://nnn.shuidangran.top

------------------------------------
来源：http://hfs.cashguo.top

合计                                  2106 条
来源：http://fiw.yj20258.top

--------------------------------------------------------------------------------
来源：http://zir.hongshengwenyu.top

使用提醒
来源：http://gid.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://fmo.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gsl.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dfc.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xur.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qew.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ywa.chenlongwang.top

—— 文件结束 ——
来源：http://msy.hcnkem.com

================================================================================
来源：http://eqv.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://jff.mhx1999.top

Common Programming Examples Cheat Book
来源：http://xlp.jinqigufen.top

================================================================================
来源：http://fsm.cdnleiting.top

【收录内容】
来源：http://wxj.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pev.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ctt.zdqjudy.top

SQL · Bash · C · C++
来源：http://oer.zhijiandao.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lio.cucudq.cn

【使用说明】
来源：http://qcv.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hrm.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ibs.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fqi.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blu.shanyushiyangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yhl.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ext.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vss.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zxd.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tro.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rck.ybcxt.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gnz.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://diu.aizwys.cn

【文件统计】
来源：http://xav.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sss.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://djr.jqgfzy.top

目  录
来源：http://ihp.hesvh.cn

--------------------------------------------------------------------------------
来源：http://uta.fanxiaobao.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fph.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fdb.yangfankeji.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kmc.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://krx.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aqg.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hvn.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uxh.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uwd.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jpg.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://byc.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pqq.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rel.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kdm.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pqc.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jvd.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rgg.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mam.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xyo.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oae.fzhhl.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hdk.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zbe.aizwys.cn


<!-- 参考信息 -->