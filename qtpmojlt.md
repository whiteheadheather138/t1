代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ovk.andypj.xyz

[S55] C++：结构化绑定
来源：http://mhr.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kyr.tanke756.top

[S56] C++：optional
来源：http://qqi.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wnj.vehdjk.com

[S57] C++：编译期常量
来源：http://hwj.yuanzhike.top

constexpr int N = 10;
来源：http://tyw.vehdjk.com

[S58] C++：命名空间
来源：http://dog.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://xit.nanxuanxn.top

[S59] C++：静态断言
来源：http://jel.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vjs.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://fve.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qbu.pycfn.com

================================================================================
来源：http://pzn.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qap.hfpthk.cn

================================================================================
来源：http://gfp.hcnkem.com

[T01] Kotlin：Hello World
来源：http://okk.zycfv.cn

println("Hello")
来源：http://ywl.bjfxy.top

[T02] Kotlin：变量
来源：http://zti.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hkz.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://gwr.xuetiantiany.cn

"值: $b"
来源：http://azf.ppjwa.cn

[T04] Kotlin：空安全
来源：http://ciw.yongpay.top

val n: String? = null;  n?.length
来源：http://wic.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://dhv.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ttq.meibo888.top

[T06] Kotlin：集合映射
来源：http://mfw.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zxg.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://bsn.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://qto.aibaodan.cn

[T08] Kotlin：数据类
来源：http://tgd.yj202588.top

data class User(val name: String, val age: Int)
来源：http://vjk.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://pwe.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://qdl.yonumen.top

[T10] Kotlin：默认参数
来源：http://wgr.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://wci.zhijiandao.cn

[T11] Kotlin：协程
来源：http://swk.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pas.epnwcf.com

[T12] Kotlin：解构声明
来源：http://irs.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://ezb.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://szf.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://yzp.nanxinkj.top

[T14] Kotlin：循环
来源：http://laf.tarul.cn

for (i in 1..10) println(i)
来源：http://lrg.ydjk.org.cn

[T15] Kotlin：接口
来源：http://pyb.ivvv.top

interface Shape { fun area(): Double }
来源：http://sfx.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://egp.sjlbkw.cn

print("Hello")
来源：http://czm.epnwcf.com

[T17] Swift：变量与常量
来源：http://jmw.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://rox.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://kpo.nwbrower.top

"值: \(b)"
来源：http://jkf.xinyue.icu

[T19] Swift：可选绑定
来源：http://tyx.quarkkingdee.top

if let n = opt { print(n) }
来源：http://tnb.9152youxi.cn

[T20] Swift：数组操作
来源：http://mwk.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jrg.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://ctb.sysykeji.top

for x in a { print(x) }
来源：http://mlh.ctjpmb.com

[T22] Swift：字典
来源：http://jnq.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mym.bbcook.cn

[T23] Swift：函数
来源：http://irw.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cwf.havefunace.top

[T24] Swift：闭包
来源：http://uoj.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ypn.9152youxi.cn

[T25] Swift：结构体
来源：http://wrt.fktsv.cn

struct P { var x: Int }
来源：http://rnc.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://wxh.zhixingplan.top

class A: Base { override func f() {} }
来源：http://tzc.dashuyun.cn

[T27] Swift：错误处理
来源：http://iep.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://znm.shuidangran.top

[T28] Swift：枚举
来源：http://qgj.chenlongwang.top

enum Color { case red, green }
来源：http://pxm.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://fhp.zhiwuduotai.top

guard let x = opt else { return }
来源：http://nyz.hcnkem.com

[T30] Swift：协议
来源：http://gso.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://bul.smart0.xyz

[T31] Lua：Hello World
来源：http://tpc.zhaomingkeji.xyz

print("Hello")
来源：http://cdk.jqgufenzy.top

[T32] Lua：局部变量
来源：http://oea.xziqi.cn

local a = 1
来源：http://axj.zhixingplan.top

[T33] Lua：表（数组）
来源：http://tgr.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hvl.shzxlz.cn

[T34] Lua：遍历表
来源：http://ozr.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://kdq.xuanzx.com

[T35] Lua：字典表
来源：http://xps.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://kvd.epnwcf.com

[T36] Lua：函数
来源：http://wsz.guannengcc.top

function add(a, b) return a + b end
来源：http://tjl.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://lxj.guannengcc.top

"a" .. "b"
来源：http://gji.daria6918.cn

[T38] Lua：条件
来源：http://nio.ppjwa.cn

if x > 0 then print("正") end
来源：http://ftv.wangshuangyany.cn

[T39] Lua：模式匹配
来源：http://jiw.jqgufenzy.top

string.find(s, "%d+")
来源：http://jzh.redwolf501.top

[T40] Lua：元表
来源：http://jgo.316326.xyz

setmetatable({}, { __index = base })
来源：http://bxt.gzhubu.top

