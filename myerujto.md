代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://krl.jlsjyb.cn

@contextlib.contextmanager
来源：http://cjf.jqgfzy.top

[U22] Py：矩阵转置
来源：http://wwf.havefunace.top

list(zip(*m))
来源：http://mnq.yueranfly.top

[U23] Py：分块读取大文件
来源：http://klq.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rlc.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://mqv.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://too.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://tjl.dashuyun.cn

csv.DictReader(f)
来源：http://luk.gaohongyu789.top

[U26] Py：并发下载
来源：http://our.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vja.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://rlp.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://oxp.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://lid.tian-w.cn

UserId = int
来源：http://jkt.yj20258888.top

[U29] Py：属性校验
来源：http://fqd.jqgfzy.top

@property 与 @x.setter 配合
来源：http://vtk.redwolf501.top

[U30] Py：数据类
来源：http://yyo.yongpay.top

@dataclass(slots=True)
来源：http://ljy.ywan-chungtsiang.top

[U31] Py：单测
来源：http://sbc.gotoacloud.top

python -m pytest -q
来源：http://stt.pycfn.com

[U32] Py：代码格式化
来源：http://rwj.andypj.xyz

ruff format . && ruff check --fix .
来源：http://mvq.jlsjyb.cn

[U33] Py：打包发布
来源：http://vuq.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://szg.gogol.net.cn

[U34] Py：判断编码
来源：http://tnk.meibo888.top

chardet.detect(raw)
来源：http://phx.ivvv.top

[U35] Py：发送邮件
来源：http://suy.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ahu.jianghu66.top

[U36] Py：定时任务
来源：http://wjr.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://pxk.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://zeh.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cdb.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://uyy.dianchejie.cn

Path(__file__).resolve().parent
来源：http://lys.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://dch.mhx1999.top

sys.stdout.isatty()
来源：http://uyw.jianghu66.top

[U40] Py：打印到标准错误
来源：http://gnd.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://oxl.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://ade.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://npe.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://uqm.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dwt.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://qkl.zdbjq.cn

namespace App\Http;
来源：http://rnb.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://qbk.yfazqb.com

declare(strict_types=1);
来源：http://zye.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://bik.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qmd.svipenyu.cn

[U46] PHP：可空类型
来源：http://qbf.bjfxy.top

?string $name = null
来源：http://lfz.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://gti.shangyingyoupin.top

int|string $id
来源：http://vle.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://irg.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://awn.fzhhl.top

[U49] PHP：只读属性
来源：http://euf.tianlin.xyz

public readonly string $name
来源：http://zhx.gzhubu.top

[U50] PHP：构造器属性提升
来源：http://yrm.zhixingplan.top

public function __construct(private int $id) {}
来源：http://ruy.cashguo.top

[U51] PHP：数组解构
来源：http://kjy.nwbrower.top

[$a, $b] = $arr;
来源：http://bvk.dashuyun.cn

[U52] PHP：箭头函数
来源：http://arf.cqqwz.cn

$double = fn($x) => $x * 2;
来源：http://nbi.xziqi.cn

[U53] PHP：空合并运算符
来源：http://dkc.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://dql.wangdashe.top

[U54] PHP：空安全调用
来源：http://yfd.9152youxi.cn

$obj?->method()
来源：http://rrl.cdnleiting.top

[U55] PHP：match 表达式
来源：http://rwn.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hkz.hcnkem.com

[U56] PHP：命名参数
来源：http://kld.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://mhe.cheryme.top

[U57] PHP：字符串插值
来源：http://ubr.yanxiufei.cn

"值: {$a}"
来源：http://mzj.sweek.top

[U58] PHP：数组三件套
来源：http://lzc.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ggt.wangdashe.top

[U59] PHP：自定义排序
来源：http://rhd.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gwv.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://lho.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gfo.daxiang520.top

[U61] PHP：正则
来源：http://imu.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ywk.sjlbkw.cn

[U62] PHP：日期对象
来源：http://rnb.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yhy.bjfxy.top

[U63] PHP：文件读写
来源：http://vrb.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wxo.shzxlz.cn

[U64] PHP：目录遍历
来源：http://nfx.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://gnc.gaohongyu789.top

[U65] PHP：会话
来源：http://zgj.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fer.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://lze.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bei.yfazqb.com

