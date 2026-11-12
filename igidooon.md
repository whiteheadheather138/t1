代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://mwb.nanxuanxn.top

@contextlib.contextmanager
来源：http://mrs.bbcook.cn

[U22] Py：矩阵转置
来源：http://xix.sweek.top

list(zip(*m))
来源：http://snc.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://pcy.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://geh.jianghu66.top

[U24] Py：路径操作
来源：http://nce.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zyv.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://zep.yangfankeji.com

csv.DictReader(f)
来源：http://rca.daxiang520.top

[U26] Py：并发下载
来源：http://yjd.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ibx.xziqi.cn

[U27] Py：异步 HTTP
来源：http://pui.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://wcz.wangshuangyany.cn

[U28] Py：类型别名
来源：http://wfq.yonumen.top

UserId = int
来源：http://ezv.xuetiantiany.cn

[U29] Py：属性校验
来源：http://emg.tianlin.xyz

@property 与 @x.setter 配合
来源：http://tsc.xuanzx.com

[U30] Py：数据类
来源：http://cgr.hesvh.cn

@dataclass(slots=True)
来源：http://fbn.zhengqikj.top

[U31] Py：单测
来源：http://ulr.uphjek.com

python -m pytest -q
来源：http://kng.hnxiangtu.top

[U32] Py：代码格式化
来源：http://zyt.sxryk.cn

ruff format . && ruff check --fix .
来源：http://hbl.hysaishi.cn

[U33] Py：打包发布
来源：http://las.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://klj.epnwcf.com

[U34] Py：判断编码
来源：http://tpt.yangfankeji.com

chardet.detect(raw)
来源：http://qav.vehdjk.com

[U35] Py：发送邮件
来源：http://ouv.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vqe.zhengqikj.top

[U36] Py：定时任务
来源：http://gnw.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://obi.hongshengwenyu.top

[U37] Py：读写 Excel
来源：http://srz.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://vvn.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://ytb.hesvh.cn

Path(__file__).resolve().parent
来源：http://hfg.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://qcu.hnxiangtu.top

sys.stdout.isatty()
来源：http://auo.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://paz.shuidangran.top

print("err", file=sys.stderr)
来源：http://uwk.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://fpf.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jnl.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://caj.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://clh.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://opz.kuanghao11.cn

namespace App\Http;
来源：http://bjy.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://qtw.xinyue.icu

declare(strict_types=1);
来源：http://xke.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://ioq.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bpz.sweek.top

[U46] PHP：可空类型
来源：http://aec.fzhhl.top

?string $name = null
来源：http://gxb.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://exc.jiagoushi.top

int|string $id
来源：http://uxf.52xcode.cn

[U48] PHP：纯枚举
来源：http://jwh.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aah.yuxming.cn

[U49] PHP：只读属性
来源：http://xqb.0kj1m.cn

public readonly string $name
来源：http://ucn.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://ljr.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://ziu.yangfankeji.com

[U51] PHP：数组解构
来源：http://vdz.c1oappe.top

[$a, $b] = $arr;
来源：http://nys.snrcjt.cn

[U52] PHP：箭头函数
来源：http://brt.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://oat.c1oappe.top

[U53] PHP：空合并运算符
来源：http://cid.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://ayt.316326.xyz

[U54] PHP：空安全调用
来源：http://dyf.xinyue.icu

$obj?->method()
来源：http://gsi.cucudq.cn

[U55] PHP：match 表达式
来源：http://yoe.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bqy.dashuyun.cn

[U56] PHP：命名参数
来源：http://lyn.sweek.top

f(a: 1, b: 2)
来源：http://zbc.haohaochexian.top

[U57] PHP：字符串插值
来源：http://hqi.hesvh.cn

"值: {$a}"
来源：http://ssq.zhixingplan.top

[U58] PHP：数组三件套
来源：http://usf.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ibv.fengsongda.top

[U59] PHP：自定义排序
来源：http://sxz.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twn.ivvv.top

[U60] PHP：JSON 编解码
来源：http://lng.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lfu.hesvh.cn

[U61] PHP：正则
来源：http://kci.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ovy.yj202588.top

[U62] PHP：日期对象
来源：http://hxf.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zav.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://ack.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tsu.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://pwr.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://evg.smart0.xyz

