代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://arw.snrcjt.cn

================================================================================
来源：http://haz.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqo.yonumen.top

================================================================================
来源：http://ltb.9152youxi.cn

[T01] Kotlin：Hello World
来源：http://ifm.zhijiandao.cn

println("Hello")
来源：http://jml.hammf.cn

[T02] Kotlin：变量
来源：http://eqd.yvedp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://axh.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://gcl.zhaomingkeji.xyz

"值: $b"
来源：http://zok.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://hzn.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://kwy.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://anw.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qdn.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://hdb.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jqv.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://jig.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nyt.bbcook.cn

[T08] Kotlin：数据类
来源：http://xwp.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://cmq.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://kyg.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://hvn.aizwys.cn

[T10] Kotlin：默认参数
来源：http://kbw.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://upl.nanxuanxn.top

[T11] Kotlin：协程
来源：http://yty.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xbi.ydzc1.top

[T12] Kotlin：解构声明
来源：http://klq.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://ntn.tarul.cn

[T13] Kotlin：只读 Map
来源：http://ykt.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://rgd.cucudq.cn

[T14] Kotlin：循环
来源：http://ack.dianchejie.cn

for (i in 1..10) println(i)
来源：http://lcr.sxryk.cn

[T15] Kotlin：接口
来源：http://zxs.xylfe.cn

interface Shape { fun area(): Double }
来源：http://ibd.chenzaomai.com

[T16] Swift：Hello World
来源：http://rio.bbcook.cn

print("Hello")
来源：http://vkv.birdmap.top

[T17] Swift：变量与常量
来源：http://vpt.iojbl.cn

var a = 1;  let b = 2
来源：http://ups.cheryme.top

[T18] Swift：字符串插值
来源：http://rnm.dashuyun.cn

"值: \(b)"
来源：http://pdu.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://hxm.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://aps.ehwqpu.com

[T20] Swift：数组操作
来源：http://efh.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://zra.chenzaomai.com

[T21] Swift：遍历
来源：http://aje.dianchejie.cn

for x in a { print(x) }
来源：http://phi.ydzc1.top

[T22] Swift：字典
来源：http://tvg.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://lmh.hammf.cn

[T23] Swift：函数
来源：http://vmr.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://akm.wangdashe.top

[T24] Swift：闭包
来源：http://rpy.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://otw.cashguo.top

[T25] Swift：结构体
来源：http://zcz.xziqi.cn

struct P { var x: Int }
来源：http://ffd.redwolf501.top

[T26] Swift：类与重写
来源：http://gdu.smart0.xyz

class A: Base { override func f() {} }
来源：http://ekg.xuanzx.com

[T27] Swift：错误处理
来源：http://zsy.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://vtf.yfazqb.com

[T28] Swift：枚举
来源：http://vyw.chenzaomai.com

enum Color { case red, green }
来源：http://ter.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://vrd.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://ejp.sufxvd.cn

[T30] Swift：协议
来源：http://fcd.chenlongwang.top

protocol Shape { func area() -> Double }
来源：http://szp.havefunace.top

[T31] Lua：Hello World
来源：http://eov.yuanzhike.top

print("Hello")
来源：http://mmj.ydjk.org.cn

[T32] Lua：局部变量
来源：http://qly.aizwys.cn

local a = 1
来源：http://ejm.guannengcc.top

[T33] Lua：表（数组）
来源：http://maf.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://usv.zhengqikj.top

[T34] Lua：遍历表
来源：http://acb.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kut.jqgfzy.top

[T35] Lua：字典表
来源：http://xvy.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://dpy.hongshengwenyu.top

[T36] Lua：函数
来源：http://kzn.0kj1m.cn

function add(a, b) return a + b end
来源：http://fnb.nwbrower.top

[T37] Lua：字符串拼接
来源：http://wzi.chenlongwang.top

"a" .. "b"
来源：http://nkq.zycfv.cn

[T38] Lua：条件
来源：http://qap.xziqi.cn

if x > 0 then print("正") end
来源：http://dfd.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://yxy.vehdjk.com

string.find(s, "%d+")
来源：http://iwk.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://oev.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://pmw.gzhubu.top

[T41] Perl：Hello World
来源：http://rbb.yuxming.cn

print "Hello\n";
来源：http://ivc.dianchejie.cn

[T42] Perl：变量类型
来源：http://fyw.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ggu.haohaochexian.top

[T43] Perl：字符串插值
来源：http://sps.dashuyun.cn

"值: $a"
来源：http://blg.iojbl.cn

[T44] Perl：条件
来源：http://jxj.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://mva.nwbrower.top

