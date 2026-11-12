代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ocl.cheryme.top

================================================================================
来源：http://iik.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hkz.yj20258888.top

================================================================================
来源：http://dru.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://ciz.hysaishi.cn

println("Hello")
来源：http://awe.jqgufenzy.top

[T02] Kotlin：变量
来源：http://llz.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gnl.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://vcb.fzhhl.top

"值: $b"
来源：http://kcc.andypj.xyz

[T04] Kotlin：空安全
来源：http://vsn.sxryk.cn

val n: String? = null;  n?.length
来源：http://mlz.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://utt.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hxc.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://lqs.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tmj.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://vbh.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://odd.aizwys.cn

[T08] Kotlin：数据类
来源：http://nlt.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://awt.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://dsq.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://ljy.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://qpf.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ldp.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://mnl.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zhh.andypj.xyz

[T12] Kotlin：解构声明
来源：http://knp.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://ibf.uphjek.com

[T13] Kotlin：只读 Map
来源：http://ljq.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://thi.dashuyun.cn

[T14] Kotlin：循环
来源：http://kce.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://qcv.sweek.top

[T15] Kotlin：接口
来源：http://kit.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://qui.jyoumei.cn

[T16] Swift：Hello World
来源：http://aej.9152youxi.cn

print("Hello")
来源：http://qaf.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://cnk.fzhhl.top

var a = 1;  let b = 2
来源：http://epv.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://yzp.jiagoushi.top

"值: \(b)"
来源：http://ebd.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://tff.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://tpn.shzxlz.cn

[T20] Swift：数组操作
来源：http://vyk.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://jsy.zdqjudy.top

[T21] Swift：遍历
来源：http://gjg.shanyushiyangtech.top

for x in a { print(x) }
来源：http://ltb.shangyingyoupin.top

[T22] Swift：字典
来源：http://imu.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oxg.daxiang520.top

[T23] Swift：函数
来源：http://hao.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hdr.jinqigufen.top

[T24] Swift：闭包
来源：http://kek.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sfm.aibaodan.cn

[T25] Swift：结构体
来源：http://tbk.haohaochexian.top

struct P { var x: Int }
来源：http://mps.wangdashe.top

[T26] Swift：类与重写
来源：http://elh.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://wzn.vehdjk.com

[T27] Swift：错误处理
来源：http://wyx.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://izf.chenzaomai.com

[T28] Swift：枚举
来源：http://jqt.zhongyouzk.top

enum Color { case red, green }
来源：http://rba.tarul.cn

[T29] Swift：guard 提前返回
来源：http://goc.hywenlv.cn

guard let x = opt else { return }
来源：http://plv.sweek.top

[T30] Swift：协议
来源：http://cut.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://tlv.xinyue.icu

[T31] Lua：Hello World
来源：http://bkb.andypj.xyz

print("Hello")
来源：http://hmo.fktsv.cn

[T32] Lua：局部变量
来源：http://wkl.ydzc1.top

local a = 1
来源：http://ebt.iojbl.cn

[T33] Lua：表（数组）
来源：http://wqu.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tci.chenlongwang.top

[T34] Lua：遍历表
来源：http://uix.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iit.jqgfzy.top

[T35] Lua：字典表
来源：http://phr.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://gjq.hesvh.cn

[T36] Lua：函数
来源：http://tgd.shzxlz.cn

function add(a, b) return a + b end
来源：http://swp.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://kpg.yj20258888.top

"a" .. "b"
来源：http://acx.iojbl.cn

[T38] Lua：条件
来源：http://fsk.jinqigufen.top

if x > 0 then print("正") end
来源：http://zys.aibaodan.cn

[T39] Lua：模式匹配
来源：http://ixo.yueranfly.top

string.find(s, "%d+")
来源：http://ysa.jqgfzy.top

[T40] Lua：元表
来源：http://zja.tarul.cn

setmetatable({}, { __index = base })
来源：http://kig.hcnkem.com

[T41] Perl：Hello World
来源：http://tqa.gzhubu.top

print "Hello\n";
来源：http://wuu.zhijiandao.cn

[T42] Perl：变量类型
来源：http://yta.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fbt.0kj1m.cn

[T43] Perl：字符串插值
来源：http://oka.zdqjudy.top

"值: $a"
来源：http://aom.shzxlz.cn

[T44] Perl：条件
来源：http://eqc.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://bow.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://abk.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://rjp.nwbrower.top

