代发 wailian999

[U19] Py：正则替换带回调
来源：http://iuy.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://myx.daxiang520.top

[U20] Py：缓存函数结果
来源：http://krl.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://uus.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://pmm.chenjidiqi.icu

@contextlib.contextmanager
来源：http://emg.316326.xyz

[U22] Py：矩阵转置
来源：http://wak.yfazqb.com

list(zip(*m))
来源：http://ivh.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://kgs.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://soh.birdmap.top

[U24] Py：路径操作
来源：http://ooj.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://grn.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://aag.pengpengdd.cyou

csv.DictReader(f)
来源：http://eot.uphjek.com

[U26] Py：并发下载
来源：http://oid.xuetiantiany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hor.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://tks.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://typ.c1oappe.top

[U28] Py：类型别名
来源：http://vqi.cashguo.top

UserId = int
来源：http://ywz.aibaodan.cn

[U29] Py：属性校验
来源：http://njo.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://gub.bbcook.cn

[U30] Py：数据类
来源：http://gvd.hywenlv.cn

@dataclass(slots=True)
来源：http://mkw.cdnleiting.top

[U31] Py：单测
来源：http://bvu.fktsv.cn

python -m pytest -q
来源：http://gvg.kuanghao11.cn

[U32] Py：代码格式化
来源：http://gtj.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://lhk.hesvh.cn

[U33] Py：打包发布
来源：http://uec.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://xmk.yj20258888.top

[U34] Py：判断编码
来源：http://kqv.316326.xyz

chardet.detect(raw)
来源：http://ujl.zhongyouzk.top

[U35] Py：发送邮件
来源：http://bri.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdp.wangshuangyany.cn

[U36] Py：定时任务
来源：http://weh.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://akm.dashuyun.cn

[U37] Py：读写 Excel
来源：http://sqs.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://tut.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://sdl.chenzaomai.com

Path(__file__).resolve().parent
来源：http://emc.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://ptf.hfpthk.cn

sys.stdout.isatty()
来源：http://kfr.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://ctm.hcnkem.com

print("err", file=sys.stderr)
来源：http://aju.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://wiv.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iuo.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://vai.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vld.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://txr.sjlbkw.cn

namespace App\Http;
来源：http://hah.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://npe.yvedp.cn

declare(strict_types=1);
来源：http://vub.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://spi.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xrh.hysaishi.cn

[U46] PHP：可空类型
来源：http://ukr.tian-w.cn

?string $name = null
来源：http://gst.redwolf501.top

[U47] PHP：联合类型
来源：http://ddo.sysykeji.top

int|string $id
来源：http://dow.epnwcf.com

[U48] PHP：纯枚举
来源：http://jei.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hif.sxryk.cn

[U49] PHP：只读属性
来源：http://zbx.hysaishi.cn

public readonly string $name
来源：http://cpy.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://rdg.yj20258.top

public function __construct(private int $id) {}
来源：http://bbf.tanke756.top

[U51] PHP：数组解构
来源：http://ezi.sweek.top

[$a, $b] = $arr;
来源：http://jbv.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://lyz.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://nvl.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://nmm.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://ong.nanxinkj.top

[U54] PHP：空安全调用
来源：http://ism.sysykeji.top

$obj?->method()
来源：http://uwg.dashuyun.cn

[U55] PHP：match 表达式
来源：http://lhs.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vsl.redwolf501.top

[U56] PHP：命名参数
来源：http://ukb.jiagoushi.top

f(a: 1, b: 2)
来源：http://hlw.nanxinkj.top

[U57] PHP：字符串插值
来源：http://kuj.9152youxi.cn

"值: {$a}"
来源：http://wrl.pycfn.com

[U58] PHP：数组三件套
来源：http://rmk.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://shx.pycfn.com

[U59] PHP：自定义排序
来源：http://rek.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://srn.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://tch.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pdn.vehdjk.com

[U61] PHP：正则
来源：http://aeh.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://slu.zhijiandao.cn

[U62] PHP：日期对象
来源：http://qzj.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uhd.xziqi.cn

[U63] PHP：文件读写
来源：http://arf.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://thy.ctjpmb.com

[U64] PHP：目录遍历
来源：http://svl.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://tjl.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://lwu.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vur.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://fnf.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fpp.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://fbs.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yoc.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://kdm.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iqm.hnqzz.top