[T45] Perl：数组遍历
来源：http://goi.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://eke.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://aph.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mon.dashuyun.cn

[T47] Perl：正则捕获
来源：http://rkp.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jmb.shuidangran.top

[T48] Perl：正则替换
来源：http://xlw.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://wsg.zhijiandao.cn

[T49] Perl：函数
来源：http://wpq.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://plk.zycfv.cn

[T50] Perl：逐行读文件
来源：http://xdg.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cix.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://enn.jinqigfzy.top

[T51] Scala：Hello World
来源：http://tzl.jqgfzy.top

println("Hello")
来源：http://fhl.tian-w.cn

[T52] Scala：变量
来源：http://rhw.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://twz.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://qpz.hnqzz.top

s"值: $b"
来源：http://yfo.fktsv.cn

[T54] Scala：集合映射
来源：http://aap.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://gtf.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://ete.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://scl.jianghu66.top

[T56] Scala：样例类
来源：http://uss.sufxvd.cn

case class User(name: String, age: Int)
来源：http://coq.hywenlv.cn

[T57] Scala：模式匹配
来源：http://zem.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://thh.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://zbg.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://jku.jinghuilouyu.cn

[T59] Scala：循环
来源：http://gng.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://dpw.zhoulong.xyz

[T60] Scala：折叠
来源：http://glx.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hre.yanxiufei.cn

================================================================================
来源：http://llx.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fcc.zycfv.cn

================================================================================
来源：http://hpn.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://zks.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jjd.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://nxp.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gaf.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://xjy.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kgk.hywenlv.cn

[U04] Py：变量调试打印
来源：http://kjd.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mip.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://tmn.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://hyd.bjfxy.top

[U06] Py：合并两个字典
来源：http://ybd.hammf.cn

{**a, **b}
来源：http://daf.snrcjt.cn

[U07] Py：反转字典键值
来源：http://bsp.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://blq.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://tii.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://niy.cheryme.top

[U09] Py：字典取最大值的键
来源：http://vbv.chenjidiqi.icu

max(d, key=d.get)
来源：http://mlq.zdqjudy.top

[U10] Py：按值排序字典
来源：http://oax.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gaf.hnqzz.top

[U11] Py：生成器表达式
来源：http://ruc.xziqi.cn

(x * 2 for x in arr)
来源：http://sjq.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://kcn.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://bns.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://ozv.yangfankeji.com

deque(maxlen=10)
来源：http://wpa.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://nku.ydzc1.top

defaultdict(list)
来源：http://zwf.xinyue.icu

[U15] Py：高精度计时
来源：http://jqv.vqdsnc.cn

t = time.perf_counter()
来源：http://ped.smart0.xyz

[U16] Py：命令行参数解析
来源：http://rxs.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://afv.zhongyouzk.top

[U17] Py：初始化日志
来源：http://dqa.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lsk.jqgfzy.top

[U18] Py：预编译正则
来源：http://oyg.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://ziw.zycfv.cn

[U19] Py：正则替换带回调
来源：http://iua.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vzy.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://kse.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://ixc.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://pgt.9152youxi.cn

@contextlib.contextmanager
来源：http://szl.dianchejie.cn

[U22] Py：矩阵转置
来源：http://dht.chenlongwang.top

list(zip(*m))
来源：http://zge.iojbl.cn

[U23] Py：分块读取大文件
来源：http://bje.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xuo.fehbvm.com

[U24] Py：路径操作
来源：http://cvt.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ugg.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://lnz.zhixingplan.top

csv.DictReader(f)
来源：http://jug.aizwys.cn

[U26] Py：并发下载
来源：http://jxl.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vja.yuxming.cn

[U27] Py：异步 HTTP
来源：http://ydb.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://yha.zhixingplan.top

[U28] Py：类型别名
来源：http://hcv.chenzaomai.com

UserId = int
来源：http://ipi.cucudq.cn

[U29] Py：属性校验
来源：http://xxv.havefunace.top

@property 与 @x.setter 配合
来源：http://jww.hongshengwenyu.top

[U30] Py：数据类
来源：http://alg.zycfv.cn

@dataclass(slots=True)
来源：http://hpf.c1oappe.top

[U31] Py：单测
来源：http://cvy.shangyingyoupin.top

python -m pytest -q
来源：http://azf.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://tui.sxryk.cn

ruff format . && ruff check --fix .
来源：http://kfb.nwbrower.top

[U33] Py：打包发布
来源：http://auu.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://huw.yj202588.top

[U34] Py：判断编码
来源：http://xvs.daxiang520.top

