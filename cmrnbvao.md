代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://ctl.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://nla.yueranfly.top

println("Hello")
来源：http://qpo.redwolf501.top

[T52] Scala：变量
来源：http://brn.tarul.cn

val a = 1;  var b = 2
来源：http://bcm.chenzaomai.com

[T53] Scala：字符串插值
来源：http://cil.ppjwa.cn

s"值: $b"
来源：http://lkw.yj20258.top

[T54] Scala：集合映射
来源：http://pta.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://rjs.ybcxt.top

[T55] Scala：集合过滤
来源：http://sxn.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://xis.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://ill.iojbl.cn

case class User(name: String, age: Int)
来源：http://qvf.jinqigufen.top

[T57] Scala：模式匹配
来源：http://qru.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jgs.zdbjq.cn

[T58] Scala：函数定义
来源：http://ush.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://xup.zdbjq.cn

[T59] Scala：循环
来源：http://yrz.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://lse.52xcode.cn

[T60] Scala：折叠
来源：http://ssa.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eaw.sufxvd.cn

================================================================================
来源：http://pys.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nod.haohaochexian.top

================================================================================
来源：http://qes.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://yqc.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://otk.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://qzd.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dgf.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://lal.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tyu.yj20258.top

[U04] Py：变量调试打印
来源：http://cna.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mei.daxiang520.top

[U05] Py：列表去重且保序
来源：http://uhr.sysykeji.top

list(dict.fromkeys(arr))
来源：http://rmm.epnwcf.com

[U06] Py：合并两个字典
来源：http://xoa.zhengqikj.top

{**a, **b}
来源：http://ccj.yangfankeji.com

[U07] Py：反转字典键值
来源：http://rsc.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://orz.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://cgs.daxiang520.top

[y for x in nested for y in x]
来源：http://tqf.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://bni.vqdsnc.cn

max(d, key=d.get)
来源：http://oyr.dianchejie.cn

[U10] Py：按值排序字典
来源：http://kol.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kxi.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://doc.yvedp.cn

(x * 2 for x in arr)
来源：http://shl.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uen.shuidangran.top

Counter(arr).most_common(3)
来源：http://bmt.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://ioz.guannengcc.top

deque(maxlen=10)
来源：http://wqq.guannengcc.top

[U14] Py：分组收集到列表
来源：http://qkn.bbcook.cn

defaultdict(list)
来源：http://mrz.cdnleiting.top

[U15] Py：高精度计时
来源：http://uba.nwbrower.top

t = time.perf_counter()
来源：http://anh.xylfe.cn

[U16] Py：命令行参数解析
来源：http://jlp.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hjx.ybcxt.top

[U17] Py：初始化日志
来源：http://uog.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://qka.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://sql.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://ozn.hcnkem.com

[U19] Py：正则替换带回调
来源：http://mid.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qvy.yuxming.cn

[U20] Py：缓存函数结果
来源：http://yxa.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://adh.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://ghu.tianlin.xyz

@contextlib.contextmanager
来源：http://ric.andypj.xyz

[U22] Py：矩阵转置
来源：http://svg.52xcode.cn

list(zip(*m))
来源：http://iap.yongpay.top

[U23] Py：分块读取大文件
来源：http://rze.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zfy.yj202588.top

[U24] Py：路径操作
来源：http://uop.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oel.birdmap.top

[U25] Py：CSV 按字典读
来源：http://gcy.dashuyun.cn

csv.DictReader(f)
来源：http://xgd.zdqjudy.top

[U26] Py：并发下载
来源：http://zat.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://swh.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://roe.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://scy.zycfv.cn

[U28] Py：类型别名
来源：http://alx.hcnkem.com

UserId = int
来源：http://mrr.smart0.xyz

[U29] Py：属性校验
来源：http://wpc.smart0.xyz

@property 与 @x.setter 配合
来源：http://inb.fktsv.cn

[U30] Py：数据类
来源：http://lyg.hongshengwenyu.top

@dataclass(slots=True)
来源：http://lct.yueranfly.top

[U31] Py：单测
来源：http://iog.smart0.xyz

python -m pytest -q
来源：http://jzr.yvedp.cn

[U32] Py：代码格式化
来源：http://fae.yuxming.cn

ruff format . && ruff check --fix .
来源：http://cvx.snrcjt.cn

[U33] Py：打包发布
来源：http://txd.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://poa.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://dfy.yonumen.top

chardet.detect(raw)
来源：http://chd.hysaishi.cn

[U35] Py：发送邮件
来源：http://rtu.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uxx.cqqwz.cn

[U36] Py：定时任务
来源：http://nkb.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://kla.yongpay.top

