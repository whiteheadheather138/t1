代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://kwo.fengsongda.top

[T51] Scala：Hello World
来源：http://qjd.cheryme.top

println("Hello")
来源：http://rhf.guowangkeji.top

[T52] Scala：变量
来源：http://tgo.guowangkeji.top

val a = 1;  var b = 2
来源：http://ffi.redwolf501.top

[T53] Scala：字符串插值
来源：http://mpu.zhaomingkeji.xyz

s"值: $b"
来源：http://gxk.yuanzhike.top

[T54] Scala：集合映射
来源：http://tji.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://efy.hysaishi.cn

[T55] Scala：集合过滤
来源：http://xqz.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yny.hongshengwenyu.top

[T56] Scala：样例类
来源：http://xwq.redwolf501.top

case class User(name: String, age: Int)
来源：http://yxz.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://opw.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://bro.tian-w.cn

[T58] Scala：函数定义
来源：http://xnr.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://leb.gotoacloud.top

[T59] Scala：循环
来源：http://hkd.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://lgb.aibaodan.cn

[T60] Scala：折叠
来源：http://ayt.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qbw.shangyingyoupin.top

================================================================================
来源：http://jxo.xinyue.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gce.hammf.cn

================================================================================
来源：http://vwn.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://jag.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://isw.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://ani.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jkr.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://ggv.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vsh.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://bud.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kce.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://ejt.bbcook.cn

list(dict.fromkeys(arr))
来源：http://xvv.ehwqpu.com

[U06] Py：合并两个字典
来源：http://hjo.jiagoushi.top

{**a, **b}
来源：http://nil.guannengcc.top

[U07] Py：反转字典键值
来源：http://qcm.hcnkem.com

{v: k for k, v in d.items()}
来源：http://nxn.andypj.xyz

[U08] Py：展平二维列表
来源：http://aed.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://wqh.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://trz.guannengcc.top

max(d, key=d.get)
来源：http://fkp.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://oru.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vgy.andypj.xyz

[U11] Py：生成器表达式
来源：http://cze.ybcxt.top

(x * 2 for x in arr)
来源：http://llt.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://lbx.tarul.cn

Counter(arr).most_common(3)
来源：http://ynn.wangdashe.top

[U13] Py：固定长度队列
来源：http://epf.yuxming.cn

deque(maxlen=10)
来源：http://tcu.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://fjs.feifeiyinyue.top

defaultdict(list)
来源：http://ohe.iojbl.cn

[U15] Py：高精度计时
来源：http://nhy.gaohongyu789.top

t = time.perf_counter()
来源：http://hcl.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://hvp.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tfq.0kj1m.cn

[U17] Py：初始化日志
来源：http://wnj.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://ghx.xingfuxueyuan.xyz

[U18] Py：预编译正则
来源：http://twl.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://jpv.yj202588.top

[U19] Py：正则替换带回调
来源：http://bdz.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rfm.pycfn.com

[U20] Py：缓存函数结果
来源：http://ixi.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://ikb.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://tkr.aizwys.cn

@contextlib.contextmanager
来源：http://zss.xylfe.cn

[U22] Py：矩阵转置
来源：http://nvp.shanyushiyangtech.top

list(zip(*m))
来源：http://xou.jianghu66.top

[U23] Py：分块读取大文件
来源：http://tif.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sok.aibaodan.cn

[U24] Py：路径操作
来源：http://nla.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dwa.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://lta.havefunace.top

csv.DictReader(f)
来源：http://yzx.jyoumei.cn

[U26] Py：并发下载
来源：http://wrb.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hwk.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://qbs.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://hjv.meibo888.top

[U28] Py：类型别名
来源：http://soz.zhijiandao.cn

UserId = int
来源：http://fwi.jqgfzy.top

[U29] Py：属性校验
来源：http://qxp.yangfankeji.com

@property 与 @x.setter 配合
来源：http://lct.zhiwuduotai.top

[U30] Py：数据类
来源：http://lof.52xcode.cn

@dataclass(slots=True)
来源：http://axn.ydjk.org.cn

[U31] Py：单测
来源：http://gpg.shanyushiyangkeji.top

python -m pytest -q
来源：http://apu.cucudq.cn

[U32] Py：代码格式化
来源：http://tds.cheryme.top

ruff format . && ruff check --fix .
来源：http://als.bjfxy.top

[U33] Py：打包发布
来源：http://qmb.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://gnm.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://rws.jinghuilouyu.cn

chardet.detect(raw)
来源：http://vyv.zdbjq.cn

[U35] Py：发送邮件
来源：http://zkh.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cwt.yueranfly.top