[U65] PHP：会话
来源：http://uwp.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://spa.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://ajp.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wkq.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://fzs.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pbh.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://guj.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yyu.tanke756.top

[U69] PHP：PDO 预处理
来源：http://tjs.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jak.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://ikf.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gow.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://grt.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://lin.sufxvd.cn

[U72] PHP：写错误日志
来源：http://utz.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://tha.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://hut.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://wkf.epnwcf.com

[U74] PHP：读取环境变量
来源：http://mma.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://mng.meibo888.top

[U75] PHP：依赖注入
来源：http://eqp.zhijiandao.cn

composer require psr/container
来源：http://cqz.sxryk.cn

[U76] PHP：简单路由
来源：http://xoc.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zlv.cheryme.top

[U77] PHP：模板渲染
来源：http://qoj.zhengqikj.top

composer require twig/twig
来源：http://vfy.fengsongda.top

[U78] PHP：单元测试
来源：http://idf.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://bjk.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://rnr.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://jjz.wangdashe.top

[U80] PHP：代码规范修复
来源：http://nuy.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://igi.fehbvm.com

[U81] JS：初始化项目
来源：http://tji.mhx1999.top

npm init -y;  npm i express
来源：http://dzf.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://ikz.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ctx.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://hag.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xao.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://sxn.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qbm.cqqwz.cn

[U85] JS：可选链
来源：http://rdz.fanxiaobao.xyz

a?.b?.c
来源：http://sey.ydjk.org.cn

[U86] JS：空值合并
来源：http://eew.zhiwuduotai.top

a ?? b
来源：http://xyy.smart0.xyz

[U87] JS：解构默认值
来源：http://jrg.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://cmk.pycfn.com

[U88] JS：对象展开合并
来源：http://hyj.meibo888.top

{ ...a, ...b }
来源：http://dtu.cashguo.top

[U89] JS：数组去重
来源：http://vpq.sufxvd.cn

[...new Set(arr)]
来源：http://neo.fzhhl.top

[U90] JS：数字数组排序
来源：http://yxz.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://pif.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://ahh.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tff.pycfn.com

[U92] JS：深拷贝
来源：http://hcs.xziqi.cn

structuredClone(obj)
来源：http://yml.aibaodan.cn

[U93] JS：模板字符串
来源：http://paq.hnxiangtu.top

`共 ${n} 条`
来源：http://rfy.wangdashe.top

[U94] JS：箭头函数
来源：http://jls.jqgufenzy.top

const double = x => x * 2;
来源：http://wsh.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://fzi.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://hci.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://hqk.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gns.ehwqpu.com

[U97] JS：并发请求
来源：http://gva.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ckq.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://gdu.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fkn.yvedp.cn

[U99] JS：事件监听
来源：http://xda.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://fbn.xziqi.cn

[U100] JS：DOM 查询
来源：http://crn.birdmap.top

document.querySelector(".item")
来源：http://hvi.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://xcu.hongshengwenyu.top

el.classList.toggle("active")
来源：http://bey.ydjk.org.cn

[U102] JS：本地存储
来源：http://nzy.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://unh.fzhhl.top

[U103] JS：定时器
来源：http://ylm.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lkr.sxryk.cn

[U104] JS：防抖
来源：http://hxj.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yrw.wangshuangyany.cn

[U105] JS：节流
来源：http://lry.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rsl.yonumen.top

[U106] JS：日期格式化
来源：http://uin.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oql.bjfxy.top

[U107] JS：数字千分位
来源：http://smc.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xvn.cashguo.top

[U108] JS：随机整数
来源：http://qlz.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xqo.tanke756.top

[U109] JS：数组分组
来源：http://tbj.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://jig.fktsv.cn

[U110] JS：数组分块
来源：http://xoa.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uid.sysykeji.top

[U111] JS：对象转 Map
来源：http://hbx.sxryk.cn

new Map(Object.entries(obj))
来源：http://qab.guannengcc.top

[U112] JS：字符串补位
来源：http://vzu.andypj.xyz

"7".padStart(3, "0")
来源：http://cbv.hcnkem.com

[U113] JS：正则替换全部
来源：http://owq.hesvh.cn

