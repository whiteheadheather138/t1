代发 wailian999

[U17] Py：初始化日志
来源：http://dix.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://dxv.dashuyun.cn

[U18] Py：预编译正则
来源：http://lok.hnqzz.top

pat = re.compile(r"\d+")
来源：http://oso.meibo888.top

[U19] Py：正则替换带回调
来源：http://jsq.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sux.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://lkd.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://yea.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://awy.snrcjt.cn

@contextlib.contextmanager
来源：http://ydu.cheryme.top

[U22] Py：矩阵转置
来源：http://fhx.kuanghao11.cn

list(zip(*m))
来源：http://ztp.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://mxr.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lsb.hesvh.cn

[U24] Py：路径操作
来源：http://hvy.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pta.ivvv.top

[U25] Py：CSV 按字典读
来源：http://ugi.dashuyun.cn

csv.DictReader(f)
来源：http://hdf.wangdashe.top

[U26] Py：并发下载
来源：http://vba.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iga.yvedp.cn

[U27] Py：异步 HTTP
来源：http://sbi.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://jyl.sweek.top

[U28] Py：类型别名
来源：http://cke.shanyushiyangkeji.top

UserId = int
来源：http://dhf.smart0.xyz

[U29] Py：属性校验
来源：http://tyf.dianchejie.cn

@property 与 @x.setter 配合
来源：http://qbr.ehwqpu.com

[U30] Py：数据类
来源：http://rmf.c1oappe.top

@dataclass(slots=True)
来源：http://dxr.tianlin.xyz

[U31] Py：单测
来源：http://eks.hesvh.cn

python -m pytest -q
来源：http://vkn.jinqigfzy.top

[U32] Py：代码格式化
来源：http://tue.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://xfa.kuanghao11.cn

[U33] Py：打包发布
来源：http://fke.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://ccs.zhoulong.xyz

[U34] Py：判断编码
来源：http://hpi.wangdashe.top

chardet.detect(raw)
来源：http://wdd.cheryme.top

[U35] Py：发送邮件
来源：http://lkr.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oyb.sxryk.cn

[U36] Py：定时任务
来源：http://pai.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://wvb.jianghu66.top

[U37] Py：读写 Excel
来源：http://bnl.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://xhc.yfazqb.com

[U38] Py：获取脚本所在目录
来源：http://gsp.dianchejie.cn

Path(__file__).resolve().parent
来源：http://tay.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://hlj.quarkkingdee.top

sys.stdout.isatty()
来源：http://hyr.tarul.cn

[U40] Py：打印到标准错误
来源：http://xnn.epnwcf.com

print("err", file=sys.stderr)
来源：http://trq.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://vgm.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hjo.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://hdw.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ouo.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://fhn.hcnkem.com

namespace App\Http;
来源：http://wbf.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://aei.gogol.net.cn

declare(strict_types=1);
来源：http://hza.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://ykf.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xvb.guannengcc.top

[U46] PHP：可空类型
来源：http://qbp.havefunace.top

?string $name = null
来源：http://ura.jianghu66.top

[U47] PHP：联合类型
来源：http://ros.sweek.top

int|string $id
来源：http://tnk.yvedp.cn

[U48] PHP：纯枚举
来源：http://clh.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nef.fehbvm.com

[U49] PHP：只读属性
来源：http://ctg.gzhubu.top

public readonly string $name
来源：http://uet.yongpay.top

[U50] PHP：构造器属性提升
来源：http://ubr.birdmap.top

public function __construct(private int $id) {}
来源：http://ldo.hnxiangtu.top

[U51] PHP：数组解构
来源：http://tyt.meibo888.top

[$a, $b] = $arr;
来源：http://xdf.shuidangran.top

[U52] PHP：箭头函数
来源：http://vbn.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://uti.fktsv.cn

[U53] PHP：空合并运算符
来源：http://sne.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://hsn.fktsv.cn

[U54] PHP：空安全调用
来源：http://hjw.tianlin.xyz

$obj?->method()
来源：http://nxy.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://klu.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sar.dashuyun.cn

[U56] PHP：命名参数
来源：http://tti.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://xjl.yuanzhike.top

[U57] PHP：字符串插值
来源：http://uhr.wangshuangyany.cn

"值: {$a}"
来源：http://xut.316326.xyz

[U58] PHP：数组三件套
来源：http://dcb.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://smr.hysaishi.cn

[U59] PHP：自定义排序
来源：http://ulp.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kay.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://udx.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hkh.yuxming.cn

[U61] PHP：正则
来源：http://ihq.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vsx.jiagoushi.top

