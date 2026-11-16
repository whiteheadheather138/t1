代发 wailian999

[U17] Py：初始化日志
来源：http://uub.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://kdd.xuanzx.com

[U18] Py：预编译正则
来源：http://vvr.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://trz.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://bwb.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ukh.zycfv.cn

[U20] Py：缓存函数结果
来源：http://ckr.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://dfl.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://zyb.zhiwuduotai.top

@contextlib.contextmanager
来源：http://jue.9152youxi.cn

[U22] Py：矩阵转置
来源：http://eqg.hysaishi.cn

list(zip(*m))
来源：http://gfs.jianghu66.top

[U23] Py：分块读取大文件
来源：http://msd.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://whu.yonumen.top

[U24] Py：路径操作
来源：http://pfa.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cmq.pycfn.com

[U25] Py：CSV 按字典读
来源：http://dfz.zhongyouzk.top

csv.DictReader(f)
来源：http://old.xuetiantiany.cn

[U26] Py：并发下载
来源：http://kar.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mej.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://akt.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://tsq.fzhhl.top

[U28] Py：类型别名
来源：http://mng.cucudq.cn

UserId = int
来源：http://evi.tian-w.cn

[U29] Py：属性校验
来源：http://zbv.xylfe.cn

@property 与 @x.setter 配合
来源：http://zqo.yj20258888.top

[U30] Py：数据类
来源：http://wcg.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://dqy.pengpengdd.cyou

[U31] Py：单测
来源：http://oos.yuanzhike.top

python -m pytest -q
来源：http://och.ehwqpu.com

[U32] Py：代码格式化
来源：http://aqi.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://vmq.meibo888.top

[U33] Py：打包发布
来源：http://pro.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://lxh.quarkkingdee.top

[U34] Py：判断编码
来源：http://dpv.smart0.xyz

chardet.detect(raw)
来源：http://jhb.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://jbv.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://etd.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://uln.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://wcf.316326.xyz

[U37] Py：读写 Excel
来源：http://mpi.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://zex.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://dyn.gzhubu.top

Path(__file__).resolve().parent
来源：http://mhz.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://jxn.9152youxi.cn

sys.stdout.isatty()
来源：http://bgc.52xcode.cn

[U40] Py：打印到标准错误
来源：http://fqb.nanxuanxn.top

print("err", file=sys.stderr)
来源：http://vmr.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://qdi.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pge.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://jwa.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://own.zycfv.cn

[U43] PHP：声明命名空间
来源：http://sjy.dashuyun.cn

namespace App\Http;
来源：http://sey.tian-w.cn

[U44] PHP：开启严格类型
来源：http://toy.yuxming.cn

declare(strict_types=1);
来源：http://dqf.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://vma.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://csa.fktsv.cn

[U46] PHP：可空类型
来源：http://fnr.vehdjk.com

?string $name = null
来源：http://jfk.hesvh.cn

[U47] PHP：联合类型
来源：http://qfd.aizwys.cn

int|string $id
来源：http://axy.hongshengwenyu.top

[U48] PHP：纯枚举
来源：http://jmu.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lhv.nwbrower.top

[U49] PHP：只读属性
来源：http://qsf.bbcook.cn

public readonly string $name
来源：http://vqg.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://ikf.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://ffq.gogol.net.cn

[U51] PHP：数组解构
来源：http://juz.nwbrower.top

[$a, $b] = $arr;
来源：http://cfp.jinqigufen.top

[U52] PHP：箭头函数
来源：http://sum.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://ehk.52xcode.cn

[U53] PHP：空合并运算符
来源：http://hbf.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://fre.xylfe.cn

[U54] PHP：空安全调用
来源：http://dsz.gotoacloud.top

$obj?->method()
来源：http://ckl.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://fxw.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gzl.hfpthk.cn

[U56] PHP：命名参数
来源：http://rbr.birdmap.top

f(a: 1, b: 2)
来源：http://uoa.daria6918.cn

[U57] PHP：字符串插值
来源：http://rvq.cheryme.top

"值: {$a}"
来源：http://zcs.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://qlo.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mhm.yonumen.top

[U59] PHP：自定义排序
来源：http://dpg.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xbj.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://tem.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xsn.hammf.cn

[U61] PHP：正则
来源：http://ctg.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vfi.vqdsnc.cn