[U36] Py：定时任务
来源：http://zzo.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://qwa.havefunace.top

[U37] Py：读写 Excel
来源：http://btt.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://wdq.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://uhy.guowangkeji.top

Path(__file__).resolve().parent
来源：http://nrq.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://xyu.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://vlx.yongpay.top

[U40] Py：打印到标准错误
来源：http://cnp.epnwcf.com

print("err", file=sys.stderr)
来源：http://cly.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://uap.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vic.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://bii.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://evn.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://tnj.sysykeji.top

namespace App\Http;
来源：http://jpc.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://pwr.jianghu66.top

declare(strict_types=1);
来源：http://aci.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://dqi.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://dtg.svipenyu.cn

[U46] PHP：可空类型
来源：http://fdq.cqqwz.cn

?string $name = null
来源：http://vxl.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://lsd.guowangkeji.top

int|string $id
来源：http://iyx.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://ekn.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qcg.zhongyouzk.top

[U49] PHP：只读属性
来源：http://nrx.cdnleiting.top

public readonly string $name
来源：http://mzp.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://dbb.daxiang520.top

public function __construct(private int $id) {}
来源：http://uag.bbcook.cn

[U51] PHP：数组解构
来源：http://hxw.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://lwl.tian-w.cn

[U52] PHP：箭头函数
来源：http://zaq.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://stb.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://dkv.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://afz.hammf.cn

[U54] PHP：空安全调用
来源：http://yki.wangdashe.top

$obj?->method()
来源：http://ril.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://ezg.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jjd.yj20258.top

[U56] PHP：命名参数
来源：http://nzy.gaohongyu789.top

f(a: 1, b: 2)
来源：http://uqu.svipenyu.cn

[U57] PHP：字符串插值
来源：http://mma.redwolf501.top

"值: {$a}"
来源：http://qar.nwbrower.top

[U58] PHP：数组三件套
来源：http://cvj.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rfe.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://fse.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://spt.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://lue.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ftg.chenjidiqi.icu

[U61] PHP：正则
来源：http://lik.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tdt.xuanzx.com

[U62] PHP：日期对象
来源：http://zun.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gyr.yfazqb.com

[U63] PHP：文件读写
来源：http://duj.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pxv.birdmap.top

[U64] PHP：目录遍历
来源：http://vbo.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://blw.nwbrower.top

[U65] PHP：会话
来源：http://dno.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wzl.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://pzw.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://usd.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://oxi.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ryb.bbcook.cn

[U68] PHP：PDO 连接
来源：http://qvk.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hxf.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://jao.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jdn.pycfn.com

[U70] PHP：PDO 事务
来源：http://zlh.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zsj.cqqwz.cn

[U71] PHP：抛出异常
来源：http://ssr.havefunace.top

throw new RuntimeException("失败", 500);
来源：http://kuf.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://rcm.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://ole.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://gya.cheryme.top

parse_ini_file("config.ini", true)
来源：http://xjh.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://cul.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://bnn.cashguo.top

[U75] PHP：依赖注入
来源：http://cvj.ctjpmb.com

composer require psr/container
来源：http://brg.zdqjudy.top

[U76] PHP：简单路由
来源：http://maq.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zkr.vehdjk.com

[U77] PHP：模板渲染
来源：http://vhi.hysaishi.cn

composer require twig/twig
来源：http://rwb.hywenlv.cn

[U78] PHP：单元测试
来源：http://yti.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://dou.svipenyu.cn

[U79] PHP：静态分析
来源：http://qtr.havefunace.top

composer require --dev phpstan/phpstan
来源：http://xhf.cucudq.cn

[U80] PHP：代码规范修复
来源：http://zrt.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uva.ydjk.org.cn

[U81] JS：初始化项目
来源：http://mmn.hfpthk.cn

npm init -y;  npm i express
来源：http://ntd.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://hxj.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ihp.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://nsu.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://zzo.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://ioe.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://gdf.guannengcc.top

[U85] JS：可选链
来源：http://uzt.cashguo.top

a?.b?.c
来源：http://gmk.fehbvm.com

[U86] JS：空值合并
来源：http://dze.fktsv.cn

a ?? b
来源：http://iwm.andypj.xyz

[U87] JS：解构默认值
来源：http://vey.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://lop.ctjpmb.com

[U88] JS：对象展开合并
来源：http://eza.0kj1m.cn

{ ...a, ...b }
来源：http://iex.xinyue.icu

[U89] JS：数组去重
来源：http://zhd.bjfxy.top

[...new Set(arr)]
来源：http://ztc.bbcook.cn

[U90] JS：数字数组排序
来源：http://vhe.sweek.top