[U62] PHP：日期对象
来源：http://zva.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dsu.mhx1999.top

[U63] PHP：文件读写
来源：http://vzs.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bpx.haohaochexian.top

[U64] PHP：目录遍历
来源：http://det.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://bwb.jinyuanbaomall.cn

[U65] PHP：会话
来源：http://ura.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zqw.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://ldy.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://moa.daria6918.cn

[U67] PHP：处理文件上传
来源：http://aso.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qsb.yongpay.top

[U68] PHP：PDO 连接
来源：http://jkr.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rvs.ivvv.top

[U69] PHP：PDO 预处理
来源：http://qrq.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dvl.hammf.cn

[U70] PHP：PDO 事务
来源：http://yrn.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rws.ydzc1.top

[U71] PHP：抛出异常
来源：http://nrj.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://wgs.andypj.xyz

[U72] PHP：写错误日志
来源：http://kgc.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://hgk.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://jnw.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://adf.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://crf.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://tga.yueranfly.top

[U75] PHP：依赖注入
来源：http://xrw.fanxiaobao.xyz

composer require psr/container
来源：http://jkw.xziqi.cn

[U76] PHP：简单路由
来源：http://pkg.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ufm.yfazqb.com

[U77] PHP：模板渲染
来源：http://pwo.zhaomingkeji.xyz

composer require twig/twig
来源：http://civ.cashguo.top

[U78] PHP：单元测试
来源：http://lpl.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://cjg.nanxinkj.top

[U79] PHP：静态分析
来源：http://ygd.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://ywr.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://mtp.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ubv.iojbl.cn

[U81] JS：初始化项目
来源：http://aso.yfazqb.com

npm init -y;  npm i express
来源：http://jjq.hesvh.cn

[U82] JS：package.json 脚本
来源：http://cyv.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oge.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://nlc.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://que.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://her.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://jra.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://hka.xylfe.cn

a?.b?.c
来源：http://glx.yj202588.top

[U86] JS：空值合并
来源：http://tlf.hcnkem.com

a ?? b
来源：http://olm.wangdashe.top

[U87] JS：解构默认值
来源：http://wos.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://glr.cdnleiting.top

[U88] JS：对象展开合并
来源：http://vjf.c1oappe.top

{ ...a, ...b }
来源：http://mjx.sweek.top

[U89] JS：数组去重
来源：http://cxz.hongshengwenyu.top

[...new Set(arr)]
来源：http://cls.daxiang520.top

[U90] JS：数字数组排序
来源：http://otj.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://ais.haohaochexian.top

[U91] JS：对象键值遍历
来源：http://hub.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gtt.yuxming.cn

[U92] JS：深拷贝
来源：http://jzj.hnxiangtu.top

structuredClone(obj)
来源：http://pkx.ivvv.top

[U93] JS：模板字符串
来源：http://agb.316326.xyz

`共 ${n} 条`
来源：http://yid.yangfankeji.com

[U94] JS：箭头函数
来源：http://odi.aibaodan.cn

const double = x => x * 2;
来源：http://spo.cqqwz.cn

[U95] JS：Promise 包装
来源：http://qwo.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://itr.aizwys.cn

[U96] JS：async/await 与异常
来源：http://mcx.zhoulong.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cvq.zycfv.cn

[U97] JS：并发请求
来源：http://hke.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ucn.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://nxb.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nhr.yuxming.cn

[U99] JS：事件监听
来源：http://zlh.fktsv.cn

el.addEventListener("click", e => {})
来源：http://kvp.andypj.xyz

[U100] JS：DOM 查询
来源：http://zdr.cdnleiting.top

document.querySelector(".item")
来源：http://ceb.jqgufenzy.top

[U101] JS：classList 操作
来源：http://rcr.shzxlz.cn

el.classList.toggle("active")
来源：http://rou.zhongyouzk.top

[U102] JS：本地存储
来源：http://qpk.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://mbj.dianchejie.cn

[U103] JS：定时器
来源：http://ndw.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jgv.xinyue.icu

[U104] JS：防抖
来源：http://sxz.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lae.jinghuilouyu.cn

[U105] JS：节流
来源：http://nxg.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bgk.tanke756.top

[U106] JS：日期格式化
来源：http://imu.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://osq.yangfankeji.com

[U107] JS：数字千分位
来源：http://aky.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uyg.hcnkem.com

[U108] JS：随机整数
来源：http://php.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ubt.hysaishi.cn

[U109] JS：数组分组
来源：http://ppn.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://mdj.daria6918.cn