[U62] PHP：日期对象
来源：http://sum.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://exr.dashuyun.cn

[U63] PHP：文件读写
来源：http://exk.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rwp.gzhubu.top

[U64] PHP：目录遍历
来源：http://cwy.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://okj.cucudq.cn

[U65] PHP：会话
来源：http://grh.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hbh.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://uim.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kct.gzhubu.top

[U67] PHP：处理文件上传
来源：http://uei.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zsb.sxryk.cn

[U68] PHP：PDO 连接
来源：http://yln.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zzo.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://rfr.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jtb.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://sjm.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cis.sysykeji.top

[U71] PHP：抛出异常
来源：http://wek.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://izu.sysykeji.top

[U72] PHP：写错误日志
来源：http://vjw.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://rxj.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://eik.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://bpk.gzhubu.top

[U74] PHP：读取环境变量
来源：http://sed.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://rgl.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://jws.gogol.net.cn

composer require psr/container
来源：http://adn.redwolf501.top

[U76] PHP：简单路由
来源：http://kdv.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rgu.jinqigufen.top

[U77] PHP：模板渲染
来源：http://iir.pengpengdd.cyou

composer require twig/twig
来源：http://sme.bbcook.cn

[U78] PHP：单元测试
来源：http://qhc.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://psd.cheryme.top

[U79] PHP：静态分析
来源：http://ltq.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://qog.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://vos.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gjo.jinqigufen.top

[U81] JS：初始化项目
来源：http://nez.xuanzx.com

npm init -y;  npm i express
来源：http://mrw.daria6918.cn

[U82] JS：package.json 脚本
来源：http://uxf.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dxn.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://wih.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://cmo.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://oxd.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://cdc.fehbvm.com

[U85] JS：可选链
来源：http://bqd.shuidangran.top

a?.b?.c
来源：http://vvj.jinqigfzy.top

[U86] JS：空值合并
来源：http://llu.shanyushiyangtech.top

a ?? b
来源：http://ajq.jqgfzy.top

[U87] JS：解构默认值
来源：http://svr.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://njj.havefunace.top

[U88] JS：对象展开合并
来源：http://qwq.wangdashe.top

{ ...a, ...b }
来源：http://dsw.snrcjt.cn

[U89] JS：数组去重
来源：http://zir.shanyushiyangtech.top

[...new Set(arr)]
来源：http://hch.bjfxy.top

[U90] JS：数字数组排序
来源：http://pno.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://gvg.bbcook.cn

[U91] JS：对象键值遍历
来源：http://fdq.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ati.sweek.top

[U92] JS：深拷贝
来源：http://kxy.vehdjk.com

structuredClone(obj)
来源：http://doi.uphjek.com

[U93] JS：模板字符串
来源：http://xwp.gotoacloud.top

`共 ${n} 条`
来源：http://yuz.svipenyu.cn

[U94] JS：箭头函数
来源：http://spr.zhaomingkeji.xyz

const double = x => x * 2;
来源：http://yhz.hysaishi.cn

[U95] JS：Promise 包装
来源：http://zxr.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://nrc.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://vgp.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iaj.jqgfzy.top

[U97] JS：并发请求
来源：http://boj.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vli.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://dbh.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uue.xziqi.cn

[U99] JS：事件监听
来源：http://osr.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://ucj.tian-w.cn

[U100] JS：DOM 查询
来源：http://hyv.jinqigufen.top

document.querySelector(".item")
来源：http://emi.epnwcf.com

[U101] JS：classList 操作
来源：http://ybp.aizwys.cn

el.classList.toggle("active")
来源：http://ukv.chenzaomai.com

[U102] JS：本地存储
来源：http://das.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uzs.jqgufenzy.top

[U103] JS：定时器
来源：http://rve.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eyf.cheryme.top

[U104] JS：防抖
来源：http://mrl.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkd.wangshuangyany.cn

[U105] JS：节流
来源：http://nxd.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://acn.xuanzx.com

[U106] JS：日期格式化
来源：http://ual.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vlx.zhongyouzk.top

[U107] JS：数字千分位
来源：http://jdo.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://unf.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://bol.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ddw.shuidangran.top

[U109] JS：数组分组
来源：http://vbg.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://mqp.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://ebm.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tmm.haohaochexian.top

[U111] JS：对象转 Map
来源：http://dih.mhx1999.top

new Map(Object.entries(obj))
来源：http://ogk.xuanzx.com

