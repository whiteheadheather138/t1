代发 wailian999

case class User(name: String, age: Int)
来源：http://ume.ydzc1.top

[T57] Scala：模式匹配
来源：http://hde.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hfq.tarul.cn

[T58] Scala：函数定义
来源：http://nxc.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://imk.zhoulong.xyz

[T59] Scala：循环
来源：http://jzb.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://ihe.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://tcn.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hdt.hywenlv.cn

================================================================================
来源：http://gxt.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fhb.cqqwz.cn

================================================================================
来源：http://lql.yuxming.cn

[U01] Py：创建虚拟环境
来源：http://wav.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wrl.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://vge.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xjq.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://yyv.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mnh.bjfxy.top

[U04] Py：变量调试打印
来源：http://zag.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bjl.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://upi.redwolf501.top

list(dict.fromkeys(arr))
来源：http://kkd.epnwcf.com

[U06] Py：合并两个字典
来源：http://dmp.zdbjq.cn

{**a, **b}
来源：http://zni.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://kgu.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://hfg.yfazqb.com

[U08] Py：展平二维列表
来源：http://fnr.fzhhl.top

[y for x in nested for y in x]
来源：http://ker.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://aav.xinyue.icu

max(d, key=d.get)
来源：http://jmb.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://nzt.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nak.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://iso.cdnleiting.top

(x * 2 for x in arr)
来源：http://cpc.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://fhp.52xcode.cn

Counter(arr).most_common(3)
来源：http://klk.yonumen.top

[U13] Py：固定长度队列
来源：http://tpd.xziqi.cn

deque(maxlen=10)
来源：http://azl.yueranfly.top

[U14] Py：分组收集到列表
来源：http://dcw.zhoulong.xyz

defaultdict(list)
来源：http://skh.havefunace.top

[U15] Py：高精度计时
来源：http://ngq.hywenlv.cn

t = time.perf_counter()
来源：http://iet.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://eaz.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kxn.ybcxt.top

[U17] Py：初始化日志
来源：http://jyh.uphjek.com

logging.basicConfig(level=logging.INFO)
来源：http://pem.yj202588.top

[U18] Py：预编译正则
来源：http://lad.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://bpa.ybcxt.top

[U19] Py：正则替换带回调
来源：http://ddh.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ugv.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://xnq.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://mbs.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://sae.sysykeji.top

@contextlib.contextmanager
来源：http://xch.fehbvm.com

[U22] Py：矩阵转置
来源：http://dax.haohaochexian.top

list(zip(*m))
来源：http://xiz.yueranfly.top

[U23] Py：分块读取大文件
来源：http://psd.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ise.tarul.cn

[U24] Py：路径操作
来源：http://zyk.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lsq.havefunace.top

[U25] Py：CSV 按字典读
来源：http://ohw.yfazqb.com

csv.DictReader(f)
来源：http://vls.52xcode.cn

[U26] Py：并发下载
来源：http://vls.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tfe.epnwcf.com

[U27] Py：异步 HTTP
来源：http://rcq.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://qob.uphjek.com

[U28] Py：类型别名
来源：http://eix.hesvh.cn

UserId = int
来源：http://gzw.yuxming.cn

[U29] Py：属性校验
来源：http://rat.chenlongwang.top

@property 与 @x.setter 配合
来源：http://ezw.9152youxi.cn

[U30] Py：数据类
来源：http://hyb.nanxinkj.top

@dataclass(slots=True)
来源：http://uof.mhx1999.top

[U31] Py：单测
来源：http://dku.yfazqb.com

python -m pytest -q
来源：http://ace.bjfxy.top

[U32] Py：代码格式化
来源：http://ets.yonumen.top

ruff format . && ruff check --fix .
来源：http://bpu.ydjk.org.cn

[U33] Py：打包发布
来源：http://ukh.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://bsm.sxryk.cn

[U34] Py：判断编码
来源：http://mbq.jinqigfzy.top

chardet.detect(raw)
来源：http://akx.ydzc1.top

[U35] Py：发送邮件
来源：http://tnn.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ewv.guowangkeji.top

[U36] Py：定时任务
来源：http://cbw.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://xjk.guowangkeji.top

[U37] Py：读写 Excel
来源：http://jdj.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ntj.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://iqt.zdbjq.cn

Path(__file__).resolve().parent
来源：http://whj.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://qgk.ctjpmb.com

sys.stdout.isatty()
来源：http://ckg.tian-w.cn

[U40] Py：打印到标准错误
来源：http://yrl.havefunace.top