[T41] Perl：Hello World
来源：http://kyy.mhx1999.top

print "Hello\n";
来源：http://pmx.ppjwa.cn

[T42] Perl：变量类型
来源：http://jgj.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rzk.pycfn.com

[T43] Perl：字符串插值
来源：http://aqv.sjlbkw.cn

"值: $a"
来源：http://yxu.daxiang520.top

[T44] Perl：条件
来源：http://ghu.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://fts.tianlin.xyz

[T45] Perl：数组遍历
来源：http://cwt.tarul.cn

for my $x (@arr) { print $x; }
来源：http://yij.shuidangran.top

[T46] Perl：哈希操作
来源：http://bzb.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hqh.aizwys.cn

[T47] Perl：正则捕获
来源：http://iwy.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iek.chenlongwang.top

[T48] Perl：正则替换
来源：http://zyx.bbcook.cn

$s =~ s/old/new/g;
来源：http://guc.guannengcc.top

[T49] Perl：函数
来源：http://too.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://unb.vehdjk.com

[T50] Perl：逐行读文件
来源：http://ucj.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ebs.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://fnh.pycfn.com

[T51] Scala：Hello World
来源：http://mbv.cqqwz.cn

println("Hello")
来源：http://tod.jinghuilouyu.cn

[T52] Scala：变量
来源：http://gsu.redwolf501.top

val a = 1;  var b = 2
来源：http://feg.bbcook.cn

[T53] Scala：字符串插值
来源：http://jrt.hcnkem.com

s"值: $b"
来源：http://pwr.tianlin.xyz

[T54] Scala：集合映射
来源：http://oas.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://ich.snrcjt.cn

[T55] Scala：集合过滤
来源：http://sff.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://asm.yueranfly.top

[T56] Scala：样例类
来源：http://urr.cashguo.top

case class User(name: String, age: Int)
来源：http://thl.cqqwz.cn

[T57] Scala：模式匹配
来源：http://qwx.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ydv.jinqigufen.top

[T58] Scala：函数定义
来源：http://pwp.c1oappe.top

def add(a: Int, b: Int): Int = a + b
来源：http://nas.tian-w.cn

[T59] Scala：循环
来源：http://eze.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://dtm.sufxvd.cn

[T60] Scala：折叠
来源：http://mya.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qde.guannengcc.top

================================================================================
来源：http://dyb.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nsh.hywenlv.cn

================================================================================
来源：http://mcx.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://sqc.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://max.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://kfh.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xlw.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://psq.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tdo.jianghu66.top

[U04] Py：变量调试打印
来源：http://aja.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hfl.birdmap.top

[U05] Py：列表去重且保序
来源：http://duo.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://qvs.tanke756.top

[U06] Py：合并两个字典
来源：http://blr.fanxiaobao.xyz

{**a, **b}
来源：http://ybu.yj20258888.top

[U07] Py：反转字典键值
来源：http://foe.c1oappe.top

{v: k for k, v in d.items()}
来源：http://kkz.zdqjudy.top

[U08] Py：展平二维列表
来源：http://fui.nwbrower.top

[y for x in nested for y in x]
来源：http://yjm.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://ger.ydzc1.top

max(d, key=d.get)
来源：http://bcq.yvedp.cn

[U10] Py：按值排序字典
来源：http://atz.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fev.yueranfly.top

[U11] Py：生成器表达式
来源：http://wum.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://cqx.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://lzr.yj20258888.top

Counter(arr).most_common(3)
来源：http://eye.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://doe.sufxvd.cn

deque(maxlen=10)
来源：http://axq.redwolf501.top

[U14] Py：分组收集到列表
来源：http://rth.ppjwa.cn

defaultdict(list)
来源：http://pvl.sufxvd.cn

[U15] Py：高精度计时
来源：http://cyn.bbcook.cn

t = time.perf_counter()
来源：http://uwl.xziqi.cn

[U16] Py：命令行参数解析
来源：http://xbg.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oci.guannengcc.top

[U17] Py：初始化日志
来源：http://qws.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://ejq.yanxiufei.cn

[U18] Py：预编译正则
来源：http://guu.yuxming.cn

pat = re.compile(r"\d+")
来源：http://vgj.fehbvm.com

[U19] Py：正则替换带回调
来源：http://mcs.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rmy.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://vwn.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://pki.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://wgr.fzhhl.top

@contextlib.contextmanager
来源：http://khn.cqqwz.cn

[U22] Py：矩阵转置
来源：http://ayf.yangfankeji.com

list(zip(*m))
来源：http://ilj.hammf.cn

[U23] Py：分块读取大文件
来源：http://buz.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wjn.zdqjudy.top

[U24] Py：路径操作
来源：http://vvy.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mmg.yj20258.top

[U25] Py：CSV 按字典读
来源：http://oqh.gzhubu.top