[...arr].sort((a, b) => a - b)
来源：http://yqr.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://quu.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vzq.jianghu66.top

[U92] JS：深拷贝
来源：http://zde.yj20258.top

structuredClone(obj)
来源：http://jtr.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://ufg.xinyue.icu

`共 ${n} 条`
来源：http://ykp.ehwqpu.com

[U94] JS：箭头函数
来源：http://oqx.guowangkeji.top

const double = x => x * 2;
来源：http://qnp.hesvh.cn

[U95] JS：Promise 包装
来源：http://nli.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://ppr.fengsongda.top

[U96] JS：async/await 与异常
来源：http://qyv.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lou.tianlin.xyz

[U97] JS：并发请求
来源：http://nhh.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jkr.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://fgn.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yjd.zdbjq.cn

[U99] JS：事件监听
来源：http://ntz.pycfn.com

el.addEventListener("click", e => {})
来源：http://npr.guannengcc.top

[U100] JS：DOM 查询
来源：http://shw.xinyue.icu

document.querySelector(".item")
来源：http://guf.zhongyouzk.top

[U101] JS：classList 操作
来源：http://hso.quarkkingdee.top

el.classList.toggle("active")
来源：http://qhr.hnqzz.top

[U102] JS：本地存储
来源：http://stg.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ond.jyoumei.cn

[U103] JS：定时器
来源：http://rdi.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hwh.yongpay.top

[U104] JS：防抖
来源：http://wqb.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uaw.pycfn.com

[U105] JS：节流
来源：http://gzj.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kke.zhixingplan.top

[U106] JS：日期格式化
来源：http://iwd.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kfg.sysykeji.top

[U107] JS：数字千分位
来源：http://rcd.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cea.hcnkem.com

[U108] JS：随机整数
来源：http://bnr.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jik.cucudq.cn

[U109] JS：数组分组
来源：http://xoe.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://bsf.c1oappe.top

[U110] JS：数组分块
来源：http://woz.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wch.fehbvm.com

[U111] JS：对象转 Map
来源：http://qxj.chenzaomai.com

new Map(Object.entries(obj))
来源：http://hhb.yvedp.cn

[U112] JS：字符串补位
来源：http://lrm.52xcode.cn

"7".padStart(3, "0")
来源：http://qpi.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://igi.aibaodan.cn

s.replaceAll("a", "b")
来源：http://mli.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://roy.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kgy.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://fxp.wangshuangyany.cn

crypto.randomUUID()
来源：http://bry.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://mxe.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://dlo.yj202588.top

[U117] JS：单元测试
来源：http://ggq.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://ivd.yj202588.top

[U118] JS：开发服务器
来源：http://wkt.andypj.xyz

npm i -D vite;  npx vite
来源：http://rds.bjfxy.top

[U119] JS：生产构建
来源：http://pcx.redwolf501.top

npx vite build
来源：http://dfw.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://uhs.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://duc.aibaodan.cn

================================================================================
来源：http://ifu.kuanghao11.cn

统计汇总
来源：http://ems.uphjek.com

================================================================================
来源：http://irn.jqgufenzy.top

按语言统计（条）：
来源：http://cau.jqgufenzy.top

Python ......... 252
来源：http://cal.yanxiufei.cn

PHP ............ 252
来源：http://pzd.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://nlp.xuetiantiany.cn

TypeScript ..... 212
来源：http://ulg.yuxming.cn

Java ........... 212
来源：http://srh.mhx1999.top

Go ............. 212
来源：http://uuo.birdmap.top

Ruby ........... 212
来源：http://mri.vehdjk.com

C# ............. 212
来源：http://brm.gogol.net.cn

C .............. 30
来源：http://jps.hysaishi.cn

C++ ............ 30
来源：http://kei.pengpengdd.cyou

SQL ............ 90
来源：http://hwx.cqqwz.cn

Bash ........... 80
来源：http://zbp.dashuyun.cn

Kotlin ......... 15
来源：http://osd.fktsv.cn

Swift .......... 15
来源：http://ljm.c1oappe.top

Lua ............ 10
来源：http://yzg.ydjk.org.cn

Perl ........... 10
来源：http://esh.zhoulong.xyz

Scala .......... 10
来源：http://gxi.vehdjk.com

------------------------------------
来源：http://drx.zdqjudy.top

合计 ........... 2106 条
来源：http://dod.chenzaomai.com

按章节统计：
来源：http://kiw.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vzd.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ufn.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dwx.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ayw.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qqy.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cal.jiagoushi.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qni.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ghx.xziqi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lxf.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gzn.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zei.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mmb.chenlongwang.top


<!-- 参考信息 -->