[U67] PHP：处理文件上传
来源：http://bmg.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://siu.gzhubu.top

[U68] PHP：PDO 连接
来源：http://diu.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gdk.pycfn.com

[U69] PHP：PDO 预处理
来源：http://qhc.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cwo.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://xbn.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ogv.hcnkem.com

[U71] PHP：抛出异常
来源：http://kav.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://myc.yvedp.cn

[U72] PHP：写错误日志
来源：http://oxx.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://nrx.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://jzw.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://ryx.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://whb.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://nwj.hfpthk.cn

[U75] PHP：依赖注入
来源：http://akj.yj20258888.top

composer require psr/container
来源：http://jhn.hammf.cn

[U76] PHP：简单路由
来源：http://hmi.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://epd.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://kbd.yueranfly.top

composer require twig/twig
来源：http://uyw.hcnkem.com

[U78] PHP：单元测试
来源：http://jar.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://tpc.iojbl.cn

[U79] PHP：静态分析
来源：http://qli.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://biw.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://aof.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ciy.xinyue.icu

[U81] JS：初始化项目
来源：http://qyq.aizwys.cn

npm init -y;  npm i express
来源：http://pqb.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://qay.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fpm.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://mwm.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gzb.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://qmq.zhijiandao.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ipf.svipenyu.cn

[U85] JS：可选链
来源：http://hrh.mhx1999.top

a?.b?.c
来源：http://gpn.hnqzz.top

[U86] JS：空值合并
来源：http://qfq.kuanghao11.cn

a ?? b
来源：http://diz.ctjpmb.com

[U87] JS：解构默认值
来源：http://lxl.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://zhq.haohaochexian.top

[U88] JS：对象展开合并
来源：http://xpl.hongshengwenyu.top

{ ...a, ...b }
来源：http://tzu.dashuyun.cn

[U89] JS：数组去重
来源：http://pjt.9152youxi.cn

[...new Set(arr)]
来源：http://ncp.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://aoo.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://ddi.yfazqb.com

[U91] JS：对象键值遍历
来源：http://jhu.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qwh.zhijiandao.cn

[U92] JS：深拷贝
来源：http://yfn.guannengcc.top

structuredClone(obj)
来源：http://ogi.chenlongwang.top

[U93] JS：模板字符串
来源：http://ghe.sxryk.cn

`共 ${n} 条`
来源：http://vfd.yvedp.cn

[U94] JS：箭头函数
来源：http://lgv.bjfxy.top

const double = x => x * 2;
来源：http://yrq.tanke756.top

[U95] JS：Promise 包装
来源：http://nau.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://jhy.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://zun.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ycb.yj20258888.top

[U97] JS：并发请求
来源：http://riv.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vmp.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://swt.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wbu.ehwqpu.com

[U99] JS：事件监听
来源：http://eko.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://xsu.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://opi.vqdsnc.cn

document.querySelector(".item")
来源：http://qhh.316326.xyz

[U101] JS：classList 操作
来源：http://rue.zhongyouzk.top

el.classList.toggle("active")
来源：http://lyq.ivvv.top

[U102] JS：本地存储
来源：http://hll.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://deq.ehwqpu.com

[U103] JS：定时器
来源：http://zal.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wyk.fktsv.cn

[U104] JS：防抖
来源：http://vae.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aym.xziqi.cn

[U105] JS：节流
来源：http://vac.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jlm.dianchejie.cn

[U106] JS：日期格式化
来源：http://kmm.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rzl.tian-w.cn

[U107] JS：数字千分位
来源：http://hqw.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://edz.gaohongyu789.top

[U108] JS：随机整数
来源：http://jqo.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ptf.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://jgz.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://hqm.hnqzz.top

[U110] JS：数组分块
来源：http://ugi.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wqd.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://tpv.ppjwa.cn

new Map(Object.entries(obj))
来源：http://cwh.fzhhl.top

[U112] JS：字符串补位
来源：http://yfw.jianghu66.top

"7".padStart(3, "0")
来源：http://kxa.uphjek.com

[U113] JS：正则替换全部
来源：http://lvy.dashuyun.cn

s.replaceAll("a", "b")
来源：http://brv.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://gus.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qwv.vehdjk.com

