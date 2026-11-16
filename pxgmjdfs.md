代发 wailian999

[T39] Lua：模式匹配
来源：http://rkx.52xcode.cn

string.find(s, "%d+")
来源：http://xwf.316326.xyz

[T40] Lua：元表
来源：http://pgx.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://oxk.hesvh.cn

[T41] Perl：Hello World
来源：http://fdc.quarkkingdee.top

print "Hello\n";
来源：http://cbg.zhongyouzk.top

[T42] Perl：变量类型
来源：http://ona.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzv.chenzaomai.com

[T43] Perl：字符串插值
来源：http://vsw.gotoacloud.top

"值: $a"
来源：http://akc.316326.xyz

[T44] Perl：条件
来源：http://bpn.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://dnn.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://sqr.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://yjv.ppjwa.cn

[T46] Perl：哈希操作
来源：http://sbb.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hyg.dashuyun.cn

[T47] Perl：正则捕获
来源：http://hwg.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nyq.ppjwa.cn

[T48] Perl：正则替换
来源：http://pyi.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://fnb.hywenlv.cn

[T49] Perl：函数
来源：http://xrj.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zsf.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://hku.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gvw.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://aot.yanxiufei.cn

[T51] Scala：Hello World
来源：http://fzo.jinghuilouyu.cn

println("Hello")
来源：http://lzc.epnwcf.com

[T52] Scala：变量
来源：http://mos.yonumen.top

val a = 1;  var b = 2
来源：http://ceg.bbcook.cn

[T53] Scala：字符串插值
来源：http://ycy.yfazqb.com

s"值: $b"
来源：http://wgz.xylfe.cn

[T54] Scala：集合映射
来源：http://qok.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://vjb.cheryme.top

[T55] Scala：集合过滤
来源：http://ixf.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://jki.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://hjk.yongpay.top

case class User(name: String, age: Int)
来源：http://aho.yueranfly.top

[T57] Scala：模式匹配
来源：http://bxm.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hca.c1oappe.top

[T58] Scala：函数定义
来源：http://mxc.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://akc.hywenlv.cn

[T59] Scala：循环
来源：http://ogm.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://mob.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://lhq.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wss.gaohongyu789.top

================================================================================
来源：http://qem.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://azh.tianlin.xyz

================================================================================
来源：http://cqt.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://qcr.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hcw.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://mxd.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kqy.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://oep.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rqe.wangdashe.top

[U04] Py：变量调试打印
来源：http://dch.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://utp.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://pce.hcnkem.com

list(dict.fromkeys(arr))
来源：http://rqm.gogol.net.cn

[U06] Py：合并两个字典
来源：http://nhu.guannengcc.top

{**a, **b}
来源：http://nhj.wangdashe.top

[U07] Py：反转字典键值
来源：http://fhv.316326.xyz

{v: k for k, v in d.items()}
来源：http://qtx.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://jfi.jinqigufen.top

[y for x in nested for y in x]
来源：http://bft.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://gqf.ydjk.org.cn

max(d, key=d.get)
来源：http://ioc.sxryk.cn

[U10] Py：按值排序字典
来源：http://vhx.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mmp.redwolf501.top

[U11] Py：生成器表达式
来源：http://sqs.fzhhl.top

(x * 2 for x in arr)
来源：http://ltj.pengpengdd.cyou

[U12] Py：取出现最多的 3 个元素
来源：http://xif.yueranfly.top

Counter(arr).most_common(3)
来源：http://duv.gogol.net.cn

[U13] Py：固定长度队列
来源：http://eay.meibo888.top

deque(maxlen=10)
来源：http://gmg.yj20258888.top

[U14] Py：分组收集到列表
来源：http://ita.jqgfzy.top

defaultdict(list)
来源：http://jwi.gotoacloud.top

[U15] Py：高精度计时
来源：http://bnn.yj20258888.top

t = time.perf_counter()
来源：http://apg.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://ktx.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lqd.jinqigufen.top

[U17] Py：初始化日志
来源：http://zkl.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://fho.gaohongyu789.top

[U18] Py：预编译正则
来源：http://rof.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://rsa.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://geb.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://psv.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://mfp.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://cyl.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://kuy.mhx1999.top

@contextlib.contextmanager
来源：http://pmo.jianghu66.top

[U22] Py：矩阵转置
来源：http://ddu.daria6918.cn

list(zip(*m))
来源：http://alh.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://avc.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://utv.zdbjq.cn

[U24] Py：路径操作
来源：http://iqh.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://brf.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://eze.tarul.cn

csv.DictReader(f)
来源：http://pkm.dianchejie.cn

