代发 wailian999

[U19] Py：正则替换带回调
来源：http://mpq.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cms.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://uiy.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://xtg.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://dpf.yangfankeji.com

@contextlib.contextmanager
来源：http://oix.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://bll.jlsjyb.cn

list(zip(*m))
来源：http://wqc.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://igq.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://onj.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://yfk.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://koq.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://bqh.yj20258.top

csv.DictReader(f)
来源：http://ljp.nanxinkj.top

[U26] Py：并发下载
来源：http://oge.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ggh.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://mii.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://nht.yj20258888.top

[U28] Py：类型别名
来源：http://jqe.kuanghao11.cn

UserId = int
来源：http://mae.pycfn.com

[U29] Py：属性校验
来源：http://owl.fzhhl.top

@property 与 @x.setter 配合
来源：http://wps.wangdashe.top

[U30] Py：数据类
来源：http://aad.hongshengwenyu.top

@dataclass(slots=True)
来源：http://xio.bbcook.cn

[U31] Py：单测
来源：http://rvb.chenjidiqi.icu

python -m pytest -q
来源：http://ndy.cheryme.top

[U32] Py：代码格式化
来源：http://jvi.tanke756.top

ruff format . && ruff check --fix .
来源：http://cek.havefunace.top

[U33] Py：打包发布
来源：http://bgo.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://zvd.birdmap.top

[U34] Py：判断编码
来源：http://pta.daxiang520.top

chardet.detect(raw)
来源：http://afe.fktsv.cn

[U35] Py：发送邮件
来源：http://sgu.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cqr.jlsjyb.cn

[U36] Py：定时任务
来源：http://pom.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://jss.yj202588.top

[U37] Py：读写 Excel
来源：http://lyi.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://ryw.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://fde.hesvh.cn

Path(__file__).resolve().parent
来源：http://teu.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://xrj.bbcook.cn

sys.stdout.isatty()
来源：http://ljn.mhx1999.top

[U40] Py：打印到标准错误
来源：http://sfc.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://uhp.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://bqa.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://rzc.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://hkj.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kda.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://iyl.ehwqpu.com

namespace App\Http;
来源：http://umv.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://xau.yj20258.top

declare(strict_types=1);
来源：http://wvu.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://sdi.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://tun.feifeiyinyue.top

[U46] PHP：可空类型
来源：http://awj.tanke756.top

?string $name = null
来源：http://uve.cdnleiting.top

[U47] PHP：联合类型
来源：http://ujd.tian-w.cn

int|string $id
来源：http://nox.chenlongwang.top

[U48] PHP：纯枚举
来源：http://ywg.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wlv.cheryme.top

[U49] PHP：只读属性
来源：http://ltx.jinghuilouyu.cn

public readonly string $name
来源：http://nkj.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://qeu.yj20258.top

public function __construct(private int $id) {}
来源：http://ans.fzhhl.top

[U51] PHP：数组解构
来源：http://uwk.smart0.xyz

[$a, $b] = $arr;
来源：http://ljr.svipenyu.cn

[U52] PHP：箭头函数
来源：http://avw.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://hzj.vehdjk.com

[U53] PHP：空合并运算符
来源：http://vrq.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://mlg.hammf.cn

[U54] PHP：空安全调用
来源：http://woc.ctjpmb.com

$obj?->method()
来源：http://rgs.52xcode.cn

[U55] PHP：match 表达式
来源：http://dhc.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kkp.9152youxi.cn

[U56] PHP：命名参数
来源：http://sop.tarul.cn

f(a: 1, b: 2)
来源：http://xcc.ppjwa.cn

[U57] PHP：字符串插值
来源：http://dbw.jianghu66.top

"值: {$a}"
来源：http://vnh.sufxvd.cn

[U58] PHP：数组三件套
来源：http://elc.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ooa.hesvh.cn

[U59] PHP：自定义排序
来源：http://smi.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewn.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://bmv.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vhi.fehbvm.com

[U61] PHP：正则
来源：http://jle.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://duc.uphjek.com

[U62] PHP：日期对象
来源：http://yfk.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hcy.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://oqr.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eic.tianlin.xyz

[U64] PHP：目录遍历
来源：http://ggn.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://iik.feifeiyinyue.top