[U110] JS：数组分块
来源：http://auf.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fyp.xziqi.cn

[U111] JS：对象转 Map
来源：http://dhl.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://gxs.svipenyu.cn

[U112] JS：字符串补位
来源：http://mmg.xuanzx.com

"7".padStart(3, "0")
来源：http://ejr.cucudq.cn

[U113] JS：正则替换全部
来源：http://kwr.epnwcf.com

s.replaceAll("a", "b")
来源：http://rde.hysaishi.cn

[U114] JS：JSON 深比较
来源：http://xex.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://byi.iojbl.cn

[U115] JS：生成 UUID
来源：http://gqh.zhixingplan.top

crypto.randomUUID()
来源：http://lii.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://ryk.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://kmk.nanxinkj.top

[U117] JS：单元测试
来源：http://hit.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://qii.fengsongda.top

[U118] JS：开发服务器
来源：http://ary.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://mrj.nanxinkj.top

[U119] JS：生产构建
来源：http://rqc.zhaomingkeji.xyz

npx vite build
来源：http://pzc.jlsjyb.cn

[U120] JS：读取环境变量（Vite）
来源：http://ran.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://gvq.aibaodan.cn

================================================================================
来源：http://swe.snrcjt.cn

统计汇总
来源：http://dqm.gzhubu.top

================================================================================
来源：http://syv.9152youxi.cn

按语言统计（条）：
来源：http://rml.fzhhl.top

Python ......... 252
来源：http://hpp.kuanghao11.cn

PHP ............ 252
来源：http://eoe.svipenyu.cn

JavaScript ..... 252
来源：http://ljg.redwolf501.top

TypeScript ..... 212
来源：http://hcf.mhx1999.top

Java ........... 212
来源：http://uxt.hongshengwenyu.top

Go ............. 212
来源：http://ppa.shzxlz.cn

Ruby ........... 212
来源：http://qvl.xuetiantiany.cn

C# ............. 212
来源：http://lch.yanxiufei.cn

C .............. 30
来源：http://fdt.birdmap.top

C++ ............ 30
来源：http://xgh.meibo888.top

SQL ............ 90
来源：http://jzi.quarkkingdee.top

Bash ........... 80
来源：http://vng.hysaishi.cn

Kotlin ......... 15
来源：http://hvg.fehbvm.com

Swift .......... 15
来源：http://vzz.ydzc1.top

Lua ............ 10
来源：http://aeg.ybcxt.top

Perl ........... 10
来源：http://rqn.bjfxy.top

Scala .......... 10
来源：http://ecw.zhijiandao.cn

------------------------------------
来源：http://psr.chenjidiqi.icu

合计 ........... 2106 条
来源：http://gyt.52xcode.cn

按章节统计：
来源：http://nmy.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oxr.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://haq.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cje.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cpx.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sgr.guowangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qnu.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nfl.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xrs.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://umf.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qzc.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xur.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lqr.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mhn.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dhn.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tno.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cvg.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://rdl.xuetiantiany.cn

R Bash 专题                             80
来源：http://doj.ydzc1.top

S C / C++ 专题                          60
来源：http://woq.tarul.cn

T 其他语言补充                          60
来源：http://xuy.hesvh.cn

U 高频实用片段                         120
来源：http://kzz.gzhubu.top

------------------------------------
来源：http://tvm.wangdashe.top

合计                                  2106 条
来源：http://wym.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://qka.wangshuangyany.cn

使用提醒
来源：http://zfo.bjfxy.top

--------------------------------------------------------------------------------
来源：http://ttz.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qcu.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jry.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lgz.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rkd.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jcw.bjfxy.top

—— 文件结束 ——
来源：http://aen.gaohongyu789.top

================================================================================
来源：http://nbl.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://khr.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://vnx.gogol.net.cn

================================================================================
来源：http://kko.meibo888.top

【收录内容】
来源：http://jde.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pbi.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dps.sxryk.cn

SQL · Bash · C · C++
来源：http://vmb.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nzf.hnqzz.top

【使用说明】
来源：http://jww.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tsw.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tbv.hfpthk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://olr.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qtk.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zoi.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bkn.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mru.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pef.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hjp.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jwi.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rnf.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jdn.hesvh.cn

【文件统计】
来源：http://wuj.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hcc.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://evx.ydjk.org.cn

目  录
来源：http://pnm.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://okt.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dxf.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tgt.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ldo.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kdt.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fps.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cmy.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://udc.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://inu.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vgo.ybcxt.top


<!-- 参考信息 -->