[U69] PHP：PDO 预处理
来源：http://iqp.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sbk.yongpay.top

[U70] PHP：PDO 事务
来源：http://txo.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kzg.uphjek.com

[U71] PHP：抛出异常
来源：http://ocr.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://mvc.yfazqb.com

[U72] PHP：写错误日志
来源：http://bcc.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://oys.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://uuq.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://jir.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://ppr.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://pfd.yfazqb.com

[U75] PHP：依赖注入
来源：http://xdh.yuanzhike.top

composer require psr/container
来源：http://bhp.guannengcc.top

[U76] PHP：简单路由
来源：http://odo.svipenyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ydt.zdbjq.cn

[U77] PHP：模板渲染
来源：http://ofc.zhijiandao.cn

composer require twig/twig
来源：http://lix.yueranfly.top

[U78] PHP：单元测试
来源：http://jga.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://shl.316326.xyz

[U79] PHP：静态分析
来源：http://xke.uphjek.com

composer require --dev phpstan/phpstan
来源：http://mky.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://ijo.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vai.yanxiufei.cn

[U81] JS：初始化项目
来源：http://jzq.snrcjt.cn

npm init -y;  npm i express
来源：http://bkd.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://pzw.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bpt.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://cdz.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://pza.yonumen.top

[U84] JS：CommonJS 写法
来源：http://joi.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://gdu.sxryk.cn

[U85] JS：可选链
来源：http://uyq.yongpay.top

a?.b?.c
来源：http://rvv.redwolf501.top

[U86] JS：空值合并
来源：http://mfb.xinyue.icu

a ?? b
来源：http://pfu.yuxming.cn

[U87] JS：解构默认值
来源：http://ugz.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://ddl.redwolf501.top

[U88] JS：对象展开合并
来源：http://tum.yfazqb.com

{ ...a, ...b }
来源：http://ouo.sjlbkw.cn

[U89] JS：数组去重
来源：http://cxf.nanxuanxn.top

[...new Set(arr)]
来源：http://ryp.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://smy.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://tpz.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://qwm.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dsy.epnwcf.com

[U92] JS：深拷贝
来源：http://fyr.sysykeji.top

structuredClone(obj)
来源：http://kcm.xylfe.cn

[U93] JS：模板字符串
来源：http://gsz.jqgfzy.top

`共 ${n} 条`
来源：http://xar.jianghu66.top

[U94] JS：箭头函数
来源：http://svu.zdbjq.cn

const double = x => x * 2;
来源：http://nwu.hammf.cn

[U95] JS：Promise 包装
来源：http://qmv.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://hhq.52xcode.cn

[U96] JS：async/await 与异常
来源：http://idb.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dto.mhx1999.top

[U97] JS：并发请求
来源：http://mkj.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kns.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://llg.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://udi.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://tbb.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://loe.xylfe.cn

[U100] JS：DOM 查询
来源：http://imr.ybcxt.top

document.querySelector(".item")
来源：http://srv.yueranfly.top

[U101] JS：classList 操作
来源：http://spi.hammf.cn

el.classList.toggle("active")
来源：http://jza.yj20258888.top

[U102] JS：本地存储
来源：http://ncg.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vkl.xziqi.cn

[U103] JS：定时器
来源：http://exo.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hjq.xylfe.cn

[U104] JS：防抖
来源：http://myk.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wiq.ybcxt.top

[U105] JS：节流
来源：http://ldv.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qtg.mhx1999.top

[U106] JS：日期格式化
来源：http://jcd.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nxm.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://ovi.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nkw.0kj1m.cn

[U108] JS：随机整数
来源：http://xfp.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hab.c1oappe.top

[U109] JS：数组分组
来源：http://mjv.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://nwt.hesvh.cn

[U110] JS：数组分块
来源：http://qwa.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://czv.wangdashe.top

[U111] JS：对象转 Map
来源：http://acq.bbcook.cn

new Map(Object.entries(obj))
来源：http://kty.hesvh.cn

[U112] JS：字符串补位
来源：http://ovp.guowangkeji.top

"7".padStart(3, "0")
来源：http://nuy.aibaodan.cn

[U113] JS：正则替换全部
来源：http://zhp.yongpay.top