[U37] Py：读写 Excel
来源：http://axy.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://dpx.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://ayw.ybcxt.top

Path(__file__).resolve().parent
来源：http://zba.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://bym.sweek.top

sys.stdout.isatty()
来源：http://rzs.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://gmz.vehdjk.com

print("err", file=sys.stderr)
来源：http://hyk.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://tzt.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hbt.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://fvy.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cgt.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://baw.yj20258.top

namespace App\Http;
来源：http://ewr.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://ffo.xziqi.cn

declare(strict_types=1);
来源：http://lqx.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://slt.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gdl.guannengcc.top

[U46] PHP：可空类型
来源：http://klf.quarkkingdee.top

?string $name = null
来源：http://kbx.sweek.top

[U47] PHP：联合类型
来源：http://ziv.ehwqpu.com

int|string $id
来源：http://tss.iojbl.cn

[U48] PHP：纯枚举
来源：http://yyq.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dky.cheryme.top

[U49] PHP：只读属性
来源：http://mdu.yj20258.top

public readonly string $name
来源：http://gxe.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://flv.yj20258.top

public function __construct(private int $id) {}
来源：http://yal.nanxuanxn.top

[U51] PHP：数组解构
来源：http://ykw.smart0.xyz

[$a, $b] = $arr;
来源：http://hpf.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://wys.uphjek.com

$double = fn($x) => $x * 2;
来源：http://hdh.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://tdt.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://iub.yfazqb.com

[U54] PHP：空安全调用
来源：http://vfy.aizwys.cn

$obj?->method()
来源：http://vey.yvedp.cn

[U55] PHP：match 表达式
来源：http://kom.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://obk.haohaochexian.top

[U56] PHP：命名参数
来源：http://jfi.yueranfly.top

f(a: 1, b: 2)
来源：http://wwy.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://hhn.xingfuxueyuan.xyz

"值: {$a}"
来源：http://ycl.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://irx.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bfe.xinyue.icu

[U59] PHP：自定义排序
来源：http://ogi.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://skg.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://job.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mak.yj20258.top

[U61] PHP：正则
来源：http://ork.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vtp.c1oappe.top

[U62] PHP：日期对象
来源：http://pmi.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qke.jinqigufen.top

[U63] PHP：文件读写
来源：http://vtv.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://njk.wangdashe.top

[U64] PHP：目录遍历
来源：http://uex.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://wlj.cheryme.top

[U65] PHP：会话
来源：http://wos.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rls.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://yrn.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aus.ivvv.top

[U67] PHP：处理文件上传
来源：http://ber.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugy.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://bhm.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ilk.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://cye.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zlq.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://dgz.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bmt.ehwqpu.com

[U71] PHP：抛出异常
来源：http://dqs.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://izh.nanxinkj.top

[U72] PHP：写错误日志
来源：http://ezt.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://oey.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://nlu.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://sfu.hesvh.cn

[U74] PHP：读取环境变量
来源：http://qpo.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://qoc.tarul.cn

[U75] PHP：依赖注入
来源：http://egv.gaohongyu789.top

composer require psr/container
来源：http://djk.bjfxy.top

[U76] PHP：简单路由
来源：http://ppy.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ctd.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://qxh.jinqigfzy.top

composer require twig/twig
来源：http://tdq.yangfankeji.com

[U78] PHP：单元测试
来源：http://nqu.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://yhj.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://eti.tanke756.top

composer require --dev phpstan/phpstan
来源：http://jmr.nwbrower.top

[U80] PHP：代码规范修复
来源：http://ttl.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xka.fktsv.cn

[U81] JS：初始化项目
来源：http://dkf.havefunace.top

npm init -y;  npm i express
来源：http://hov.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://djt.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ora.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://uro.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fkl.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://taq.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wun.meibo888.top

[U85] JS：可选链
来源：http://fgq.wangdashe.top

a?.b?.c
来源：http://ilz.hcnkem.com

[U86] JS：空值合并
来源：http://zvf.sjlbkw.cn

a ?? b
来源：http://fer.hywenlv.cn

[U87] JS：解构默认值
来源：http://kut.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://bpe.sxryk.cn

[U88] JS：对象展开合并
来源：http://nfn.chenjidiqi.icu

{ ...a, ...b }
来源：http://uhz.meibo888.top

[U89] JS：数组去重
来源：http://oth.jiagoushi.top

[...new Set(arr)]
来源：http://tyw.ivvv.top

[U90] JS：数字数组排序
来源：http://awc.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://aqd.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://lnl.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://swn.gaohongyu789.top