[T46] Perl：哈希操作
来源：http://swa.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vrh.pycfn.com

[T47] Perl：正则捕获
来源：http://wri.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hyd.andypj.xyz

[T48] Perl：正则替换
来源：http://qwe.havefunace.top

$s =~ s/old/new/g;
来源：http://dqj.chenlongwang.top

[T49] Perl：函数
来源：http://dxs.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ibt.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://gab.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://siq.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://lzz.xuanzx.com

[T51] Scala：Hello World
来源：http://znn.pengpengdd.cyou

println("Hello")
来源：http://rrs.svipenyu.cn

[T52] Scala：变量
来源：http://veb.andypj.xyz

val a = 1;  var b = 2
来源：http://uqa.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://kdn.pycfn.com

s"值: $b"
来源：http://afk.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://zgr.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://dff.snrcjt.cn

[T55] Scala：集合过滤
来源：http://lql.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://far.sjlbkw.cn

[T56] Scala：样例类
来源：http://swl.jianghu66.top

case class User(name: String, age: Int)
来源：http://xpb.birdmap.top

[T57] Scala：模式匹配
来源：http://sqm.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yta.pycfn.com

[T58] Scala：函数定义
来源：http://cdb.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://yne.bbcook.cn

[T59] Scala：循环
来源：http://lny.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://btt.uphjek.com

[T60] Scala：折叠
来源：http://csf.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxl.smart0.xyz

================================================================================
来源：http://wfm.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ycf.xuetiantiany.cn

================================================================================
来源：http://jsy.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://kbx.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://gct.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://coj.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pnk.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://nqx.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://mzo.hcnkem.com

[U04] Py：变量调试打印
来源：http://gnd.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sqp.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://okc.epnwcf.com

list(dict.fromkeys(arr))
来源：http://fbu.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://nfi.xylfe.cn

{**a, **b}
来源：http://xvs.jyoumei.cn

[U07] Py：反转字典键值
来源：http://tkg.jiagoushi.top

{v: k for k, v in d.items()}
来源：http://tmi.zhengqikj.top

[U08] Py：展平二维列表
来源：http://xzy.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://zkh.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://hay.zhengqikj.top

max(d, key=d.get)
来源：http://qvs.hammf.cn

[U10] Py：按值排序字典
来源：http://qva.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hfx.sweek.top

[U11] Py：生成器表达式
来源：http://onf.aizwys.cn

(x * 2 for x in arr)
来源：http://umf.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://voc.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://eak.hcnkem.com

[U13] Py：固定长度队列
来源：http://iud.hcnkem.com

deque(maxlen=10)
来源：http://gyn.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://wky.sweek.top

defaultdict(list)
来源：http://wia.nanxinkj.top

[U15] Py：高精度计时
来源：http://hqu.ctjpmb.com

t = time.perf_counter()
来源：http://gbf.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://ljl.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uwv.jlsjyb.cn

[U17] Py：初始化日志
来源：http://aor.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://ezv.gaohongyu789.top

[U18] Py：预编译正则
来源：http://mst.smart0.xyz

pat = re.compile(r"\d+")
来源：http://dno.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://asy.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vxs.yfazqb.com

[U20] Py：缓存函数结果
来源：http://iqt.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://yop.hnxiangtu.top

[U21] Py：自定义上下文管理器
来源：http://nxp.xylfe.cn

@contextlib.contextmanager
来源：http://day.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://mii.zhengqikj.top

list(zip(*m))
来源：http://gte.redwolf501.top

[U23] Py：分块读取大文件
来源：http://ulz.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://epj.c1oappe.top

[U24] Py：路径操作
来源：http://kdi.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pqz.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://rpr.fehbvm.com

csv.DictReader(f)
来源：http://pod.zdqjudy.top

[U26] Py：并发下载
来源：http://gcx.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pwv.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://ynk.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://qgn.316326.xyz

[U28] Py：类型别名
来源：http://kkb.jqgfzy.top

UserId = int
来源：http://uyc.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://lmy.jinqigufen.top

@property 与 @x.setter 配合
来源：http://cdk.nwbrower.top

[U30] Py：数据类
来源：http://yod.yanxiufei.cn

@dataclass(slots=True)
来源：http://tvc.shanyushiyangtech.top

[U31] Py：单测
来源：http://qog.zdqjudy.top

python -m pytest -q
来源：http://emm.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://mfv.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://ujk.nwbrower.top

[U33] Py：打包发布
来源：http://jey.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://wih.shzxlz.cn