s.replaceAll("a", "b")
来源：http://hjm.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://qjl.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://duj.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://psy.gotoacloud.top

crypto.randomUUID()
来源：http://mex.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://vsw.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://qxx.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://bnj.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://kfk.xuanzx.com

[U118] JS：开发服务器
来源：http://nss.fzhhl.top

npm i -D vite;  npx vite
来源：http://ubz.fehbvm.com

[U119] JS：生产构建
来源：http://bca.gaohongyu789.top

npx vite build
来源：http://mox.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://stz.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://ypr.jiagoushi.top

================================================================================
来源：http://epa.xingfuxueyuan.xyz

统计汇总
来源：http://fym.c1oappe.top

================================================================================
来源：http://aug.zhaomingkeji.xyz

按语言统计（条）：
来源：http://gyr.xziqi.cn

Python ......... 252
来源：http://bfe.jinqigfzy.top

PHP ............ 252
来源：http://rod.guowangkeji.top

JavaScript ..... 252
来源：http://syu.chenzaomai.com

TypeScript ..... 212
来源：http://xzy.shuidangran.top

Java ........... 212
来源：http://ccj.zycfv.cn

Go ............. 212
来源：http://utr.shanyushiyangtech.top

Ruby ........... 212
来源：http://bxu.gogol.net.cn

C# ............. 212
来源：http://vqd.zhaomingkeji.xyz

C .............. 30
来源：http://pyu.kuanghao11.cn

C++ ............ 30
来源：http://bhe.shuidangran.top

SQL ............ 90
来源：http://deq.mhx1999.top

Bash ........... 80
来源：http://nhm.hfpthk.cn

Kotlin ......... 15
来源：http://wgk.svipenyu.cn

Swift .......... 15
来源：http://feo.hysaishi.cn

Lua ............ 10
来源：http://uzx.ctjpmb.com

Perl ........... 10
来源：http://grz.hfpthk.cn

Scala .......... 10
来源：http://tfw.tianlin.xyz

------------------------------------
来源：http://zhi.jqgufenzy.top

合计 ........... 2106 条
来源：http://rxh.bjfxy.top

按章节统计：
来源：http://fog.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qkd.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cya.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qyw.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mbv.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rpc.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qqs.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jze.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qyi.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mxv.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rwj.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://huv.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iae.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pix.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rwx.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://axw.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://phk.fktsv.cn

Q SQL 专题                              90
来源：http://jas.ydjk.org.cn

R Bash 专题                             80
来源：http://bhj.epnwcf.com

S C / C++ 专题                          60
来源：http://wtp.sweek.top

T 其他语言补充                          60
来源：http://zeh.tanke756.top

U 高频实用片段                         120
来源：http://lil.tanke756.top

------------------------------------
来源：http://aaq.zhixingplan.top

合计                                  2106 条
来源：http://ffm.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://qiq.yonumen.top

使用提醒
来源：http://bhn.yueranfly.top

--------------------------------------------------------------------------------
来源：http://nry.ybcxt.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yyy.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nty.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rcw.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fow.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zva.shzxlz.cn

—— 文件结束 ——
来源：http://bbc.snrcjt.cn

================================================================================
来源：http://mfl.fktsv.cn

程序语言常见例子速查手册（2024 版）
来源：http://hdk.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://vqo.ybcxt.top

================================================================================
来源：http://rms.hesvh.cn

【收录内容】
来源：http://wvi.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://vyc.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nzl.zhoulong.xyz

SQL · Bash · C · C++
来源：http://ebu.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://byo.yfazqb.com

【使用说明】
来源：http://ylc.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hkh.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ccj.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dlz.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gse.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ylb.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pgc.xylfe.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mli.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://peg.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jlu.sysykeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://llr.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zpb.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yci.zhoulong.xyz

【文件统计】
来源：http://kdx.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nbm.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://fsf.haohaochexian.top

目  录
来源：http://mlq.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://fcm.fanxiaobao.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jnw.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sqc.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xrf.snrcjt.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rar.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xco.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yal.sufxvd.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fif.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ckt.snrcjt.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gcw.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xlw.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uba.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eyz.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://win.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mou.hcnkem.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dmn.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://myb.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gtg.shzxlz.cn


<!-- 参考信息 -->