代发 wailian999

[U17] Py：初始化日志
来源：http://poh.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://sym.tanke756.top

[U18] Py：预编译正则
来源：http://xkq.316326.xyz

pat = re.compile(r"\d+")
来源：http://vib.316326.xyz

[U19] Py：正则替换带回调
来源：http://tws.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mri.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://qot.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://fxy.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://yxu.uphjek.com

@contextlib.contextmanager
来源：http://ijg.redwolf501.top

[U22] Py：矩阵转置
来源：http://wog.zdbjq.cn

list(zip(*m))
来源：http://wik.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://oif.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zvy.tianlin.xyz

[U24] Py：路径操作
来源：http://zgl.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://myr.hammf.cn

[U25] Py：CSV 按字典读
来源：http://jwi.pengpengdd.cyou

csv.DictReader(f)
来源：http://sre.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://cfc.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xcf.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://hdw.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://tjs.sxryk.cn

[U28] Py：类型别名
来源：http://tsi.haohaochexian.top

UserId = int
来源：http://dqb.hesvh.cn

[U29] Py：属性校验
来源：http://epf.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://yuz.hesvh.cn

[U30] Py：数据类
来源：http://wwd.zhijiandao.cn

@dataclass(slots=True)
来源：http://voa.yongpay.top

[U31] Py：单测
来源：http://qda.svipenyu.cn

python -m pytest -q
来源：http://fpm.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://qng.pycfn.com

ruff format . && ruff check --fix .
来源：http://afd.birdmap.top

[U33] Py：打包发布
来源：http://opo.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://hyh.ctjpmb.com

[U34] Py：判断编码
来源：http://boj.zhengqikj.top

chardet.detect(raw)
来源：http://jdl.kuanghao11.cn

[U35] Py：发送邮件
来源：http://izu.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ntl.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://owa.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://fii.chenlongwang.top

[U37] Py：读写 Excel
来源：http://gez.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://smi.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://qop.xuanzx.com

Path(__file__).resolve().parent
来源：http://jov.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://tbp.wangshuangyany.cn

sys.stdout.isatty()
来源：http://ecg.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://vxy.chenjidiqi.icu

print("err", file=sys.stderr)
来源：http://qtl.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://poj.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jyr.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://grq.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uqm.yueranfly.top

[U43] PHP：声明命名空间
来源：http://ggc.ywan-chungtsiang.top

namespace App\Http;
来源：http://jjl.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://bux.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://fzf.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://xeh.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pua.cashguo.top

[U46] PHP：可空类型
来源：http://dnm.yvedp.cn

?string $name = null
来源：http://hnj.tanke756.top

[U47] PHP：联合类型
来源：http://elb.ctjpmb.com

int|string $id
来源：http://iqu.c1oappe.top

[U48] PHP：纯枚举
来源：http://lup.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://exj.gogol.net.cn

[U49] PHP：只读属性
来源：http://vbh.jqgfzy.top

public readonly string $name
来源：http://aky.cashguo.top

[U50] PHP：构造器属性提升
来源：http://yoa.tian-w.cn

public function __construct(private int $id) {}
来源：http://qxu.hnqzz.top

[U51] PHP：数组解构
来源：http://ryh.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://dmu.fktsv.cn

[U52] PHP：箭头函数
来源：http://pos.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://pkk.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://skp.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://gwc.mhx1999.top

[U54] PHP：空安全调用
来源：http://hiq.andypj.xyz

$obj?->method()
来源：http://acf.sysykeji.top

[U55] PHP：match 表达式
来源：http://yvk.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fhd.xuanzx.com

[U56] PHP：命名参数
来源：http://vzw.hcnkem.com

f(a: 1, b: 2)
来源：http://vcu.yfazqb.com

[U57] PHP：字符串插值
来源：http://ofc.yj20258888.top

"值: {$a}"
来源：http://pjn.yangfankeji.com

[U58] PHP：数组三件套
来源：http://vuk.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zso.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://jwd.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnf.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://hka.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sna.nanxinkj.top

[U61] PHP：正则
来源：http://xgu.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://syh.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://twd.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oef.hesvh.cn

[U63] PHP：文件读写
来源：http://avz.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ndy.9152youxi.cn

[U64] PHP：目录遍历
来源：http://pyn.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://jfa.shzxlz.cn