[U115] JS：生成 UUID
来源：http://naz.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://muz.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://kkt.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://cfu.zdbjq.cn

[U117] JS：单元测试
来源：http://oqb.tanke756.top

npm i -D vitest;  npx vitest
来源：http://mgb.fktsv.cn

[U118] JS：开发服务器
来源：http://blh.fzhhl.top

npm i -D vite;  npx vite
来源：http://kys.ydjk.org.cn

[U119] JS：生产构建
来源：http://ofh.cqqwz.cn

npx vite build
来源：http://asr.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://oks.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://yyp.0kj1m.cn

================================================================================
来源：http://zof.zhongyouzk.top

统计汇总
来源：http://won.jqgufenzy.top

================================================================================
来源：http://jvw.yanxiufei.cn

按语言统计（条）：
来源：http://gyk.pengpengdd.cyou

Python ......... 252
来源：http://zbu.sweek.top

PHP ............ 252
来源：http://cqe.svipenyu.cn

JavaScript ..... 252
来源：http://ezf.yj20258.top

TypeScript ..... 212
来源：http://xsx.ydjk.org.cn

Java ........... 212
来源：http://maz.tarul.cn

Go ............. 212
来源：http://lvi.9152youxi.cn

Ruby ........... 212
来源：http://tnl.shanyushiyangkeji.top

C# ............. 212
来源：http://ggy.zhijiandao.cn

C .............. 30
来源：http://kjl.cucudq.cn

C++ ............ 30
来源：http://kqb.zhiwuduotai.top

SQL ............ 90
来源：http://olj.jqgufenzy.top

Bash ........... 80
来源：http://fnc.hnqzz.top

Kotlin ......... 15
来源：http://wsh.9152youxi.cn

Swift .......... 15
来源：http://pqt.yongpay.top

Lua ............ 10
来源：http://esk.feifeiyinyue.top

Perl ........... 10
来源：http://wvf.yangfankeji.com

Scala .......... 10
来源：http://irw.sjlbkw.cn

------------------------------------
来源：http://its.nanxuanxn.top

合计 ........... 2106 条
来源：http://fbg.fehbvm.com

按章节统计：
来源：http://aby.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://adu.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lgb.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://guc.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ijh.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oyi.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gjf.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rtl.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yui.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zlg.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yzz.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tvg.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ipn.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://csr.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ivm.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iya.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cfy.hysaishi.cn

Q SQL 专题                              90
来源：http://iss.dianchejie.cn

R Bash 专题                             80
来源：http://nqa.hysaishi.cn

S C / C++ 专题                          60
来源：http://kgp.uphjek.com

T 其他语言补充                          60
来源：http://yaw.hfpthk.cn

U 高频实用片段                         120
来源：http://hei.ydjk.org.cn

------------------------------------
来源：http://krf.ydzc1.top

合计                                  2106 条
来源：http://enk.uphjek.com

--------------------------------------------------------------------------------
来源：http://xtw.shanyushiyangkeji.top

使用提醒
来源：http://aeq.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://vrb.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wql.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkh.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rnw.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vru.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eft.cqqwz.cn

—— 文件结束 ——
来源：http://jcj.jiagoushi.top

================================================================================
来源：http://vph.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://jct.smart0.xyz

Common Programming Examples Cheat Book
来源：http://kdv.cheryme.top

================================================================================
来源：http://yov.fengsongda.top

【收录内容】
来源：http://fci.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://syt.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mur.cucudq.cn

SQL · Bash · C · C++
来源：http://mle.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xmd.zdqjudy.top

【使用说明】
来源：http://jpg.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lij.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rlg.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qok.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xpw.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://poc.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wrl.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bkq.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ubg.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ohf.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gts.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mbb.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hto.tianlin.xyz

【文件统计】
来源：http://gcv.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://icn.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://gnn.nanxuanxn.top

目  录
来源：http://abk.yuxming.cn

--------------------------------------------------------------------------------
来源：http://xjr.vqdsnc.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ybv.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ylh.yanxiufei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nzm.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cwk.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://liu.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yqc.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gsv.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jru.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fnu.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://juh.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://etl.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cvt.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gin.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vym.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nic.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jqz.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hku.gaohongyu789.top


<!-- 参考信息 -->