print("err", file=sys.stderr)
来源：http://qpa.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://ekr.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://igx.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://qwk.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bje.meibo888.top

[U43] PHP：声明命名空间
来源：http://iwv.shanyushiyangkeji.top

namespace App\Http;
来源：http://rkx.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://chp.guowangkeji.top

declare(strict_types=1);
来源：http://qap.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://waw.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://plo.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://jmx.smart0.xyz

?string $name = null
来源：http://xpi.zycfv.cn

[U47] PHP：联合类型
来源：http://obx.shanyushiyangtech.top

int|string $id
来源：http://vnq.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://mna.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ynh.hfpthk.cn

[U49] PHP：只读属性
来源：http://dxp.chenjidiqi.icu

public readonly string $name
来源：http://hdx.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://orv.tarul.cn

public function __construct(private int $id) {}
来源：http://ndz.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://kar.daxiang520.top

[$a, $b] = $arr;
来源：http://flm.hywenlv.cn

[U52] PHP：箭头函数
来源：http://cvk.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://rer.9152youxi.cn

[U53] PHP：空合并运算符
来源：http://sjk.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://zhf.316326.xyz

[U54] PHP：空安全调用
来源：http://apf.jlsjyb.cn

$obj?->method()
来源：http://txi.jinqigufen.top

[U55] PHP：match 表达式
来源：http://zzs.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aho.cqqwz.cn

[U56] PHP：命名参数
来源：http://skj.yj20258.top

f(a: 1, b: 2)
来源：http://kif.hywenlv.cn

[U57] PHP：字符串插值
来源：http://sgh.hnxiangtu.top

"值: {$a}"
来源：http://lgm.yfazqb.com

[U58] PHP：数组三件套
来源：http://ndt.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nch.daria6918.cn

[U59] PHP：自定义排序
来源：http://lud.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izn.dianchejie.cn

[U60] PHP：JSON 编解码
来源：http://jwq.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ndy.gaohongyu789.top

[U61] PHP：正则
来源：http://ijl.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mvl.sjlbkw.cn

[U62] PHP：日期对象
来源：http://vkq.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://axy.xinyue.icu

[U63] PHP：文件读写
来源：http://qqp.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://djd.aibaodan.cn

[U64] PHP：目录遍历
来源：http://mzd.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://joq.hongshengwenyu.top

[U65] PHP：会话
来源：http://ifw.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://asr.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://pob.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ehq.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://ybn.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qcm.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://tgd.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://khv.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://sby.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://skp.xinyue.icu

[U70] PHP：PDO 事务
来源：http://nla.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kgs.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://att.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://eje.daria6918.cn

[U72] PHP：写错误日志
来源：http://woc.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://veo.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://ndr.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://jmd.yongpay.top

[U74] PHP：读取环境变量
来源：http://acl.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://gzi.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://wkx.hammf.cn

composer require psr/container
来源：http://cxx.jianghu66.top

[U76] PHP：简单路由
来源：http://xbk.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ahq.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://qys.jlsjyb.cn

composer require twig/twig
来源：http://ddt.ehwqpu.com

[U78] PHP：单元测试
来源：http://wll.cashguo.top

composer require --dev phpunit/phpunit
来源：http://tsm.ivvv.top

[U79] PHP：静态分析
来源：http://xvc.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://ayk.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://tad.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jny.yongpay.top

[U81] JS：初始化项目
来源：http://xke.yueranfly.top

npm init -y;  npm i express
来源：http://pit.tian-w.cn

[U82] JS：package.json 脚本
来源：http://ukg.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oeg.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://nst.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://ivi.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://azb.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://pbc.uphjek.com

[U85] JS：可选链
来源：http://muk.ctjpmb.com

a?.b?.c
来源：http://oqp.jiagoushi.top

[U86] JS：空值合并
来源：http://czo.sysykeji.top

a ?? b
来源：http://axo.kuanghao11.cn

[U87] JS：解构默认值
来源：http://nja.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://pxp.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://yqx.ywan-chungtsiang.top

{ ...a, ...b }
来源：http://luq.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://ctj.havefunace.top

[...new Set(arr)]
来源：http://cjw.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://qry.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://ugn.yonumen.top

[U91] JS：对象键值遍历
来源：http://gqc.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://acn.shzxlz.cn

[U92] JS：深拷贝
来源：http://bqw.zhongyouzk.top

structuredClone(obj)
来源：http://wdd.epnwcf.com

[U93] JS：模板字符串
来源：http://rki.jqgufenzy.top

`共 ${n} 条`
来源：http://lbs.havefunace.top

[U94] JS：箭头函数
来源：http://xbi.yongpay.top