[U65] PHP：会话
来源：http://gqz.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dtp.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://all.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ltk.fengsongda.top

[U67] PHP：处理文件上传
来源：http://nrk.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lzo.hammf.cn

[U68] PHP：PDO 连接
来源：http://yjc.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ttd.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://lmj.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fwe.316326.xyz

[U70] PHP：PDO 事务
来源：http://nxr.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwx.tarul.cn

[U71] PHP：抛出异常
来源：http://vrt.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://ssh.yj20258888.top

[U72] PHP：写错误日志
来源：http://oju.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://eml.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://hnv.uphjek.com

parse_ini_file("config.ini", true)
来源：http://qux.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://abs.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://ayd.sweek.top

[U75] PHP：依赖注入
来源：http://zvn.dashuyun.cn

composer require psr/container
来源：http://qpk.yvedp.cn

[U76] PHP：简单路由
来源：http://gog.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mms.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://ikp.redwolf501.top

composer require twig/twig
来源：http://hjg.aizwys.cn

[U78] PHP：单元测试
来源：http://wca.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://srl.gogol.net.cn

[U79] PHP：静态分析
来源：http://msd.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://cil.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://gig.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://chb.cqqwz.cn

[U81] JS：初始化项目
来源：http://zvv.jqgufenzy.top

npm init -y;  npm i express
来源：http://glr.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://ldr.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ncs.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://ejb.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fnx.sweek.top

[U84] JS：CommonJS 写法
来源：http://ezd.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://zku.chenlongwang.top

[U85] JS：可选链
来源：http://xpc.nanxuanxn.top

a?.b?.c
来源：http://nwa.chenjidiqi.icu

[U86] JS：空值合并
来源：http://vel.pycfn.com

a ?? b
来源：http://xji.yj20258888.top

[U87] JS：解构默认值
来源：http://see.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://joq.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://eyk.sjlbkw.cn

{ ...a, ...b }
来源：http://rbk.havefunace.top

[U89] JS：数组去重
来源：http://wiw.cqqwz.cn

[...new Set(arr)]
来源：http://dnp.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://awq.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://ifa.gzhubu.top

[U91] JS：对象键值遍历
来源：http://hze.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gaz.xinyue.icu

[U92] JS：深拷贝
来源：http://ada.fanxiaobao.xyz

structuredClone(obj)
来源：http://igr.jinqigfzy.top

[U93] JS：模板字符串
来源：http://tjh.hongshengwenyu.top

`共 ${n} 条`
来源：http://sps.fzhhl.top

[U94] JS：箭头函数
来源：http://pfo.ydjk.org.cn

const double = x => x * 2;
来源：http://zwb.guowangkeji.top

[U95] JS：Promise 包装
来源：http://rcd.cheryme.top

new Promise((resolve, reject) => {})
来源：http://imy.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://eaj.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yum.mhx1999.top

[U97] JS：并发请求
来源：http://nsw.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jrx.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://sbb.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wrv.gaohongyu789.top

[U99] JS：事件监听
来源：http://oyr.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://aiw.ppjwa.cn

[U100] JS：DOM 查询
来源：http://pqd.mhx1999.top

document.querySelector(".item")
来源：http://mmn.c1oappe.top

[U101] JS：classList 操作
来源：http://nxf.gzhubu.top

el.classList.toggle("active")
来源：http://lms.mhx1999.top

[U102] JS：本地存储
来源：http://mjx.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xjz.zhongyouzk.top

[U103] JS：定时器
来源：http://dmt.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oyd.zhoulong.xyz

[U104] JS：防抖
来源：http://zhy.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryr.haohaochexian.top

[U105] JS：节流
来源：http://rpx.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dho.ybcxt.top

[U106] JS：日期格式化
来源：http://ayi.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nvd.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://oyl.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sjy.redwolf501.top

[U108] JS：随机整数
来源：http://hbz.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nkx.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://udw.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://csm.aibaodan.cn

[U110] JS：数组分块
来源：http://vgk.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mkx.yonumen.top

[U111] JS：对象转 Map
来源：http://gtx.fktsv.cn

new Map(Object.entries(obj))
来源：http://fpc.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://fzf.xinyue.icu

"7".padStart(3, "0")
来源：http://eth.snrcjt.cn