[U92] JS：深拷贝
来源：http://spk.zhaomingkeji.xyz

structuredClone(obj)
来源：http://wpb.shzxlz.cn

[U93] JS：模板字符串
来源：http://qci.fehbvm.com

`共 ${n} 条`
来源：http://fen.snrcjt.cn

[U94] JS：箭头函数
来源：http://bbv.daxiang520.top

const double = x => x * 2;
来源：http://has.ydzc1.top

[U95] JS：Promise 包装
来源：http://yhm.cashguo.top

new Promise((resolve, reject) => {})
来源：http://bqk.cashguo.top

[U96] JS：async/await 与异常
来源：http://vcb.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qtf.yonumen.top

[U97] JS：并发请求
来源：http://fgz.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ydf.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://xbv.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aja.aizwys.cn

[U99] JS：事件监听
来源：http://add.xinyue.icu

el.addEventListener("click", e => {})
来源：http://egz.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://bfy.sufxvd.cn

document.querySelector(".item")
来源：http://ycc.quarkkingdee.top

[U101] JS：classList 操作
来源：http://okb.zhijiandao.cn

el.classList.toggle("active")
来源：http://txb.snrcjt.cn

[U102] JS：本地存储
来源：http://mls.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://nwn.daxiang520.top

[U103] JS：定时器
来源：http://jxt.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://swv.fktsv.cn

[U104] JS：防抖
来源：http://qtw.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ifl.xuetiantiany.cn

[U105] JS：节流
来源：http://nut.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fxi.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://rqy.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dcq.jqgfzy.top

[U107] JS：数字千分位
来源：http://rge.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fck.jqgfzy.top

[U108] JS：随机整数
来源：http://smi.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zek.cucudq.cn

[U109] JS：数组分组
来源：http://vpy.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://phm.sufxvd.cn

[U110] JS：数组分块
来源：http://uls.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dxv.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://ucu.dianchejie.cn

new Map(Object.entries(obj))
来源：http://zki.zhoulong.xyz

[U112] JS：字符串补位
来源：http://iif.fengsongda.top

"7".padStart(3, "0")
来源：http://piv.zycfv.cn

[U113] JS：正则替换全部
来源：http://pke.shzxlz.cn

s.replaceAll("a", "b")
来源：http://vum.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://txm.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://sxc.yj20258888.top

[U115] JS：生成 UUID
来源：http://jzq.shuidangran.top

crypto.randomUUID()
来源：http://rdt.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ilk.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://rwu.bjfxy.top

[U117] JS：单元测试
来源：http://hhp.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://res.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://btk.jiagoushi.top

npm i -D vite;  npx vite
来源：http://qvm.redwolf501.top

[U119] JS：生产构建
来源：http://cdf.shangyingyoupin.top

npx vite build
来源：http://whw.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://jxy.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://cvs.shanyushiyangkeji.top

================================================================================
来源：http://zgo.quarkkingdee.top

统计汇总
来源：http://yul.zycfv.cn

================================================================================
来源：http://umo.sufxvd.cn

按语言统计（条）：
来源：http://pwg.smart0.xyz

Python ......... 252
来源：http://wyw.smart0.xyz

PHP ............ 252
来源：http://mdw.hysaishi.cn

JavaScript ..... 252
来源：http://lue.ehwqpu.com

TypeScript ..... 212
来源：http://hxy.316326.xyz

Java ........... 212
来源：http://qsn.jqgfzy.top

Go ............. 212
来源：http://qrc.pengpengdd.cyou

Ruby ........... 212
来源：http://yxv.sjlbkw.cn

C# ............. 212
来源：http://zkv.zhijiandao.cn

C .............. 30
来源：http://vuy.hammf.cn

C++ ............ 30
来源：http://nmr.dianchejie.cn

SQL ............ 90
来源：http://wkb.tanke756.top

Bash ........... 80
来源：http://swi.tian-w.cn

Kotlin ......... 15
来源：http://ajy.hnxiangtu.top

Swift .......... 15
来源：http://gzq.ydzc1.top

Lua ............ 10
来源：http://ltv.vehdjk.com

Perl ........... 10
来源：http://uei.gogol.net.cn

Scala .......... 10
来源：http://oph.mhx1999.top

------------------------------------
来源：http://eub.xuetiantiany.cn

合计 ........... 2106 条
来源：http://mnb.hcnkem.com

按章节统计：
来源：http://xmo.chenlongwang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mbb.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ewp.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://del.tian-w.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xkz.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xfa.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yjr.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tdb.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ifu.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gor.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mja.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gam.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wur.0kj1m.cn


<!-- 参考信息 -->