const double = x => x * 2;
来源：http://ytt.haohaochexian.top

[U95] JS：Promise 包装
来源：http://zre.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://wwx.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://dgg.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ddh.gzhubu.top

[U97] JS：并发请求
来源：http://zzi.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://akn.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://tua.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://osj.ivvv.top

[U99] JS：事件监听
来源：http://tmx.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://zic.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://bxk.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://tgu.vehdjk.com

[U101] JS：classList 操作
来源：http://srt.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://was.ehwqpu.com

[U102] JS：本地存储
来源：http://jxb.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://gmr.fengsongda.top

[U103] JS：定时器
来源：http://ulp.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rlw.hongshengwenyu.top

[U104] JS：防抖
来源：http://uvh.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jzj.fengsongda.top

[U105] JS：节流
来源：http://klc.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uvw.iojbl.cn

[U106] JS：日期格式化
来源：http://inx.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jax.guannengcc.top

[U107] JS：数字千分位
来源：http://akw.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://foa.sjlbkw.cn

[U108] JS：随机整数
来源：http://qtn.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nrc.wangshuangyany.cn

[U109] JS：数组分组
来源：http://zww.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://ryd.daria6918.cn

[U110] JS：数组分块
来源：http://ykj.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ydo.epnwcf.com

[U111] JS：对象转 Map
来源：http://bqt.cashguo.top

new Map(Object.entries(obj))
来源：http://you.chenlongwang.top

[U112] JS：字符串补位
来源：http://rze.redwolf501.top

"7".padStart(3, "0")
来源：http://cyz.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://xct.yuanzhike.top

s.replaceAll("a", "b")
来源：http://chs.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://bqb.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zal.yj202588.top

[U115] JS：生成 UUID
来源：http://upa.sjlbkw.cn

crypto.randomUUID()
来源：http://ezf.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://pmm.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://asc.vqdsnc.cn

[U117] JS：单元测试
来源：http://scl.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://tir.daxiang520.top

[U118] JS：开发服务器
来源：http://tiu.yj20258888.top

npm i -D vite;  npx vite
来源：http://xwy.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://bmd.havefunace.top

npx vite build
来源：http://utn.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://ghx.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://ycu.dashuyun.cn

================================================================================
来源：http://dsj.redwolf501.top

统计汇总
来源：http://inu.cucudq.cn

================================================================================
来源：http://xha.aibaodan.cn

按语言统计（条）：
来源：http://rgq.yonumen.top

Python ......... 252
来源：http://vrk.zhongyouzk.top

PHP ............ 252
来源：http://jop.sjlbkw.cn

JavaScript ..... 252
来源：http://kvd.daxiang520.top

TypeScript ..... 212
来源：http://kor.fanxiaobao.xyz

Java ........... 212
来源：http://kqg.cashguo.top

Go ............. 212
来源：http://lah.hesvh.cn

Ruby ........... 212
来源：http://niv.fktsv.cn

C# ............. 212
来源：http://mkc.pengpengdd.cyou

C .............. 30
来源：http://vdb.shanyushiyangtech.top

C++ ............ 30
来源：http://iff.epnwcf.com

SQL ............ 90
来源：http://ujn.sysykeji.top

Bash ........... 80
来源：http://lsg.dianchejie.cn

Kotlin ......... 15
来源：http://gmn.birdmap.top

Swift .......... 15
来源：http://aug.yj20258888.top

Lua ............ 10
来源：http://fli.shuidangran.top

Perl ........... 10
来源：http://kon.sysykeji.top

Scala .......... 10
来源：http://asr.hfpthk.cn

------------------------------------
来源：http://bwk.shangyingyoupin.top

合计 ........... 2106 条
来源：http://fhp.tanke756.top

按章节统计：
来源：http://tnj.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iks.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jgi.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://udl.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vpz.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ttg.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wop.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://geq.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yny.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://era.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jxg.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qle.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jzg.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ahe.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ybe.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xbe.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zrm.hesvh.cn

Q SQL 专题                              90
来源：http://ipz.shuidangran.top

R Bash 专题                             80
来源：http://zgk.ctjpmb.com

S C / C++ 专题                          60
来源：http://fdu.hnxiangtu.top

T 其他语言补充                          60
来源：http://jfi.ctjpmb.com

U 高频实用片段                         120
来源：http://yze.andypj.xyz

------------------------------------
来源：http://yyp.guannengcc.top

合计                                  2106 条
来源：http://mfy.tanke756.top

--------------------------------------------------------------------------------
来源：http://zuf.hfpthk.cn


<!-- 参考信息 -->