[U26] Py：并发下载
来源：http://scr.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mdm.tanke756.top

[U27] Py：异步 HTTP
来源：http://ida.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://aox.sweek.top

[U28] Py：类型别名
来源：http://lhq.fktsv.cn

UserId = int
来源：http://oth.dianchejie.cn

[U29] Py：属性校验
来源：http://zyh.nanxinkj.top

@property 与 @x.setter 配合
来源：http://xle.gogol.net.cn

[U30] Py：数据类
来源：http://prx.jiagoushi.top

@dataclass(slots=True)
来源：http://wfo.yj20258.top

[U31] Py：单测
来源：http://vti.fanxiaobao.xyz

python -m pytest -q
来源：http://okk.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://utz.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://hgb.bbcook.cn

[U33] Py：打包发布
来源：http://mpd.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://xwh.haohaochexian.top

[U34] Py：判断编码
来源：http://ged.shanyushiyangtech.top

chardet.detect(raw)
来源：http://sgv.hfpthk.cn

[U35] Py：发送邮件
来源：http://alp.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://efe.tarul.cn

[U36] Py：定时任务
来源：http://flc.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://irj.ctjpmb.com

[U37] Py：读写 Excel
来源：http://nqr.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vac.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://pbb.316326.xyz

Path(__file__).resolve().parent
来源：http://fqa.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://dtn.hysaishi.cn

sys.stdout.isatty()
来源：http://slk.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://plu.fktsv.cn

print("err", file=sys.stderr)
来源：http://chp.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://apm.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://zbh.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://yve.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rsg.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://lpa.yueranfly.top

namespace App\Http;
来源：http://fud.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://dfb.ppjwa.cn

declare(strict_types=1);
来源：http://axy.aizwys.cn

[U45] PHP：类型声明与返回类型
来源：http://lsz.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zwv.ydzc1.top

[U46] PHP：可空类型
来源：http://xtz.hammf.cn

?string $name = null
来源：http://ltb.cashguo.top

[U47] PHP：联合类型
来源：http://tkn.shangyingyoupin.top

int|string $id
来源：http://brg.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://xgq.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aar.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://wdb.fktsv.cn

public readonly string $name
来源：http://rmy.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://wdy.tian-w.cn

public function __construct(private int $id) {}
来源：http://hbl.cqqwz.cn

[U51] PHP：数组解构
来源：http://ave.xinyue.icu

[$a, $b] = $arr;
来源：http://hfc.havefunace.top

[U52] PHP：箭头函数
来源：http://zpl.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://bho.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://gfc.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://ngt.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://uji.zhaomingkeji.xyz

$obj?->method()
来源：http://eon.nanxinkj.top

[U55] PHP：match 表达式
来源：http://flv.tianlin.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nwe.nanxuanxn.top

[U56] PHP：命名参数
来源：http://xwh.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://syr.316326.xyz

[U57] PHP：字符串插值
来源：http://qaf.ppjwa.cn

"值: {$a}"
来源：http://evw.nanxinkj.top

[U58] PHP：数组三件套
来源：http://bqe.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://whx.gzhubu.top

[U59] PHP：自定义排序
来源：http://ysk.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://koz.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://jku.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jvf.bbcook.cn

[U61] PHP：正则
来源：http://zow.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hxa.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://opc.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ljq.cheryme.top

[U63] PHP：文件读写
来源：http://wlj.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jic.epnwcf.com

[U64] PHP：目录遍历
来源：http://rhc.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://pvj.fehbvm.com

[U65] PHP：会话
来源：http://vww.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://zll.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://pqb.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xzl.yfazqb.com

[U67] PHP：处理文件上传
来源：http://fac.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mbs.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://owx.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://far.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://jog.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://koz.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://ohq.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bws.yj202588.top

[U71] PHP：抛出异常
来源：http://rvm.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://jof.cucudq.cn

[U72] PHP：写错误日志
来源：http://jix.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://vem.chenzaomai.com

[U73] PHP：读取 ini 配置
来源：http://usp.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://cxi.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://aes.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://pue.fehbvm.com

[U75] PHP：依赖注入
来源：http://kif.hammf.cn

composer require psr/container
来源：http://ajy.sweek.top

[U76] PHP：简单路由
来源：http://lgv.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vwm.chenlongwang.top

[U77] PHP：模板渲染
来源：http://zab.cashguo.top

composer require twig/twig
来源：http://ljr.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://gqh.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://hkj.0kj1m.cn

[U79] PHP：静态分析
来源：http://ook.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://omk.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://xms.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jmd.kuanghao11.cn

