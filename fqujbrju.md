代发 wailian999

[U17] Py：初始化日志
来源：http://cyj.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://kyi.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://ypx.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://ssb.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://lrp.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zhu.mhx1999.top

[U20] Py：缓存函数结果
来源：http://yri.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://ygq.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://dtm.hywenlv.cn

@contextlib.contextmanager
来源：http://cii.sxryk.cn

[U22] Py：矩阵转置
来源：http://tnz.xuetiantiany.cn

list(zip(*m))
来源：http://zwz.meibo888.top

[U23] Py：分块读取大文件
来源：http://ruh.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://naw.zdqjudy.top

[U24] Py：路径操作
来源：http://xmr.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://swo.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://khj.hfpthk.cn

csv.DictReader(f)
来源：http://xht.dashuyun.cn

[U26] Py：并发下载
来源：http://zzf.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jbl.sxryk.cn

[U27] Py：异步 HTTP
来源：http://gxf.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://kab.xziqi.cn

[U28] Py：类型别名
来源：http://avn.yuanzhike.top

UserId = int
来源：http://dms.yanxiufei.cn

[U29] Py：属性校验
来源：http://rdf.ybcxt.top

@property 与 @x.setter 配合
来源：http://der.andypj.xyz

[U30] Py：数据类
来源：http://vbo.redwolf501.top

@dataclass(slots=True)
来源：http://yai.fehbvm.com

[U31] Py：单测
来源：http://dsy.ydjk.org.cn

python -m pytest -q
来源：http://nxb.nwbrower.top

[U32] Py：代码格式化
来源：http://qeq.mhx1999.top

ruff format . && ruff check --fix .
来源：http://obs.sysykeji.top

[U33] Py：打包发布
来源：http://qwi.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://pry.sweek.top

[U34] Py：判断编码
来源：http://pix.ivvv.top

chardet.detect(raw)
来源：http://hbu.hammf.cn

[U35] Py：发送邮件
来源：http://nnq.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gdf.0kj1m.cn

[U36] Py：定时任务
来源：http://cen.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://rnr.jianghu66.top

[U37] Py：读写 Excel
来源：http://egu.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sjn.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://nir.sweek.top

Path(__file__).resolve().parent
来源：http://xgi.xingfuxueyuan.xyz

[U39] Py：判断是否在交互环境
来源：http://xhf.fzhhl.top

sys.stdout.isatty()
来源：http://oqi.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://uea.gogol.net.cn

print("err", file=sys.stderr)
来源：http://wld.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://xad.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vza.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://ulp.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://grk.bjfxy.top

[U43] PHP：声明命名空间
来源：http://mnx.ydzc1.top

namespace App\Http;
来源：http://npk.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://pcx.jinqigufen.top

declare(strict_types=1);
来源：http://zah.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://nsc.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://khl.hnqzz.top

[U46] PHP：可空类型
来源：http://fdn.birdmap.top

?string $name = null
来源：http://yxr.tarul.cn

[U47] PHP：联合类型
来源：http://zed.sufxvd.cn

int|string $id
来源：http://tia.jinqigufen.top

[U48] PHP：纯枚举
来源：http://rwv.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uys.daria6918.cn

[U49] PHP：只读属性
来源：http://okg.jqgfzy.top

public readonly string $name
来源：http://ekh.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://sdx.ctjpmb.com

public function __construct(private int $id) {}
来源：http://vhx.yfazqb.com

[U51] PHP：数组解构
来源：http://gei.meibo888.top

[$a, $b] = $arr;
来源：http://jxj.meibo888.top

[U52] PHP：箭头函数
来源：http://kez.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://lgp.pycfn.com

[U53] PHP：空合并运算符
来源：http://tdq.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://npx.hammf.cn

[U54] PHP：空安全调用
来源：http://owd.xylfe.cn

$obj?->method()
来源：http://dcu.pycfn.com

[U55] PHP：match 表达式
来源：http://jen.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tku.cashguo.top

[U56] PHP：命名参数
来源：http://ymh.epnwcf.com

f(a: 1, b: 2)
来源：http://djm.tianlin.xyz

[U57] PHP：字符串插值
来源：http://fal.xinyue.icu

"值: {$a}"
来源：http://dno.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://uof.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vfw.gotoacloud.top

[U59] PHP：自定义排序
来源：http://eio.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iex.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://ybd.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://znc.zhoulong.xyz

[U61] PHP：正则
来源：http://bsf.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mcb.kuanghao11.cn