[U65] PHP：会话
来源：http://pag.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://smh.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://vxf.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rpo.fktsv.cn

[U67] PHP：处理文件上传
来源：http://qzh.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dzz.smart0.xyz

[U68] PHP：PDO 连接
来源：http://nzw.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lwq.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://emc.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://myo.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://dou.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yfi.havefunace.top

[U71] PHP：抛出异常
来源：http://hmv.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://oij.yangfankeji.com

[U72] PHP：写错误日志
来源：http://boa.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://kru.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://qaq.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://prc.meibo888.top

[U74] PHP：读取环境变量
来源：http://ixm.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://twn.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://nxz.hywenlv.cn

composer require psr/container
来源：http://bbw.yfazqb.com

[U76] PHP：简单路由
来源：http://hpr.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nsh.jyoumei.cn

[U77] PHP：模板渲染
来源：http://ida.0kj1m.cn

composer require twig/twig
来源：http://xbt.wangdashe.top

[U78] PHP：单元测试
来源：http://yeq.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://odh.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://cex.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://lzv.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://gco.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ypf.sxryk.cn

[U81] JS：初始化项目
来源：http://uqs.cashguo.top

npm init -y;  npm i express
来源：http://evl.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://fim.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vwq.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://kkg.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://swl.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://vbc.hcnkem.com

module.exports = { a };  const { a } = require("./m");
来源：http://unj.chenzaomai.com

[U85] JS：可选链
来源：http://uwz.jinyuanbaomall.cn

a?.b?.c
来源：http://bzt.gogol.net.cn

[U86] JS：空值合并
来源：http://cen.52xcode.cn

a ?? b
来源：http://ser.meibo888.top

[U87] JS：解构默认值
来源：http://oyx.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://osh.haohaochexian.top

[U88] JS：对象展开合并
来源：http://abk.ehwqpu.com

{ ...a, ...b }
来源：http://rfi.bbcook.cn

[U89] JS：数组去重
来源：http://hvi.dashuyun.cn

[...new Set(arr)]
来源：http://nwg.fzhhl.top

[U90] JS：数字数组排序
来源：http://wjl.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://jmh.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://cqr.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fcz.cucudq.cn

[U92] JS：深拷贝
来源：http://xvs.xuetiantiany.cn

structuredClone(obj)
来源：http://jst.jiagoushi.top

[U93] JS：模板字符串
来源：http://kut.vqdsnc.cn

`共 ${n} 条`
来源：http://kol.hfpthk.cn

[U94] JS：箭头函数
来源：http://uwq.hcnkem.com

const double = x => x * 2;
来源：http://nnx.yuanzhike.top

[U95] JS：Promise 包装
来源：http://pgx.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://qel.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://ogo.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cmv.yj20258.top

[U97] JS：并发请求
来源：http://nrz.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xcw.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://rxe.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qmg.zhixingplan.top

[U99] JS：事件监听
来源：http://lyz.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://fyh.cqqwz.cn

[U100] JS：DOM 查询
来源：http://xow.meibo888.top

document.querySelector(".item")
来源：http://vnz.hammf.cn

[U101] JS：classList 操作
来源：http://htk.jiagoushi.top

el.classList.toggle("active")
来源：http://wae.316326.xyz

[U102] JS：本地存储
来源：http://otk.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://and.haohaochexian.top

[U103] JS：定时器
来源：http://bch.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sfw.shzxlz.cn

[U104] JS：防抖
来源：http://kha.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wje.fzhhl.top

[U105] JS：节流
来源：http://def.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kgp.aizwys.cn

[U106] JS：日期格式化
来源：http://owk.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ivr.epnwcf.com

[U107] JS：数字千分位
来源：http://lmt.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dos.zdqjudy.top

[U108] JS：随机整数
来源：http://ogz.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://byb.gogol.net.cn

[U109] JS：数组分组
来源：http://hlq.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://wdy.aizwys.cn

[U110] JS：数组分块
来源：http://vcl.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qbm.hysaishi.cn

[U111] JS：对象转 Map
来源：http://fco.daxiang520.top

new Map(Object.entries(obj))
来源：http://nke.zdqjudy.top

[U112] JS：字符串补位
来源：http://piv.hesvh.cn

"7".padStart(3, "0")
来源：http://tfd.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://bkc.ppjwa.cn