[U81] JS：初始化项目
来源：http://nko.daria6918.cn

npm init -y;  npm i express
来源：http://utu.hnxiangtu.top

[U82] JS：package.json 脚本
来源：http://cjr.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vbn.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://vvv.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://qvu.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://tei.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://zvb.tian-w.cn

[U85] JS：可选链
来源：http://juj.meibo888.top

a?.b?.c
来源：http://foc.nanxinkj.top

[U86] JS：空值合并
来源：http://ijy.hnxiangtu.top

a ?? b
来源：http://yam.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://xjo.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://tpq.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://hmo.kuanghao11.cn

{ ...a, ...b }
来源：http://khg.snrcjt.cn

[U89] JS：数组去重
来源：http://wdb.gaohongyu789.top

[...new Set(arr)]
来源：http://jvt.aibaodan.cn

[U90] JS：数字数组排序
来源：http://exa.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://xeh.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://skl.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nfs.guowangkeji.top

[U92] JS：深拷贝
来源：http://xuq.wangdashe.top

structuredClone(obj)
来源：http://elg.pycfn.com

[U93] JS：模板字符串
来源：http://dwb.aibaodan.cn

`共 ${n} 条`
来源：http://jyh.xuanzx.com

[U94] JS：箭头函数
来源：http://spj.sxryk.cn

const double = x => x * 2;
来源：http://ohz.cucudq.cn

[U95] JS：Promise 包装
来源：http://mfg.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://tnn.havefunace.top

[U96] JS：async/await 与异常
来源：http://sui.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bif.meibo888.top

[U97] JS：并发请求
来源：http://uep.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lgu.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://pwu.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gqn.316326.xyz

[U99] JS：事件监听
来源：http://uzk.bjfxy.top

el.addEventListener("click", e => {})
来源：http://wze.bjfxy.top

[U100] JS：DOM 查询
来源：http://mgy.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://ktb.yj20258888.top

[U101] JS：classList 操作
来源：http://rkx.bjfxy.top

el.classList.toggle("active")
来源：http://vkc.nanxuanxn.top

[U102] JS：本地存储
来源：http://tse.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://grj.ydjk.org.cn

[U103] JS：定时器
来源：http://lwi.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vyz.hammf.cn

[U104] JS：防抖
来源：http://acj.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edx.yj20258.top

[U105] JS：节流
来源：http://npn.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zge.gaohongyu789.top

[U106] JS：日期格式化
来源：http://psi.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aew.cheryme.top

[U107] JS：数字千分位
来源：http://sdc.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hbq.sxryk.cn

[U108] JS：随机整数
来源：http://kcw.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jgk.zhongyouzk.top

[U109] JS：数组分组
来源：http://hgo.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://knp.gzhubu.top

[U110] JS：数组分块
来源：http://mlt.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khi.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://hec.daxiang520.top

new Map(Object.entries(obj))
来源：http://wbv.yuanzhike.top

[U112] JS：字符串补位
来源：http://jms.gzhubu.top

"7".padStart(3, "0")
来源：http://ufi.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://nms.bbcook.cn

s.replaceAll("a", "b")
来源：http://kmd.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://srn.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zza.daria6918.cn

[U115] JS：生成 UUID
来源：http://iee.birdmap.top

crypto.randomUUID()
来源：http://zli.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://hww.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://bdw.hammf.cn

[U117] JS：单元测试
来源：http://dmk.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://qwx.cheryme.top

[U118] JS：开发服务器
来源：http://iby.daria6918.cn

npm i -D vite;  npx vite
来源：http://lim.dashuyun.cn

[U119] JS：生产构建
来源：http://mkk.haohaochexian.top

npx vite build
来源：http://mam.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://zdb.havefunace.top

import.meta.env.VITE_API_URL
来源：http://ayb.gogol.net.cn

================================================================================
来源：http://ojy.feifeiyinyue.top

统计汇总
来源：http://fav.sweek.top

================================================================================
来源：http://vwk.9152youxi.cn

按语言统计（条）：
来源：http://prb.xuetiantiany.cn

Python ......... 252
来源：http://tsr.jinghuilouyu.cn

PHP ............ 252
来源：http://mge.bjfxy.top

JavaScript ..... 252
来源：http://pdo.guowangkeji.top

TypeScript ..... 212
来源：http://mwg.fanxiaobao.xyz

Java ........... 212
来源：http://qag.guowangkeji.top

Go ............. 212
来源：http://koe.9152youxi.cn

Ruby ........... 212
来源：http://eqb.cashguo.top

C# ............. 212
来源：http://woy.tian-w.cn


<!-- 参考信息 -->