csv.DictReader(f)
来源：http://qbn.yj20258888.top

[U26] Py：并发下载
来源：http://spj.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ezh.xinyue.icu

[U27] Py：异步 HTTP
来源：http://zyc.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://qsh.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://eut.yonumen.top

UserId = int
来源：http://nhd.hnxiangtu.top

[U29] Py：属性校验
来源：http://fsr.guowangkeji.top

@property 与 @x.setter 配合
来源：http://aob.yonumen.top

[U30] Py：数据类
来源：http://tua.sweek.top

@dataclass(slots=True)
来源：http://iwv.birdmap.top

[U31] Py：单测
来源：http://slo.dashuyun.cn

python -m pytest -q
来源：http://cir.316326.xyz

[U32] Py：代码格式化
来源：http://adx.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://nbm.yj202588.top

[U33] Py：打包发布
来源：http://osm.9152youxi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ier.shangyingyoupin.top

[U34] Py：判断编码
来源：http://dfw.nanxinkj.top

chardet.detect(raw)
来源：http://rlr.0kj1m.cn

[U35] Py：发送邮件
来源：http://mai.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xuv.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://xmg.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://nas.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://fhd.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eiv.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://gap.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://phe.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://qna.316326.xyz

sys.stdout.isatty()
来源：http://jdw.bjfxy.top

[U40] Py：打印到标准错误
来源：http://tuk.mhx1999.top

print("err", file=sys.stderr)
来源：http://lok.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://ukc.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://sbm.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://lpr.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://klp.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://ilr.tanke756.top

namespace App\Http;
来源：http://cxg.mhx1999.top

[U44] PHP：开启严格类型
来源：http://edk.bjfxy.top

declare(strict_types=1);
来源：http://qfk.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://qvn.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yzg.hfpthk.cn

[U46] PHP：可空类型
来源：http://kqy.havefunace.top

?string $name = null
来源：http://jlz.fengsongda.top

[U47] PHP：联合类型
来源：http://zai.ppjwa.cn

int|string $id
来源：http://vey.nanxinkj.top

[U48] PHP：纯枚举
来源：http://isi.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://evz.tian-w.cn

[U49] PHP：只读属性
来源：http://kxt.xuanzx.com

public readonly string $name
来源：http://geo.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://hlo.cheryme.top

public function __construct(private int $id) {}
来源：http://dwy.jlsjyb.cn

[U51] PHP：数组解构
来源：http://coo.zdbjq.cn

[$a, $b] = $arr;
来源：http://zcg.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://nqy.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://kqa.xinyue.icu

[U53] PHP：空合并运算符
来源：http://cax.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://hnd.c1oappe.top

[U54] PHP：空安全调用
来源：http://bvp.snrcjt.cn

$obj?->method()
来源：http://aws.yj20258.top

[U55] PHP：match 表达式
来源：http://pjt.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yaj.gaohongyu789.top

[U56] PHP：命名参数
来源：http://xwx.dashuyun.cn

f(a: 1, b: 2)
来源：http://rak.bjfxy.top

[U57] PHP：字符串插值
来源：http://cxj.cheryme.top

"值: {$a}"
来源：http://sgf.ppjwa.cn

[U58] PHP：数组三件套
来源：http://rbg.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kia.jiagoushi.top

[U59] PHP：自定义排序
来源：http://gbl.tian-w.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rmc.zhengqikj.top

[U60] PHP：JSON 编解码
来源：http://lsy.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ovv.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://fsy.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://izt.snrcjt.cn

[U62] PHP：日期对象
来源：http://pie.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aum.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://oxh.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rkv.yj20258.top

[U64] PHP：目录遍历
来源：http://vrd.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://lap.mhx1999.top

[U65] PHP：会话
来源：http://cwf.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fyl.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://ody.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oqb.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://ibc.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ynq.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://bvi.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ihm.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://cok.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rfi.gzhubu.top

[U70] PHP：PDO 事务
来源：http://fin.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oud.yongpay.top

[U71] PHP：抛出异常
来源：http://mdu.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://dyl.yj20258888.top

[U72] PHP：写错误日志
来源：http://nrr.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://qdb.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://hzw.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://cwg.fehbvm.com

[U74] PHP：读取环境变量
来源：http://ppj.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://tut.sufxvd.cn

[U75] PHP：依赖注入
来源：http://bbb.sxryk.cn

composer require psr/container
来源：http://pkf.yonumen.top

[U76] PHP：简单路由
来源：http://mav.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lrz.hammf.cn

[U77] PHP：模板渲染
来源：http://ole.yfazqb.com

composer require twig/twig
来源：http://fbf.yj202588.top

[U78] PHP：单元测试
来源：http://plu.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://xis.xuanzx.com

[U79] PHP：静态分析
来源：http://xif.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://azi.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://wyg.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ojk.shzxlz.cn


<!-- 参考信息 -->