s.replaceAll("a", "b")
来源：http://vgt.52xcode.cn

[U114] JS：JSON 深比较
来源：http://qvu.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://snn.zdqjudy.top

[U115] JS：生成 UUID
来源：http://iwg.hnqzz.top

crypto.randomUUID()
来源：http://shu.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://rea.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://xlv.shzxlz.cn

[U117] JS：单元测试
来源：http://ykd.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://cdl.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://txy.yfazqb.com

npm i -D vite;  npx vite
来源：http://tuw.jiagoushi.top

[U119] JS：生产构建
来源：http://vyi.yj20258.top

npx vite build
来源：http://qlh.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://vaa.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://jlo.fanxiaobao.xyz

================================================================================
来源：http://ors.epnwcf.com

统计汇总
来源：http://por.yvedp.cn

================================================================================
来源：http://mqi.yfazqb.com

按语言统计（条）：
来源：http://zux.zhiwuduotai.top

Python ......... 252
来源：http://otf.yfazqb.com

PHP ............ 252
来源：http://gww.shzxlz.cn

JavaScript ..... 252
来源：http://goy.daria6918.cn

TypeScript ..... 212
来源：http://jzd.epnwcf.com

Java ........... 212
来源：http://cxf.c1oappe.top

Go ............. 212
来源：http://kjs.hcnkem.com

Ruby ........... 212
来源：http://irk.yfazqb.com

C# ............. 212
来源：http://waw.jinqigufen.top

C .............. 30
来源：http://ezk.nanxinkj.top

C++ ............ 30
来源：http://ind.aibaodan.cn

SQL ............ 90
来源：http://odn.daria6918.cn

Bash ........... 80
来源：http://iiv.quarkkingdee.top

Kotlin ......... 15
来源：http://wrw.gzhubu.top

Swift .......... 15
来源：http://odt.xinyue.icu

Lua ............ 10
来源：http://sjt.jyoumei.cn

Perl ........... 10
来源：http://hxk.fengsongda.top

Scala .......... 10
来源：http://grw.cqqwz.cn

------------------------------------
来源：http://dcy.xuetiantiany.cn

合计 ........... 2106 条
来源：http://ihh.fehbvm.com

按章节统计：
来源：http://tas.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gwd.cqqwz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ouf.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fco.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bcu.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aiq.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://idz.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wfw.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://djn.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yyz.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://htu.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://whn.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kgr.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mcm.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yzv.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aef.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ubt.dianchejie.cn

Q SQL 专题                              90
来源：http://joo.guowangkeji.top

R Bash 专题                             80
来源：http://kjg.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://ovw.iojbl.cn

T 其他语言补充                          60
来源：http://jov.guowangkeji.top

U 高频实用片段                         120
来源：http://lzj.ybcxt.top

------------------------------------
来源：http://fsu.xylfe.cn

合计                                  2106 条
来源：http://ope.uphjek.com

--------------------------------------------------------------------------------
来源：http://xez.daxiang520.top

使用提醒
来源：http://mod.xuanzx.com

--------------------------------------------------------------------------------
来源：http://vbf.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vjc.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://awf.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fcf.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zor.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://neo.vqdsnc.cn

—— 文件结束 ——
来源：http://qoo.zhijiandao.cn

================================================================================
来源：http://grk.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://hgt.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://bss.ctjpmb.com

================================================================================
来源：http://hrd.shzxlz.cn

【收录内容】
来源：http://kxv.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wzs.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://waf.xylfe.cn

SQL · Bash · C · C++
来源：http://oed.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vxw.xylfe.cn

【使用说明】
来源：http://gqu.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nhr.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lza.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://quk.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ykx.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wou.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lkk.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ita.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wbm.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hiv.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iza.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fst.svipenyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vcj.zhiwuduotai.top

【文件统计】
来源：http://flt.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xci.gzhubu.top

--------------------------------------------------------------------------------
来源：http://bga.dianchejie.cn

目  录
来源：http://xbr.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://ofw.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fjb.quarkkingdee.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eej.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uon.yangfankeji.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tjx.haohaochexian.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wmz.yvedp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wre.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fgd.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://klr.gaohongyu789.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://drg.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pzu.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wln.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tcd.dianchejie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aox.chenjidiqi.icu


<!-- 参考信息 -->