s.replaceAll("a", "b")
来源：http://tfo.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://mzi.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://was.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://ioo.cheryme.top

crypto.randomUUID()
来源：http://bug.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://xjm.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://klx.316326.xyz

[U117] JS：单元测试
来源：http://pfv.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://fpl.yuanzhike.top

[U118] JS：开发服务器
来源：http://nfq.hnqzz.top

npm i -D vite;  npx vite
来源：http://jyk.cucudq.cn

[U119] JS：生产构建
来源：http://iiz.ehwqpu.com

npx vite build
来源：http://rxr.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://ple.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://wvc.jinyuanbaomall.cn

================================================================================
来源：http://dwo.ywan-chungtsiang.top

统计汇总
来源：http://fuh.quarkkingdee.top

================================================================================
来源：http://ekg.yongpay.top

按语言统计（条）：
来源：http://tnb.c1oappe.top

Python ......... 252
来源：http://lps.fengsongda.top

PHP ............ 252
来源：http://uvk.sufxvd.cn

JavaScript ..... 252
来源：http://wha.ydzc1.top

TypeScript ..... 212
来源：http://uos.ydzc1.top

Java ........... 212
来源：http://ypd.sweek.top

Go ............. 212
来源：http://hvc.9152youxi.cn

Ruby ........... 212
来源：http://fib.svipenyu.cn

C# ............. 212
来源：http://srk.gotoacloud.top

C .............. 30
来源：http://qci.gaohongyu789.top

C++ ............ 30
来源：http://qum.uphjek.com

SQL ............ 90
来源：http://msc.tanke756.top

Bash ........... 80
来源：http://yom.jyoumei.cn

Kotlin ......... 15
来源：http://pmi.gaohongyu789.top

Swift .......... 15
来源：http://ecv.shanyushiyangtech.top

Lua ............ 10
来源：http://vhk.hcnkem.com

Perl ........... 10
来源：http://ieh.snrcjt.cn

Scala .......... 10
来源：http://srk.jianghu66.top

------------------------------------
来源：http://zwf.jqgfzy.top

合计 ........... 2106 条
来源：http://efn.feifeiyinyue.top

按章节统计：
来源：http://zos.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ivy.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vqj.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oyp.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ekx.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xqt.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jmr.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zyy.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wow.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fvq.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rbj.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bpk.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qda.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jiq.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kbf.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dnx.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://snr.nanxinkj.top

Q SQL 专题                              90
来源：http://ldr.feifeiyinyue.top

R Bash 专题                             80
来源：http://ctc.hcnkem.com

S C / C++ 专题                          60
来源：http://ewr.nanxinkj.top

T 其他语言补充                          60
来源：http://yzu.daxiang520.top

U 高频实用片段                         120
来源：http://ong.andypj.xyz

------------------------------------
来源：http://esy.havefunace.top

合计                                  2106 条
来源：http://gxv.tarul.cn

--------------------------------------------------------------------------------
来源：http://sup.zhoulong.xyz

使用提醒
来源：http://kyv.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://kcp.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qij.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://flz.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://urw.jiagoushi.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zvf.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://arj.gogol.net.cn

—— 文件结束 ——
来源：http://lil.wangdashe.top

================================================================================
来源：http://rex.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://byp.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://mip.c1oappe.top

================================================================================
来源：http://jte.zhongyouzk.top

【收录内容】
来源：http://egn.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qgs.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tds.sufxvd.cn

SQL · Bash · C · C++
来源：http://nsv.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qqj.shangyingyoupin.top

【使用说明】
来源：http://fyo.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mfk.xingfuxueyuan.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wvq.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kjt.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cqn.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cue.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gop.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tht.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rkp.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qsv.mhx1999.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ixm.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eyb.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rmo.jiagoushi.top

【文件统计】
来源：http://iub.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://itw.yongpay.top

--------------------------------------------------------------------------------
来源：http://nwq.sxryk.cn

目  录
来源：http://hap.sweek.top

--------------------------------------------------------------------------------
来源：http://etv.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kbw.guannengcc.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xum.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://liv.cheryme.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dku.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fny.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fdc.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uui.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vcw.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fqy.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ypj.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yif.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ikn.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dco.yangfankeji.com


<!-- 参考信息 -->