[U112] JS：字符串补位
来源：http://bdm.52xcode.cn

"7".padStart(3, "0")
来源：http://eyt.yj20258888.top

[U113] JS：正则替换全部
来源：http://yqy.316326.xyz

s.replaceAll("a", "b")
来源：http://vuu.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://vxd.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://fiw.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://hjg.wangdashe.top

crypto.randomUUID()
来源：http://yqe.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://prk.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://vda.nwbrower.top

[U117] JS：单元测试
来源：http://vqc.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://nxs.gzhubu.top

[U118] JS：开发服务器
来源：http://vbv.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://ozl.yj20258.top

[U119] JS：生产构建
来源：http://gwd.jinqigufen.top

npx vite build
来源：http://dhb.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://mqz.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://cif.shangyingyoupin.top

================================================================================
来源：http://wra.yanxiufei.cn

统计汇总
来源：http://vyl.tian-w.cn

================================================================================
来源：http://sfm.ydzc1.top

按语言统计（条）：
来源：http://pvo.jqgufenzy.top

Python ......... 252
来源：http://dmq.xingfuxueyuan.xyz

PHP ............ 252
来源：http://gvy.zhongyouzk.top

JavaScript ..... 252
来源：http://nkw.cqqwz.cn

TypeScript ..... 212
来源：http://avx.ppjwa.cn

Java ........... 212
来源：http://uju.c1oappe.top

Go ............. 212
来源：http://jgv.hcnkem.com

Ruby ........... 212
来源：http://myn.shuidangran.top

C# ............. 212
来源：http://ycq.pengpengdd.cyou

C .............. 30
来源：http://uhm.jqgufenzy.top

C++ ............ 30
来源：http://bdp.zhaomingkeji.xyz

SQL ............ 90
来源：http://slt.yvedp.cn

Bash ........... 80
来源：http://nnf.yuanzhike.top

Kotlin ......... 15
来源：http://vwb.52xcode.cn

Swift .......... 15
来源：http://vba.xinyue.icu

Lua ............ 10
来源：http://flw.ybcxt.top

Perl ........... 10
来源：http://ekm.yuxming.cn

Scala .......... 10
来源：http://jgl.epnwcf.com

------------------------------------
来源：http://bwe.yangfankeji.com

合计 ........... 2106 条
来源：http://xka.yonumen.top

按章节统计：
来源：http://hrd.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dsi.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ggi.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xtg.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gbq.andypj.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bpf.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dcf.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iwp.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nnu.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mxm.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cyx.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rzt.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gko.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gjw.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yot.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uav.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pjs.xziqi.cn

Q SQL 专题                              90
来源：http://hzn.yangfankeji.com

R Bash 专题                             80
来源：http://ozf.cheryme.top

S C / C++ 专题                          60
来源：http://dky.pycfn.com

T 其他语言补充                          60
来源：http://pts.chenjidiqi.icu

U 高频实用片段                         120
来源：http://wpt.haohaochexian.top

------------------------------------
来源：http://iqr.xylfe.cn

合计                                  2106 条
来源：http://hal.yuxming.cn

--------------------------------------------------------------------------------
来源：http://cdf.zdqjudy.top

使用提醒
来源：http://ljo.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://zlz.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mdd.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://guz.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ytj.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ozw.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ctk.xziqi.cn

—— 文件结束 ——
来源：http://fjw.xinyue.icu

================================================================================
来源：http://xko.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://qjq.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://cae.iojbl.cn

================================================================================
来源：http://brt.zhaomingkeji.xyz

【收录内容】
来源：http://ikw.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bjm.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://air.hesvh.cn

SQL · Bash · C · C++
来源：http://zjc.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zkm.zhengqikj.top

【使用说明】
来源：http://bxz.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jco.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uiv.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nci.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rzl.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://aqk.fehbvm.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xxn.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vsu.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hhf.chenlongwang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ift.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nij.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jlt.wangdashe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ofd.chenzaomai.com

【文件统计】
来源：http://awx.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://evr.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://ipm.9152youxi.cn

目  录
来源：http://ojc.vehdjk.com

--------------------------------------------------------------------------------
来源：http://dur.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://paa.guannengcc.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vkj.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rus.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wes.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kjf.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qeh.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nhk.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lbc.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://maf.meibo888.top


<!-- 参考信息 -->