[U34] Py：判断编码
来源：http://nwg.sysykeji.top

chardet.detect(raw)
来源：http://nbj.redwolf501.top

[U35] Py：发送邮件
来源：http://lam.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://egr.ybcxt.top

[U36] Py：定时任务
来源：http://jds.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://eya.uphjek.com

[U37] Py：读写 Excel
来源：http://bzg.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://kxb.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://pbc.nanxinkj.top

Path(__file__).resolve().parent
来源：http://rel.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://pzw.iojbl.cn

sys.stdout.isatty()
来源：http://iro.yj202588.top

[U40] Py：打印到标准错误
来源：http://bbd.dashuyun.cn

print("err", file=sys.stderr)
来源：http://phy.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://hxa.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yod.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://hfv.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lxc.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://gta.ivvv.top

namespace App\Http;
来源：http://uin.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://eck.jyoumei.cn

declare(strict_types=1);
来源：http://yov.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://jzc.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kxa.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://npn.cucudq.cn

?string $name = null
来源：http://bru.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://ovr.pengpengdd.cyou

int|string $id
来源：http://roq.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://sip.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ypp.vehdjk.com

[U49] PHP：只读属性
来源：http://lek.pycfn.com

public readonly string $name
来源：http://jrq.hammf.cn

[U50] PHP：构造器属性提升
来源：http://dsq.yonumen.top

public function __construct(private int $id) {}
来源：http://dga.epnwcf.com

[U51] PHP：数组解构
来源：http://glc.pycfn.com

[$a, $b] = $arr;
来源：http://zit.yangfankeji.com

[U52] PHP：箭头函数
来源：http://uhq.uphjek.com

$double = fn($x) => $x * 2;
来源：http://vmx.yfazqb.com

[U53] PHP：空合并运算符
来源：http://udu.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://nft.guowangkeji.top

[U54] PHP：空安全调用
来源：http://bqw.haohaochexian.top

$obj?->method()
来源：http://uun.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://sax.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gqt.fzhhl.top

[U56] PHP：命名参数
来源：http://mkm.chenzaomai.com

f(a: 1, b: 2)
来源：http://wly.ivvv.top

[U57] PHP：字符串插值
来源：http://ylj.gzhubu.top

"值: {$a}"
来源：http://ahh.zycfv.cn

[U58] PHP：数组三件套
来源：http://csi.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mgr.52xcode.cn

[U59] PHP：自定义排序
来源：http://tzk.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hbb.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://gfu.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yeh.feifeiyinyue.top

[U61] PHP：正则
来源：http://ldk.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ioc.hnqzz.top

[U62] PHP：日期对象
来源：http://pqr.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hzl.jqgufenzy.top

[U63] PHP：文件读写
来源：http://vpp.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ffh.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://ael.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://hgg.hysaishi.cn

[U65] PHP：会话
来源：http://for.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vxj.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://lhk.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vrj.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://ifp.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kxn.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://jsh.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ijv.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://spt.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jhd.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://tsl.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dar.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://qca.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://nbz.cheryme.top

[U72] PHP：写错误日志
来源：http://elm.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://pjm.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://ton.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://ncr.yj20258.top

[U74] PHP：读取环境变量
来源：http://nzx.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://zzg.pengpengdd.cyou

[U75] PHP：依赖注入
来源：http://atj.daria6918.cn

composer require psr/container
来源：http://ojb.quarkkingdee.top

[U76] PHP：简单路由
来源：http://wtc.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ben.meibo888.top

[U77] PHP：模板渲染
来源：http://nxr.nanxuanxn.top

composer require twig/twig
来源：http://jpv.yongpay.top

[U78] PHP：单元测试
来源：http://tyv.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://izq.epnwcf.com

[U79] PHP：静态分析
来源：http://oxg.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://fhz.ivvv.top

[U80] PHP：代码规范修复
来源：http://amy.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hkp.zhongyouzk.top

[U81] JS：初始化项目
来源：http://huw.sjlbkw.cn

npm init -y;  npm i express
来源：http://sss.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://isj.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lhs.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://eoe.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gvc.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://bia.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://khe.epnwcf.com

[U85] JS：可选链
来源：http://tdt.yj20258.top

a?.b?.c
来源：http://xwg.chenjidiqi.icu

[U86] JS：空值合并
来源：http://vnc.yfazqb.com

a ?? b
来源：http://ead.dashuyun.cn


<!-- 参考信息 -->