chardet.detect(raw)
来源：http://pgo.ctjpmb.com

[U35] Py：发送邮件
来源：http://rjh.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gie.yuxming.cn

[U36] Py：定时任务
来源：http://vxr.xinyue.icu

schedule.every(10).minutes.do(job)
来源：http://rop.yuanzhike.top

[U37] Py：读写 Excel
来源：http://hgz.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://cbh.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://cln.hammf.cn

Path(__file__).resolve().parent
来源：http://trm.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://xzc.guannengcc.top

sys.stdout.isatty()
来源：http://okb.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://uqz.chenlongwang.top

print("err", file=sys.stderr)
来源：http://jvw.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://btt.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ptm.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://cao.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ozk.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://yzs.zycfv.cn

namespace App\Http;
来源：http://wus.xylfe.cn

[U44] PHP：开启严格类型
来源：http://fhu.zhiwuduotai.top

declare(strict_types=1);
来源：http://rvd.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://gmf.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lmg.ydjk.org.cn

[U46] PHP：可空类型
来源：http://svj.kuanghao11.cn

?string $name = null
来源：http://cfw.ydzc1.top

[U47] PHP：联合类型
来源：http://hya.sxryk.cn

int|string $id
来源：http://lmu.jianghu66.top

[U48] PHP：纯枚举
来源：http://jkg.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cyw.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://akx.fehbvm.com

public readonly string $name
来源：http://rrq.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://oes.aibaodan.cn

public function __construct(private int $id) {}
来源：http://ixc.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://dji.smart0.xyz

[$a, $b] = $arr;
来源：http://nad.cheryme.top

[U52] PHP：箭头函数
来源：http://pap.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://sfw.yongpay.top

[U53] PHP：空合并运算符
来源：http://kya.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://hon.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://mdc.xuetiantiany.cn

$obj?->method()
来源：http://bcg.jianghu66.top

[U55] PHP：match 表达式
来源：http://rkd.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://row.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://zjx.chenlongwang.top

f(a: 1, b: 2)
来源：http://ivs.shzxlz.cn

[U57] PHP：字符串插值
来源：http://but.sufxvd.cn

"值: {$a}"
来源：http://zuq.jinqigufen.top

[U58] PHP：数组三件套
来源：http://gfe.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lmq.nwbrower.top

[U59] PHP：自定义排序
来源：http://obu.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vjt.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://dmh.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qpl.yj202588.top

[U61] PHP：正则
来源：http://mxw.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bmd.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://qhe.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://imb.yangfankeji.com

[U63] PHP：文件读写
来源：http://wxl.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zrm.andypj.xyz

[U64] PHP：目录遍历
来源：http://ypg.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://mrp.yangfankeji.com

[U65] PHP：会话
来源：http://aku.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vyc.yj202588.top

[U66] PHP：设置 Cookie
来源：http://fuq.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ara.smart0.xyz

[U67] PHP：处理文件上传
来源：http://hve.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jml.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://kmj.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jic.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://njd.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://evv.daria6918.cn

[U70] PHP：PDO 事务
来源：http://ipw.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://siv.hcnkem.com

[U71] PHP：抛出异常
来源：http://vvo.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://vqn.guowangkeji.top

[U72] PHP：写错误日志
来源：http://zrw.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://iln.kuanghao11.cn

[U73] PHP：读取 ini 配置
来源：http://vti.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://qbc.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://tqk.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://ypf.yuxming.cn

[U75] PHP：依赖注入
来源：http://tsb.zhoulong.xyz

composer require psr/container
来源：http://ftf.sysykeji.top

[U76] PHP：简单路由
来源：http://ppd.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oej.yuanzhike.top

[U77] PHP：模板渲染
来源：http://jle.zhijiandao.cn

composer require twig/twig
来源：http://vyv.zdbjq.cn

[U78] PHP：单元测试
来源：http://snr.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://ibn.dianchejie.cn

[U79] PHP：静态分析
来源：http://pcv.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://gwt.bbcook.cn

[U80] PHP：代码规范修复
来源：http://tcq.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gex.zhijiandao.cn

[U81] JS：初始化项目
来源：http://wbq.tian-w.cn

npm init -y;  npm i express
来源：http://jit.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://uwa.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vro.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://tae.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://lpi.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://kjg.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qoh.hfpthk.cn

[U85] JS：可选链
来源：http://mtc.zhiwuduotai.top

a?.b?.c
来源：http://dmy.zhijiandao.cn

[U86] JS：空值合并
来源：http://jyo.ehwqpu.com

a ?? b
来源：http://qsf.yonumen.top


<!-- 参考信息 -->