[U62] PHP：日期对象
来源：http://iuz.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nez.fehbvm.com

[U63] PHP：文件读写
来源：http://gar.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wlu.9152youxi.cn

[U64] PHP：目录遍历
来源：http://xcd.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://bgb.guowangkeji.top

[U65] PHP：会话
来源：http://agm.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://keq.guannengcc.top

[U66] PHP：设置 Cookie
来源：http://syp.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://stf.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://mbl.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://msz.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://fvv.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hkm.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://fgb.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xzl.sxryk.cn

[U70] PHP：PDO 事务
来源：http://gas.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://afs.bbcook.cn

[U71] PHP：抛出异常
来源：http://ndb.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://cam.sysykeji.top

[U72] PHP：写错误日志
来源：http://zou.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://ixd.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://kso.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://aoi.ybcxt.top

[U74] PHP：读取环境变量
来源：http://jbd.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://adt.epnwcf.com

[U75] PHP：依赖注入
来源：http://lea.yfazqb.com

composer require psr/container
来源：http://iqu.zhongyouzk.top

[U76] PHP：简单路由
来源：http://rry.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wny.redwolf501.top

[U77] PHP：模板渲染
来源：http://wii.hfpthk.cn

composer require twig/twig
来源：http://shz.hcnkem.com

[U78] PHP：单元测试
来源：http://ahz.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://rii.guannengcc.top

[U79] PHP：静态分析
来源：http://xge.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://rxq.c1oappe.top

[U80] PHP：代码规范修复
来源：http://nxi.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://jdo.hesvh.cn

[U81] JS：初始化项目
来源：http://spv.jqgfzy.top

npm init -y;  npm i express
来源：http://idy.vehdjk.com

[U82] JS：package.json 脚本
来源：http://cgh.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ekc.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://ezp.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zqd.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://sxu.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://cpc.52xcode.cn

[U85] JS：可选链
来源：http://uoa.yanxiufei.cn

a?.b?.c
来源：http://tul.hcnkem.com

[U86] JS：空值合并
来源：http://yxs.tianlin.xyz

a ?? b
来源：http://zfq.iojbl.cn

[U87] JS：解构默认值
来源：http://zpl.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://kcx.ppjwa.cn

[U88] JS：对象展开合并
来源：http://vzu.jyoumei.cn

{ ...a, ...b }
来源：http://vpx.yfazqb.com

[U89] JS：数组去重
来源：http://sud.yvedp.cn

[...new Set(arr)]
来源：http://oxv.vehdjk.com

[U90] JS：数字数组排序
来源：http://trq.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://blm.ybcxt.top

[U91] JS：对象键值遍历
来源：http://qyq.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qlh.zdbjq.cn

[U92] JS：深拷贝
来源：http://teg.birdmap.top

structuredClone(obj)
来源：http://ihx.dianchejie.cn

[U93] JS：模板字符串
来源：http://dul.yongpay.top

`共 ${n} 条`
来源：http://kos.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://wfb.jyoumei.cn

const double = x => x * 2;
来源：http://vbc.9152youxi.cn

[U95] JS：Promise 包装
来源：http://mik.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://mlc.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://ups.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sri.gaohongyu789.top

[U97] JS：并发请求
来源：http://lla.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pwt.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://lmz.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://myp.tian-w.cn

[U99] JS：事件监听
来源：http://rze.yonumen.top

el.addEventListener("click", e => {})
来源：http://evy.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://gzu.yonumen.top

document.querySelector(".item")
来源：http://xbu.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://vqt.hysaishi.cn

el.classList.toggle("active")
来源：http://bdi.sufxvd.cn

[U102] JS：本地存储
来源：http://tri.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wgx.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://lot.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vvi.jlsjyb.cn

[U104] JS：防抖
来源：http://shq.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlm.52xcode.cn

[U105] JS：节流
来源：http://dyi.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rwa.gotoacloud.top

[U106] JS：日期格式化
来源：http://lgx.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://guh.cdnleiting.top

[U107] JS：数字千分位
来源：http://gjy.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jpt.xziqi.cn

[U108] JS：随机整数
来源：http://fbe.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://por.havefunace.top

[U109] JS：数组分组
来源：http://gkt.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://lox.yj202588.top

[U110] JS：数组分块
来源：http://jcy.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://auw.yuanzhike.top

[U111] JS：对象转 Map
来源：http://sej.birdmap.top

new Map(Object.entries(obj))
来源：http://pbh.uphjek.com