[U113] JS：正则替换全部
来源：http://oya.uphjek.com

s.replaceAll("a", "b")
来源：http://dia.dianchejie.cn

[U114] JS：JSON 深比较
来源：http://wbt.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xae.hesvh.cn

[U115] JS：生成 UUID
来源：http://umu.nwbrower.top

crypto.randomUUID()
来源：http://qvj.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://utq.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://kyp.fktsv.cn

[U117] JS：单元测试
来源：http://pin.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://atm.ybcxt.top

[U118] JS：开发服务器
来源：http://nvp.xinyue.icu

npm i -D vite;  npx vite
来源：http://ggw.yvedp.cn

[U119] JS：生产构建
来源：http://fgx.ctjpmb.com

npx vite build
来源：http://kwf.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://evh.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://wsf.cqqwz.cn

================================================================================
来源：http://vum.xziqi.cn

统计汇总
来源：http://rxe.c1oappe.top

================================================================================
来源：http://uwd.jinqigufen.top

按语言统计（条）：
来源：http://nxb.ehwqpu.com

Python ......... 252
来源：http://lnr.mhx1999.top

PHP ............ 252
来源：http://npk.xuanzx.com

JavaScript ..... 252
来源：http://tsw.jqgfzy.top

TypeScript ..... 212
来源：http://jwj.ivvv.top

Java ........... 212
来源：http://kwt.52xcode.cn

Go ............. 212
来源：http://cme.dashuyun.cn

Ruby ........... 212
来源：http://ucr.ehwqpu.com

C# ............. 212
来源：http://xto.yonumen.top

C .............. 30
来源：http://rqq.yj202588.top

C++ ............ 30
来源：http://jtl.xingfuxueyuan.xyz

SQL ............ 90
来源：http://lhw.yj20258.top

Bash ........... 80
来源：http://xvr.ydjk.org.cn

Kotlin ......... 15
来源：http://dsw.gotoacloud.top

Swift .......... 15
来源：http://tjc.jyoumei.cn

Lua ............ 10
来源：http://wms.xinyue.icu

Perl ........... 10
来源：http://lqr.jinqigufen.top

Scala .......... 10
来源：http://ebq.yfazqb.com

------------------------------------
来源：http://ivu.wangdashe.top

合计 ........... 2106 条
来源：http://rlc.andypj.xyz

按章节统计：
来源：http://zri.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tro.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sgk.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fpb.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gqi.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vaz.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mix.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tsm.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yzp.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lcj.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yow.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qxe.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pji.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rdq.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rbh.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mbs.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://czu.yangfankeji.com

Q SQL 专题                              90
来源：http://jlo.yvedp.cn

R Bash 专题                             80
来源：http://fbl.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://jii.chenzaomai.com

T 其他语言补充                          60
来源：http://vmh.jqgufenzy.top

U 高频实用片段                         120
来源：http://iml.hywenlv.cn

------------------------------------
来源：http://yfb.hnqzz.top

合计                                  2106 条
来源：http://xxl.smart0.xyz

--------------------------------------------------------------------------------
来源：http://gst.cqqwz.cn

使用提醒
来源：http://hro.yuxming.cn

--------------------------------------------------------------------------------
来源：http://pph.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nje.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sou.xylfe.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ksc.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ezi.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dkv.andypj.xyz

—— 文件结束 ——
来源：http://jxc.hysaishi.cn

================================================================================
来源：http://tvw.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://aqj.daxiang520.top

Common Programming Examples Cheat Book
来源：http://yut.zhongyouzk.top

================================================================================
来源：http://ruv.jianghu66.top

【收录内容】
来源：http://oiv.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://aws.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jyw.yongpay.top

SQL · Bash · C · C++
来源：http://ddv.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pfl.gaohongyu789.top

【使用说明】
来源：http://smp.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hga.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bpc.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://len.dashuyun.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tij.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fgv.dashuyun.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ogg.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bsj.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pbu.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xnr.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pmb.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gag.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ooq.yueranfly.top

【文件统计】
来源：http://qua.kuanghao11.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hds.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://djw.hysaishi.cn

目  录
来源：http://cnv.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://ftm.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oyy.ydzc1.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nqy.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://whz.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vhc.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gym.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vgv.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qqa.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hmu.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ygq.yangfankeji.com


<!-- 参考信息 -->