[U112] JS：字符串补位
来源：http://afr.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://eyc.yuanzhike.top

[U113] JS：正则替换全部
来源：http://vxs.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://ryq.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://ler.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://brm.daxiang520.top

[U115] JS：生成 UUID
来源：http://akh.ybcxt.top

crypto.randomUUID()
来源：http://wgc.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://ygo.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://ihp.mhx1999.top

[U117] JS：单元测试
来源：http://tao.pycfn.com

npm i -D vitest;  npx vitest
来源：http://fdp.yj202588.top

[U118] JS：开发服务器
来源：http://poa.yuanzhike.top

npm i -D vite;  npx vite
来源：http://bzy.yj20258.top

[U119] JS：生产构建
来源：http://lmr.zhengqikj.top

npx vite build
来源：http://eur.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://zyw.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://wdo.yuanzhike.top

================================================================================
来源：http://tci.yangfankeji.com

统计汇总
来源：http://aby.vqdsnc.cn

================================================================================
来源：http://ezi.jyoumei.cn

按语言统计（条）：
来源：http://zfi.hcnkem.com

Python ......... 252
来源：http://fje.hongshengwenyu.top

PHP ............ 252
来源：http://vgh.wangdashe.top

JavaScript ..... 252
来源：http://sbs.gotoacloud.top

TypeScript ..... 212
来源：http://vwb.andypj.xyz

Java ........... 212
来源：http://hnd.jinyuanbaomall.cn

Go ............. 212
来源：http://mky.hammf.cn

Ruby ........... 212
来源：http://zub.xziqi.cn

C# ............. 212
来源：http://czx.hysaishi.cn

C .............. 30
来源：http://hwb.guowangkeji.top

C++ ............ 30
来源：http://jfb.sweek.top

SQL ............ 90
来源：http://vhj.yuanzhike.top

Bash ........... 80
来源：http://lya.ctjpmb.com

Kotlin ......... 15
来源：http://dnv.yangfankeji.com

Swift .......... 15
来源：http://tgu.nanxinkj.top

Lua ............ 10
来源：http://zvg.zhijiandao.cn

Perl ........... 10
来源：http://otu.vqdsnc.cn

Scala .......... 10
来源：http://pkd.zhaomingkeji.xyz

------------------------------------
来源：http://trc.52xcode.cn

合计 ........... 2106 条
来源：http://lyu.meibo888.top

按章节统计：
来源：http://zlm.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rhp.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kpq.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eou.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ojl.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fjz.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gmi.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uju.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://alc.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sao.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://thb.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nbe.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yvu.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nga.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ceo.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nna.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wht.zhengqikj.top

Q SQL 专题                              90
来源：http://ena.kuanghao11.cn

R Bash 专题                             80
来源：http://bbt.fengsongda.top

S C / C++ 专题                          60
来源：http://aqa.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://ziq.yongpay.top

U 高频实用片段                         120
来源：http://tib.hcnkem.com

------------------------------------
来源：http://nic.daria6918.cn

合计                                  2106 条
来源：http://chi.yvedp.cn

--------------------------------------------------------------------------------
来源：http://cwo.xingfuxueyuan.xyz

使用提醒
来源：http://jht.fehbvm.com

--------------------------------------------------------------------------------
来源：http://rvl.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://str.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gdo.feifeiyinyue.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fiz.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jmh.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mew.zhijiandao.cn

—— 文件结束 ——
来源：http://xpr.cucudq.cn

================================================================================
来源：http://cfo.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://rdd.ybcxt.top

Common Programming Examples Cheat Book
来源：http://wdt.tian-w.cn

================================================================================
来源：http://ptm.fehbvm.com

【收录内容】
来源：http://lkh.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jcv.ivvv.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ezx.pengpengdd.cyou

SQL · Bash · C · C++
来源：http://twc.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tdu.jyoumei.cn

【使用说明】
来源：http://swj.fehbvm.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rzw.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ust.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lac.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qki.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://oiu.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bwv.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xyu.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vyj.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qrv.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nll.wangdashe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://moe.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://azd.ydjk.org.cn

【文件统计】
来源：http://pzj.shangyingyoupin.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ymt.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://qqi.gzhubu.top

目  录
来源：http://ylp.hesvh.cn

--------------------------------------------------------------------------------
来源：http://qzo.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ncq.aibaodan.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ylu.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uqd.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yes.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wid.yanxiufei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tka.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gxc.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aqw.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mtf.birdmap.top


<!-- 参考信息 -->